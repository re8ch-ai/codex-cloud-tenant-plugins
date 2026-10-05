# Re8ch for Claude

Re8ch gives Claude one OAuth connection to tenant services and any platform
tools authorized for the signed-in account. Users can discover their available
services, inspect resources and usage, plan changes, and request supported
operations. The server determines the tenant and permissions from the login
session. A reviewer account can use a dedicated sample tenant; it does not
change the connection or grant access to another tenant.

The plugin connects to `https://tools.service.re8ch.com/tenant-native/mcp`.
Authentication uses the RE8CH identity service. Requests and tool results are
sent to this RE8CH server to provide the requested operation. Installers must
have a RE8CH account with the appropriate tenant grants. The public plugin
files contain no credentials and installation alone grants no cloud access.

To get started, install the plugin, connect with your RE8CH account, then ask
Claude to show the capabilities available to your tenant. For changes, ask
Claude to plan first and review the plan before requesting execution.

The [privacy policy](./PRIVACY.md) describes RE8CH's data practices. For help,
use the [support form](https://re8ch.com/en/feedback/) or email
`contact@re8ch.com`. The plugin source is MIT licensed. The RE8CH name and
logo remain trademarks of their owner.
