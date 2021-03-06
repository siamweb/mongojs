## Change Log

### 2.5.0 / 2018-02-04

  * 2.5.0
  * Use === instead of == to please the standard
  * Execute geotag pkg optional
  * Adapt to exec shelljs api changes
  * Update dependencies
  * Use cursor sort order to avoid tests fail due to sort order
  * Add test to verify issue [#337](https://github.com/mafintosh/mongojs/issues/337)
  * Update mongodb dependency
  * Merge pull request [#332](https://github.com/mafintosh/mongojs/issues/332) from ChuanyuWang/master
    Work around for property 'Symbol(Symbol.toPrimitive)' in Proxy handler
  * Merge branch 'master' into master
  * Update standard and fix code style issues
  * Merge pull request [#318](https://github.com/mafintosh/mongojs/issues/318) from drcircuit/addDeletedCount
    Add deleted count property to the return object of the .remove method
  * Add node 7 and 8 and mongodb 3.4 to build matrix and update mongodb versions
  * Merge branch 'master' of github.com:mafintosh/mongojs
  * Fixes [#265](https://github.com/mafintosh/mongojs/issues/265) by breaking operations if max bulk size is exceeded
  * Merge pull request [#327](https://github.com/mafintosh/mongojs/issues/327) from orta/module_import
    Adds support for ES6 default module import syntax
  * Update changelog fixes [#311](https://github.com/mafintosh/mongojs/issues/311) [#303](https://github.com/mafintosh/mongojs/issues/303)

### 2.4.1 / 2017-08-08

  * 2.4.1
  * Geotag package for release
  * Update thunky to version ^1.0.2 to fix [#321](https://github.com/mafintosh/mongojs/issues/321)
  * Fix problem that newer versions of mongodb do not expose connection url in options
  * Merge pull request [#334](https://github.com/mafintosh/mongojs/issues/334) from lukechilds/patch-1
    Fix Markdown
  * Fix Markdown

### 2.4.0 / 2016-04-28

  * 2.4.0
  * Geotag package for release
  * Merge branch 'master' of github.com:mafintosh/mongojs
  * Fix shelljs output check
  * Add node.js 6 to travis build matrix
  * Update dev dependencies
  * Return the created proxy instead of assigning it to a var p
  * Merge pull request [#301](https://github.com/mafintosh/mongojs/issues/301) from JonnyBurger/master
    Fix for node 6
  * Remove semicolon
  * Fix coding style
  * Fix for node 6
  * Merge pull request [#298](https://github.com/mafintosh/mongojs/issues/298) from bendytree/patch-1
    Updated readme with connection options example
  * Updated readme with connection options example
  * Merge pull request [#295](https://github.com/mafintosh/mongojs/issues/295) from olegam/master
    Added test case find-sort-many
  * Style changed to be compliant with javascript standard style
  * Fixed indentation to use spaces
  * Added (failing) test case find-sort-many to demonstrate that sort does not work for more than 1000 results
  * Merge pull request [#276](https://github.com/mafintosh/mongojs/issues/276) from ForbesLindesay/patch-4
    Make `Bulk.toString()` actually return a string
  * Merge pull request [#285](https://github.com/mafintosh/mongojs/issues/285) from mafintosh/saintedlama/travis-non-legacy
    Saintedlama/travis non legacy
  * Remove mongodb 2.4 from test matrix due to compatibility issues
  * Merge branch 'master' into saintedlama/travis-non-legacy
  * Temporary bug fix for tape sporadic errors - see https://github.com/substack/tape/issues/223
  * Merge pull request [#284](https://github.com/mafintosh/mongojs/issues/284) from mafintosh/saintedlama/tap-spec
    Run tests with tap-spec
  * Run tests with tap-spec
  * Check if opts is a function so a callback can be passed as second argument
  * Add test for rename
  * Adjust code style in argument sanitizing
  * Remove semicolons
  * Fix PR [#280](https://github.com/mafintosh/mongojs/issues/280)

### 2.3.0 / 2016-01-14

  * 2.3.0
  * Geotag package for release
  * Merge pull request [#280](https://github.com/mafintosh/mongojs/issues/280) from mrvautin/master
    Wrapper to rename a collection
  * no message
  * Added wrapper to rename a collection
  * Fix test for bulk.toString
  * Merge pull request [#277](https://github.com/mafintosh/mongojs/issues/277) from naartjie/fix/one-more-test-case-for-217
    add one more test case for [#217](https://github.com/mafintosh/mongojs/issues/217) dot in collections
  * add one more test case for [#217](https://github.com/mafintosh/mongojs/issues/217) dot in collections
  * Make `Bulk.toString()` actually return a string
    Before this change it returns an object, which seems confusing.

### 2.2.2 / 2015-12-15

  * 2.2.2
  * Geotag package for release
  * Merge pull request [#274](https://github.com/mafintosh/mongojs/issues/274) from ForbesLindesay/patch-4
    Fix handling default arguments in ensureIndex
  * Fix handling default arguments in ensureIndex
  * Remove mongodb 2.8.0
  * Pipe output to dev/null
  * Move waiting for mongodb to first before script
  * Move to non legacy infrastructure of travis
  * Add changelog generated with github-changes npm module
  * Add test to verify collections with a dot are working. Closes [#217](https://github.com/mafintosh/mongojs/issues/217)

### v2.2.1 (2015/12/15 08:56 +00:00)
- [8c67514](https://github.com/mafintosh/mongojs/commit/8c675143a234a7c939532347e3f280c395b67b41) 2.2.1 (@saintedlama)
- [9cd87a5](https://github.com/mafintosh/mongojs/commit/9cd87a525d9ba221cadebf2b60f0c9117711ead6) Geotag package for release (@saintedlama)
- [5a7b643](https://github.com/mafintosh/mongojs/commit/5a7b643d59c068550043fe0e8afbd80749549316) Use setImmediate(loop) instead of process.nextTick(loop) to please node 0.10 (@saintedlama)
- [6d78fea](https://github.com/mafintosh/mongojs/commit/6d78feacb9d678b90d621a6d6e47577aa6eccd3b) Fix #270 by using process.nextTick in loop (@saintedlama)
- [04d1231](https://github.com/mafintosh/mongojs/commit/04d1231d799b5f3815eaf408f472b3819ada1b4a) Add test to test queries in large collections to reproduce possible stack trace maximum exceeded errors (@saintedlama)
- [3b8fe9b](https://github.com/mafintosh/mongojs/commit/3b8fe9ba82cb8130ad4e7e267d2317795e0c3853) Add documentation for db.collection.aggregate with options including mongodb documentation link (@saintedlama)
- [79cac0b](https://github.com/mafintosh/mongojs/commit/79cac0bf395c0a95c48550c94659896adf87df8f) Remove unused callback "done" (@saintedlama)
- [b6a755b](https://github.com/mafintosh/mongojs/commit/b6a755b809f3cfda8907ec76401577adab1d0ce9) Cleanup test (@saintedlama)
- [f6b6f2e](https://github.com/mafintosh/mongojs/commit/f6b6f2efbbef40d7f76afd409a6f15394e1bdda7) Add feature to pass options to aggregate. Closes #249 (@saintedlama)
- [23000f2](https://github.com/mafintosh/mongojs/commit/23000f2b1e552aa43adf9a836717031dc0e243cc) Remove superfluous dependency "pump" (@saintedlama)

### v2.2.0 (2015/12/14 08:46 +00:00)
- [6ae95dc](https://github.com/mafintosh/mongojs/commit/6ae95dcce22a6f76a8044b553afc7b3194c08062) 2.2.0 (@saintedlama)
- [6f3a303](https://github.com/mafintosh/mongojs/commit/6f3a30371629e61633aaec2aa1424edf6bc4513e) Geotag package for release (@saintedlama)
- [9729a4d](https://github.com/mafintosh/mongojs/commit/9729a4d9a0f08c7e52a68a4ba76da593572e4263) Use mongodb-native mapReduce implementation (@saintedlama)
- [a368c1f](https://github.com/mafintosh/mongojs/commit/a368c1f154d61ab41659ac8faf8b2089ed80f84d) Rename map reduce tests (@saintedlama)
- [#272](https://github.com/mafintosh/mongojs/pull/272) Merge pull request #272 from lionvs/master (@lionvs)
- [670bc71](https://github.com/mafintosh/mongojs/commit/670bc71bd2499403389b5cd7602be9658b74be6c) Add tests for bulk.toString and bulk.find.replaceOne (@lionvs)
- [e9fac7a](https://github.com/mafintosh/mongojs/commit/e9fac7ab57507c96e86d5068cc1d42cfd33ac285) Add bulk.toString() and bulk.find.replaceOne(), update doc (@lionvs)
- [#269](https://github.com/mafintosh/mongojs/pull/269) Merge pull request #269 from lionvs/master (@lionvs)
- [2e50e22](https://github.com/mafintosh/mongojs/commit/2e50e2299a621a55d7eda128a394ca06f6a3dce6) Fix bulk to json function, add tests to this function (@lionvs)
- [d4dbdb7](https://github.com/mafintosh/mongojs/commit/d4dbdb711cb76661de0ae331668d3901141e99ba) Rename cursor tests to fit naming schema (@saintedlama)
- [865d6e6](https://github.com/mafintosh/mongojs/commit/865d6e6dbca012de9f8f6592a48029622d9a3cd5) Add documentation for aggregate (@saintedlama)
- [77eef29](https://github.com/mafintosh/mongojs/commit/77eef29f6886b2b6fee5b8e8d69b78af44eee16d) Allow passing opts including writeOps to save (@saintedlama)
- [edb5b6d](https://github.com/mafintosh/mongojs/commit/edb5b6daa25215f1642b01aadfc457c1ea1f142e) Merge opts with default writeOps in update (@saintedlama)
- [0345349](https://github.com/mafintosh/mongojs/commit/034534953e53b5e0b6e6f70eb4ff6835d0d71a56) Rename options argument to opts to match code style (@saintedlama)
- [6b6e2df](https://github.com/mafintosh/mongojs/commit/6b6e2df309e70d3ecfdd9395c79870c73cbd2bf5) Align collection.prototype.save argument correction style to mongojs code style (@saintedlama)
- [60573fc](https://github.com/mafintosh/mongojs/commit/60573fc4d2e54aa8e390b6c67c8ca2fe7e1bd06a) Add documentation stub for db.collection.remove with options object (@saintedlama)
- [b7a27aa](https://github.com/mafintosh/mongojs/commit/b7a27aabbb749daf07711354e797bd58e1a83f9b) Update readme to reflect new version 2.x (@saintedlama)

### v2.1.0 (2015/12/09 08:52 +00:00)
- [0639284](https://github.com/mafintosh/mongojs/commit/06392844ec8454fb9ed516e30c65169ccf48f73b) 2.1.0 (@saintedlama)
- [a38dc6d](https://github.com/mafintosh/mongojs/commit/a38dc6d11c0b7fa1e798a29fc37b5fd6365a382c) Geotag package for release (@saintedlama)
- [303c2f9](https://github.com/mafintosh/mongojs/commit/303c2f9bc2f9bcf0b0e84cf013c2c62d3e534839) Run the correct script to geo tag the pkg. Really! (@saintedlama)
- [9d87de7](https://github.com/mafintosh/mongojs/commit/9d87de73ad20e9f8c076e024284e81049c425033) Run geopkg npm script correctly (@saintedlama)
- [e64ef5c](https://github.com/mafintosh/mongojs/commit/e64ef5c9f3156e01096a2a1c2bb941b71ad44161) Add back check for git status in release script (@saintedlama)
- [b5e5632](https://github.com/mafintosh/mongojs/commit/b5e56326528a47f4463d6621ae27547c409f09d6) Fix code style to adhere to the standard (@saintedlama)
- [1f72797](https://github.com/mafintosh/mongojs/commit/1f72797b1f1e2b8432f20131f7e20d9d45f6eb78) Add shelljs based release script (@saintedlama)
- [1248b5e](https://github.com/mafintosh/mongojs/commit/1248b5e03f9fb4636f2f0cd854fa2c91d3ac6184) Fix pushing null commands to bulk pipeline in case no bulk operation was added (@saintedlama)
- [4c407e3](https://github.com/mafintosh/mongojs/commit/4c407e3f53ca40147a750d6479ad216b777afa12) Implement listCollections and use listCollections to implement getCollectionNames (@saintedlama)
- [7b27dc6](https://github.com/mafintosh/mongojs/commit/7b27dc60ef0918583304ec0d5d8e0ed1ed806e74) Adhere to the standard (@saintedlama)
- [9b77c8d](https://github.com/mafintosh/mongojs/commit/9b77c8d1c27cbf3f3179062bd4556852778ad377) Implement some missing cursor methods (@saintedlama)
- [#253](https://github.com/mafintosh/mongojs/pull/253) Merge pull request #253 from mortenanders/finalize (@mortenanders)
- [709f67a](https://github.com/mafintosh/mongojs/commit/709f67a3c276d2fe22b3d8c771efe3bee89eefc5) Implement optional callback in db.collection.remove (@saintedlama)
- [3e19869](https://github.com/mafintosh/mongojs/commit/3e19869a4ca35acf36baf650e76e02af105b10ae) Rely on mongodb native ensure index and create index commands and compatibility handling for mongodb versions < 2.8 (@saintedlama)
- [08e8d99](https://github.com/mafintosh/mongojs/commit/08e8d99cf4d62fb86b1557602fa272cbc5d8843a) Add option to execute a bulk without passing a callback function (@saintedlama)
- [6d365d2](https://github.com/mafintosh/mongojs/commit/6d365d280d5badfc52f7561699d4a2c525879f5e) Correct connection string examples URL (@saintedlama)

### v2.0.0 (2015/12/02 09:04 +00:00)
- [a427564](https://github.com/mafintosh/mongojs/commit/a427564168e230481ee693bff29c0fafb29f71a9) 2.0.0 (@saintedlama)
- [12a639c](https://github.com/mafintosh/mongojs/commit/12a639c02337886453327b4f57003ffb0d0efd38) Test mongojs in node.js 5 environments (@saintedlama)
- [#256](https://github.com/mafintosh/mongojs/pull/256) Merge pull request #256 from mafintosh/saintedlama/mongodb-native (@mafintosh)
- [3c59a49](https://github.com/mafintosh/mongojs/commit/3c59a49f5c5c3cbe6cc900cf14d239ca9c41b8ce) Run geotag update instead of plain geotag in geotag npm script (@saintedlama)
- [689f161](https://github.com/mafintosh/mongojs/commit/689f16183e7ffaf929cf54f9cc6b8ae29e0e6994) Correct connecting section (@saintedlama)
- [ea1b07a](https://github.com/mafintosh/mongojs/commit/ea1b07a1053e299d9280694adf8e3cb1dd78938b) Add tests for mongojs bson type exports (@saintedlama)
- [c864aef](https://github.com/mafintosh/mongojs/commit/c864aef13c0514e7686270ebe07da91deb7c2fc1) Expose NumberLong alias for shell compatibility (@saintedlama)
- [cb973f0](https://github.com/mafintosh/mongojs/commit/cb973f0c25437f153ff2491fc6540cafcaf1a4b2) Fix connection string building for connection strings omitting mongodb:// prefix or host of db (@saintedlama)
- [3426d64](https://github.com/mafintosh/mongojs/commit/3426d64223ae66720c0c26438f138c14d94239fe) Add a connection error handler (@saintedlama)
- [f9ab363](https://github.com/mafintosh/mongojs/commit/f9ab36395a7c6b3a284fbdf43e87a8d060dbd016) Add tests for connection string parsing (@saintedlama)
- [56f1eb8](https://github.com/mafintosh/mongojs/commit/56f1eb83ac29e03e6b601e03f1714125f6df1a83) Implement workaround for harmony proxy in combination with event emitter inheritance (@saintedlama)
- [6f5ecd0](https://github.com/mafintosh/mongojs/commit/6f5ecd086577c88930fad1269a314dda7b153978) Adhere to standard code style (@saintedlama)
- [7b01fa9](https://github.com/mafintosh/mongojs/commit/7b01fa9db3375313231f7212054ffef207aded70) Fix checks for insert and (@saintedlama)
- [67acfa2](https://github.com/mafintosh/mongojs/commit/67acfa2d4b442bdf3f87593d6c39009c39b061fd) Simplify remove (@saintedlama)
- [d079280](https://github.com/mafintosh/mongojs/commit/d07928084bee2326aaab2a396982654b6fd53828) Make checking for err object less verbose (@saintedlama)
- [54a9ab9](https://github.com/mafintosh/mongojs/commit/54a9ab98440c062f8bc8c771b3f44b101e9a9249) Fix code style to match standard version 5 code style (@saintedlama)
- [0268423](https://github.com/mafintosh/mongojs/commit/026842392ea22d79b68d78de48659de371c3d7c3) Update dependencies and move to standard version 5 (@saintedlama)
- [99811b5](https://github.com/mafintosh/mongojs/commit/99811b5fa48f284eaa2b96cabc381f7da2156f26) Ignore vi temporary files (@saintedlama)
- [37c690b](https://github.com/mafintosh/mongojs/commit/37c690b162c6a82ee5f20a023ea5a360d85219af) Increase coverage by adding tests for eval, drop database, db stats, create and drop users (@saintedlama)
- [f49c38e](https://github.com/mafintosh/mongojs/commit/f49c38e602f4000a3a081382add19542762e02a4) Cleanup getCollectionNames implementation by using mongodb-native functionality (@saintedlama)
- [3d375f8](https://github.com/mafintosh/mongojs/commit/3d375f8f96011bd67f5a92398686e864b22dd71f) Generate functions to set limit, batchSize, sort and skip (@saintedlama)
- [bbb030c](https://github.com/mafintosh/mongojs/commit/bbb030cc85e53d85f7270a07a37d3e8964cc6176) Remove duplicate code from aggregate (@saintedlama)
- [44b8ee8](https://github.com/mafintosh/mongojs/commit/44b8ee85b75e28a7b4365f50da9e7db6ca89563f) Introduce _getCollection to avoid duplicate _getConnection + connection.collection(this._fullName) code (@saintedlama)
- [f240a7e](https://github.com/mafintosh/mongojs/commit/f240a7eadeecc7bc536dc2dc9e1a7628af62768b) Clarify comment (@saintedlama)
- [26cc395](https://github.com/mafintosh/mongojs/commit/26cc39503d3926aecf539e37a287f0d80b0ad6b1) Call EventEmitter constructor (@saintedlama)
- [6e182e3](https://github.com/mafintosh/mongojs/commit/6e182e33ac30172d3f24a4c8c84a06a904ca75ed) Test toString implementations for mongos and replica set connection strings (@saintedlama)
- [cb70b55](https://github.com/mafintosh/mongojs/commit/cb70b552a3e4168ec39315f304bd0af22298b0f0) Make database an EventEmitter and emit events for error and connect (@saintedlama)
- [11b513d](https://github.com/mafintosh/mongojs/commit/11b513d5d257b07e586f74d51d71155bf33096e3) Remove destroy event test (@saintedlama)

### v1.4.1 (2015/10/12 08:24 +00:00)
- [5e04437](https://github.com/mafintosh/mongojs/commit/5e04437306b07e18c2e40d295d9135d3f595b473) 1.4.1 (@watson)
- [6341c35](https://github.com/mafintosh/mongojs/commit/6341c35b2e6a9efc699d0d33fbaab8aba36db44f) Rename ready event to connect in README.md (@watson)
- [48a00df](https://github.com/mafintosh/mongojs/commit/48a00dfae513a3f37cb5d5890b7eb1114db50c26) Add test to verify that connecting to a non existing database yields an error in the provided operation callback (@saintedlama)
- [60297a3](https://github.com/mafintosh/mongojs/commit/60297a3779612b84b18f4f62cf289f2328b01872) Implement mongojs and mongodb-native connection passing (@saintedlama)
- [3a89ec7](https://github.com/mafintosh/mongojs/commit/3a89ec7a0215dab98ed7c619caac32ce53d864eb) Implement passing mongojs connections (@saintedlama)
- [143c836](https://github.com/mafintosh/mongojs/commit/143c836910400a7681dbc2947d121f967b32a231) Fix next implementation by checking if the cursor was closed and quite in a graceful manner (@saintedlama)
- [73a79ac](https://github.com/mafintosh/mongojs/commit/73a79ac2aeeb6179b24294fa15ec6a9049befe55) Implement aggregations (@saintedlama)
- [bae604e](https://github.com/mafintosh/mongojs/commit/bae604e620473afb8a427768fa16b9354c855609) Fix code style issues (@saintedlama)
- [d461975](https://github.com/mafintosh/mongojs/commit/d46197501a24129af90fea097e7eb4d3ec596414) Fix code style issues (@saintedlama)
- [e5a60d1](https://github.com/mafintosh/mongojs/commit/e5a60d105160a845c91ea57991266d3de7140f20) Implement bulk operations (@saintedlama)
- [180abe8](https://github.com/mafintosh/mongojs/commit/180abe8b364d112c61fa9f58c53019ae37dca87a) Implement isCapped (@saintedlama)
- [31d98d2](https://github.com/mafintosh/mongojs/commit/31d98d2c89d73a89e0426a35cbf6f20431f1e28d) Implement group (@saintedlama)
- [d95e6a6](https://github.com/mafintosh/mongojs/commit/d95e6a6335e7db5d26b40697adb26bc6842b034e) Implement cursor destroy/close (@saintedlama)
- [1df7336](https://github.com/mafintosh/mongojs/commit/1df73360b0a15a714f1135aa2ebbaa9826a62085) Implement update and getIndexes (@saintedlama)
- [482cb84](https://github.com/mafintosh/mongojs/commit/482cb8402b8d82d1c18be40336f4e934816485c9) Implement cursor operations (@saintedlama)
- [b66eb5b](https://github.com/mafintosh/mongojs/commit/b66eb5be6297b7245d3493588328312ad1521b21) Implement close (@saintedlama)
- [4257022](https://github.com/mafintosh/mongojs/commit/4257022e81183e2e4a1c5b92ed8e6de6d794d0e1) Implement find using cursor (@saintedlama)
- [bad1461](https://github.com/mafintosh/mongojs/commit/bad14616fe36a2a13ac8da4d353c59cad8a0240b) Add TODO concerning command interface hits (@saintedlama)
- [37c2fb5](https://github.com/mafintosh/mongojs/commit/37c2fb5703be35e4b9aeb41e25b93e0640bf6fd6) Test stats (@saintedlama)
- [749dfd7](https://github.com/mafintosh/mongojs/commit/749dfd76cf4ee85d7d98d411d7af148f1505b943) Implement command execution on collection level (@saintedlama)
- [ac5c2fc](https://github.com/mafintosh/mongojs/commit/ac5c2fc0709f811b1cb4a1e3a0e2878e35ca0dd3) Fix distinct tests (@saintedlama)
- [246976e](https://github.com/mafintosh/mongojs/commit/246976ee7028323eb527f46e76cebf8d3b16be00) Implement basic functionality to insert and remove documents to drive all further tests (@saintedlama)
- [54bae03](https://github.com/mafintosh/mongojs/commit/54bae0340f9afdfa1d21dfce5967dbc473f4a52f) Fix code style (@saintedlama)
- [3026b7f](https://github.com/mafintosh/mongojs/commit/3026b7f4ab0d991495caa7d2b0d87a23d3d0ca3d) Use mongodb instead of mongodb-core and add minimal test to require mongojs and access all bson types (@saintedlama)
- [c67fbbf](https://github.com/mafintosh/mongojs/commit/c67fbbf3e9ee12cef801c14814ae3a6ef13eac26) Add support for finalize in mapReduce (@mortenanders)

### v1.4.0 (2015/10/06 12:27 +00:00)
- [a5b706f](https://github.com/mafintosh/mongojs/commit/a5b706f5e1a7ff9e36a96f5ef17c95c90fca4217) 1.4.0 (@watson)
- [#251](https://github.com/mafintosh/mongojs/pull/251) Merge pull request #251 from mafintosh/watson/expose-bson (@mafintosh)
- [c7de0cc](https://github.com/mafintosh/mongojs/commit/c7de0cc8da14e42e1840105ccd14be289a627be9) Expose bson stuff visible in the shell (@watson)
- [ebf6bc8](https://github.com/mafintosh/mongojs/commit/ebf6bc8d9485fed94fe8bc8d8d6c302345a341ed) Fix build of MongoDB >2.4 on Travis (@watson)
- [0e1b573](https://github.com/mafintosh/mongojs/commit/0e1b5737e1c4075a9d67b66430ed9a58d8dd4f3d) Run tests against Node.js v4.x instead of iojs (@watson)

### v1.3.0 (2015/08/14 09:34 +00:00)
- [f801df6](https://github.com/mafintosh/mongojs/commit/f801df644f469507f1f7f0b956cbab08ecce60e4) 1.3.0 (@saintedlama)
- [469f48c](https://github.com/mafintosh/mongojs/commit/469f48c9b3f50da5422660ca573553b76d208e7f) Add test for pull request #237 "Fixed insert error detection and passing" (@saintedlama)
- [#237](https://github.com/mafintosh/mongojs/pull/237) Merge pull request #237 from AMKohn/patch-1 (@AMKohn)
- [#240](https://github.com/mafintosh/mongojs/pull/240) Merge pull request #240 from kapetan/return-on-connection-error (@kapetan)
- [d9c5fac](https://github.com/mafintosh/mongojs/commit/d9c5facd66ecdfbe4ad1940b163e2a67e8538976) Return on connection error (@kapetan)
- [d2773ec](https://github.com/mafintosh/mongojs/commit/d2773ec2893fa74c4f6f8d994e01ed5a9d1fe8cd) Added more existence checks to insert (@AMKohn)
- [3a1286e](https://github.com/mafintosh/mongojs/commit/3a1286eba10d9a82640ced54915c4a380a4df4ad) Fixed insert error detection and passing (@AMKohn)
- [ba18f23](https://github.com/mafintosh/mongojs/commit/ba18f23676c085ff27567b41631c8f0b26890f83) Remove events not working from Upgrading notice (@saintedlama)
- [27939a7](https://github.com/mafintosh/mongojs/commit/27939a7c4c8badeb98909aa8ced357c72bd822ca) Pass options to mongodb topology instance constructor (@saintedlama)
- [#229](https://github.com/mafintosh/mongojs/pull/229) Merge pull request #229 from mafintosh/saintedlama/events (@mafintosh)
- [f11bcd1](https://github.com/mafintosh/mongojs/commit/f11bcd10abadef44a10a711f7c9a5a773a7c2540) Merge options and connString + cols object into options object (@saintedlama)
- [9d49f53](https://github.com/mafintosh/mongojs/commit/9d49f538b5dd5057f891e187854d32debba6d537) Fix upgrading section (@saintedlama)
- [8d06cfe](https://github.com/mafintosh/mongojs/commit/8d06cfeaa00c7029de95f0db6c8639c0ee37b252) Insert final newline to adhere to standard code style (@saintedlama)
- [bf7473e](https://github.com/mafintosh/mongojs/commit/bf7473e82acb6ed09bf2f078fdeef7b8fab22a72) Add test to assure an unopened db can be closed (@saintedlama)
- [e4ad950](https://github.com/mafintosh/mongojs/commit/e4ad95031fbaa9ac1ba1eab0d7592a8325fc8395) Implement events (@saintedlama)

### v1.2.1 (2015/07/26 06:39 +00:00)
- [7ba25ec](https://github.com/mafintosh/mongojs/commit/7ba25ec1b89a6c747107f96cdb8b11cd1283054a) 1.2.1 (@watson)
- [#228](https://github.com/mafintosh/mongojs/pull/228) Merge pull request #228 from mafintosh/watson/deps (@mafintosh)
- [581a6db](https://github.com/mafintosh/mongojs/commit/581a6db33c9aee8864dd60776ccc52f537717beb) No need to use custom npm version when node.js v0.8 isn't tested (@watson)
- [af83bf0](https://github.com/mafintosh/mongojs/commit/af83bf0105fa5a339cd0c5f50a451c674fdd909a) Fix Travis-CI build to properly test against MongoDB 3.0 (@watson)
- [54f927d](https://github.com/mafintosh/mongojs/commit/54f927d93bc33e5e6eeab9cb7ce73e172ce3e3ab) Upgrade dependencies (@watson)
- [a0caa82](https://github.com/mafintosh/mongojs/commit/a0caa82b57142c7cc365e9df3b9a5f1718a53e2d) Upgrade all dev-dependency modules (@watson)
- [8c4a2df](https://github.com/mafintosh/mongojs/commit/8c4a2dfa846ec9fa191f8caef26a1f70efac778d) Clean up README.md (@watson)
- [7b163a9](https://github.com/mafintosh/mongojs/commit/7b163a9140c4e2b39f80bcdea4ee4c309e8acd96) Practise what we preach: Use standard code style in examples (@watson)
- [578dcc7](https://github.com/mafintosh/mongojs/commit/578dcc733e0fb72e5530f45368731074548f9245) Add warning block for MongoDB 3 auth (@saintedlama)
- [8a6c786](https://github.com/mafintosh/mongojs/commit/8a6c786d900ac970a001ec01cd0a10408eefa3e3) Add editorconfig (@saintedlama)
- [885d529](https://github.com/mafintosh/mongojs/commit/885d52995a7a1f457379af5f90668cd7009c8648) Add contribution guidelines (@saintedlama)
- [3795d14](https://github.com/mafintosh/mongojs/commit/3795d142567115dfba4ec39de50e0bf1d163533b) Bump copyright year (@watson)

### v1.2.0 (2015/07/25 11:34 +00:00)
- [af8f384](https://github.com/mafintosh/mongojs/commit/af8f384a840870234b32e1c4a0546a7db3f1a21a) 1.2.0 (@watson)
- [933eacb](https://github.com/mafintosh/mongojs/commit/933eacba2c9dd328321726b25f36e5b9c63ebc19) Upgrade readable-stream to ^2.0.2 (@watson)
- [#227](https://github.com/mafintosh/mongojs/pull/227) Merge pull request #227 from mafintosh/watson/standard (@mafintosh)
- [a61b451](https://github.com/mafintosh/mongojs/commit/a61b4515c2866398086892fd119d0fa979d28f39) Add standard code style badge to README.md (@watson)
- [31ea45e](https://github.com/mafintosh/mongojs/commit/31ea45e01b5e373530d09ac253b3d2378f4d40b3) Remove trailing comma in object literal (@watson)
- [8973b36](https://github.com/mafintosh/mongojs/commit/8973b362a1670bb79428eea27e0d91f6af8b5400) Disable linter for problematic JavaScript running inside MongoDB (@watson)
- [6912f95](https://github.com/mafintosh/mongojs/commit/6912f95620bec3a545f2f527553968b91625a1ac) Don't overwrite setImmediate (@watson)
- [2a589ae](https://github.com/mafintosh/mongojs/commit/2a589ae065f5c7855a73222372bed002c9f17d38) Don't assign while returning (@watson)
- [60c1036](https://github.com/mafintosh/mongojs/commit/60c1036af2f0174fb46c951449a98ae248e4de7b) Insert proper spaces in ternaries (@watson)
- [7b56b0f](https://github.com/mafintosh/mongojs/commit/7b56b0fb42db2b7c86652054f82ba9483d8ef938) Remove spaces before colon in object literals (@watson)
- [560795b](https://github.com/mafintosh/mongojs/commit/560795b9807441f50dac297e6af9a9582d71dde5) Add space before opening function curly brackets (@watson)
- [e964661](https://github.com/mafintosh/mongojs/commit/e964661231e89632e275143515ca3c756ce14e82) Fix indentation (@watson)
- [90af4b4](https://github.com/mafintosh/mongojs/commit/90af4b4d4f264254c83894d9572c41d995b47c17) Remove unused variables (@watson)
- [737ceb8](https://github.com/mafintosh/mongojs/commit/737ceb8cb6c373d604f853cc0e5f6c955c359627) Remove trailing spaces (@watson)
- [fcce1f7](https://github.com/mafintosh/mongojs/commit/fcce1f73de9bbc9ab700cf54b911e861b020f22f) Remove spaces before comma (@watson)
- [b00dabb](https://github.com/mafintosh/mongojs/commit/b00dabbfd96dd08c536cfd5a3e78a6964a1e0bdd) Insert space between comma and next value (@watson)
- [481935a](https://github.com/mafintosh/mongojs/commit/481935aef751f5a65cfa8e5059c8c6fbbc8f6301) Handle all errors (@watson)
- [65b7acf](https://github.com/mafintosh/mongojs/commit/65b7acf3ccc8e165fda0e1043d767efd1d72796f) Use t.error to handle errors instead of t.ok(!err) and friends (@watson)
- [1372ed6](https://github.com/mafintosh/mongojs/commit/1372ed6a1d488f37688f24e719e054bf94f9faf1) Use single quotes when defining strings (@watson)
- [ac9f4db](https://github.com/mafintosh/mongojs/commit/ac9f4db029e59ad9570ea371a29b88e6dd5c505f) Ensure while loops evaluate a conditional expression (@watson)
- [e7146c8](https://github.com/mafintosh/mongojs/commit/e7146c823736ffe182b5d4978616a63c83a1c106) Remove semicolons (@watson)
- [e59971e](https://github.com/mafintosh/mongojs/commit/e59971e743a294b58d6f072ce61d535ec288b4d2) Insert space between colon and value in object literals (@watson)
- [8945d41](https://github.com/mafintosh/mongojs/commit/8945d41044c619237c8238654efc328e5d9da074) Insert space before function opening bracket (@watson)
- [0945e27](https://github.com/mafintosh/mongojs/commit/0945e270458647e9cad589d2349b4637b0289335) Add Thomas Watson as contributer (@watson)
- [195ffce](https://github.com/mafintosh/mongojs/commit/195ffcefb52dba9cbbbd604754c86f8f56e0ae0f) Add standard test (@watson)
- [14d3e0c](https://github.com/mafintosh/mongojs/commit/14d3e0c3ee53159590599b0fd05f047c975ebeb6) Don't run subsequent tests if previous tests fail (@watson)
- [9924c3b](https://github.com/mafintosh/mongojs/commit/9924c3bec0946c389eda8993b83616e61c7ce2da) remove tip jar (@mafintosh)

### v1.1.0 (2015/07/25 08:39 +00:00)
- [975ec58](https://github.com/mafintosh/mongojs/commit/975ec58d109ea6355fa3f9ac8b4f91faaa67ed6d) 1.1.0 (@saintedlama)
- [7c4cad4](https://github.com/mafintosh/mongojs/commit/7c4cad497252e41efa24a926bbb941d5f031eccb) Close connection to test closing connections (@saintedlama)
- [d4bf755](https://github.com/mafintosh/mongojs/commit/d4bf7556f721c275277e6b8b9e4f6e4258ecab49) Remove unused require('each-series') (@saintedlama)
- [2f0c62b](https://github.com/mafintosh/mongojs/commit/2f0c62ba40f8e7742979c7992045823d4f822f1a) Remove superfluous ; (@saintedlama)
- [ec3ef7d](https://github.com/mafintosh/mongojs/commit/ec3ef7da50b0e051779ef33a002c73931b9c6c19) Fix naming and reference ScamSHA1 via mongodb.ScamSHA1 (@saintedlama)
- [#209](https://github.com/mafintosh/mongojs/pull/209) Merge pull request #209 from dustinblackman/auth_mechanisms (@dustinblackman)
- [5d96ebb](https://github.com/mafintosh/mongojs/commit/5d96ebbd2ec5b54c69af3377a5d8b1d46b2711d3) Split set upsert to true and return this for readability (@saintedlama)
- [#213](https://github.com/mafintosh/mongojs/pull/213) Merge pull request #213 from Avengis/master (@Avengis)
- [2bcbed3](https://github.com/mafintosh/mongojs/commit/2bcbed3262a8d8da6e58dd697c0cfcc421e39ad2) Added tests for upsert() method (@Avengis)
- [70d6bc5](https://github.com/mafintosh/mongojs/commit/70d6bc5a7b77fa195d61a30dd51843c48dbcd06b) Add aggregation pipeline breaking changes to Upgrading from 0.x.x to 1.0.x (@saintedlama)
- [772dff2](https://github.com/mafintosh/mongojs/commit/772dff2d569ec343416318f942617d34dd65df3b) Add `npm run geotag` script (@watson)
- [e1157b0](https://github.com/mafintosh/mongojs/commit/e1157b04628d83f41b3e2ca3710c2cdec89a7dd8) Add "Upgrading from 0.x.x to 1.0.x" section (@saintedlama)
- [c9025bb](https://github.com/mafintosh/mongojs/commit/c9025bb6ff0c9c72f462fd3fe0d8f405277d0e5d) add support for SCRAM-SHA-1 auth mechanism. (@dustinblackman)
- [d467340](https://github.com/mafintosh/mongojs/commit/d46734016f3da23538df41c9bdaf685a6fd53e93) Fix harmony tests and coverage commands by adding --harmony-proxies flag to enable Proxy functionality (@saintedlama)
- [#204](https://github.com/mafintosh/mongojs/pull/204) Merge pull request #204 from papajuans/master (@papajuans)
- [fa90791](https://github.com/mafintosh/mongojs/commit/fa90791684ec30c9d3e18450572867efcf8d956d) Add "npm run cover" command using istanbul for coverage and ignore coverage dir (@saintedlama)

### v1.0.2 (2015/06/27 15:47 +00:00)
- [1d6bbf2](https://github.com/mafintosh/mongojs/commit/1d6bbf2485f788b008eefa9f8b107f79330f829f) 1.0.2 (@watson)
- [0b01039](https://github.com/mafintosh/mongojs/commit/0b0103964028c7e00cdcafcede08d2cac0b19761) Test against Node.js 0.12 instead of 0.11 on Travis CI (@watson)
- [4899908](https://github.com/mafintosh/mongojs/commit/4899908ce6bb685d00825fcf0e244b4fd84c51e6) Use cursor.kill instead of cursor.close (@shakefu)
- [030d585](https://github.com/mafintosh/mongojs/commit/030d585161e6e6454723722550813f0729a939ab) Update to latest mongodb-core. (@shakefu)
- [aebc43c](https://github.com/mafintosh/mongojs/commit/aebc43cdddda481967f3527fb1cf2036a76ab9c2) Use Number.MAX_VALUE instead of -1 for tailable cursor retries. (@shakefu)
- [63a4b7b](https://github.com/mafintosh/mongojs/commit/63a4b7bce9af260877485faa0486fb620907eb56) Test all branches on Travis-CI (@watson)
- [453b522](https://github.com/mafintosh/mongojs/commit/453b5229811bb8112f336a89c9964d52ed89ae7c) Use SVG build status from travis master branch builds (@saintedlama)
- [#1](https://github.com/mafintosh/mongojs/pull/1) Merge pull request #1 from Avengis/Avengis-patch-1 (@Avengis)
- [15c053b](https://github.com/mafintosh/mongojs/commit/15c053b9ba345222b72c1c771273ed91b29117f7) Update bulk.js (@Avengis)
- [#203](https://github.com/mafintosh/mongojs/pull/203) Merge pull request #203 from saintedlama/fix-ensure-index (@saintedlama)
- [7dd97fd](https://github.com/mafintosh/mongojs/commit/7dd97fdd78e1e666695accabd0f10dc499a9a76e) Allow array-base aggregation pipelines (@papajuans)
- [9eae343](https://github.com/mafintosh/mongojs/commit/9eae343f413135ee1ee5139e40f39afb2fbda050) Add check for cb undefined to prevent calls to ensureIndex with index field and options given but without cb throw an error (@saintedlama)

### v1.0.1 (2015/06/16 12:23 +00:00)
- [540f561](https://github.com/mafintosh/mongojs/commit/540f561f194f745409c44661916ecc1d41dbb197) 1.0.1 (@sorribas)
- [#198](https://github.com/mafintosh/mongojs/pull/198) Merge pull request #198 from shakefu/master (@shakefu)
- [4443c94](https://github.com/mafintosh/mongojs/commit/4443c94b27d1b6ca99d992657c4e19a10700e8c0) Update mongodb-core patch level. (@shakefu)

### v1.0.0 (2015/06/10 18:04 +00:00)
- [e1373bc](https://github.com/mafintosh/mongojs/commit/e1373bc80169de5cc713713dcd4f752c5107f025) 1.0.0 (@sorribas)
- [bf9b801](https://github.com/mafintosh/mongojs/commit/bf9b80196deffa414a98bf5fe40b24d5e478e03f) Update travis to use recent mongodb versions and iojs. (@sorribas)
- [#194](https://github.com/mafintosh/mongojs/pull/194) Merge pull request #194 from mcollina/tailable (@mcollina)
- [#195](https://github.com/mafintosh/mongojs/pull/195) Merge pull request #195 from lpinca/add/license-field (@lpinca)
- [ab66cc9](https://github.com/mafintosh/mongojs/commit/ab66cc9422f0275dcbfba61ef40e9d1548ec21fb) Add license field to package.json (@lpinca)
- [d820996](https://github.com/mafintosh/mongojs/commit/d820996ce515eecf4bf9bb9dbf676b819c60dc81) Added back tailable cursor support. (@mcollina)

### v1.0.0-beta4 (2015/05/02 18:54 +00:00)
- [5a60466](https://github.com/mafintosh/mongojs/commit/5a604665a0cac48292bfdff571290c963b370f10) 1.0.0-beta4 (@sorribas)
- [63496e8](https://github.com/mafintosh/mongojs/commit/63496e8075216dee40e897b682582552d67c3bd8) Expose ObjectId in module. (@sorribas)

### v0.17.1 (2015/05/02 18:52 +00:00)
- [#188](https://github.com/mafintosh/mongojs/pull/188) Merge pull request #188 from prabhu/code_cleanup (@prabhu)
- [0c5698b](https://github.com/mafintosh/mongojs/commit/0c5698b5c507503916fea867d60f6e0684775640) Removed unused noop
- [c1d9449](https://github.com/mafintosh/mongojs/commit/c1d9449d85af939cc989106581bf09e81e33beab) Cleanup. Removed unused vars and imports
- [67235a3](https://github.com/mafintosh/mongojs/commit/67235a3ae1e1d57d7404b5c13ce84f900c02c2b9) Test on io.js (@sorribas)

### v1.0.0-beta3 (2015/03/21 20:23 +00:00)
- [62877cc](https://github.com/mafintosh/mongojs/commit/62877ccfa7e979375d839f30699c09448900c8de) 1.0.0-beta3 (@sorribas)
- [f279cbb](https://github.com/mafintosh/mongojs/commit/f279cbbb01d6ef3cd462006d22ce9fca8ebf004f) Always use readable-stream. (@sorribas)

### v1.0.0-beta2 (2015/03/21 20:21 +00:00)
- [9f8dda2](https://github.com/mafintosh/mongojs/commit/9f8dda24b72dbbe7d306ffb00d84455a77e9dde4) 1.0.0-beta2 (@sorribas)
- [4291eec](https://github.com/mafintosh/mongojs/commit/4291eececd2e54ca6ae810e079bca6a40e3abcac) Update deps. (@sorribas)
- [c9f5d92](https://github.com/mafintosh/mongojs/commit/c9f5d92e8e83f6c376c0bd1fefadfa6c77dfd993) Fix foreach. (@sorribas)
- [a27cdcc](https://github.com/mafintosh/mongojs/commit/a27cdcc7fae8e6bc98e3c4fff8b9e7c5429f870d) Check for last error on foreach. (@sorribas)
- [23c1a82](https://github.com/mafintosh/mongojs/commit/23c1a829d1d630aec12afad64a8e221d00cc6e2c) Remove unused dependency and stop using cursor._apply. (@sorribas)

### v1.0.0-beta1 (2015/03/21 19:24 +00:00)
- [208a43d](https://github.com/mafintosh/mongojs/commit/208a43d4c0cc10469fe36c6acb97b6f739f5bab3) 1.0.0-beta1 (@sorribas)
- [a167c18](https://github.com/mafintosh/mongojs/commit/a167c18b68a8e574a57667497f7e36cd320f8cbd) Add some docs for 1.0 with mongodb 2.4 (@sorribas)
- [0324967](https://github.com/mafintosh/mongojs/commit/0324967490a36b2d8d690561471d01da875d1c2e) mongodb-core rewrite. (@sorribas)

### v0.18.2 (2015/03/02 12:15 +00:00)
- [9768651](https://github.com/mafintosh/mongojs/commit/9768651a728f0f0a45af87527d8749c839a328c0) 0.18.2 (@sorribas)
- [#182](https://github.com/mafintosh/mongojs/pull/182) Merge pull request #182 from saintedlama/master (@saintedlama)
- [eef59fd](https://github.com/mafintosh/mongojs/commit/eef59fd7de2f642d2abe5e6da3f2e4b8dc37514a) Update to mongodb 1.4.32 (@saintedlama)
- [#177](https://github.com/mafintosh/mongojs/pull/177) Merge pull request #177 from watson/patch-1 (@watson)
- [536c14e](https://github.com/mafintosh/mongojs/commit/536c14eeeda1b676d8c33836ebdb7f90a620a1d9) Change Travis-CI badge to only show master status (@watson)
- [a598537](https://github.com/mafintosh/mongojs/commit/a598537e3e44cc182e4d31810c842b855d3a1272) Allow travis builds for other branches. (@sorribas)

### v0.18.1 (2015/01/17 15:11 +00:00)
- [78ee4fc](https://github.com/mafintosh/mongojs/commit/78ee4fc674135a5e70b43fae5fc62137f00b1687) 0.18.1 (@sorribas)
- [0cddc6e](https://github.com/mafintosh/mongojs/commit/0cddc6eec1cd95bf641e831a2ede5408d36d49a2) Allow to call bulk.update() without callback. Fixes #166. (@sorribas)
- [d0ab7b2](https://github.com/mafintosh/mongojs/commit/d0ab7b28e2bab78ec66f2f8aff890d2d63738adb) Add docs for readPref, Fixes #165 (@sorribas)

### v0.18.0 (2014/12/09 17:20 +00:00)
- [e760c80](https://github.com/mafintosh/mongojs/commit/e760c809a0c7827b5056c5f58a4c9c61c3d78c5c) 0.18.0 (@sorribas)
- [35018a7](https://github.com/mafintosh/mongojs/commit/35018a7ee10e853800cf0225917899054335c9f0) added cursor.readPref. (@sorribas)
- [37602dd](https://github.com/mafintosh/mongojs/commit/37602ddec8118eebd8fe2673cd680ddbf778420d) Add test for mapReduce. (@sorribas)
- [270d195](https://github.com/mafintosh/mongojs/commit/270d1958a6d4449b607419d50c4ff699d33a1c20) Add some more docs to the distinct test. (@sorribas)
- [2a52649](https://github.com/mafintosh/mongojs/commit/2a526492465457967a41a49a63488b753a84f1bb) Fix example indentiation style. (@sorribas)
- [#160](https://github.com/mafintosh/mongojs/pull/160) Merge pull request #160 from longbill/master (@longbill)
- [34c5315](https://github.com/mafintosh/mongojs/commit/34c5315989cc94c63d4111919452f1d09e9306ee) update readme (@longbill)
- [9ac4ff6](https://github.com/mafintosh/mongojs/commit/9ac4ff6f21a8e532223ed4ed9c355723c12bda24) update readme (@longbill)
- [38469ec](https://github.com/mafintosh/mongojs/commit/38469ec0d03880d3e13d7a991b010a3eb0d9459f) Added test for cursor.count. (@sorribas)
- [bf75333](https://github.com/mafintosh/mongojs/commit/bf75333d4700b26a6a1181c209e6288bb2b38954) Add test for cursor.rewind. (@sorribas)
- [e7b0bcc](https://github.com/mafintosh/mongojs/commit/e7b0bccfdbdba2ebe2e8ea67351e8a9734bdbb64) Test for cursor.forEach (@sorribas)
- [5c571ef](https://github.com/mafintosh/mongojs/commit/5c571ef8651e90b2888bde3b50720de8d74b771b) Add sort test. (@sorribas)
- [18f6145](https://github.com/mafintosh/mongojs/commit/18f6145e1b99518b98aeb59c8f08a34ecbb5257d) Only test on master. (@sorribas)
- [ff8d119](https://github.com/mafintosh/mongojs/commit/ff8d11966e79d99cf1477a5f8547a1b5804d208a) drop 0.8 support. (@sorribas)

### v0.17.0 (2014/11/07 15:34 +00:00)
- [6646401](https://github.com/mafintosh/mongojs/commit/6646401d11b8da4c51752db718b48b347c0dd13b) 0.17.0 (@sorribas)
- [9d01685](https://github.com/mafintosh/mongojs/commit/9d01685ce2e33663cb0cb192b96a973bd69e26d8) Add dropIndexes. (@sorribas)
- [17d4be5](https://github.com/mafintosh/mongojs/commit/17d4be5b8c8b3be124a1a2e6ee1f7e67d202f59e) Add test for dropIndexes. (@sorribas)
- [b793b4d](https://github.com/mafintosh/mongojs/commit/b793b4d010dc8b2ab3873678bb5dad5a1f19ce09) Add test for aggregate. (@sorribas)

### v0.16.0 (2014/11/07 15:20 +00:00)
- [c491e0f](https://github.com/mafintosh/mongojs/commit/c491e0fef9f1e8c6d8e94374554b7b39390ef378) 0.16.0 (@sorribas)
- [6d331ce](https://github.com/mafintosh/mongojs/commit/6d331ce09d5d022f8ed0ead16b2e0206bbce4eb0) Make aggregate return a stream. Fixes #154. (@sorribas)
- [c533e5a](https://github.com/mafintosh/mongojs/commit/c533e5a25d7343ef9b2741730548bb8b90f7922a) Bump driver. (@sorribas)
- [ae77aa6](https://github.com/mafintosh/mongojs/commit/ae77aa66f4c3f77d6c489ed818f1adfd23949112) Remove toJSON function (@sorribas)

### v0.15.1 (2014/10/05 16:07 +00:00)
- [af4d245](https://github.com/mafintosh/mongojs/commit/af4d245108877af3caf355ac9d3a34ea0e68ac6e) 0.15.1 (@sorribas)
- [de4f9a4](https://github.com/mafintosh/mongojs/commit/de4f9a44b6c40dc6aa0b5e35b596a2e9731b63b1) Ignore bulk tests in case db version < 2.6 (travis). (@sorribas)

### v0.15.0 (2014/10/05 15:47 +00:00)
- [c3aeaff](https://github.com/mafintosh/mongojs/commit/c3aeaff6f8425a6f6de5b06547574d2c718777dd) 0.15.0 (@sorribas)
- [76ecb43](https://github.com/mafintosh/mongojs/commit/76ecb43029e19407b41e4b2a3cc25d5d280812f8) Bump driver. (@sorribas)
- [e708924](https://github.com/mafintosh/mongojs/commit/e708924d24e399bb266df349718f86d6cdb5aedc) Emit error on connection error. Closes #149 (@sorribas)
- [d52e1ea](https://github.com/mafintosh/mongojs/commit/d52e1eabe168aa2f97bd42f17d494c1c6b64e8e0) Docs for bulk updates (@sorribas)
- [a025aa2](https://github.com/mafintosh/mongojs/commit/a025aa238fa35e02b475f10c0e1cdf6649d7743e) Add support for bulk updates. Refs #152 (@sorribas)

### v0.14.2 (2014/09/26 12:23 +00:00)
- [13444fe](https://github.com/mafintosh/mongojs/commit/13444fec1cc481d772b0c23e301289b2f5691286) 0.14.2 (@sorribas)
- [43db686](https://github.com/mafintosh/mongojs/commit/43db686c8643025108e6ac864a83ce1a194640f9) Bump mongodb. (@sorribas)
- [02fd31c](https://github.com/mafintosh/mongojs/commit/02fd31cc652c93e8976d15243f49b6c98f0e43f6) Update docs. (@sorribas)
- [e3e8bcf](https://github.com/mafintosh/mongojs/commit/e3e8bcf58c300a7e9d44b2fd63c8016280dca3ab) Add gratipay. (@sorribas)
- [#150](https://github.com/mafintosh/mongojs/pull/150) Merge pull request #150 from countable/master (@countable)
- [9893b71](https://github.com/mafintosh/mongojs/commit/9893b71aa40125d186a0142c95130c88e9e7d69d) test for distinct (@countable)

### v0.14.1 (2014/08/28 16:24 +00:00)
- [952f504](https://github.com/mafintosh/mongojs/commit/952f504fcdd25da6b03613d0d8f7c3be35df33a5) 0.14.1 (@sorribas)
- [4a73373](https://github.com/mafintosh/mongojs/commit/4a733739706cb149683aec1154b4fbda3468d318) Bump driver. (@sorribas)
- [03b90eb](https://github.com/mafintosh/mongojs/commit/03b90eb54db911b5315d23b40d0fc9caa99fa6f1) Fix tests for 0.8. (@sorribas)
- [abab80b](https://github.com/mafintosh/mongojs/commit/abab80b4c29f81dbcbf313eadfb70dc143af84aa) Refactor tests so you can run them individually and they exit. (@sorribas)
- [#147](https://github.com/mafintosh/mongojs/pull/147) Merge pull request #147 from watson/patch-2 (@watson)
- [ccdf216](https://github.com/mafintosh/mongojs/commit/ccdf2168d69faf3d97fac8b18d6f94395a0174d6) Add cursor API docs for .rewind() and .destroy() (@watson)

### v0.14.0 (2014/08/20 20:25 +00:00)
- [2edc57e](https://github.com/mafintosh/mongojs/commit/2edc57ef40af0f86693d610b37aaf4255c6a978e) 0.14.0 (@sorribas)
- [f1ded41](https://github.com/mafintosh/mongojs/commit/f1ded41d579c378f6b746e854deb3f9ffc5091e4) Minor test refactor. (@sorribas)
- [ebb6b02](https://github.com/mafintosh/mongojs/commit/ebb6b02c9ba54dc6e3e79152901f7496404aab26) Update docs. (@sorribas)
- [94622be](https://github.com/mafintosh/mongojs/commit/94622bec0c3fb7aafae1b5dcfec2dd2fa868f4f8) If we receive a mongojs instance we connect and recreate the instance, (@sorribas)
- [940dff5](https://github.com/mafintosh/mongojs/commit/940dff501812d7fc688b38263c153a468fc57fc4) Add support to pass a driver db or a mongojs db instead of the connection string. (@sorribas)
- [#146](https://github.com/mafintosh/mongojs/pull/146) Merge pull request #146 from watson/patch-1 (@watson)
- [b935e74](https://github.com/mafintosh/mongojs/commit/b935e74a14be6bcdde40eec78147be3359cf0a4e) Add API documentation for db.close() (@watson)
- [b5c140c](https://github.com/mafintosh/mongojs/commit/b5c140c14ec2d209c04301d9f73f5202a0bd5cc8) ocd. (@sorribas)
- [79319b4](https://github.com/mafintosh/mongojs/commit/79319b42a2c6c2cee675bfc3a9fbd40e437cdedd) Fix api docs for getCollectionNames. Refs #54 (@sorribas)
- [d42d7a0](https://github.com/mafintosh/mongojs/commit/d42d7a0c3cb3a92c0131e21db59ee3561200d0e2) Restructure the group function to multiple lines. (@sorribas)
- [b2f3bbd](https://github.com/mafintosh/mongojs/commit/b2f3bbdf9201f98e353a59ed48edfd724068c3d2) Fix travis. (@sorribas)
- [e560204](https://github.com/mafintosh/mongojs/commit/e560204bf9549394eccd59e59e443529945dd9c5) Refactor tests to use tape. (@sorribas)
- [f46c14e](https://github.com/mafintosh/mongojs/commit/f46c14e19c4367e7a080c7497ec2bb1b7c8d99ae) Give me some space. (@sorribas)
- [a16dd33](https://github.com/mafintosh/mongojs/commit/a16dd33e2c2b592f129f9d760554397ddce606e7) Minor refactor. (@sorribas)

### v0.13.1 (2014/07/25 15:03 +00:00)
- [83d9344](https://github.com/mafintosh/mongojs/commit/83d93445af87a473ee87c0c28da2ef975dbd6f39) 0.13.1 (@sorribas)
- [da252d9](https://github.com/mafintosh/mongojs/commit/da252d98e2baaa247b7d58d452e1326a00f57722) Stop using err.lastErrorObject (it's not in the driver anymore). (@sorribas)
- [f487584](https://github.com/mafintosh/mongojs/commit/f487584c91dd01b309b55a58183f2430ebec7975) bump driver. (@sorribas)
- [8e77037](https://github.com/mafintosh/mongojs/commit/8e77037de55c8f15a9cc7dd2bbf102ba115b89b6) revert bump (@mafintosh)
- [1cbaeb2](https://github.com/mafintosh/mongojs/commit/1cbaeb2cc0be9f9610d8a498cba20ca633780153) bump driver (@mafintosh)
- [#137](https://github.com/mafintosh/mongojs/pull/137) Merge pull request #137 from amaurymedeiros/patch-1 (@amaurymedeiros)
- [c194b12](https://github.com/mafintosh/mongojs/commit/c194b1214641b67786028debf055f96f46985413) Update README.md (@amaurymedeiros)
- [b35a744](https://github.com/mafintosh/mongojs/commit/b35a744942424e3f315e075896a8705f09455251) more harmony docs (@mafintosh)

### v0.13.0 (2014/04/26 17:31 +00:00)
- [fd608b1](https://github.com/mafintosh/mongojs/commit/fd608b12b72146cf79594cb45c3649b2f3e3927d) 0.13.0 (@sorribas)
- [8a6fa48](https://github.com/mafintosh/mongojs/commit/8a6fa48080bc1166dfeb8267ec7a03d70ac31676) Document the harmony proxy feature. (@sorribas)
- [c6e8f5c](https://github.com/mafintosh/mongojs/commit/c6e8f5c6cf82b0acacc592f7ca121fe71c4718f5) Collection proxy with harmony. (@sorribas)
- [c62133a](https://github.com/mafintosh/mongojs/commit/c62133a80ea110bfba97ccdc3696da9e0fc8d8c6) Run both with and without --harmony on every node version. (@sorribas)
- [1aeaba2](https://github.com/mafintosh/mongojs/commit/1aeaba2902e9718fb0a49cd7cd94bb50316e345c) Add node 0.11 to travis. (@sorribas)

### v0.12.1 (2014/04/19 08:06 +00:00)
- [42fecf6](https://github.com/mafintosh/mongojs/commit/42fecf6330b6fb6a90ddb1745d8ca164eaa2c8f7) 0.12.1 (@mafintosh)
- [edaae8f](https://github.com/mafintosh/mongojs/commit/edaae8f39320b177429fe978210917502f363667) tweak docs for #135 (@mafintosh)
- [20e4b33](https://github.com/mafintosh/mongojs/commit/20e4b33a9580d6c8f95fea8845be5a0a986815e7) ensure optional callbacks for write ops. cc #135 (@mafintosh)
- [d2be4b9](https://github.com/mafintosh/mongojs/commit/d2be4b93ce37cc355fb0e3e5d1de8112db4a5558) added test for optional callbacks. cc #135 (@mafintosh)

### v0.12.0 (2014/04/16 14:32 +00:00)
- [e816698](https://github.com/mafintosh/mongojs/commit/e8166987ed1177c9f2c170808b97cc869f9d130a) 0.12.0 (@sorribas)
- [2bdd19b](https://github.com/mafintosh/mongojs/commit/2bdd19b44e97925a75b051273a9fae38adcd8a5e) Stop inhereting collection prototype methods. Fixes #132. (@sorribas)
- [809252c](https://github.com/mafintosh/mongojs/commit/809252cd0ea24f5cbe614ac1a2d82547025a77d9) Stop inhereting db prototype methods. Refs #132. (@sorribas)

### v0.11.1 (2014/04/09 17:08 +00:00)
- [eb5ab13](https://github.com/mafintosh/mongojs/commit/eb5ab133a876222897a3de062b86466c798dee62) 0.11.1 (@sorribas)
- [536743f](https://github.com/mafintosh/mongojs/commit/536743fe89e213e6d1ee0b570ecdd30888af75fd) Rename prototypes. (@sorribas)
- [a802934](https://github.com/mafintosh/mongojs/commit/a802934cfa46d7e4569b506d7d363bfad14b2c82) Change cursor appply method to support mongo driver 1.4.0. Refs #126 #105 (@sorribas)
- [bc4f031](https://github.com/mafintosh/mongojs/commit/bc4f0310141285a96235a847b0b8245fd97cb89a) Update docs. All implemented functions are now included. (@sorribas)
- [cb3dec2](https://github.com/mafintosh/mongojs/commit/cb3dec2966cc44aef351ec478717d9abe0bcb720) First version of API documentation. (@sorribas)

### v0.11.0 (2014/04/01 20:29 +00:00)
- [a1f9641](https://github.com/mafintosh/mongojs/commit/a1f964185ba180d571254b9b9ca888004f83c4da) 0.11.0 (@sorribas)
- [20cf5ee](https://github.com/mafintosh/mongojs/commit/20cf5eeb4a0bce82fc1ce7682a3b7cd3d327966f) Add support for cursor.rewind. Closes #131 (@sorribas)
- [4de6a44](https://github.com/mafintosh/mongojs/commit/4de6a44805328cffa31f2f2d94cf0e1a78c29745) Add the cursor.size method (@sorribas)
- [8ca0ec2](https://github.com/mafintosh/mongojs/commit/8ca0ec288ea53a0b0f90ad95eaf6550a140aa17d) Update license date range (@sorribas)
- [d1436ff](https://github.com/mafintosh/mongojs/commit/d1436ff0847a89871efcc27a1b8ff7744d811806) Add missing semicolon (@sorribas)
- [#128](https://github.com/mafintosh/mongojs/pull/128) Merge pull request #128 from naman34/patch-1 (@naman34)
- [38bef2e](https://github.com/mafintosh/mongojs/commit/38bef2e36f029385682fb9667f7cd42bde92d566) Update License to year range (@nmn)
- [a3e50ef](https://github.com/mafintosh/mongojs/commit/a3e50ef13b42c2b6d9874beb1a3e07ac767098b6) Add the cursor.map function (@sorribas)

### v0.10.1 (2014/03/04 10:37 +00:00)
- [5d49b11](https://github.com/mafintosh/mongojs/commit/5d49b1166329cb29392de72f1401b847e043c252) 0.10.1 (@mafintosh)
- [#125](https://github.com/mafintosh/mongojs/pull/125) Merge pull request #125 from watson/patch1 (@watson)
- [649647c](https://github.com/mafintosh/mongojs/commit/649647c98eeef7a8b95a879f6c4a93f1a86bb8e9) Extract lastErrorObject from the err argument if findAndModify fails (@watson)

### v0.10.0 (2014/01/15 22:47 +00:00)
- [1f7d0f6](https://github.com/mafintosh/mongojs/commit/1f7d0f6e405fb7f8175945d54ab7c2a633f1539e) v0.10.0 (@mafintosh)
- [a6a8f14](https://github.com/mafintosh/mongojs/commit/a6a8f149703fbe97ae6f8d324aaea7405d78f13a) Fix the remove callback parameters. (@sorribas)
- [0f95a38](https://github.com/mafintosh/mongojs/commit/0f95a380f440513eaea8495c2b453f3b3c683c51) lastErrorObject on all the write functions. (@sorribas)
- [6ff4158](https://github.com/mafintosh/mongojs/commit/6ff4158a7c76b79e140a41bbe19cc0a224a2217e) Add missing error handling (@sorribas)
- [#117](https://github.com/mafintosh/mongojs/pull/117) Merge pull request #117 from kapetan/upstream (@kapetan)
- [b07daa7](https://github.com/mafintosh/mongojs/commit/b07daa7d50d6109711eb1fd7c9cb0511323baa7d) Updated README with lastErrorObject (@kapetan)
- [#116](https://github.com/mafintosh/mongojs/pull/116) Merge pull request #116 from kapetan/upstream (@kapetan)
- [c3b43a9](https://github.com/mafintosh/mongojs/commit/c3b43a985286a92babf5a97c0c3762e14bee0f39) Removed debug code (@kapetan)
- [27ad374](https://github.com/mafintosh/mongojs/commit/27ad374fa3ad33c2b2b05842b49cf6089ee5fac8) Change the insert callback to make it more intuitive. (@sorribas)
- [873cf5d](https://github.com/mafintosh/mongojs/commit/873cf5d2112ef2ebd7dd14702ea4f4c13f88ae2f) Add the lastErrorObject to the .save callback. Now the callbacks are as following. (@sorribas)
- [6dd7b4e](https://github.com/mafintosh/mongojs/commit/6dd7b4ef02f79dbd06dfad349cabc3fa8b1e9b4c) Add a remove statement to the insert test case. (@sorribas)
- [1c1dbd5](https://github.com/mafintosh/mongojs/commit/1c1dbd501dc444e663d99ba3380b9688728ca568) Change normalized callback arguments. (@sorribas)
- [#114](https://github.com/mafintosh/mongojs/pull/114) Merge pull request #114 from kapetan/upstream (@kapetan)
- [014b5d1](https://github.com/mafintosh/mongojs/commit/014b5d17c2cb56c6b760420a1d434ffec8ba969f) Normalize lastErrorObject (@kapetan)
- [3e0fa8c](https://github.com/mafintosh/mongojs/commit/3e0fa8c8a5fec108a755f0282b5ab97fbe513b64) Normalize callback arguments. Same as shell. (@kapetan)

### v0.9.11 (2013/12/25 18:50 +00:00)
- [4898d82](https://github.com/mafintosh/mongojs/commit/4898d8261fbee8aa376fef6ba7c4b8657d27839f) v0.9.11 (@mafintosh)
- [#113](https://github.com/mafintosh/mongojs/pull/113) Merge pull request #113 from kapetan/upstream (@kapetan)
- [fa37e1f](https://github.com/mafintosh/mongojs/commit/fa37e1f486117bdcf6edf45591fbe68aba21bee9) Fix query included in database name (@kapetan)

### v0.9.10 (2013/12/16 12:55 +00:00)
- [00d7134](https://github.com/mafintosh/mongojs/commit/00d7134b3e4319ecb91fa7f9dac138e76e96459f) v0.9.10 (@mafintosh)
- [80bc3eb](https://github.com/mafintosh/mongojs/commit/80bc3eb75c724aa383315322d4b2bd5295f435d8) added toString for database and collection (@mafintosh)

### v0.9.9 (2013/12/10 16:35 +00:00)
- [bcf33f6](https://github.com/mafintosh/mongojs/commit/bcf33f6a3cd1965cdad468eb3ab1dff26d25ba0e) v0.9.9 (@mafintosh)
- [dde909c](https://github.com/mafintosh/mongojs/commit/dde909c1f727237dadc5ade0d760c33249083104) bumping deps (@mafintosh)

### v0.9.8 (2013/11/22 20:57 +00:00)
- [0d64457](https://github.com/mafintosh/mongojs/commit/0d644576c01f4a0b9918b9433ca122742aeb3e52) v0.9.8 (@mafintosh)
- [a04f59f](https://github.com/mafintosh/mongojs/commit/a04f59f367d9f1096d4caa7639707741a41bec9e) shrinkwrapping mongodb to 1.3.19. fixes #105 (@mafintosh)

### v0.9.7 (2013/11/20 22:24 +00:00)
- [1bd9091](https://github.com/mafintosh/mongojs/commit/1bd909104512f5d8e8b9d580cd76d501c213bbbe) v0.9.7 (@mafintosh)
- [06bbf02](https://github.com/mafintosh/mongojs/commit/06bbf02b672d71f5d8ffc3a9e7efa920e522da50) expose bson types visible in the shell using the shell names. fixes #99 (@mafintosh)
- [#101](https://github.com/mafintosh/mongojs/pull/101) Merge pull request #101 from sorribas/master (@sorribas)
- [fde3f56](https://github.com/mafintosh/mongojs/commit/fde3f56ef60d2d4dac38fd3dae225362d9f58ecf) Avoid getIndexes crash when called with no parameters. (@sorribas)
- [#98](https://github.com/mafintosh/mongojs/pull/98) Merge pull request #98 from RG72/patch-1 (@RG72)
- [0a637ff](https://github.com/mafintosh/mongojs/commit/0a637ffb9320bd32ee5a8f0f7ce24b32941ae24f) index.js Emit ready event, when db connected (@RG72)

### v0.9.6 (2013/09/22 02:17 +00:00)
- [d1e8c0d](https://github.com/mafintosh/mongojs/commit/d1e8c0d4afdb42505b520069c61dc5fbf10ee737) v0.9.6 (@mafintosh)
- [d91831f](https://github.com/mafintosh/mongojs/commit/d91831f5b1134eccb44d20c230fec1f744e3d0f6) always closing in shutdown. see #93 (@mafintosh)

### v0.9.5 (2013/09/18 21:20 +00:00)
- [b05544b](https://github.com/mafintosh/mongojs/commit/b05544b74a34466ea24b6369bfbd7c411c417142) v0.9.5 (@mafintosh)
- [172deed](https://github.com/mafintosh/mongojs/commit/172deed5474a367726b8dceb4abc4e01587864e6) minor style tweaks (@mafintosh)
- [#93](https://github.com/mafintosh/mongojs/pull/93) Merge pull request #93 from sorribas/master (@sorribas)
- [1919c31](https://github.com/mafintosh/mongojs/commit/1919c310574b6d82bdab397b701c97953331a7c8) Manage the sutdown command. (@sorribas)
- [#90](https://github.com/mafintosh/mongojs/pull/90) Merge pull request #90 from james-gibson/patch-1 (@james-gibson)
- [7db0d89](https://github.com/mafintosh/mongojs/commit/7db0d89c88c427df5a7615ec4bde913e4d9596f6) Modified 'result' to 'res' to follow the example conventions used in the rest of the document
- [1d6475d](https://github.com/mafintosh/mongojs/commit/1d6475d95a2273814b165f05748d3025d7ab96c3) Reordered examples (@mafintosh)
- [eabccce](https://github.com/mafintosh/mongojs/commit/eabcccebc14068237a309cc2c48c14ccfc4fd354) Fixed long line (@mafintosh)
- [067066c](https://github.com/mafintosh/mongojs/commit/067066c069d9ab9033ce3c4254f635cde59bd7f3) ObjectId example. Fixes #89 (@mafintosh)

### v0.9.4 (2013/09/11 08:58 +00:00)
- [ad197b3](https://github.com/mafintosh/mongojs/commit/ad197b36ec8b348f6aee806ebc1eb3e775a76685) v0.9.4 (@mafintosh)
- [#88](https://github.com/mafintosh/mongojs/pull/88) Merge pull request #88 from sorribas/master (@sorribas)
- [89c489d](https://github.com/mafintosh/mongojs/commit/89c489d07c3daf1bc87faf6b483b3284a9ab9327) Merge remote-tracking branch 'upstream/master' (@sorribas)
- [eaae470](https://github.com/mafintosh/mongojs/commit/eaae470529063ecc42427c8b176347d5dc773757) Refactor test insert code to use the db.col.insert() function. (@sorribas)
- [#85](https://github.com/mafintosh/mongojs/pull/85) Merge pull request #85 from sorribas/master (@sorribas)
- [128f30c](https://github.com/mafintosh/mongojs/commit/128f30c2ae636add4844b348024a5f49c314e1bb) Add test for cursor explain (@sorribas)
- [1083ba0](https://github.com/mafintosh/mongojs/commit/1083ba006cab992d465cf6fb68dc25586eadac46) Delete unnecessary(and ugly) semicolon. (@sorribas)
- [#83](https://github.com/mafintosh/mongojs/pull/83) Merge pull request #83 from sorribas/master (@sorribas)
- [335d926](https://github.com/mafintosh/mongojs/commit/335d926a150b9237afe180b56a01fcb8245854c8) Fix the link to the mongo native driver. (@sorribas)
- [6d2a96e](https://github.com/mafintosh/mongojs/commit/6d2a96edc7709ee32268968648e7f9b356de71f9) travis link updated (@mafintosh)

### v0.9.3 (2013/09/02 22:37 +00:00)
- [fa957f3](https://github.com/mafintosh/mongojs/commit/fa957f30611ec88891209c91ff487a32c98b3ed9) v0.9.3 (@mafintosh)
- [fdaa96c](https://github.com/mafintosh/mongojs/commit/fdaa96ce7754b353ea4e3a0b9ed8eb07e9ddee0a) added test for createCollection (@mafintosh)
- [8e9c97f](https://github.com/mafintosh/mongojs/commit/8e9c97f137ebf5bce2d9d7bd06cfda04b91e59e0) createCollection should throw if col exists. Fixes #44 (@mafintosh)
- [ae8259f](https://github.com/mafintosh/mongojs/commit/ae8259fa200beb1cb36ef3bf2aed203086bdad59) badge below npm notice (@mafintosh)
- [1747d6c](https://github.com/mafintosh/mongojs/commit/1747d6c8a1700e832f5977799c11637aa4e2518d) v0.9.2 (@mafintosh)
- [9e9f1bb](https://github.com/mafintosh/mongojs/commit/9e9f1bb1ada6bec074981c75e8d5dd69abc35a7d) more readme formatting (@mafintosh)
- [fd2f8bb](https://github.com/mafintosh/mongojs/commit/fd2f8bbf40b9dd4876f12833f98fa4b3bed69c4b) add 0.8 to travis (@mafintosh)
- [c9442f2](https://github.com/mafintosh/mongojs/commit/c9442f2868078258003f06b1aa1a6707966df975) more readme formatting (@mafintosh)

### v0.9.2 (2013/09/02 21:03 +00:00)
- [833bb0b](https://github.com/mafintosh/mongojs/commit/833bb0baed13f39675a722096195eadd4b1ba29b) moved badge to the top (@mafintosh)
- [eaf7959](https://github.com/mafintosh/mongojs/commit/eaf7959dcf2f390552253b9e0864bf5b66753e87) travis badge (@mafintosh)
- [31ee22b](https://github.com/mafintosh/mongojs/commit/31ee22bd1f3db7763803b7396cc23dc8c8d6020c) added travis (@mafintosh)

### v0.9.1 (2013/09/02 14:21 +00:00)
- [9a29e86](https://github.com/mafintosh/mongojs/commit/9a29e86b2fdd9324b2e82843d89c34052b321020) v0.9.1 (@mafintosh)
- [534580d](https://github.com/mafintosh/mongojs/commit/534580d0240093f099728891be9d9fbaaf99445f) moved repository to mafintosh (@mafintosh)
- [#82](https://github.com/mafintosh/mongojs/pull/82) Merge pull request #82 from sorribas/master (@sorribas)
- [e3f6990](https://github.com/mafintosh/mongojs/commit/e3f69902bfaebc283259d216d2cac205f484c772) Add test for chained collection names (@sorribas)
- [f65a1e8](https://github.com/mafintosh/mongojs/commit/f65a1e8a5d7dd99192850dc7654e833e055d520e) avoiding another scrollbar in docs (@mafintosh)
- [c0382ea](https://github.com/mafintosh/mongojs/commit/c0382eaa2a4d924a20a78441f1f83da8dac834dc) avoiding scrollbar in docs (@mafintosh)

### v0.9.0 (2013/08/31 17:31 +00:00)
- [70a0cba](https://github.com/mafintosh/mongojs/commit/70a0cba10fc8132774c4eaaf890561dce4696827) v0.9.0 (@mafintosh)
- [0e31101](https://github.com/mafintosh/mongojs/commit/0e311019a89a652d41f968e88febb57dc2ad818f) support for chained col names in col array. fixes #42 (@mafintosh)

### v0.8.1 (2013/08/31 15:37 +00:00)
- [c0e0bba](https://github.com/mafintosh/mongojs/commit/c0e0bba7931dae6888105c2c75a75d6844eeea17) v0.8.1 (@mafintosh)
- [62cafcc](https://github.com/mafintosh/mongojs/commit/62cafcc28541ef76bbea7a240594a00355fe1766) updated dependencies (@mafintosh)

### v0.8.0 (2013/08/31 15:19 +00:00)
- [4db58e6](https://github.com/mafintosh/mongojs/commit/4db58e6bf4c0aa44dc0b2904ec45717e7fee6ae6) v0.8.0 (@mafintosh)
- [2ec9b9b](https://github.com/mafintosh/mongojs/commit/2ec9b9bf1670aaabc02ca3c17d70a0dead6a3d7a) added .open and some comments (@mafintosh)
- [#81](https://github.com/mafintosh/mongojs/pull/81) Merge pull request #81 from sorribas/master (@sorribas)
- [66ae6a1](https://github.com/mafintosh/mongojs/commit/66ae6a1b0c5014e7e1b2c096dca2c7addca6bc2b) Fix runCommand() bugs. (@sorribas)
- [b35dd5a](https://github.com/mafintosh/mongojs/commit/b35dd5a8b1603542dfb2c2b06cad9e3d8d78fb08) Update runCommand docs (@sorribas)
- [ba28316](https://github.com/mafintosh/mongojs/commit/ba283167dc2c756fd92804b23042d1462c8818f7) Fix runCommand() bugs and update tests (@sorribas)
- [#80](https://github.com/mafintosh/mongojs/pull/80) Merge pull request #80 from sorribas/master (@sorribas)
- [143c029](https://github.com/mafintosh/mongojs/commit/143c02940402ed46d5def2f00855bdced6793193) Add docs for runCommand() (@sorribas)
- [93588ad](https://github.com/mafintosh/mongojs/commit/93588ad3e7392b7919ac6ba32aadfc69c5b57070) moved license out of readme (@mafintosh)

### v0.7.17 (2013/08/24 09:52 +00:00)
- [95af078](https://github.com/mafintosh/mongojs/commit/95af078a9fc57033f97665281e6e74ba3b64f160) v0.7.17 (@mafintosh)
- [f36fc8f](https://github.com/mafintosh/mongojs/commit/f36fc8f5febc2a02998966963192a38458d1c4da) setting highWaterMark to 0 since the driver buffers (@mafintosh)
- [cd0d397](https://github.com/mafintosh/mongojs/commit/cd0d3975be96f3197bb70b66687f6d4afdebf029) 0.7.16 - bump (@mafintosh)
- [e839b01](https://github.com/mafintosh/mongojs/commit/e839b01ead94bae6a07bd5191c6e253d08650647) fixed test in regards to #76 and some formatting (@mafintosh)
- [80e84fe](https://github.com/mafintosh/mongojs/commit/80e84fe368d01f41041ada93e26596faf56dc72a) 0.7.15 - bump (@mafintosh)
- [#77](https://github.com/mafintosh/mongojs/pull/77) Merge pull request #77 from ForbesLindesay/patch-3 (@ForbesLindesay)
- [#76](https://github.com/mafintosh/mongojs/pull/76) Merge pull request #76 from ForbesLindesay/patch-2 (@ForbesLindesay)
- [8ec0cb9](https://github.com/mafintosh/mongojs/commit/8ec0cb9930547547838f7062411ee9406c869782) Expose `Database` so the prototype can be easily extended (@ForbesLindesay)
- [39685d9](https://github.com/mafintosh/mongojs/commit/39685d98139f7b0bd31a47bc4291faa5d2540ed4) Fix getCollectionNames so result is the second arg of callback (@ForbesLindesay)
- [bbfca87](https://github.com/mafintosh/mongojs/commit/bbfca872b4921c519b3b1ce3a04631053afa9812) 0.7.14 - bump (@mafintosh)
- [1191b51](https://github.com/mafintosh/mongojs/commit/1191b51c7bbe1c936b3c0adfa3dad83e7afaabe1) .remove returning 0 if something was removed (@mafintosh)
- [3cec302](https://github.com/mafintosh/mongojs/commit/3cec3022ef8e5367a0dc5c2a22f994e19eb66b9b) 0.7.13 - bump (@mafintosh)
- [96d5d0b](https://github.com/mafintosh/mongojs/commit/96d5d0bce27a12b1584ad9fa6a98f3381c0a63bb) return from remove if no docs are found - fixes #75 (@mafintosh)
- [9d26012](https://github.com/mafintosh/mongojs/commit/9d26012995915665dbdadf39a51b7c416e1ab682) 0.7.12 - bump (@mafintosh)
- [#73](https://github.com/mafintosh/mongojs/pull/73) Merge pull request #73 from sorribas/master (@sorribas)
- [#74](https://github.com/mafintosh/mongojs/pull/74) Merge pull request #74 from sorribas/test-fix (@sorribas)
- [2d7c8a9](https://github.com/mafintosh/mongojs/commit/2d7c8a9f657b1f128160358216369ea374d09eb8) Fix the mongojs module reference in test-crash.js (@sorribas)
- [752aec3](https://github.com/mafintosh/mongojs/commit/752aec331ba68a1526ce872c17555ab6e7f4b0d0) Add support for db.getCollectionNames() and a test case for it. (@sorribas)
- [1bf49a3](https://github.com/mafintosh/mongojs/commit/1bf49a3e933096a0f5be6b54bd4608bc5aa9a414) added a ._apply method for the db as well (@mafintosh)
- [a2d4bfa](https://github.com/mafintosh/mongojs/commit/a2d4bfa5c9bf02050a78db9aad4a9b3881b6d875) 0.7.11 - bump (@mafintosh)
- [aec1284](https://github.com/mafintosh/mongojs/commit/aec128431df2819d9e694c4100b0a48af8635eaf) reemitting error in nextTick. fixes #72 (@mafintosh)
- [5db41d5](https://github.com/mafintosh/mongojs/commit/5db41d54e6598a38f7dbd19316c7ca3a47f1fd3e) added crash test (@mafintosh)
- [#69](https://github.com/mafintosh/mongojs/pull/69) Merge pull request #69 from sorribas/master (@sorribas)
- [df3eef4](https://github.com/mafintosh/mongojs/commit/df3eef40ae109abd250aedad31cc68e4815e251e) Remove duplicate .explain function. (@sorribas)
- [abb435e](https://github.com/mafintosh/mongojs/commit/abb435ec4aa06b32de5b1e468f03399bacbda901) Add support for Cursor.explain() (@sorribas)
- [942cf51](https://github.com/mafintosh/mongojs/commit/942cf5106c08b5605efe510d9f3833610608dfd9) using util.inherits (@mafintosh)
- [4ff7ea1](https://github.com/mafintosh/mongojs/commit/4ff7ea11e23d9068673bb1e9d2dedc976a0ef337) bump (@mafintosh)
- [#67](https://github.com/mafintosh/mongojs/pull/67) Merge pull request #67 from Osterjour/patch-1 (@Osterjour)
- [3567157](https://github.com/mafintosh/mongojs/commit/356715725e9bd3b3e9eda7148644dff49370209a) Fixing problems with collection names which have the same name as functions in native (@Osterjour)
- [ac10c44](https://github.com/mafintosh/mongojs/commit/ac10c44b072c9eeaa5ed35ae463b517d82800027) changed tag line (@mafintosh)
- [9b50821](https://github.com/mafintosh/mongojs/commit/9b508215e9546186a1c018a006aadfcd94c0b16c) added destroy to cursor (@mafintosh)
- [7deb303](https://github.com/mafintosh/mongojs/commit/7deb30384da751f4bd6b3865b56d99808ca04b0d) bump (@mafintosh)
- [#65](https://github.com/mafintosh/mongojs/pull/65) Merge pull request #65 from sorribas/master (@sorribas)
- [26d17aa](https://github.com/mafintosh/mongojs/commit/26d17aa20f464b54e6079cc7c9826ba854e94e34) Add mongo native Db protptype methods to the Database prototype. (@sorribas)
- [a37030a](https://github.com/mafintosh/mongojs/commit/a37030ac9376d5a4f5ce514e951d0f8127c38532) Refactor: add a Database constructor function and move db object functions to the prototype of said function. (@sorribas)
- [a6116dc](https://github.com/mafintosh/mongojs/commit/a6116dc65c30871fcda6b83c325680b94b4b37ea) updated desc (@mafintosh)
- [8d451fd](https://github.com/mafintosh/mongojs/commit/8d451fde7bd2c9699323347239cb77aba49bc909) updated contributors (@mafintosh)
- [b4e192f](https://github.com/mafintosh/mongojs/commit/b4e192fc8a81e05452cfaa92e295ec97c37c6709) bump (@mafintosh)
- [0af4f45](https://github.com/mafintosh/mongojs/commit/0af4f457f637c08556f977eb574b728eb4f4766c) minor style normalizations (@mafintosh)
- [#64](https://github.com/mafintosh/mongojs/pull/64) Merge pull request #64 from sorribas/master (@sorribas)
- [f82d356](https://github.com/mafintosh/mongojs/commit/f82d35650eae5e8de364b61bde8a7678e754ea78) Add error handling to runCommand functions. (@sorribas)
- [a7faea3](https://github.com/mafintosh/mongojs/commit/a7faea33031e5589032500b5280e448fe213f50c) Add support for both db.runCommand and db.collection.runCommand. Fixes #62. (@sorribas)
- [#63](https://github.com/mafintosh/mongojs/pull/63) Merge pull request #63 from sorribas/master (@sorribas)
- [14d803c](https://github.com/mafintosh/mongojs/commit/14d803c700361e6a00b75fd83f4cf9d88d8b7be3) Merge remote-tracking branch 'upstream/master' (@sorribas)
- [fd3b42f](https://github.com/mafintosh/mongojs/commit/fd3b42f9437a8bfbdbfd513037014ca702ac3a02) Fix the code styling and add error handling. (@sorribas)
- [5b0099d](https://github.com/mafintosh/mongojs/commit/5b0099d6c5a22842602d2cbbcaf3fc016de3e426) better error message on bad conf (@mafintosh)
- [2884029](https://github.com/mafintosh/mongojs/commit/2884029857831e582f54acbdd0512b7a27e87ed2) bump (@mafintosh)
- [55e8e63](https://github.com/mafintosh/mongojs/commit/55e8e63cd6c6987a54edd3716b7a1fa26630515a) Added getIndexes alias (@freeall)
- [06efeee](https://github.com/mafintosh/mongojs/commit/06efeeeb2375a7107df611773576e9562f0cc9b7) tests should work even if not installed in node_modules (@mafintosh)
- [41f5625](https://github.com/mafintosh/mongojs/commit/41f562573a0c5ddca56fe839b32ad7bd38612c6d) Add the justOne option to the remove method and add tests for the remove method. fix #60 (@sorribas)
- [75cef67](https://github.com/mafintosh/mongojs/commit/75cef67bdaf739fb5f9898dfd6b873eccd69cb25) timeout is disabled in tailable example (@mafintosh)
- [8995a19](https://github.com/mafintosh/mongojs/commit/8995a19b3642e4ef5c1273d12615efbcec1b1f9d) added section on tailable cursors (@mafintosh)
- [74c3fd7](https://github.com/mafintosh/mongojs/commit/74c3fd7080ee7e36a8e3187223c16f0227c4a45a) bump (@mafintosh)
- [39c1080](https://github.com/mafintosh/mongojs/commit/39c10808c74337de70ad9c2b702135d62a931813) callback should be optional for all mutators (@mafintosh)
- [d4e6513](https://github.com/mafintosh/mongojs/commit/d4e6513ffcf67618fe51769076d08e5689b2ca5b) bump (@mafintosh)
- [#48](https://github.com/mafintosh/mongojs/pull/48) Merge pull request #48 from benediktarnold/keyf (@benediktarnold)
- [f4d5605](https://github.com/mafintosh/mongojs/commit/f4d56052d5aa2369ce0519d29b75c2535046b31e) Add compatibility support for keyf in group command (@benediktarnold)
- [9835b78](https://github.com/mafintosh/mongojs/commit/9835b782107a5b915434b7859947eab96287a705) bump (@mafintosh)
- [#47](https://github.com/mafintosh/mongojs/pull/47) Merge pull request #47 from RG72/master (@RG72)
- [34c45b3](https://github.com/mafintosh/mongojs/commit/34c45b37d1f94cbcb3324efbf142799b2a9ad316) Install mongodb refuses until the latest version does not specified directly. I don't know why.
- [#43](https://github.com/mafintosh/mongojs/pull/43) Merge pull request #43 from ForbesLindesay/patch-1 (@ForbesLindesay)
- [c52a7dc](https://github.com/mafintosh/mongojs/commit/c52a7dc5763f0d57d26f0bd26a84ed9611b82a74) Expose Constructors (@ForbesLindesay)
- [4881917](https://github.com/mafintosh/mongojs/commit/48819171b88a733175ab6f912e8710095d69945f) compat with new stream interface (@mafintosh)
- [3117fb3](https://github.com/mafintosh/mongojs/commit/3117fb3c1149401534f9d8e38a5156f2586aafc0) using thunky (@mafintosh)
- [c9c525c](https://github.com/mafintosh/mongojs/commit/c9c525c23f93f148aaa3a42c6beeb7f099ecd1c9) license info (@mafintosh)
- [1135bf0](https://github.com/mafintosh/mongojs/commit/1135bf09794fc22d5cecc3e85a5f288065a01ce0) better comment (@mafintosh)
- [bb415cc](https://github.com/mafintosh/mongojs/commit/bb415cc9a099ee0ba77f1401f868f9e009b26054) 0.7 release (@mafintosh)
- [e7326e9](https://github.com/mafintosh/mongojs/commit/e7326e92a5a94e7846e8d425641d5db59de2b503) test for streaming cursors (@mafintosh)
- [f68576f](https://github.com/mafintosh/mongojs/commit/f68576f7933b1d099fd4f29e7516cd71eb25f870) docs for streaming cursors (@mafintosh)
- [e20e689](https://github.com/mafintosh/mongojs/commit/e20e68927714ef2338df9bddc83bcdbf20ae82c0) cursor is a 0.10 and 0.8 compat readable stream (@mafintosh)
- [bf89980](https://github.com/mafintosh/mongojs/commit/bf89980b0286e32ed91ad36182f791f8b553c2d0) npm bump (@mafintosh)
- [1d340be](https://github.com/mafintosh/mongojs/commit/1d340be4e8e3dc7cda4fb71c2bfaaece82f5245c) using memolite (@mafintosh)
- [3555dde](https://github.com/mafintosh/mongojs/commit/3555dde5dc504ab417b86bc7b0342b8300a8acb4) npm bump - stricter mongodb version (@mafintosh)
- [5944380](https://github.com/mafintosh/mongojs/commit/5944380b362161dbf8c31747eadbcbc746b11285) Fixed #41 (@mafintosh)
- [b7872dc](https://github.com/mafintosh/mongojs/commit/b7872dcc163e179348207b8870cb0ceb36a0d6fb) removed old comment (@mafintosh)
- [aeaa411](https://github.com/mafintosh/mongojs/commit/aeaa4119ffe76bca773c3515b5fd4648568c2b86) more examples in readme (@mafintosh)
- [34819d8](https://github.com/mafintosh/mongojs/commit/34819d893b3fa9f5094dd03aefe832caa348b550) fixed cursor config issue (@mafintosh)
- [20f7a5b](https://github.com/mafintosh/mongojs/commit/20f7a5b89fa975f221df1f842c4d8fb1ccb5a1d3) better test coverage (@mafintosh)
- [5ef53da](https://github.com/mafintosh/mongojs/commit/5ef53daadce1d92341653b9276fc22e10752db1f) fixed group issue (@mafintosh)
- [9afee11](https://github.com/mafintosh/mongojs/commit/9afee1157616e571c0582c9d31a5f956b620ff90) 0.6.0 - complete refactor (@mafintosh)
- [6bf676c](https://github.com/mafintosh/mongojs/commit/6bf676c9dd56111ace002023cc06855e59accd8f) replSet config map deprecated but still supported (@mafintosh)
- [8eab6da](https://github.com/mafintosh/mongojs/commit/8eab6da5493c9879475beec6dba10e2244f0c97d) more docs an supporting explicit docs (@mafintosh)
- [67a77c9](https://github.com/mafintosh/mongojs/commit/67a77c931375a274cfde68cdc7db5e575c2b8bec) 0.5.2 rc (@mafintosh)
- [e25e55c](https://github.com/mafintosh/mongojs/commit/e25e55cf314f94a6040e70a8dfd18b734b56e404) sync update and cursor chain tests (@mafintosh)
- [f033377](https://github.com/mafintosh/mongojs/commit/f03337785b9a765a95d8291284efd961959076c7) fixed auth issue (@mafintosh)
- [aec5e94](https://github.com/mafintosh/mongojs/commit/aec5e948f0f517c0460c1e8f476753a2e55cb308) better connection string support (@mafintosh)
- [d51e56f](https://github.com/mafintosh/mongojs/commit/d51e56f7163e05c8f608a4bf51d9c4fdc02c450c) bump version (@mafintosh)
- [#31](https://github.com/mafintosh/mongojs/pull/31) Merge pull request #31 from lordkhonsu/master (@lordkhonsu)
- [0f6cb6c](https://github.com/mafintosh/mongojs/commit/0f6cb6c588bea7af7223193a14428ed66909adf3) adding batchSize config to Cursor (@lordkhonsu)
- [3de3b6f](https://github.com/mafintosh/mongojs/commit/3de3b6f83841005d49d49587524ee11f25243792) added npm test link (@mafintosh)
- [9a3810a](https://github.com/mafintosh/mongojs/commit/9a3810a06412264b5911af9117f11654cea473f7) git ignore (@mafintosh)
- [8f54fc0](https://github.com/mafintosh/mongojs/commit/8f54fc0524147ada3a1fbaa5f279a354117ce37a) npm bump (@mafintosh)
- [fcd1314](https://github.com/mafintosh/mongojs/commit/fcd1314be0bfdd533bee62e97386facec76542f8) docs showing single function usage (@mafintosh)
- [652e088](https://github.com/mafintosh/mongojs/commit/652e0888c49005d198fc7989becafbd251c23da3) style changes and now exporting a single function (@mafintosh)
- [#28](https://github.com/mafintosh/mongojs/pull/28) Merge pull request #28 from jakemaskiewicz/patch-1 (@jakemaskiewicz)
- [8e28a91](https://github.com/mafintosh/mongojs/commit/8e28a91481bf979b92f45796481ba92273f3b535) npm bump (@mafintosh)
- [5818a90](https://github.com/mafintosh/mongojs/commit/5818a90f9aa4325b50524186a319434479a48042) grouped public methods (@mafintosh)
- [#25](https://github.com/mafintosh/mongojs/pull/25) Merge pull request #25 from blisteringherb/master (@blisteringherb)
- [#26](https://github.com/mafintosh/mongojs/pull/26) Merge pull request #26 from xissy/master (@xissy)
- [192f20b](https://github.com/mafintosh/mongojs/commit/192f20b5978b7d2c28207d6b155bbb4ebce6d6de) updated default safe variable to false (@jakemask)
- [a534bc6](https://github.com/mafintosh/mongojs/commit/a534bc6c169311f086f967f64df19200bbd8d578) mongodb group command added. (@xissy)
- [5b0b539](https://github.com/mafintosh/mongojs/commit/5b0b539e8b3b0506c95c690ace94b4bf1aef49f4) mongodb group command added. (@xissy)
- [f599c3b](https://github.com/mafintosh/mongojs/commit/f599c3bf78d612af2728251f60a74bfb7208b2aa) Updating the result.db variable to use the correct varible name for path.
- [4a9be9a](https://github.com/mafintosh/mongojs/commit/4a9be9a19513529634af7d070926ba898a040360) Indentation fix in example. (@mafintosh)
- [44fc218](https://github.com/mafintosh/mongojs/commit/44fc21877c537b79cc0de84c7529b8a80dcd69eb) Merge branch 'master' of https://github.com/gett/mongojs (@mafintosh)
- [65cf8ae](https://github.com/mafintosh/mongojs/commit/65cf8aee74b72ae0e734af745d39024cf4040ff4) added git link to package.json (@mafintosh)
- [abf99f3](https://github.com/mafintosh/mongojs/commit/abf99f369b89707e1816be734e07d1f229b1f6f9) More typos. (@mafintosh)
- [12957bb](https://github.com/mafintosh/mongojs/commit/12957bb4348d2569bd432b4d4311b74ecf3b1181) Merge branch 'master' of https://github.com/gett/mongojs (@mafintosh)
- [fde6ad8](https://github.com/mafintosh/mongojs/commit/fde6ad87724ebe6ee5f0f6dabeb670002f34e9cb) shorthand replSet config syntax (@mafintosh)
- [6e87f2f](https://github.com/mafintosh/mongojs/commit/6e87f2f2a75eedd6f41e4d6ca8a0075e773538e8) collection should be collecitons in config (@mafintosh)
- [126220c](https://github.com/mafintosh/mongojs/commit/126220c274706ea54133d17a5b8667af290f968a) normalized the links (@mafintosh)
- [4deb11e](https://github.com/mafintosh/mongojs/commit/4deb11e9ada61dfe11626eb657ab506f2af2351e) Missing comma in example (@mafintosh)
- [8b0c428](https://github.com/mafintosh/mongojs/commit/8b0c428fdd94e89dda2ced89d9776c8eaee74863) Another mongo docs link (@mafintosh)
- [c52dc8f](https://github.com/mafintosh/mongojs/commit/c52dc8f86122358df50cb31b801ef837654a58a2) Added replication set to README (@mafintosh)
- [54f4676](https://github.com/mafintosh/mongojs/commit/54f467650b4c89ae1a5e0aadd7f2077b366dc195) support for replication sets (@mafintosh)
- [df360a7](https://github.com/mafintosh/mongojs/commit/df360a7b21e6012503ada9682cecb1b6cb921f0c) compatible with mongodb 1.x.x (@mafintosh)
- [69ddb6f](https://github.com/mafintosh/mongojs/commit/69ddb6f00eb19b264dc02e34e98c1bb83d0bcfe9) exposed native mongodb object through a .client property (@mafintosh)
- [d59f4eb](https://github.com/mafintosh/mongojs/commit/d59f4eb42f27eb1ef4ad1b5df8d95151d49c9ce2) renamed close to disconnect (@ianjorgensen)
- [b03b6e1](https://github.com/mafintosh/mongojs/commit/b03b6e18f4f4b5fdf4368347ed2543142c5ba271) added close function (@ianjorgensen)
- [#12](https://github.com/mafintosh/mongojs/pull/12) Merge pull request #12 from kevinmctigue/patch-1 (@kevinmctigue)
- [f118ee8](https://github.com/mafintosh/mongojs/commit/f118ee8a021736a9836817cdc0b0c41a515a91b1) Added an example to the connections samples to show users that the ['collections'] array is optional on connect. (@kevinmctigue)
- [#11](https://github.com/mafintosh/mongojs/pull/11) Merge pull request #11 from Erkan-Yilmaz/master (@Erkan-Yilmaz)
- [5fcb1f0](https://github.com/mafintosh/mongojs/commit/5fcb1f0f3e8f37a05e377506a1ffde85c8a20321) change 1 word: to -> we (@Erkan-Yilmaz)
- [a2bf06e](https://github.com/mafintosh/mongojs/commit/a2bf06e4255d8e0074280be3ad2e3e5fb7ee13bb) fixed typo (@ianjorgensen)
- [19a5de0](https://github.com/mafintosh/mongojs/commit/19a5de0ff474ad18974a68230f749fa62b1fc389) Merge branch 'master' of https://github.com/gett/mongojs (@mafintosh)
- [3c1a871](https://github.com/mafintosh/mongojs/commit/3c1a871996d89134388c1f43df70224431d63635) npm bump (@mafintosh)
- [dca0383](https://github.com/mafintosh/mongojs/commit/dca03834729ea5adb77b22f581b4ed1491458a9b) safe option will now always be set if a callback is given to a collection (@mafintosh)
- [f18e2a5](https://github.com/mafintosh/mongojs/commit/f18e2a542b1505c7af8b87de19e68e2179766dc0) Better docs (@mafintosh)
- [eaeadd9](https://github.com/mafintosh/mongojs/commit/eaeadd97587d065b6be40f27511de69be4d2e9a6) npm bump (@mafintosh)
- [f703899](https://github.com/mafintosh/mongojs/commit/f70389900095a16fffecc395de2d2f0ae21bed5a) no more normalizing ids (@mafintosh)
- [d419919](https://github.com/mafintosh/mongojs/commit/d419919f6df0410deb28365e305526c201c249b5) we do not require native compilation now (@mafintosh)
- [bf22b83](https://github.com/mafintosh/mongojs/commit/bf22b8336b855f62a02b29c29806b4f96e6dc468) npm version bump (@mafintosh)
- [70c06e1](https://github.com/mafintosh/mongojs/commit/70c06e14c7e594883318fb49cc4a433228d8bbf1) npm version bump (@mafintosh)
- [6d55c1b](https://github.com/mafintosh/mongojs/commit/6d55c1b25a100e6bb4c77dbe7efe05238cb6e107) removed normalize function as it serves no purpose with the new JS parser, some style tidy (@mafintosh)
- [11cb282](https://github.com/mafintosh/mongojs/commit/11cb2826e397b5c9529fbea41cf702feca180250) updated monogdb version (@ianjorgensen)
- [2f8c908](https://github.com/mafintosh/mongojs/commit/2f8c908ba6303e5d2874da8b992d071957f0572a) removed deprecated native_parser (@ianjorgensen)
- [#4](https://github.com/mafintosh/mongojs/pull/4) Merge pull request #4 from Srirangan/master (@Srirangan)
- [3c05202](https://github.com/mafintosh/mongojs/commit/3c052020c9aff66d03d7c82a8decb7a0299b1385) Use JS parser if native parser is not available (@Srirangan)
- [112df62](https://github.com/mafintosh/mongojs/commit/112df62ee3beaf511e4748de54d5c6b8dec8636c) bump (@mafintosh)
- [ebf22e9](https://github.com/mafintosh/mongojs/commit/ebf22e9aaa288b87235f9610c754cafea360a027) added auto_connect = true (@mafintosh)
- [6079f88](https://github.com/mafintosh/mongojs/commit/6079f88f7c5b171da2f018eec4a36cdae80bb121) Added native compilation (@mafintosh)
- [b7c9350](https://github.com/mafintosh/mongojs/commit/b7c9350bbacd688bc2ec01fc772add4604e53946) tidy (@mafintosh)
- [40643ca](https://github.com/mafintosh/mongojs/commit/40643ca1f496fc66c02bf174786f3a00378f3e68) Merge branch 'master' of https://github.com/gett/mongojs (@mafintosh)
- [e99d05a](https://github.com/mafintosh/mongojs/commit/e99d05aa42857eee59e6dae65ccb2ba0d74fcb51) exposed all methods from db and collection upwards (@mafintosh)
- [0939ff4](https://github.com/mafintosh/mongojs/commit/0939ff47d925e66b6ed3eb73cd4f8a8012b543cd) version bump (@mafintosh)
- [#1](https://github.com/mafintosh/mongojs/pull/1) Merge pull request #1 from walling/master (@walling)
- [6e8ffb3](https://github.com/mafintosh/mongojs/commit/6e8ffb38dc5e5b6c7a423712cc0d60f7b72d0c24) Exposing BSON constructors. (@walling)
- [8c21dc0](https://github.com/mafintosh/mongojs/commit/8c21dc0b9cd53ad40be08514f274a7826b2f3672) updated homepage, description and keywords (@mafintosh)
- [dd81982](https://github.com/mafintosh/mongojs/commit/dd81982855b3ad1a344d3f9ca491d02464fd1b19) version bump (@mafintosh)
- [3a40661](https://github.com/mafintosh/mongojs/commit/3a406615ff9aef602130935b93ecc3d2791f7a2e) fixed possible null pointer (@mafintosh)
- [aacfb51](https://github.com/mafintosh/mongojs/commit/aacfb51d61e18260d67dac689c6b2693a2d7f335) removed redundant object (@mafintosh)
- [20efefb](https://github.com/mafintosh/mongojs/commit/20efefb464d80a16740a1696d5ef1dfedb3f50d3) fixed typo (@mafintosh)
- [e87d993](https://github.com/mafintosh/mongojs/commit/e87d993ba750fa2503940b232b30e8c58f5274b9) fixed normalize bug and removed a duplicate toArray method (@mafintosh)
- [d293b21](https://github.com/mafintosh/mongojs/commit/d293b21dd97200c6c398e3a7d765eb7a0ea9eec4) fixed feature detection bug with Proxies (@mafintosh)
- [e143b01](https://github.com/mafintosh/mongojs/commit/e143b01b09126b566f1a419ddccf60eeca367330) fixed indentation (@mafintosh)
- [4ef10e3](https://github.com/mafintosh/mongojs/commit/4ef10e3e4c4f3fd0327668dbaef351935cde21bd) removed the sympathy thing (@mafintosh)
- [ed3875e](https://github.com/mafintosh/mongojs/commit/ed3875e61f3c6d2c4205e528cf15549002221485) added ian as a sympathy thing (@mafintosh)
- [787ad7d](https://github.com/mafintosh/mongojs/commit/787ad7d38829ab918901c3ef3122f30478fafab6) version bump (@mafintosh)
- [0afe687](https://github.com/mafintosh/mongojs/commit/0afe687edd7443a7bec3360303be2e80f8222e7c) collections is now optional (@mafintosh)
- [075c2cb](https://github.com/mafintosh/mongojs/commit/075c2cb56da672656ed566a0bb1b5c7857f1696a) added proxy support (@mafintosh)
- [3b5755d](https://github.com/mafintosh/mongojs/commit/3b5755d5e104684cc7a4280d2b0f71823bf8786d) mongo shell is now mongo API (@mafintosh)
- [d66171a](https://github.com/mafintosh/mongojs/commit/d66171a977a28a181be81db578af62357cbf272c) fixed requires (@mafintosh)
- [eb89ed9](https://github.com/mafintosh/mongojs/commit/eb89ed9c96e4d8e8384e988a18fa734c9ceec491) fixed npm example (@mafintosh)
- [865d281](https://github.com/mafintosh/mongojs/commit/865d281c23862e9e7843bd341644639b5927cb6a) added javascript type to examples (@mafintosh)
- [061fff5](https://github.com/mafintosh/mongojs/commit/061fff5b574ba527fa1453d21da16d3f509fadf7) first commit (@mafintosh)
