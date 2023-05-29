# github-action-fpm

GitHub action to build packages for multiple platforms using [fpm](https://github.com/jordansissel/fpm).

## Example

```
name: Example workflow yml

on: [push]

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
    - uses: actions/checkout@v3
    - name: Package
      uses: osensa/github-action-fpm@master
      with:
        fpm_args: './build'
        fpm_opts: '--debug -n mypackage -t deb -s dir'
```
## Inputs and Outputs

See [action.yml](action.yml).

## Feedback, Suggestions, Contributions, Known Limitations

See original repository: https://github.com/bpicode/github-action-fpm

Feel free to file an issue, open a pull request, etc.


