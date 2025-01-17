# Changelog

### v0.3.12 (2022-09-25)

#### Features

* **check:** filter commits made by git revert (57837e8)
* **changelog:** filter max majors/minors/patches (cb508c6)
, closes #59
* use anyhow for error handling of commands (51abd51)

### v0.3.11 (2022-07-09)

#### Features

* **commit:** use template to format message (d408340)
, closes #54
* add `--first-parent` option to changelog and check command (f3b900c)
,
closes #60 #61 #67
* add `--merges` option for changelog and check command (2248da3)
, closes #60
#61 #67
* **changelog:** Support monorepo (d42285a)
* **version:** Support monorepo (f8ed823)
* **changelog:** include hidden sections on demand (618603d)
, closes #56

#### Fixes

* use scheme of url if available (e1d3910)
, closes #68
* **check:** fail for invalid commit types (d2a34a8)
, closes #53

### v0.3.10 (2022-04-24)

#### Fixes

* **changelog:** correctly format links (0286f48)
, closes #47
* set right version for unreleased repo (2d4d673)
, closes #49
* parse issue references correctly (#50) (b31ae66)
, closes #48
* support gitlab subgroups at url (#44) (995a527)

### v0.3.9 (2022-03-02)

#### Fixes

* **commit:** take BREAKING CHANGE footer into account for major version
change (712f455)
, closes #40
* add version flag back (910781e)

### v0.3.8 (2021-12-28)

#### Features

* **commit:** improve commit command (67ecc89)
, closes #36
* **changelog:** limit number of tags (632c5ca)
, closes #35

#### Fixes

* **commit:** ensure the cursor re-appears when interrupting (2f8d9f0)
,
closes #33 #33

### v0.3.7 (2021-10-13)

#### Features

* **commit:** empty message in editor aborts commit (260a5d2)
* **changelog:** add skip empty flag (c3f4972)
, closes #30
* **check:** add max-number option (a781286)
, closes #18

#### Fixes

* **commit:** do not require save for editor (5945dca)
* **commit:** ensure leading and trailing whitespaces are removed from
different fields that make up a commit message (4c6734f)
, closes #25
* **changelog:** limit lines in changelog to default of 80 characters to
address markdownlint issue MD013 (a01e53a)
, closes #20
* **changelog:** updated templates to address markdownlint issues MD032 and
MD022 (1a87e67)
, closes #20
* **changelog:** fixes whitespace issues (91b5b72)
, closes #20
* correct `is_prerelease()` for SemVer (0e99770)

### v0.3.5 (2021-05-01)

### v0.3.4 (2021-03-15)

#### Features

* **check:** improve error message for invalid scope (0790327)

### v0.3.3 (2021-02-12)

#### Features

* **changelog:** make commit body available in template context (7ce4722)

#### Fixes

* Remove debug log (8c7b1fc)

### v0.3.2 (2020-10-29)

#### Features

* **commit:** improve commit dialog (dee58c2)

### v0.3.1 (2020-08-30)

#### Features

* **commit:** improve commit dialog (acf3aea)

## v0.3.0 (2020-08-23)

### ⚠ BREAKING CHANGE

* changes behaviour if `--bump` is used in combination with `--major`, `--minor` or `--patch`


### Features

* **commit:** validate commit message created by `convco commit` (76b8ff4)
* Allow a custom scope regex in the configuration (dc03118)
, closes #8
* **changelog:** Add option to set custom template directory in `.versionrc`
(01c9ea9)
, closes #3

### Fixes

* **version:** prioritize `--major` `--minor` `--patch` over `--bump`
(8c728a8)

### v0.2.3 (2020-05-17)

#### Features

* relax regex for scope to allow -/_ as separator (61ee293)
* allow a scope to contain numbers (768492a)

### v0.2.2 (2020-02-16)

#### Features

* **changelog:** find host, owner and repository from the origin url
(2675fcb)

### v0.2.1 (2020-01-21)

#### Features

* **version:** Change rules for major version zero (592c77c)

#### Fixes

* **commit:** make cli require the commit type (8c434c3)
* **changelog:** use stop revision if range is given (9bd679d)

## v0.2.0 (2020-01-12)

### Features

* **commit:** a new commit subcommand added (5c47789)
, closes #5

### v0.1.1 (2019-12-29)

#### Fixes

* **changelog:** take the date of the tag or last commit of a version
(bf514cd)
, closes #2

## v0.1.0 (2019-12-26)

### Features

* **version:** add option to print bump label (a0777ca)
* **changelog:** sort sections (fe2c9a2)
* **changelog:** parse issue references (bd7f08f)
* **changelog:** add breaking changes and read `.versionrc` file. (e521814)
* Introduces convco with 3 tools: check, version and changelog. (116ad53)
