<div align="center">
  <h1>@system76/renovate-config</h1>
  <h3>System76 configuration for Renovate Bot</h3>
  <br>
  <br>
</div>

<p align="center">
  <a href="https://www.npmjs.com/package/@system76/renovate-config/">
    <img src="https://img.shields.io/npm/v/@system76/renovate-config.svg" alt="npm">
  </a>

  <a href="https://travis-ci.org/system76/renovate-config">
    <img src="https://travis-ci.org/system76/renovate-config.svg" alt="travis-ci">
  </a>

  <a href="https://renovatebot.com/">
    <img src="https://img.shields.io/badge/renovate-enabled-brightgreen.svg" alt="renovate">
  </a>

  <a href="https://standardjs.com">
    <img src="https://img.shields.io/badge/code_style-standard-brightgreen.svg" alt="standard">
  </a>
</p>

---

This is the System76 organization configuration for
[Renovate Bot](https://renovatebot.com).

## Basics

- Only creates PRs during non work hours, but updates PRs at a regular interval
- Groups any non major semver packages into a single PR
- Labels all PRs with "dependencies" and "lint"

## Using

Include a top level `renovate.json` file with the following content:

```json
{
  "extends": [
    "@system76"
  ]
}
```

## Deployment

This repository uses [Angular Commit Message Conventions](https://github.com/angular/angular.js/blob/master/DEVELOPERS.md#-git-commit-guidelines)
to determine version number and auto deploy. Simply push to master and travis
will do all the work for you!
