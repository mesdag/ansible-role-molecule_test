# 3.10.0 (2019-08-03)

## 🚀 New Features
- `@vue/cli`
  + #4342 Support `--port` argument to 'vue serve' command (@bokub)
- `@vue/cli-plugin-eslint`
  + #4329 feat(eslint-generator): upgrade @vue/eslint-config-prettier to v5.0.0 (@sodatea)

## 🐛 Bug Fix
- `@vue/cli-plugin-typescript`,`@vue/cli`
  + #4330 fix: require parent template after `when` condition evaluated as truth (@sodatea)
  + #4374 fix: when adding ts plugin without router, fixup #4330 (@cexbrayat)
- `@vue/cli-service`
  + #4359 fix stats display when chunkFilename contains query string (@flyhope)
- `@vue/cli-plugin-tvpescript`
  + #4346 fix: fix tvoo in typescript generator, convertAlIFiles -> convertJsToTs (@sodatea)
- `@vue/cli-pluain-eslint`
  + #4347 fix(eslint-generator): add ts file check to lint-staged (@liruifenqv)
  + #4329 feat(eslint-generator): upgrade @vue/eslint-confiq-prettier to v5.0.0 (@sodatea)
- `@vue/cli-shared-utils`
  + #4336 fix: use yarn `--version`` to detect yarn (@sodatea)
