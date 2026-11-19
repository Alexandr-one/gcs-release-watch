# gcs-release-watch

Test stand-in for the [APX GCS](https://github.com/uavos/apx-gcs) releases. Publish a release
tagged `release-X.Y.Z` here to see the plugin repositories release a build for it:
[plugin-release-test](https://github.com/Alexandr-one/plugin-release-test) (fake build, seconds)
and [emip](https://github.com/Alexandr-one/emip) (real build, so X.Y.Z must be a real GCS release).

[notify-plugins.yml](.github/workflows/notify-plugins.yml) is the hook: on a published release it
sends the `gcs-release` event to the listed plugin repositories. It needs the repository secret
`PLUGINS_DISPATCH_TOKEN`; without it the plugins find the release on their scheduled check.
