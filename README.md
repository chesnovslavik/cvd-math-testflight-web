# CVD Math — TestFlight web-update pilot

This repository delivers signed, compiled web assets for the internal iOS TestFlight pilot only. It does not contain the source project, private signing keys, user data, or credentials.

- Supported native app: `com.cvdmath.app`, version `1.0.0`, build `6`.
- Channel: `testflight-ios-6`. Other installed builds must ignore it.
- Each ZIP and the channel payload are separately signed using RSA-SHA256.
- Existing bundle IDs are immutable. A new publication requires a higher signed sequence.
- `pilot-2` changes only the visible test revision marker; all game assets match the native baseline.
- There is no production website or App Store publication in this repository.
- Open-source dependency notices are included in the compiled bundle.

The app can continue with its installed files when this channel is unavailable. Downloads are staged for a later cold start; active lessons are never forcibly reloaded.
