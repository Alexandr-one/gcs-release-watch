# gcs-release-watch

Test stand-in for the [APX GCS](https://github.com/uavos/apx-gcs) releases. Publish a release
tagged `release-X.Y.Z` here to see the plugin repositories release a build for it:
[plugin-release-test](https://github.com/Alexandr-one/plugin-release-test) (fake build, seconds)
and [emip](https://github.com/Alexandr-one/emip) (real build, so X.Y.Z must be a real GCS release).

The plugin repositories find a new release on their own scheduled check; this repository knows
nothing about them.
