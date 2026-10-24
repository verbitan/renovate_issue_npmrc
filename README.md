# 47344

## Current behavior

Renovate is not respecting the `npmrc` configuration for the registry when
resolving dependencies, leading to incorrect package resolutions.

This is only true when there is an `.npmrc` file in the repository.

## Expected behavior

Renovate should ignore the `.npmrc` file in the repository and use the
configuration provided in the Renovate configuration property `npmrc` instead.

> If configured like this, Renovate will use this to authenticate with npm and
> will ignore any .npmrc files(s) it finds checked into the repository.

https://docs.renovatebot.com/getting-started/private-packages/#npm

## Link to the Renovate issue or Discussion

https://github.com/renovatebot/renovate/discussions/47344
