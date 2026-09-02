# Unitask.

See https://github.com/Cysharp/UniTask

Forked as-is from there by RMC simply to register it to npmjs.org

## Release a new version

This repository is already configured to publish to npm through GitHub Actions
using npm Trusted Publishing. No npm token or credential belongs in the
repository.

1. Update the `version` in `package.json`.
2. Commit and push the changes to GitHub.
3. Create and publish a GitHub Release using the same version as the package,
   such as `2.5.11`.
4. Wait for the **Publish Release On NPMJS** workflow to finish.
5. Confirm the new version on the npm package page before updating Unity.

The published GitHub Release automatically starts the npm publishing workflow.
