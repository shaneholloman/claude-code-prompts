# System Data Block: azure-access-token-script

- Source: inline

## Summary

Invoke PowerShell to get Az access token, optional tenant, secure-string conversion output JSON.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
${EXPR_1}

-NoProfile

-NonInteractive

-Command


          $tenantId = "${EXPR_2}"
          $m = Import-Module Az.Accounts -MinimumVersion ${NUM}.${NUM} -PassThru
          $useSecureString = $m.Version -ge [version]'${NUM}.${NUM}'

          $params = @{
            ResourceUrl = "${PATH}"
          }

          if ($tenantId.Length -gt ${NUM}) {
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
