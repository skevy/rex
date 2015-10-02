# REX [![Build Status](https://travis-ci.org/exponentjs/rex.svg?branch=master)](https://travis-ci.org/exponentjs/rex)

REX is a tool that takes your JavaScript source files and serves a bundle that you deploy to clients. It is a standalone version of the packager included with [React Native](https://github.com/facebook/react-native). If you need a JavaScript packager without the rest of React Native, this is your tool.

## Collaborating

We welcome collaborators, especially if you're interested in building tools that keep this repository in sync with the upstream React Native project.

Tasks we need help on:
 - Writing a little Node bot that is pinged whenever there is a commit to the upstream React Native repo
 - Checking if that commit touches any of the files or directories of interest to REX
   - This would be the `jestSupport` and `packager` directories for now
 - Create a new commit that pulls over just the relevant changes
   - We don't care about non-packager code
   - Preserve details about the original author
   - Include a link to the original PR and commit in case a person needs to look it over
 - Automatically submit a PR with the commit
 - Automatically merge the PR if Travis CI tests pass
 - If tests fail we need a way for a person to take over a PR
   - Document that process for collaborators

Please open up an issue if you start working on one of these so that we can efficiently work together.

## License

The packager is derived from the React Native project. It's [license](./LICENSE-ReactNative) and [patent grants](./PATENTS-ReactNative) are included in this repository. There is also a [BSD license](./LICENSE) for code that is not from React Native.
