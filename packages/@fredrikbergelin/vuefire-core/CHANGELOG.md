# Change Log

All notable changes to this project will be documented in this file.
See [Conventional Commits](https://conventionalcommits.org) for commit guidelines.

## [2.3.21](https://github.com/vuejs/vuefire/compare/@fredrikbergelin/vuefire-core@2.3.13...@fredrikbergelin/vuefire-core@2.3.21) (2021-08-04)

**Note:** Version bump only for package @fredrikbergelin/vuefire-core





## [2.3.13](https://github.com/vuejs/vuefire/compare/@fredrikbergelin/vuefire-core@2.3.11...@fredrikbergelin/vuefire-core@2.3.13) (2021-08-04)

**Note:** Version bump only for package @fredrikbergelin/vuefire-core





## [2.3.11](https://github.com/vuejs/vuefire/compare/@fredrikbergelin/vuefire-core@2.3.9...@fredrikbergelin/vuefire-core@2.3.11) (2021-08-04)

**Note:** Version bump only for package @fredrikbergelin/vuefire-core





## [2.3.9](https://github.com/vuejs/vuefire/compare/@fredrikbergelin/vuefire-core@2.3.7...@fredrikbergelin/vuefire-core@2.3.9) (2021-08-04)

**Note:** Version bump only for package @fredrikbergelin/vuefire-core





## [2.3.7](https://github.com/vuejs/vuefire/compare/@fredrikbergelin/vuefire-core@2.3.5...@fredrikbergelin/vuefire-core@2.3.7) (2021-08-04)

**Note:** Version bump only for package @fredrikbergelin/vuefire-core





## [2.3.5](https://github.com/vuejs/vuefire/compare/@fredrikbergelin/vuefire-core@2.3.5...@fredrikbergelin/vuefire-core@2.3.5) (2021-08-04)

**Note:** Version bump only for package @fredrikbergelin/vuefire-core





## 2.3.5 (2021-08-04)

**Note:** Version bump only for package @fredrikbergelin/vuefire-core





## [2.3.4](https://github.com/vuejs/vuefire/compare/@fredrikbergelin/vuefire-core@2.3.3...@fredrikbergelin/vuefire-core@2.3.4) (2020-12-07)

**Note:** Version bump only for package @fredrikbergelin/vuefire-core





## [2.3.3](https://github.com/vuejs/vuefire/compare/@fredrikbergelin/vuefire-core@2.3.2...@fredrikbergelin/vuefire-core@2.3.3) (2020-07-31)


### Bug Fixes

* **core:** drop raw refs when updating docs ([3d0b326](https://github.com/vuejs/vuefire/commit/3d0b326e2855f0cdab160281262b1edc8be8606c)), closes [#831](https://github.com/vuejs/vuefire/issues/831)





## [2.3.2](https://github.com/vuejs/vuefire/compare/@fredrikbergelin/vuefire-core@2.3.1...@fredrikbergelin/vuefire-core@2.3.2) (2020-07-06)


### Bug Fixes

* **core:** allow null values in arrays ([e5f2727](https://github.com/vuejs/vuefire/commit/e5f27278f446d18d6686a1c5f0aa44237996b9c0)), closes [#815](https://github.com/vuejs/vuefire/issues/815)





## [2.3.1](https://github.com/vuejs/vuefire/compare/@fredrikbergelin/vuefire-core@2.3.0...@fredrikbergelin/vuefire-core@2.3.1) (2020-03-17)


### Bug Fixes

* **firestore:** array with objects with references ([b50ac72](https://github.com/vuejs/vuefire/commit/b50ac72e3c4165fa20c72410e185604960b48ba4)), closes [#576](https://github.com/vuejs/vuefire/issues/576)





# [2.3.0](https://github.com/vuejs/vuefire/compare/@fredrikbergelin/vuefire-core@2.2.0...@fredrikbergelin/vuefire-core@2.3.0) (2019-12-31)


### Bug Fixes

* **core:** allow writing to default options ([d440e2f](https://github.com/vuejs/vuefire/commit/d440e2fe874dd0a37f4b78333cd8be10e3330634))
* **core:** preserve empty references in objects and arrays ([1397e47](https://github.com/vuejs/vuefire/commit/1397e472bb0171febb4225f7847b4c21e34b4ab8)), closes [#325](https://github.com/vuejs/vuefire/issues/325)
* **core:** preserve refs in documents in bound collections ([519fd9f](https://github.com/vuejs/vuefire/commit/519fd9f2ad9301196c5ad98cf5eed265c398a48b))
* **core:** resolve non existant docs and collections ([9089291](https://github.com/vuejs/vuefire/commit/9089291a6c11551f1b6dfc33b4c3b9c73c7550d0)), closes [#539](https://github.com/vuejs/vuefire/issues/539)


### Features

* wip non enumerable properties ([57e8f1c](https://github.com/vuejs/vuefire/commit/57e8f1c43b244e314a152dde026561ea2a468de4))
* **core:** preserve non enumerable properties ([3469c45](https://github.com/vuejs/vuefire/commit/3469c45889bb2ed285c0f0d672821d4b3b73246a))


### Performance Improvements

* **core:** reduce package size ([3359a67](https://github.com/vuejs/vuefire/commit/3359a676336ae1258ad44518150c4844210753dd))





# [2.2.0](https://github.com/vuejs/vuefire/compare/@fredrikbergelin/vuefire-core@2.1.2...@fredrikbergelin/vuefire-core@2.2.0) (2019-10-10)


### Bug Fixes

* **core:** reset is ignored when unbinding if passed to bind ([8c5bd69](https://github.com/vuejs/vuefire/commit/8c5bd69))


### Features

* **core:** add wait option for firestore ([67560c0](https://github.com/vuejs/vuefire/commit/67560c0))
* **core:** add wait option to rtdb ([b431a28](https://github.com/vuejs/vuefire/commit/b431a28))
* **core:** allow reset option in unbind rtdb ([aad5f08](https://github.com/vuejs/vuefire/commit/aad5f08))
* **core:** allow reset option to be passed to unbind firestore ([634f51f](https://github.com/vuejs/vuefire/commit/634f51f))





## [2.1.2](https://github.com/vuejs/vuefire/compare/@fredrikbergelin/vuefire-core@2.1.1...@fredrikbergelin/vuefire-core@2.1.2) (2019-08-06)


### Bug Fixes

* remove usage of fill to support IE ([1346b90](https://github.com/vuejs/vuefire/commit/1346b90)), closes [#332](https://github.com/vuejs/vuefire/issues/332)





## [2.1.1](https://github.com/vuejs/vuefire/compare/@fredrikbergelin/vuefire-core@2.1.0...@fredrikbergelin/vuefire-core@2.1.1) (2019-08-05)

**Note:** Version bump only for package @fredrikbergelin/vuefire-core
