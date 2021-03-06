## 1.0.0 / 2020-09-26
- [FEATURE] Moved the player signals and methods out of `gameguard.players` and into `gameguard`.
- [FEATURE] Moved the room signals and methods out of `gmaeguard.rooms` and into `gameguard`.
- [FEATURE] Moved the system methods out of `gameguard.system` and into `gameguard`.
- [FEATURE] Removed support for mysql and streamlined the database operations.
- [FEATURE] Added convenience methods to add and update properties of players in the database.
- [TEST] Updated tests and removed unnecessary tests.
- [TEST] Updated framework tests and add npm scripts to run them.
- [DOCS] Updated documentation to reflect latest changes.
- [MISC] Updated out-of-date-dependencies to their latest versions.

## 0.14.1 / 2020-04-17
- [MISC] Updated out-of-date dependencies to their latest versions which also fixed all possible fixed security vulnerabilities.

## 0.14.0 / 2020-02-26
- [FEATURE] Made messages get send and read as binary.
- [MISC] Tested changes with latest version of gameguard-client.
- [MISC] Updated out-of-date dependencies to their latest versions. 

## 0.13.1 / 2020-02-16
- [HOTFIX] Made the initialization options have a default value if no options are provided.

## 0.13.0 / 2020-02-16
- [FEATURE] Added an option to auto-kick a player with a high latency according to a customizable `maxLatency` option.
- [FEATURE] Added a signal that gets dispatched when the player gets kicked for high latency.
- [DOCS] Added docs for new `maxLatency` option and the `timedOut` socket close message.
- [DOCS] Added docs for the timed out signal.
- [DOCS] Removed accidental typescript from code sample in README.
- [MISC] Updated dev dependencies to their latest versions.

## 0.12.0 / 2020-02-13
- [FEATURE] Added ability to customize close messages for the different events.
- [DOCS] Updated documentation for the feature added above.
- [MISC] Updated mongoose package to its latest version.

## 0.11.1 / 2020-02-11
- [DOCS] Updated docs to include information about the heartbeat and latency check.
- [MISC] Updated gameguard-client dev dependency to its latest version.

## 0.11.0 / 2020-02-11
- [FEATURE] Added a hearbeat that checks to see if clients are still connected to the server or not on a customizable interval.
- [FEATURE] Added a latency check to get the players latency on a customizable interval.
- [DOCS] Fixed random old documentation.
- [MISC] Updated dependencies to their latest versions.
- [MISC] Changed CHANGELOG formatting.
- [MISC] Removed unnecessary dependencies.

## 0.10.0 / 2020-01-28
- [FEATURE] Normalized signal names.
- [FEATURE] Changed rooms `created` to `rooms` and players `connected` to `players` since signal names changed.
- [DOCS] Updated documentation for new signal names.
- [DOCS] Added individual player documentation at docs/player.md.
- [TEST] Udpated tests.

## 0.9.0 / 2020-01-28
- [FEATURE] Changed from using events to signals.
- [DOCS] Updated documentation for signals.
- [TEST] Updated tests.
- [MISC] Updated dependencies to their latest versions.

## 0.8.0 / 2020-01-25
- [FEATURE] Added option to use mysql.
- [FEATURE] Changed the `database` option to `dbType` for more clarity.
- [FEATURE] Added option to use a .env file to specify database connection information.
- [DOCS] Added a .sample.env file to highlight the options available for use in a .env file and their default values.
- [DOCS] Updated README with lateast information.

## 0.7.0 / 2020-01-19
- [FEATURE] Matched version with gameguard-client. From this point forward both packages with matching version numbers will be guaranteed to work with each other.

## 0.5.1 / 2020-01-18
- [FEATURE] Added mongodb as the default storage method.
- [BREAKING] Local storage is broken as of this patch and so mongodb is the only option until the next storage update when support for mysql is added.
- [MISC] Added breaking change note to README.

## 0.5.0 / 2020-01-08
- [FEATURE] Moved the client-side component to its own package, see the README for more.
- [FEATURE] Messages now require a message object instead of type and content.
- [FEATURE] Changed the `player-joined` event to `player-connected`.
- [FEATURE] Changed the `player-left` event to `player-disconnected`.
- [FEATURE] Converted the project to typescript.
- [FEATURE] Changed the `players` property of the players module to be `connected`.
- [FEATURE] Changed the `rooms` property of the rooms module to `created`.
- [MISC] Removed unnecessary dependencies and moved express to a be a dev dependency which it should have been all along.
- [MISC] Updated README to reflect breaking changes.

## 0.4.3 / 2020-01-08
- [MISC] Made private methods that weren't really private public.
- [MISC] Updated dependencies to their latest versions.

## 0.4.2 / 2020-01-05
- [MISC] Slightly cleaned up docs in preparation for new functionality.

## 0.4.1 / 2020-01-05
- [HOTFIX] Added main property to package.json.
- [MISC] Updated license year to reflect new year.
- [MISC] Removed extra spacing.
- [MISC] Removed debugging statements.
- [MISC] Updated dependencies to their latest versions.

## 0.4.0 / 2019-12-24
- [MISC] Updated tests to clear database file before each one.
- [MISC] Added more test cases.
- [MISC] Moved all tests to tests folder.
- [HOTFIX] Changed the client to use window.location.host instead of localhost.
- [HOTFIX] Made secure flag change connection string to wss.

## 0.3.0 / 2019-12-24
- [FEATURE] Changed class properties to be strict and added the necessary setters/getters to be more strict.
- [MISC] Updated JSdoc comments.
- [MISC] Added badges to README and updated getters/setters documentation.
- [MISC] Updated dependencies to their latest versions.

## 0.1.0 / 2019-10-16
- Initial release
