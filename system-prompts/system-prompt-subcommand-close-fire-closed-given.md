# System Prompt: e39c3648

- Source: inline

## Summary

… <subcommand> close <code> fire ws_closed with the given code (e.g.

# Raw Prompt Text
${PATH} <subcommand>
  close <code>              fire ws_closed with the given code (e.g. ${NUM})
  poll <status> [type]      next poll throws BridgeFatalError(status, type)
  poll transient            next poll throws axios-style rejection (5xx${PATH})
  register fail [N]         next N registers transient-fail (default ${NUM})
  register fatal            next register 403s (terminal)
  reconnect-session fail    next POST ${PATH} fails
  heartbeat <status>        next heartbeat throws BridgeFatalError(status)
  reconnect                 call reconnectEnvironmentWithSession directly
  status                    print bridge state
