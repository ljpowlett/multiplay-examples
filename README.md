# mp-game-server-sample-go

This repository represents a sample game server capable of running on the [Unity Multiplay platform](https://unity.com/products/multiplay).
The [prebuilt releases](https://github.com/Unity-Technologies/mp-game-server-sample-go/releases) are ready for you to upload to Multiplay to try out the service without writing a single line of code!

The capabilities of this sample are as follows:

- Handling of [Multiplay allocation lifecycle](https://docs.unity.com/multiplay/Content/shared/allocation-flow.htm)
  - Achieved by watching for file events on the provided configuration file
  - When allocated, the sample starts a TCP server on the configured `Port` which listens for client connections
  - When de-allocated, this TCP server is stopped
- Dynamic server query results
  - Data such as number of players, map name, etc. are handled appropriately
  - `sqp` and `a2s` query protocols over the configured UDP `QueryPort`

---
_Disclaimer: The repo owners will not (cannot) accept pull requests, GitHub review requests, or any other GitHub-hosted issue management requests._
