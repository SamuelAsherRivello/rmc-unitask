# Unitask.

See https://github.com/Cysharp/UniTask

Forked as-is from there by RMC simply to register it to npmjs.org

## Release a new version

This package is published to npm by GitHub Actions when a GitHub Release is
published. The repository must have an `NPM_TOKEN` GitHub Actions secret.

1. Update the `version` in `package.json`.
2. Commit and push the changes to GitHub.
3. Create a GitHub Release using the same version as the package, such as
   `2.3.33`, and publish the release.
4. Wait for the **Publish Release On NPMJS** workflow to finish.
5. Confirm the new version on the npm package page before updating Unity.

The workflow runs `npm publish --access public` with the repository's
`NPM_TOKEN`; no npm login is needed on the local computer.
