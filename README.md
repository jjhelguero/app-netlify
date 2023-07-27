# APP-NETLIFY

This repo showcases an instance where a the web app and web app e2e tests are in separate repos, [app-netlify-cypress-tests](https://github.com/jjhelguero/app-netlify-cypress-tests).

When a PR is created in this repo and an associated branch to update e2e tests is exists in the test repo, then [netlify-plugin-github-dispatch](https://github.com/bahmutov/netlify-plugin-github-dispatch) will trigger the e2e test workflow in the test repo with the same branch name.

Example [PR](https://github.com/jjhelguero/app-netlify/pull/11) in web app repo where PR environment is deployed and [tests](https://github.com/jjhelguero/app-netlify-cypress-tests/actions/runs/5684914773) are triggered to run against it.