# Change Log

All notable changes to this project will be documented in this file.
See [Conventional Commits](https://conventionalcommits.org) for commit guidelines.

## [0.3.0](https://github.com/Agoric/agoric-sdk/compare/@agoric/telemetry@0.2.1...@agoric/telemetry@0.3.0) (2022-09-20)


### Features

* **cosmic-swingset:** add commit-block slog events ([8335928](https://github.com/Agoric/agoric-sdk/commit/8335928e933b96dc7db78a0895a7582b93ef4f73))
* **cosmic-swingset:** break up inbound queue processing ([e0d844d](https://github.com/Agoric/agoric-sdk/commit/e0d844da0cae132f63039404c42e5979c12977ce))
* **telemetry:** `otel-and-flight-recorder.js` for the best of both ([a191b34](https://github.com/Agoric/agoric-sdk/commit/a191b34bd6a4b14f7280b0886fcfd44b5a42b6b5))
* **telemetry:** flatten nested attributes ([2fc39ca](https://github.com/Agoric/agoric-sdk/commit/2fc39cab8ce3a080c96304af2d772943a653e420))


### Bug Fixes

* **telemetry:** handle missing slog events ([8e353da](https://github.com/Agoric/agoric-sdk/commit/8e353daf4eceac2eb90fddb6f651bc77f24d299c))
* Use new `||` assert style, but when TS confused use `if` instead ([#6174](https://github.com/Agoric/agoric-sdk/issues/6174)) ([94625d3](https://github.com/Agoric/agoric-sdk/commit/94625d38c3bb5333b00a69dd3086b1ac13490f62))
* **kv-string-store:** allow keys to overwrite ([c28b393](https://github.com/Agoric/agoric-sdk/commit/c28b39332c40d4e1def80fee9e7b70588d0c592a))
* **slog-to-otel:** more `methargs` parsing ([42a9bc0](https://github.com/Agoric/agoric-sdk/commit/42a9bc08dfa66f4653253a9cfc104307b44c908c))
* **Swingset:** add crank details to slog event ([be1f443](https://github.com/Agoric/agoric-sdk/commit/be1f443bdfd49325316607142f116ca3153e296f))
* **telemetry:** cleanup slot-to-otel output ([97c695f](https://github.com/Agoric/agoric-sdk/commit/97c695f60fce031bf9307fe8237d3df756d2a4e1))
* **telemetry:** close store iterator on has check ([6199337](https://github.com/Agoric/agoric-sdk/commit/6199337d40e42ffb4057f5a653f9cecfb21afe3f))
* **telemetry:** COMMIT should exit the txn ([36bf35c](https://github.com/Agoric/agoric-sdk/commit/36bf35c4daef7a42456aee7d917eba597abeb887))
* **telemetry:** do not mutate the original slog object ([#5705](https://github.com/Agoric/agoric-sdk/issues/5705)) ([4018a28](https://github.com/Agoric/agoric-sdk/commit/4018a28fcc9ea3ecd28d09e54e5c7cd2d64907b6))
* **telemetry:** ingest script should not skip lines on time backtrack ([785a5c0](https://github.com/Agoric/agoric-sdk/commit/785a5c0974ad8ed62501ad6e02245dd77d7c7815))
* **telemetry:** Use transactions for tmp telemetry DB ([dea1a2a](https://github.com/Agoric/agoric-sdk/commit/dea1a2ac31586cf16216e57162ad2951f07dc178))



### [0.2.1](https://github.com/Agoric/agoric-sdk/compare/@agoric/telemetry@0.2.0...@agoric/telemetry@0.2.1) (2022-05-28)


### Bug Fixes

* **slog-to-otel:** ignore `vatstoreGetAfter` syscall ([7baed8e](https://github.com/Agoric/agoric-sdk/commit/7baed8ea1c7513d57bd33edb8c4b6a80dd5182ed))



## [0.2.0](https://github.com/Agoric/agoric-sdk/compare/@agoric/telemetry@0.1.1...@agoric/telemetry@0.2.0) (2022-04-18)


### ⚠ BREAKING CHANGES

* consistent Node engine requirement (>=14.15.0)

### Features

* **telemetry:** `echo 2022-02-18T12:00:00Z | ./ingest.sh f.slog` ([bede363](https://github.com/Agoric/agoric-sdk/commit/bede363018656bad32b6764a5216acaaf2ca19bc))
* **telemetry:** upgrade to latest `[@opentelemetry](https://github.com/opentelemetry)` ([de82224](https://github.com/Agoric/agoric-sdk/commit/de82224eb08a40e139f20e74d6f1038e50fbfa40))


### Bug Fixes

* **telemetry:** clean up scripts and leave pointers ([1830c55](https://github.com/Agoric/agoric-sdk/commit/1830c55edeb814b79f25f9fbacdbebbac7c2a26f))
* **telemetry:** count work duration per block, not between blocks ([b95a124](https://github.com/Agoric/agoric-sdk/commit/b95a124d17fca6edf04232f8e3a7eeef196e5b43))
* **telemetry:** ingest rate limiting ([fd164c8](https://github.com/Agoric/agoric-sdk/commit/fd164c82d56f416309071b85c60da1af34af7821))
* **telemetry:** rework Prometheus metrics ([38a1922](https://github.com/Agoric/agoric-sdk/commit/38a1922ce2c21e4f31b4a1bedd634bbe627990f9))


### Miscellaneous Chores

* consistent Node engine requirement (>=14.15.0) ([ddc40fa](https://github.com/Agoric/agoric-sdk/commit/ddc40fa525f845ed900512c38b99f01458a3d131))



### 0.1.1 (2022-02-21)


### Features

* **telemetry:** `frcat` script to extract `flight-recorder.bin` ([7ee4091](https://github.com/Agoric/agoric-sdk/commit/7ee409102269ab41a1f3f5d5a0bdd29b6eb12a36))
* **telemetry:** add `@agoric/telemetry/src/flight-recorder.js` ([b02b0c8](https://github.com/Agoric/agoric-sdk/commit/b02b0c8086136d8e780b687ae65df41796946eec))
* **telemetry:** introduce for opentelemetry.io integration ([4e382dc](https://github.com/Agoric/agoric-sdk/commit/4e382dcede81717a4c9941266b0377ad531b8b38))
* **telemetry:** use `makeSlogSenderFromModule` ([2892da9](https://github.com/Agoric/agoric-sdk/commit/2892da96eff902c5f616424d6fb9946aaaef1b0f))


### Bug Fixes

* Remove extraneous eslint globals ([17087e4](https://github.com/Agoric/agoric-sdk/commit/17087e4605db7d3b30dfccf2434b2850b45e3408))
* **telemetry:** make flight recorder big-endian on all platforms ([bfe877e](https://github.com/Agoric/agoric-sdk/commit/bfe877e8825d551b9ea6f80e2623fb450883dab0))
