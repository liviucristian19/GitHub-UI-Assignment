Development
How this action works
This action works by evaluating the user input as the body of an asynchronous JavaScript function. See main.ts for details.

Building
Before the action can be used, it needs to be compiled to JavaScript:

bash> npm run build
It also has a pre-commit hook configured via husky that should run the build script before each commit. Additionally, this hook formats code and lints it, as well.

Releasing
Releases are done manually, for now:

Ensure that the build is up to date with npm run build.
Bump the package.json and package-lock.json version numbers and commit them.
Update documentation (including updated version numbers).
Tag main with the new version number and create a GitHub release.
