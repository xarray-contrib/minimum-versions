# minimum-dependency-versions

Check that the minimum dependency versions follow `xarray`'s policy.

## Usage

To use the `minimum-dependency-versions` action in workflows, simply add a new step:

```yaml
jobs:
  my-job:
    ...

    - uses: xarray-contrib/minimum-dependency-versions@version
      with:
        ...
```
