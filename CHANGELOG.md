# Change Log

All notable changes to this project will be documented in this file.
See [Conventional Commits](https://conventionalcommits.org) for commit guidelines.

# 3.0.0 (2022-10-22)


### BREAKING CHANGES

* This release drops support for node.js 12 and 14. It also drops support for the browser specific compilation, as the entire toolchain was deprecated. I am open to this being re-added if someone wants to take it on :)
* Drops support for node.js 8.x, which is EOL. 
* This release drops support for node.js 6, which is EOL. Please upgrade with care ❤️ 



### 🐛　Bug Fixes

* non-zero delay between first attempt and first retry for linear and exp strategy ([#163](https://github.com/JustinBeckwith/retry-axios/issues/163)) ([e63ca08](https://github.com/JustinBeckwith/retry-axios/commit/e63ca084f5372f03debe5c082e6b924684072345)), closes [#122](https://github.com/JustinBeckwith/retry-axios/issues/122) [#122](https://github.com/JustinBeckwith/retry-axios/issues/122) [#122](https://github.com/JustinBeckwith/retry-axios/issues/122)
* cannot set propery raxConfig of undefined ([#114](https://github.com/JustinBeckwith/retry-axios/issues/114)) ([0be8578](https://github.com/JustinBeckwith/retry-axios/commit/0be857823f4e4845e72891ba63cef08d006cefc8))
* added check for cancel tokens ([#99](https://github.com/JustinBeckwith/retry-axios/issues/99)) ([734a93f](https://github.com/JustinBeckwith/retry-axios/commit/734a93ff45de7dfd827f17ec7e7545636a3e8add))
* Don't store counter on input config object ([#98](https://github.com/JustinBeckwith/retry-axios/issues/98)) ([c8ceec0](https://github.com/JustinBeckwith/retry-axios/commit/c8ceec0e16e57297edbc0739f40b99a836e3254e)), closes [#61](https://github.com/JustinBeckwith/retry-axios/issues/61)
* handle arrays that are converted to objects ([#83](https://github.com/JustinBeckwith/retry-axios/issues/83)) ([554fd4c](https://github.com/JustinBeckwith/retry-axios/commit/554fd4ca444a0dd5237bccdc3d156c481cce8f42))
* ensure config is set ([#81](https://github.com/JustinBeckwith/retry-axios/issues/81)) ([88ffd00](https://github.com/JustinBeckwith/retry-axios/commit/88ffd005a9a659ee75f545d3b1b4df8d00b78ceb))
* include files in the release ([#29](https://github.com/JustinBeckwith/retry-axios/issues/29)) ([30663b3](https://github.com/JustinBeckwith/retry-axios/commit/30663b362bd1eddf33c6390e4df8123fa295d37e))
* fix instructions and test for non-static instnaces ([544c2a6](https://github.com/JustinBeckwith/retry-axios/commit/544c2a6563c3c4df69d5d441bbaf872a0a59d83f))
* **deps:** update dependency gts to v1 ([#45](https://github.com/JustinBeckwith/retry-axios/issues/45)) ([1dc0f2f](https://github.com/JustinBeckwith/retry-axios/commit/1dc0f2f77b52cd6fcbec69f31c70fc5f2e0f084e))
* **typescript:** include raxConfig in native axios types ([#85](https://github.com/JustinBeckwith/retry-axios/issues/85)) ([b8b0456](https://github.com/JustinBeckwith/retry-axios/commit/b8b04565004b100cc36ac1f5ee32dfde34f0770f))


### ✨　Features

* support the latest versions of node.js ([#188](https://github.com/JustinBeckwith/retry-axios/issues/188)) ([ef74217](https://github.com/JustinBeckwith/retry-axios/commit/ef74217113cf611af420564421d844858d70701b))
* configurable maxRetryDelay ([#165](https://github.com/JustinBeckwith/retry-axios/issues/165)) ([b8842d7](https://github.com/JustinBeckwith/retry-axios/commit/b8842d751482caf31bc1c090cda3c7923d1f23fa))
* support retry-after header ([#142](https://github.com/JustinBeckwith/retry-axios/issues/142)) ([5c6cace](https://github.com/JustinBeckwith/retry-axios/commit/5c6cace7fbf418285c3b0f114f5806cb573b0a64))
* allow retryDelay to be 0 ([#132](https://github.com/JustinBeckwith/retry-axios/issues/132)) ([57ba46f](https://github.com/JustinBeckwith/retry-axios/commit/57ba46f563561e6b9e4f1e2ca39daefe2993d399))
* export the shouldRetryRequest method ([#74](https://github.com/JustinBeckwith/retry-axios/issues/74)) ([694d638](https://github.com/JustinBeckwith/retry-axios/commit/694d638ccc0d91727cbcd9990690a9b29815353c))
* produce es, common, and umd bundles ([#107](https://github.com/JustinBeckwith/retry-axios/issues/107)) ([62cabf5](https://github.com/JustinBeckwith/retry-axios/commit/62cabf58c86ffc8169b74b8912f2aac94a703733))
* add configurable backoffType ([#76](https://github.com/JustinBeckwith/retry-axios/issues/76)) ([6794d85](https://github.com/JustinBeckwith/retry-axios/commit/6794d85c6cdd8e27bc59f613392caff8ddada985))
* drop support for node.js 6, add 12 ([78ea044](https://github.com/JustinBeckwith/retry-axios/commit/78ea044f17b0d1900509994b36bda31da17ea360))
* accept promises on config.onRetryAttempt ([#23](https://github.com/JustinBeckwith/retry-axios/issues/23)) ([acfbe39](https://github.com/JustinBeckwith/retry-axios/commit/acfbe399f7017a607c4f49c578250a82834c448c))
* umd compatibility with babel 7.x ([#21](https://github.com/JustinBeckwith/retry-axios/issues/21)) ([f1b336c](https://github.com/JustinBeckwith/retry-axios/commit/f1b336c00a03f56ba7874a9565955c89c32b1d68))
* add support for noResponseRetries ([d2cfde7](https://github.com/JustinBeckwith/retry-axios/commit/d2cfde70e6314bc298dcf9291bacb3385c130cdf))
* add support for overriding shouldRetry ([76fcff5](https://github.com/JustinBeckwith/retry-axios/commit/76fcff59849b7b9de428f9638ff5057c159a1a3d))
* add support for onRetryAttempt handler ([fa17de4](https://github.com/JustinBeckwith/retry-axios/commit/fa17de46bd6c6c33db99aca5668a3d58a81c761e))
* add support for statusCodesToRetry ([9283c9e](https://github.com/JustinBeckwith/retry-axios/commit/9283c9e40970eaf359ac664ce5ac6517087c3257))
* add support for configurable http methods ([819855c](https://github.com/JustinBeckwith/retry-axios/commit/819855c99e3fda19615e9f0d704988d985df5036))


### 📚　Documentation

* add comment to 'noResponseRetries' setting. ([#184](https://github.com/JustinBeckwith/retry-axios/issues/184)) ([7387695](https://github.com/JustinBeckwith/retry-axios/commit/73876954fde3bfec4aa3499e6bdeaf76587ec5e9))
* exponential backoff formula in comment ([#146](https://github.com/JustinBeckwith/retry-axios/issues/146)) ([b51b6a1](https://github.com/JustinBeckwith/retry-axios/commit/b51b6a1cd8f0c20492ee47f2abdd9fb3f37337a0))
* clarify 'retryDelay' is only for static strategy ([#126](https://github.com/JustinBeckwith/retry-axios/issues/126)) ([c93568e](https://github.com/JustinBeckwith/retry-axios/commit/c93568e02ba5ff361713d62de4fa801e0174bccd))
* add info on using es modules ([#86](https://github.com/JustinBeckwith/retry-axios/issues/86)) ([17a2a87](https://github.com/JustinBeckwith/retry-axios/commit/17a2a8704b7fb7e9a22c30c8f56cbcc9cb561861))
* fix samples and remove axios 0.19.0 note ([#84](https://github.com/JustinBeckwith/retry-axios/issues/84)) ([2219194](https://github.com/JustinBeckwith/retry-axios/commit/22191943ebdd157270491b21920908560a01b810))
* add a note about axios 0.19.0 not working ([#69](https://github.com/JustinBeckwith/retry-axios/issues/69)) ([d6393a1](https://github.com/JustinBeckwith/retry-axios/commit/d6393a1558530e5ae955dc1fad691e757a1dcda7))
* do not override axios defaults ([#30](https://github.com/JustinBeckwith/retry-axios/issues/30)) ([4801ccb](https://github.com/JustinBeckwith/retry-axios/commit/4801ccbcd27ef5605f7217acc326c967cf5fe7bf))
* clean up readme badges ([073216e](https://github.com/JustinBeckwith/retry-axios/commit/073216ecc59239761ba2d838cb73e06c5d8bc18f))


### 🚨　Tests

* add link checking of readme ([#137](https://github.com/JustinBeckwith/retry-axios/issues/137)) ([d00692b](https://github.com/JustinBeckwith/retry-axios/commit/d00692be31ee0b85141b9eb36371e67a7cbe9aed))
* should accept defaults on a new instance ([#91](https://github.com/JustinBeckwith/retry-axios/issues/91)) ([fca9674](https://github.com/JustinBeckwith/retry-axios/commit/fca9674ab4d534eac52c11f30e0aca8547215f63))
* fix undefined vs 0 check ([a8defe0](https://github.com/JustinBeckwith/retry-axios/commit/a8defe01059fff98f1b2a056fd3df62e9bc22021))
* fix assert.fail bugs and check nock scopes ([358bc28](https://github.com/JustinBeckwith/retry-axios/commit/358bc28de4cd4ee97b5995ec9358fcb2b1163f52))
* coverage up to 100% ([154887c](https://github.com/JustinBeckwith/retry-axios/commit/154887c664e8b70c8e9c58c8960e155801155987))


### 🛠　Build System

* use `@bluelovers/tsdx` ([adb5999](https://github.com/JustinBeckwith/retry-axios/commit/adb599989fe98bb01465e0b32b47aea37d96a386))
* add release main config ([#161](https://github.com/JustinBeckwith/retry-axios/issues/161)) ([3f001c8](https://github.com/JustinBeckwith/retry-axios/commit/3f001c87babdb460187840080c05386a4c2282b4))
* remove often broken david dm badge ([#162](https://github.com/JustinBeckwith/retry-axios/issues/162)) ([f9b65d6](https://github.com/JustinBeckwith/retry-axios/commit/f9b65d6d99c0f742ad325bb660ccdd5cb8ed5fe8))
* run CI on node 16 ([#160](https://github.com/JustinBeckwith/retry-axios/issues/160)) ([2128c50](https://github.com/JustinBeckwith/retry-axios/commit/2128c504de938fc754db59280e2a4a2d668052f5))
* specify main branch in ci ([#159](https://github.com/JustinBeckwith/retry-axios/issues/159)) ([94d5fff](https://github.com/JustinBeckwith/retry-axios/commit/94d5fff1fcddd08d232752d2f9b022c21e84965c))
* use main branch in CI ([#141](https://github.com/JustinBeckwith/retry-axios/issues/141)) ([06c2386](https://github.com/JustinBeckwith/retry-axios/commit/06c2386df896299b5390969951b408931902c0d3))
* switch to github actions ([#112](https://github.com/JustinBeckwith/retry-axios/issues/112)) ([c0f78cc](https://github.com/JustinBeckwith/retry-axios/commit/c0f78ccd33a74de5f79f3e70df4a8497c9dd274a))
* fix linting issues ([#80](https://github.com/JustinBeckwith/retry-axios/issues/80)) ([381148c](https://github.com/JustinBeckwith/retry-axios/commit/381148c8f8a337cfd91efa0dc95e0b3305815d64))
* use commitlint bot ([#57](https://github.com/JustinBeckwith/retry-axios/issues/57)) ([7a23968](https://github.com/JustinBeckwith/retry-axios/commit/7a23968e0564c5dbf133bdc7ff21528673c4e185))
* fix semantic-release command ([#27](https://github.com/JustinBeckwith/retry-axios/issues/27)) ([1ea60bc](https://github.com/JustinBeckwith/retry-axios/commit/1ea60bc236e904a9e38d8df77e67dd73149828eb))
* modernize the build ([#26](https://github.com/JustinBeckwith/retry-axios/issues/26)) ([80a0a13](https://github.com/JustinBeckwith/retry-axios/commit/80a0a13861b328e6530417ecc6a86901f2552f4b))


### ♻️　Chores

* fix lint issues ([#109](https://github.com/JustinBeckwith/retry-axios/issues/109)) ([8f8e2f8](https://github.com/JustinBeckwith/retry-axios/commit/8f8e2f8211cf13ac7188b6d4bcef4a7821b13ba8))
* drop support for nodejs 8.x ([#82](https://github.com/JustinBeckwith/retry-axios/issues/82)) ([d259697](https://github.com/JustinBeckwith/retry-axios/commit/d259697ab5e9931c7ceaddff6c48d43180dda6c6))
* bump dev dependencies and use c8 ([#58](https://github.com/JustinBeckwith/retry-axios/issues/58)) ([cbd7b73](https://github.com/JustinBeckwith/retry-axios/commit/cbd7b73bfba44cb06764827ddd3c2e429e213421))
* drop support for node.js 4.x, add 10/11 to CI ([1d6c78f](https://github.com/JustinBeckwith/retry-axios/commit/1d6c78f7af9dbbf3dfbc6154fe8c15fa7b3aaf7e))
* ignore package-lock.json ([1ead26a](https://github.com/JustinBeckwith/retry-axios/commit/1ead26a01d080dd9c8096bb40f27d77d13a45352))
* upgrade dependencies ([d291f82](https://github.com/JustinBeckwith/retry-axios/commit/d291f82297412c0a7d1f7b3d7061a2b48bff4e68))
* upgrade all dependencies ([d713c8e](https://github.com/JustinBeckwith/retry-axios/commit/d713c8ef06662107b89e319232aadaec90039e41))
* release 3.2 ([a091b45](https://github.com/JustinBeckwith/retry-axios/commit/a091b45a7e296aac980349e2eac5ef7727d4b463))
* update all deps ([e7485bf](https://github.com/JustinBeckwith/retry-axios/commit/e7485bf63ab6f9d2d761e6dc0ac3f786c01284a2))
* release 0.3.0 ([06d7c5e](https://github.com/JustinBeckwith/retry-axios/commit/06d7c5efc392c74e4e82cac9c20145cd9bf5abaa))
* release 0.2.0 ([60d4cba](https://github.com/JustinBeckwith/retry-axios/commit/60d4cba1d5d92112ba0bd814e68e469645d3d362))
* bump to 0.1.0 ([42a8a1a](https://github.com/JustinBeckwith/retry-axios/commit/42a8a1a38ea3d802d3dcd4b6d7e3763074c01ba8))
* update readme ([ba45b37](https://github.com/JustinBeckwith/retry-axios/commit/ba45b37b74dcf700ec8e2a2a816183ed133713f2))
* run gtx fix ([e632c8b](https://github.com/JustinBeckwith/retry-axios/commit/e632c8b18e80ef91acc1611fc7b6c7cb6558e348))
* **deps:** update dependency @types/mocha to v10 ([#200](https://github.com/JustinBeckwith/retry-axios/issues/200)) ([979520c](https://github.com/JustinBeckwith/retry-axios/commit/979520c4aaebccf183df0c435f2905375de76068))
* **deps:** update dependency typescript to ~4.8.0 ([#199](https://github.com/JustinBeckwith/retry-axios/issues/199)) ([31058f9](https://github.com/JustinBeckwith/retry-axios/commit/31058f967310893eb6e257b99b5b6c828041a4a4))
* **deps:** update dependency typescript to ~4.7.0 ([#194](https://github.com/JustinBeckwith/retry-axios/issues/194)) ([003bb90](https://github.com/JustinBeckwith/retry-axios/commit/003bb90ac357debe401031d290ad119f0796b4f4))
* **deps:** update dependency sinon to v14 ([#190](https://github.com/JustinBeckwith/retry-axios/issues/190)) ([e4ebe5e](https://github.com/JustinBeckwith/retry-axios/commit/e4ebe5e10dd216755abcf7a9342e75070406fe8a))
* **deps:** update dependency axios to ^0.27.0 ([#186](https://github.com/JustinBeckwith/retry-axios/issues/186)) ([5b4ef3c](https://github.com/JustinBeckwith/retry-axios/commit/5b4ef3c3673bd2c47c766c5f0682891f51534e6c))
* **deps:** update codecov/codecov-action action to v3 ([#185](https://github.com/JustinBeckwith/retry-axios/issues/185)) ([a2cfde0](https://github.com/JustinBeckwith/retry-axios/commit/a2cfde057b1471c99591b5bbdbcce7f4255b7c3e))
* **deps:** update dependency axios to ^0.26.0 ([#180](https://github.com/JustinBeckwith/retry-axios/issues/180)) ([1be27a6](https://github.com/JustinBeckwith/retry-axios/commit/1be27a65230f9b0ac6c95ea7c1234fe62f0ead35))
* **deps:** update actions/checkout action to v3 ([#183](https://github.com/JustinBeckwith/retry-axios/issues/183)) ([26da0a1](https://github.com/JustinBeckwith/retry-axios/commit/26da0a195d47ebd50d0720e36a8da9d89892fea1))
* **deps:** update actions/setup-node action to v3 ([#182](https://github.com/JustinBeckwith/retry-axios/issues/182)) ([34eb022](https://github.com/JustinBeckwith/retry-axios/commit/34eb02215ebb21d7a1acaf8c0d317f8ac080b276))
* **deps:** update dependency sinon to v13 ([#179](https://github.com/JustinBeckwith/retry-axios/issues/179)) ([2f8be7d](https://github.com/JustinBeckwith/retry-axios/commit/2f8be7d631c75754a95c6760ceac82e036ebee94))
* **deps:** update dependency axios to ^0.25.0 ([#170](https://github.com/JustinBeckwith/retry-axios/issues/170)) ([c28b386](https://github.com/JustinBeckwith/retry-axios/commit/c28b38675fa7531cb18684b2e8e29629a093bfe6))
* **deps:** update dependency @types/node to v16 ([#173](https://github.com/JustinBeckwith/retry-axios/issues/173)) ([d87d905](https://github.com/JustinBeckwith/retry-axios/commit/d87d9056167d9c429865f1a1cc6fe5b252d22bcf))
* **deps:** update dependency sinon to v12 ([#175](https://github.com/JustinBeckwith/retry-axios/issues/175)) ([cfd2616](https://github.com/JustinBeckwith/retry-axios/commit/cfd261640cdfcb45165768a63d83968ad895509c))
* **deps:** update dependency semantic-release to v18 ([#169](https://github.com/JustinBeckwith/retry-axios/issues/169)) ([19788c6](https://github.com/JustinBeckwith/retry-axios/commit/19788c6860c1800ade545a53395f8864b355f8b2))
* **deps:** update dependency mocha to v9 ([#151](https://github.com/JustinBeckwith/retry-axios/issues/151)) ([7baad4b](https://github.com/JustinBeckwith/retry-axios/commit/7baad4b045b68b2fad94effa66016495517aeff5))
* **deps:** update dependency sinon to v11 ([#153](https://github.com/JustinBeckwith/retry-axios/issues/153)) ([669477c](https://github.com/JustinBeckwith/retry-axios/commit/669477cf3ea863aa080b20de1721aa0d2ce394ca))
* **deps:** update dependency @types/sinon to v10 ([#152](https://github.com/JustinBeckwith/retry-axios/issues/152)) ([fc6670a](https://github.com/JustinBeckwith/retry-axios/commit/fc6670af0e6a76d62c56bd0dbc19158f771d0d41))
* **deps:** update codecov/codecov-action action to v2 ([#155](https://github.com/JustinBeckwith/retry-axios/issues/155)) ([b6d6965](https://github.com/JustinBeckwith/retry-axios/commit/b6d696537e79142c8d85b7554a95d6196b302b41))
* **deps:** update dependency typescript to ~4.3.0 ([#149](https://github.com/JustinBeckwith/retry-axios/issues/149)) ([be045e7](https://github.com/JustinBeckwith/retry-axios/commit/be045e7ad84896aa2eb2db743b3f168b5b16d100))
* **deps:** update dependency @types/node to v14 ([#150](https://github.com/JustinBeckwith/retry-axios/issues/150)) ([6ccc78b](https://github.com/JustinBeckwith/retry-axios/commit/6ccc78bfc033a8b6a6995ec195361ef7f494eacd))
* **deps:** update dependency typescript to ~4.2.0 ([#143](https://github.com/JustinBeckwith/retry-axios/issues/143)) ([97937ce](https://github.com/JustinBeckwith/retry-axios/commit/97937ce75b8af78d60332ba8d4194df40645925d))
* **deps:** update dependency js-green-licenses to v3 ([#140](https://github.com/JustinBeckwith/retry-axios/issues/140)) ([e198b4c](https://github.com/JustinBeckwith/retry-axios/commit/e198b4ce3d22d46e402d5b053fbf403d7ac7c64e))
* **deps:** update actions/setup-node action to v2 ([#134](https://github.com/JustinBeckwith/retry-axios/issues/134)) ([1143841](https://github.com/JustinBeckwith/retry-axios/commit/1143841427810a9045a57b9dded42281d2fea4f7))
* **deps:** upgrade to TypeScript ~4.1.0 ([#131](https://github.com/JustinBeckwith/retry-axios/issues/131)) ([74e1873](https://github.com/JustinBeckwith/retry-axios/commit/74e18731647fb8a4607284c264664dc5f5b48aaa))
* **deps:** update dependency gts to v3 ([#128](https://github.com/JustinBeckwith/retry-axios/issues/128)) ([b5201ed](https://github.com/JustinBeckwith/retry-axios/commit/b5201ed0e32af27c831bc016f48795a37a83e87a))
* **deps:** update dependency axios to ^0.21.0 ([#124](https://github.com/JustinBeckwith/retry-axios/issues/124)) ([8070501](https://github.com/JustinBeckwith/retry-axios/commit/8070501c7fd732ab2442c453b24f9e56f0e6b800))
* **deps:** update dependency typescript to v4 ([#123](https://github.com/JustinBeckwith/retry-axios/issues/123)) ([fd8aafa](https://github.com/JustinBeckwith/retry-axios/commit/fd8aafaad941b7c397cb3ce35b53e8876377608a))
* **deps:** update dependency @types/mocha to v8 ([#120](https://github.com/JustinBeckwith/retry-axios/issues/120)) ([c284310](https://github.com/JustinBeckwith/retry-axios/commit/c2843108e7d9758097cd1af89e09cd78c99bcebf))
* **deps:** update dependency nock to v13 ([#118](https://github.com/JustinBeckwith/retry-axios/issues/118)) ([386989a](https://github.com/JustinBeckwith/retry-axios/commit/386989aa4fb9d30e44e04cc29f3256d9e1808cb9))
* **deps:** update dependency mocha to v8 ([#115](https://github.com/JustinBeckwith/retry-axios/issues/115)) ([f996b0c](https://github.com/JustinBeckwith/retry-axios/commit/f996b0cbaaa48277b894dc6ae8606213895f8956))
* **deps:** update dependency typescript to ~3.9.0 ([#111](https://github.com/JustinBeckwith/retry-axios/issues/111)) ([d311e99](https://github.com/JustinBeckwith/retry-axios/commit/d311e99f80f49e65a1a56f1cd59e26c57ef6e199))
* **deps:** update dependency js-green-licenses to v2 ([#110](https://github.com/JustinBeckwith/retry-axios/issues/110)) ([5ddc262](https://github.com/JustinBeckwith/retry-axios/commit/5ddc262a2f414cb35ab23b85341a99198127214a))
* **deps:** upgrade to gts v2 ([#103](https://github.com/JustinBeckwith/retry-axios/issues/103)) ([fc8117e](https://github.com/JustinBeckwith/retry-axios/commit/fc8117e838c4e6764969e844707354bb8f85816d))
* **deps:** update dependency typescript to ~3.8.0 ([#97](https://github.com/JustinBeckwith/retry-axios/issues/97)) ([672adb6](https://github.com/JustinBeckwith/retry-axios/commit/672adb63ac97975744bb5056c4802612a298513f))
* **deps:** update dependency nock to v12 ([#96](https://github.com/JustinBeckwith/retry-axios/issues/96)) ([588df1d](https://github.com/JustinBeckwith/retry-axios/commit/588df1dda8a106cb59feeedfa48e02f0477ed8c2))
* **deps:** update dependency @types/mocha to v7 ([#88](https://github.com/JustinBeckwith/retry-axios/issues/88)) ([7fe186c](https://github.com/JustinBeckwith/retry-axios/commit/7fe186c8043d925cc5e718d2e00e1270bed8b6d5))
* **deps:** update dependency semantic-release to v17 ([#87](https://github.com/JustinBeckwith/retry-axios/issues/87)) ([76fd5ea](https://github.com/JustinBeckwith/retry-axios/commit/76fd5ea875db7b2c984f5dcf3914c60c4aff2ffb))
* **deps:** update dependency axios to ^0.19.0 ([#56](https://github.com/JustinBeckwith/retry-axios/issues/56)) ([d26d297](https://github.com/JustinBeckwith/retry-axios/commit/d26d297b036dead84557f8f13d12ba4530540d33))
* **deps:** update dependency typescript to ~3.7.0 ([#75](https://github.com/JustinBeckwith/retry-axios/issues/75)) ([aaeb80e](https://github.com/JustinBeckwith/retry-axios/commit/aaeb80e7b32b342c25dc8cdad22a78cfb68459e5))
* **deps:** update dependency mocha to v7 ([#78](https://github.com/JustinBeckwith/retry-axios/issues/78)) ([97dacf9](https://github.com/JustinBeckwith/retry-axios/commit/97dacf912889fbbe754bf9fe66e20a5cd23b3f30))
* **deps:** update dependency c8 to v7 ([#77](https://github.com/JustinBeckwith/retry-axios/issues/77)) ([919de4c](https://github.com/JustinBeckwith/retry-axios/commit/919de4cc08f54524cceeb1e2ae0205585b67ebb3))
* **deps:** update dependency semantic-release to v16 ([#79](https://github.com/JustinBeckwith/retry-axios/issues/79)) ([8fd56df](https://github.com/JustinBeckwith/retry-axios/commit/8fd56df05f1288069af81a098bbc1ac3327bfafa))
* **deps:** update dependency nock to v11 ([#66](https://github.com/JustinBeckwith/retry-axios/issues/66)) ([b2be0ac](https://github.com/JustinBeckwith/retry-axios/commit/b2be0ace3abb8dbbc4f52db9a8e877027bbabe23))
* **deps:** update dependency c8 to v6 ([#71](https://github.com/JustinBeckwith/retry-axios/issues/71)) ([26def05](https://github.com/JustinBeckwith/retry-axios/commit/26def052803eb6e31f471c3d0779dae6c4640c6b))
* **deps:** update dependency typescript to ~3.6.0 ([#65](https://github.com/JustinBeckwith/retry-axios/issues/65)) ([cc92d89](https://github.com/JustinBeckwith/retry-axios/commit/cc92d89fe56be4fc13bea46d60dd0cffffe6a332))
* **deps:** update commitlint monorepo to v8 (major) ([#55](https://github.com/JustinBeckwith/retry-axios/issues/55)) ([578a0bd](https://github.com/JustinBeckwith/retry-axios/commit/578a0bda08aa09d32eb4d9e7ac6f704833676a3a))
* **deps:** update dependency js-green-licenses to v1 ([#54](https://github.com/JustinBeckwith/retry-axios/issues/54)) ([5de61df](https://github.com/JustinBeckwith/retry-axios/commit/5de61df298713e77c5bb0a8be8956e41b3526d17))
* **deps:** update dependency typescript to ~3.5.0 ([#51](https://github.com/JustinBeckwith/retry-axios/issues/51)) ([7567361](https://github.com/JustinBeckwith/retry-axios/commit/7567361f041bdf00c4687c6165319a354eabadfb))
* **deps:** update dependency @types/nock to v10 ([#47](https://github.com/JustinBeckwith/retry-axios/issues/47)) ([e288e98](https://github.com/JustinBeckwith/retry-axios/commit/e288e9858d1b10b623ef4dc23e2a3e01b19ad852))
* **deps:** update dependency nyc to v14 ([#43](https://github.com/JustinBeckwith/retry-axios/issues/43)) ([f977f21](https://github.com/JustinBeckwith/retry-axios/commit/f977f2157f0ca6d8885d3cb66b5fac71f2428cbf))
* **deps:** update dependency typescript to ~3.4.0 ([#42](https://github.com/JustinBeckwith/retry-axios/issues/42)) ([07bff60](https://github.com/JustinBeckwith/retry-axios/commit/07bff6093af910a1735557b77b7efb91ab0a4588))
* **deps:** update dependency mocha to v6 ([#40](https://github.com/JustinBeckwith/retry-axios/issues/40)) ([5ff10a0](https://github.com/JustinBeckwith/retry-axios/commit/5ff10a012a5582f393c0aa8181aa95a5b9dc1044))
* **deps:** update dependency typescript to ~3.3.0 ([#36](https://github.com/JustinBeckwith/retry-axios/issues/36)) ([317bd6a](https://github.com/JustinBeckwith/retry-axios/commit/317bd6a9cda918acba148ad5e4f105b3d848a7bb))
* **deps:** update dependency typescript to ~3.2.0 ([#22](https://github.com/JustinBeckwith/retry-axios/issues/22)) ([e76c357](https://github.com/JustinBeckwith/retry-axios/commit/e76c357f6f2b1040c080949da27d1b794ab35c43))
* **deps:** update dependency nyc to v13 ([#19](https://github.com/JustinBeckwith/retry-axios/issues/19)) ([8b87273](https://github.com/JustinBeckwith/retry-axios/commit/8b8727348dfe76d147b6d0633c267376011f2264))
* **deps:** update dependency typescript to v3 ([#20](https://github.com/JustinBeckwith/retry-axios/issues/20)) ([bd63928](https://github.com/JustinBeckwith/retry-axios/commit/bd63928798f6d6cb3fbbf8eed730f28063bb7154))
* **deps:** update dependency gts to ^0.9.0 ([#17](https://github.com/JustinBeckwith/retry-axios/issues/17)) ([b21c76a](https://github.com/JustinBeckwith/retry-axios/commit/b21c76aca50607f203685de89e926786a205b5c0))
* **deps:** update dependency nock to v10 ([#18](https://github.com/JustinBeckwith/retry-axios/issues/18)) ([cf6802f](https://github.com/JustinBeckwith/retry-axios/commit/cf6802f2f6b83af48b7299a63851a8c10b8e0fc5))
* **package:** update nyc to version 12.0.2 ([#9](https://github.com/JustinBeckwith/retry-axios/issues/9)) ([fd191c3](https://github.com/JustinBeckwith/retry-axios/commit/fd191c34ef60db3c73a5471d1d3461fca38af414))
* **package:** update @types/node to version 10.0.3 ([#7](https://github.com/JustinBeckwith/retry-axios/issues/7)) ([4fcd328](https://github.com/JustinBeckwith/retry-axios/commit/4fcd32844b833bf5ea1e23182aca1239f447023b))
* **package:** update @types/mocha to version 5.0.0 ([#3](https://github.com/JustinBeckwith/retry-axios/issues/3)) ([4e12b40](https://github.com/JustinBeckwith/retry-axios/commit/4e12b40d2092edb32eb2e0241d7d8c285f01ffbf))
* **package:** update js-green-licenses to version 0.5.0 ([#2](https://github.com/JustinBeckwith/retry-axios/issues/2)) ([7f324a1](https://github.com/JustinBeckwith/retry-axios/commit/7f324a1a4e9ab84b3567723747741fc353a1d0b8))


### 🔖　Miscellaneous

* Configure Renovate (#16) ([c5d492d](https://github.com/JustinBeckwith/retry-axios/commit/c5d492d11af70933cc0e0eedc4b31ce9b0ea7470)), closes [#16](https://github.com/JustinBeckwith/retry-axios/issues/16)
* Fix documentation error (#14) ([0f768fb](https://github.com/JustinBeckwith/retry-axios/commit/0f768fb1e7f1e220f84df126153920a858dea1d8)), closes [#14](https://github.com/JustinBeckwith/retry-axios/issues/14)
* improve comments and readme ([39fe9dc](https://github.com/JustinBeckwith/retry-axios/commit/39fe9dc2482e50ef9f034b04ab96511303f248ef))
* initial commit ([18dc2ef](https://github.com/JustinBeckwith/retry-axios/commit/18dc2ef33f204e561911ad64c5877d98bb9ad2f2))
