# minimum-dependency-versions

Check that the minimum dependency versions follow `xarray`'s policy.

## Usage

To use the `minimum-dependency-versions` action in workflows, simply add a new step:

```yaml
jobs:
  my-job:
    ...
    steps:
    ...
    - uses: xarray-contrib/minimum-dependency-versions@version
      with:
        environment-paths: path/to/env.yaml
```

To analyze multiple environments at the same time, pass a multi-line string:

```yaml
jobs:
  my-job:
    ...
    steps:
    ...

    - uses: xarray-contrib/minimum-dependency-versions@version
      with:
        environment-paths: |
          path/to/env1.yaml
          path/to/env2.yaml
          path/to/env3.yaml
```
