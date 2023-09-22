## Workflow Configuration

### Action Inputs

| Input Name            | Description                                                                                                  | Type      | Default                                 | Required |
|-----------------------|--------------------------------------------------------------------------------------------------------------|-----------|-----------------------------------------|----------|
| `target`              | The target type to build scons with. Must be `editor`, `template_release`, or `template_debug`.              | `string`  | `template_release`                      | No       |
| `platform`            | The target platform for the build.                                                                           | `string`  |                                         | No       |
| `sconsflags`          | The additional scons flags to provide for the build.                                                         | `string`  |                                         | No       |
| `scons-cache`         | The scons cache path to use for the build.                                                                   | `string`  | `${{ github.workspace }}/.scons-cache/` | No       |
| `scons-cache-limit`   | The maximum size of megabytes the scons cache can be in one run.                                             | `boolean` | `7168`                                  | No       |