# After creating a repo from this template

Delete this file once you're done.

1. Replace the placeholders in `README.md`.
2. Put the real build, lint and test jobs into `.github/workflows/ci.yml`. Each job gets
   `needs: cla-gate`, and every job goes into `ci-required.needs`. Change `branches: [main]`
   if the default branch has another name.
3. Apply the org policy (label `cla-signed`; ruleset for public repos, App credentials for private ones):
   ```sh
   # from a checkout of deepnest-next/.github
   scripts/apply-repo-policy.sh <new-repo> [deepnest-cla-bot.pem]
   ```
4. For Rust or Node packages, set the licence field to
   `AGPL-3.0-or-later OR LicenseRef-Deepnest-Commercial`.

Details: https://github.com/deepnest-next/.github/blob/main/CLA-SETUP.md
