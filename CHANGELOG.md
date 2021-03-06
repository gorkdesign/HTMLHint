# [0.13.0](https://github.com/htmlhint/HTMLHint/compare/v0.12.2...v0.13.0) (2020-05-18)


### Bug Fixes

* add prettier and eslint ([#388](https://github.com/htmlhint/HTMLHint/issues/388)) ([aba3249](https://github.com/htmlhint/HTMLHint/commit/aba3249652181055f5897e0b4367b243f83ede3f))
* add semantic release test ([#399](https://github.com/htmlhint/HTMLHint/issues/399)) ([616f9cd](https://github.com/htmlhint/HTMLHint/commit/616f9cd74a9463e6596198f867f35aab24094110))
* ignore PULL_REQUEST_TEMPLATE.md ([30b0af2](https://github.com/htmlhint/HTMLHint/commit/30b0af2f86a4daa7ef3bd07e91e8220b7d4b75f3))
* use yml in semantic.yml ([86f6700](https://github.com/htmlhint/HTMLHint/commit/86f67007a32f5e978921507c05a2620edc1f9afc))


### Features

* Add tags checking rule - allows specify rules for any tag and validate that ([#384](https://github.com/htmlhint/HTMLHint/issues/384)) ([475aaca](https://github.com/htmlhint/HTMLHint/commit/475aaca431fab90a0ead7b21af7a73d4f0324514))
* added attr-no-unnecessary-whitespace rule ([#385](https://github.com/htmlhint/HTMLHint/issues/385)) ([03bfd4f](https://github.com/htmlhint/HTMLHint/commit/03bfd4f7f6b60543a4253cad74758c794fc8cd18))
* new rule: input-requires-label - All inputs require a label ([#159](https://github.com/htmlhint/HTMLHint/issues/159)) ([5bd40fb](https://github.com/htmlhint/HTMLHint/commit/5bd40fbc06b0d178cff4b9665ca992232dcb1f43))
* new website for htmlhint.com ([#395](https://github.com/htmlhint/HTMLHint/issues/395)) ([5d0d95f](https://github.com/htmlhint/HTMLHint/commit/5d0d95f39dddddf94a22d3c6294e4e50472fa0a0))

# HTMLHint change log

## ver 0.9.14 (2016-5-2)

add:

1. cli: support hint for url
2. attr-lowercase: add test case

## ver 0.9.13 (2016-5-1)

add:

1. change cli parameter: `--plugin` to `--rulesdir`
2. add formatter directory support
3. add formatters: compact, markdown
4. add cli parameter:`--nocolor`, disable color in cli
5. space-tab-mixed-disabled plugin: add space length require
6. add empty elements: track,command,source,keygen,wbr
7. add hint stdin for cli

fix:

1. report error evidence if tag attrs include `\r\n`
2. space-tab-mixed-disabled issue #119
3. attr name support all w3c defined characters

improve:

1. Parse inline ruleset after default ruleset

## ver 0.9.10 (2015-10-12)

add:

1. attr-unsafe-chars(rule): show unsafe code in message
2. support glob pattern for cli
3. support format as custom: json, junit, checkstyle
4. support plugin: `htmlhint --plugin ./plugins/`
5. add rule: inline-style-disabled
6. add rule: inline-script-disabled

fix:

1. title-require(rule): report error when `<html><title>test</title><head></head><body></body></html>`
2. title-require(rule): report error when `<html><head><title></title></head><body></body></html>`

## ver 0.9.9 (2015-10-9)

add:

1. add config loaded message to cli log
2. support async for cli

fix:

1. close issue: #79, fix exit with 0 when hint errors
2. fix end event col
3. attr-unsafe-chars(rule): exclude `\r\n`

## ver 0.9.8 (2015-10-7)

add:

1. Search `.htmlhintrc` in parent directory
2. Allow comments in json
3. Support hint any file without `.html` or `.htm` extension, just like: `htmlhint test.xhtml`
4. Support json raw format in cli
5. tag-pair(rule): Show the line of the start tag
6. space-tab-mixed-disabled(rule): Support space and tab mode, for check only space or tab
7. Make cli logs more clear to people
8. add rule: title-require, `<title>` must be present in `<head>` tag.

fix:

1. Fix issue: #77 `<link rel=icon><link rel=icon>`
2. Made the descriptions and error messages of rules more clear to people
3. head-script-disabled(fule): No head not result error

## ver 0.9.7 (2015-3-8)

fix:

1. fix 'No such file' issue on mac
2. head-script-disabled: not match template script

## ver 0.9.6 (2014-6-18)

add:

1. add rule: attr-no-duplication
2. add rule: space-tab-mixed-disabled
3. add rule: id-class-ad-disabled
4. add rule: href-abs-or-rel
5. add rule: attr-unsafe-chars
6. add default rule: attr-no-duplication
7. add inline ruleset support
8. add test spec: Set false to rule
9. add point: load default ruleset when use empty ruleset

## ver 0.9.4 (2013-9-27)

1. add rule: src-not-empty

fix:

1. fix attr-value-double-quotes rule: `<img src=''>` should result error

## ver 0.9.3 (2013-5-24)

add:

1. add ruleid to csslint message

fix:

1. fix csslint rule: del undefined of raw
2. fix parser for: `<div class="foo""><a><span">`

## ver 0.9.2 (2013-4-6)

add：

1. add rule: csslint
2. add rule: jshint
3. add rule: id-unique
4. add cli

fix：

1.  compatible with:

        <div class="foo"
        <div class"foo">
        <div class=foo">
        <div class="foo>

## ver 0.9.1 (2013-3-23)

add:

1. add rule: attr-lowercase
2. add rule: attr-value-double-quotes
3. add rule: attr-value-not-empty
4. add rule: doctype-first
5. add rule: doctype-html5
6. add rule: head-script-disabled
7. add rule: id-class-value
8. add rule: img-alt-require
9. add rule: spec-char-escape
10. add rule: style-disabled
11. add rule: tagname-lowercase
12. add rule: tag-pair
13. add rule: tag-self-close
