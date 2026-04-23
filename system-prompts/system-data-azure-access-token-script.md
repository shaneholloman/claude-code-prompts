# System Data Block: azure-access-token-script

- Source: native-reference-match

## Summary

System Data Block: azure-access-token-script - Source: inline Summary Invoke PowerShell to get Az access token, optional tenant, secure-string conversion out…

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |
| `EXPR_6` | None | None |
| `EXPR_7` | None | None |
| `EXPR_8` | None | None |

# Raw Prompt Text
# System Data Block: azure-access-token-script

- Source: inline

## Summary

Invoke PowerShell to get Az access token, optional tenant, secure-string conversion output JSON.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |

# Raw Prompt Text
${EXPR_1}

-NoProfile

-NonInteractive

-Command


          $tenantId = "${EXPR_2}"
          $m = Import-Module Az.Accounts -MinimumVersion ${EXPR_3}.${EXPR_4} -PassThru
          $useSecureString = $m.Version -ge [version]'${EXPR_5}.${EXPR_6}'

          $params = @{
            ResourceUrl = "${EXPR_7}"
          }

          if ($tenantId.Length -gt ${EXPR_8}) {
            $params["TenantId"] = $tenantId
          }

          if ($useSecureString) {
            $params["AsSecureString"] = $true
          }

          $token = Get-AzAccessToken @params

          $result = New-Object -TypeName PSObject
          $result | Add-Member -MemberType NoteProperty -Name ExpiresOn -Value $token.ExpiresOn
          if ($useSecureString) {
            $result | Add-Member -MemberType NoteProperty -Name Token -Value (ConvertFrom-SecureString -AsPlainText $token.Token)
          } else {
            $result | Add-Member -MemberType NoteProperty -Name Token -Value $token.Token
          }

          Write-Output (ConvertTo-Json $result)
