# perdicis
Perdicis project.

## Deploying
Do `npm run deploy -- -m "Commit message"` to generate a static build of the site and commit it to the live gh-pages branch.

What happens under the hood: `npm predeploy` automatically triggers before `npm deploy`, building the site and adding the perdicis.com `CNAME` into the build directory. `npm deploy` commits the build directory contents to gh-pages and `--` lets us pass additional options (in this case a message string) to the deploy script.