# Changelog

## [1.4.1](https://github.com/antmelekhin/ansible-role-nginx/compare/v1.4.0...v1.4.1) (2024-08-11)


### Fixes

* fixed the default repository URL for Amazon Linux 2 ([cfc0bfe](https://github.com/antmelekhin/ansible-role-nginx/commit/cfc0bfe67a60d21cdcbe8cee540f9094ccdab95a))

## [1.4.0](https://github.com/antmelekhin/ansible-role-nginx/compare/v1.3.0...v1.4.0) (2024-08-11)


### Features

* add `meta/argument_specs.yml` file ([#7](https://github.com/antmelekhin/ansible-role-nginx/issues/7)) ([6e9a3bf](https://github.com/antmelekhin/ansible-role-nginx/commit/6e9a3bfd8dfa02950c95760c140b64268b403f3a))

## [1.3.0](https://github.com/antmelekhin/ansible-role-nginx/compare/v1.2.0...v1.3.0) (2024-08-08)


### Features

* add `fedora` and `amazonlinux` support ([#6](https://github.com/antmelekhin/ansible-role-nginx/issues/6)) ([299b6e2](https://github.com/antmelekhin/ansible-role-nginx/commit/299b6e2df54a83656f30eac3580d383b88a31344))

## [1.2.0](https://github.com/antmelekhin/ansible-role-nginx/compare/v1.1.4...v1.2.0) (2024-08-06)


### Improvements

* merge OS-specific variables into the `vars/main.yml` file ([#5](https://github.com/antmelekhin/ansible-role-nginx/issues/5)) ([4699ac7](https://github.com/antmelekhin/ansible-role-nginx/commit/4699ac7aaae42a587def9f0a58ffb291eeb43a4c))


### Styles

* update common role style ([#4](https://github.com/antmelekhin/ansible-role-nginx/issues/4)) ([c7b24d2](https://github.com/antmelekhin/ansible-role-nginx/commit/c7b24d20674d844e48d8d79d52e723cc76dc9ceb))


### Tests

* clean version output in the default scenario ([be71ba1](https://github.com/antmelekhin/ansible-role-nginx/commit/be71ba17e093ff290319d0f2b7d921832c6b1b94))

## [1.1.4](https://github.com/antmelekhin/ansible-role-nginx/compare/v1.1.3...v1.1.4) (2024-05-13)


### Documentation

* **README:** update variables documentation ([bddbdb9](https://github.com/antmelekhin/ansible-role-nginx/commit/bddbdb98dc9b01ef934000a92a43804e8a277aad))


### Styles

* add newline to end of file ([cb03fdc](https://github.com/antmelekhin/ansible-role-nginx/commit/cb03fdcbd4f7e5ac7cbaa14d4e420d46b3e0f67a))
* quote string ([78f9b0e](https://github.com/antmelekhin/ansible-role-nginx/commit/78f9b0ef6465b1ec82f3bc5234475f5d34d6f25a))
* rename tasks ([f3e5e30](https://github.com/antmelekhin/ansible-role-nginx/commit/f3e5e30cfad803ac1cd23c495c72550223545340))

## [1.1.3](https://github.com/antmelekhin/ansible-role-nginx/compare/v1.1.2...v1.1.3) (2024-04-26)


### Documentation

* **README:** fixed examples view for Ansible Galaxy ([86a849c](https://github.com/antmelekhin/ansible-role-nginx/commit/86a849c4147c3ad99d479e00b6495fb5a6697484))


### Fixes

* fixed running a role in `check_mode` ([d7c169d](https://github.com/antmelekhin/ansible-role-nginx/commit/d7c169d682cfa0706f7b13f926de09f5ff2855be))


### Styles

* use double underline regiter variable ([d6e37c8](https://github.com/antmelekhin/ansible-role-nginx/commit/d6e37c806cd66ad91a57dabea4907896f69ded40))


### Tests

* add .tox as ignore ([c996c1c](https://github.com/antmelekhin/ansible-role-nginx/commit/c996c1c90055c8bc0ff98ea6324a0e8651440311))
* add role_name prefix to instance name ([8053c07](https://github.com/antmelekhin/ansible-role-nginx/commit/8053c07040934086b56ece9451b5894249f36dfa))
* run linters in its own workflow ([3724b48](https://github.com/antmelekhin/ansible-role-nginx/commit/3724b4882103f5e79f1d435492359a5492b72c6a))

## [1.1.2](https://github.com/antmelekhin/ansible-role-nginx/compare/v1.1.1...v1.1.2) (2024-04-18)


### Code Refactoring

* update variable names, rm conditional expression, quote strings and rm loop for `include_vars` ([#3](https://github.com/antmelekhin/ansible-role-nginx/issues/3)) ([03272db](https://github.com/antmelekhin/ansible-role-nginx/commit/03272dbbd5e9ac3692722eb6938273055126658f))

## [1.1.1](https://github.com/antmelekhin/ansible-role-nginx/compare/v1.1.0...v1.1.1) (2024-04-18)


### Continuous Integration

* update release rules ([2527de5](https://github.com/antmelekhin/ansible-role-nginx/commit/2527de5bb2093b5d0e5dae851680b22bd20c6212))
* update workflows ([b628b6e](https://github.com/antmelekhin/ansible-role-nginx/commit/b628b6e023f25703e16facc0cf30fb13093e26e4))


### Documentation

* update repo description ([7a967cf](https://github.com/antmelekhin/ansible-role-nginx/commit/7a967cf43c794242db762aef18e141561cde0b0d))
* **README:** add additional example ([39d5152](https://github.com/antmelekhin/ansible-role-nginx/commit/39d51526a0c985c22b94db2065b785b205f2ab0d))


### Styles

* add `_nginx_apt_local_gpgkey` variable ([88149fa](https://github.com/antmelekhin/ansible-role-nginx/commit/88149faec74db6fad56a34ec263355fc97d27fbd))
* rename tasks ([04522ae](https://github.com/antmelekhin/ansible-role-nginx/commit/04522ae130ad3197fd30874e0551bef70106b085))

## [1.1.0](https://github.com/antmelekhin/ansible-role-nginx/compare/v1.0.0...v1.1.0) (2024-01-04)


### Improvements

* update variable names ([#2](https://github.com/antmelekhin/ansible-role-nginx/issues/2)) ([8a62141](https://github.com/antmelekhin/ansible-role-nginx/commit/8a6214181e67fd8de860864da6aa74d499081848))

## [1.0.0](https://github.com/antmelekhin/ansible-role-nginx/compare/...v1.0.0) (2023-08-27)


### Features

* initial commit ([db5d5c4](https://github.com/antmelekhin/ansible-role-nginx/commit/db5d5c493592c0c3e60de46935274755361294dd))
* initial commit ([8af3cb0](https://github.com/antmelekhin/ansible-role-nginx/commit/8af3cb01416b8846fd03305aed1bfe83dff5d35a))
