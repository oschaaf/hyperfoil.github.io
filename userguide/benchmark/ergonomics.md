# Ergonomics

This section hosts only single property at this moment:

| Property             | Default | Description |
| -------------------- | ------- | ----------- |
| repeatCookies        | true    | Automatically parse cookies from HTTP responses, store them in session and resend them with subsequent requests. |
| userAgentFromSession | true    | Add user-agent header to each request, holding the agent name and session id. |
| privateHttpPools     | false   | Connections are not returned directly to common pool but instead to a per-session one. When retrieving a connection this private pool is consulted first. |
| autoRangeCheck       | true    | Mark 4xx and 5xx responses as invalid. You can also turn this off in each step. |
| stopOnInvalid        | true    | When the session receives an invalid response it does not execute any further steps, cancelling all requests and stopping immediately. |
| followRedirect       | NEVER   | Default value for [httpRequest.handler.followRedirect]({{ "/docs/steps/step_httpRequest.html#handler" | absolute_url }}).
