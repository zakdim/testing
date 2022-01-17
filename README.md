[![CircleCI](https://circleci.com/gh/zakdim/testing/tree/master.svg?style=svg)](https://circleci.com/gh/zakdim/testing/tree/master)

# Angular Testing

Official Angular [Developer guides > Testing](https://angular.io/guide/testing) Tutorial

## Configure project for Circle CI

https://angular.io/guide/testing#configure-project-for-circle-ci

* Add the following configuration to `karma.conf.js` for Circle CI build to work:

See: https://stackoverflow.com/a/65360395/2800303
```
browsers: ['Chrome', 'ChromeHeadless', 'ChromeHeadlessCI'],
customLaunchers: {
  ChromeHeadlessCI: {
    base: 'ChromeHeadless',
    flags: ['--no-sandbox']
  }
},
```
