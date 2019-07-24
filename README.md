# TypeScript-Standard

[![Build Status](https://travis-ci.org/codecov/TypeScript-Standard.svg?branch=master)](https://travis-ci.org/codecov/TypeScript-Standard) [![codecov](https://codecov.io/gh/codecov/TypeScript-Standard/branch/master/graph/badge.svg)](https://codecov.io/gh/codecov/TypeScript-Standard)

### Last Updated: 07/24/19 17:58:41

## What is this?

This is a **TypeScript** application, with basic unit tests, for which coverage is uploaded to Codecov on a daily basis. It can also serve as an example for how to integrate Codecov into your TypeScript project. If the build is passing for this project, then Codecov's TypeScript report processing is functional and correct on codecov.io.

## Configuration

This project is written in `TypeScript 3.5.3`. Unit tests are written with the `Jest` testing framework. Coverage reports are also generated via `Jest`. 

Unit tests: `src/index.test.ts` which tests `src/index.ts`

## Errors Generating TypeScript Reports

In some instances, there may be errors where coverage reports target transpiled JavaScript files instead of TypeScript files. This is most likely due to the fact that your test runner configuration is not set properly. 

[Example repository with Jest config](https://github.com/drazisil/mco-server/blob/master/package.json#L71-L96)


## Reporting Issues

If you've discovered an issue with this repository or with TypeScript processing in general, it is recommended to email support@codecov.io rather than post an issue here. This repository will not be checked regularly for open issues.

## Contributing

If you would like to contribute your own language specific standard to Codecov you can do so as follows:

1. Write a sample repository that contains Docker and docker-compose based orchestration for running your project easily locally
2. Your project should be as simple as possible while providing and testing the following functions:
   - A function that is fully tested and covered by tests
   - A function that is not tested at all
   - A function that contains a conditional with a tested if and/or else condition.
3. A TravisCI configuration that will run the tests and upload coverage to Codecov.

If your standard is accepted by Codecov you can transfer ownership to the Codecov Organization and will be accepted in our current [List of Standards](https://github.com/codecov/standards-scripts#list-of-standards) with credit given to the repository's original author. You can review the List of Standards to see which languages and frameworks currently need a standard submitted. If you create a standard please, email support@codecov.io with the subject line "New <Language> Standard Submission" and the team will review it for acceptance.