# cla-database

cla-database stores ["Tencent Contributor License Agreement"](Tencent-Contributor-License-Agreement.md), and signatures of tRPC contributors.

## Copyright

The copyright notice pertaining to the Tencent code in this repo was previously in the name of “THL A29 Limited.”  That entity has now been de-registered.  You should treat all previously distributed copies of the code as if the copyright notice was in the name of “Tencent.”


## GitHub Action

This repository can be integrated with [contributor-assistant/github-action](https://github.com/contributor-assistant/github-action) to automate the CLA signing process in GitHub Workflows. To enable cross-repository access, this repository provides a secret named `CLA_DATABASE_ACCESS_TOKEN`. Other repositories can set a secret with the same name and use this token to access the CLA data in this repository from their workflow scripts. Otherwise, HTTP 401 errors may occur in the workflow.

> Note: [contributor-assistant/github-action](https://github.com/contributor-assistant/github-action) has a known issue where it cannot automatically create the CLA file on the first run (see [issue #155](https://github.com/contributor-assistant/github-action/issues/155)). Therefore, you need to manually submit a PR to create the CLA file when integrating for the first time. You can refer to the merged [PR #5](https://github.com/trpc-group/cla-database/pull/5) as an example.  Otherwise, HTTP 404 errors may occur in the workflow.



