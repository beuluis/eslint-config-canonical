# Canonical ESLint Config

[![Travis build status](http://img.shields.io/travis/gajus/eslint-config-canonical/master.svg?style=flat-square)](https://travis-ci.org/gajus/eslint-config-canonical)
[![NPM version](http://img.shields.io/npm/v/eslint-config-canonical.svg?style=flat-square)](https://www.npmjs.org/package/eslint-config-canonical)

Canonical is the most comprehensive code style guide. It consists of more than 800 rules, some of which are custom written for Canonical (e.g. [eslint-plugin-jsdoc](https://github.com/gajus/eslint-plugin-jsdoc), [eslint-plugin-flowtype](https://github.com/gajus/eslint-plugin-flowtype)).

The goal of the Canonical style guide is to reduce noise in code version control and promote use of the latest ES features.

## Usage

This package includes the following configurations:

* [`canonical`](./configurations/eslintrc.json) – The Canonical code style guide.
* [`canonical/ava`](./configurations/ava.json) – To be used in addition to "canonical" configuration by projects that use [AVA](https://ava.li/).
* [`canonical/flowtype`](./configurations/flowtype.json) – To be used in addition to "canonical" configuration by projects that use [Flowtype](https://flowtype.org/).
* [`canonical/jest`](./configurations/jest.json) – To be used in addition to "canonical" configuration by projects that use [jest](https://facebook.github.io/jest/).
* [`canonical/lodash`](./configurations/lodash.json) – To be used in addition to "canonical" configuration by projects that use [lodash](https://lodash.com/).
* [`canonical/mocha`](./configurations/mocha.json) – To be used in addition to "canonical" configuration by projects that use [Mocha](https://mochajs.org/).
* [`canonical/react`](./configurations/react.json) – To be used in addition to "canonical" configuration by projects that use [React](https://facebook.github.io/react/).

Example:

```json
{
  "extends": [
    "canonical",
    "canonical/ava",
    "canonical/flowtype",
    "canonical/jest",
    "canonical/lodash",
    "canonical/mocha",
    "canonical/react"
  ]
}
```

## Versioning Policy

All breaking changes will bump the major version as per the semver convention. Therefore, every new rule addition will increase the major version.

## Table of comparison

This how Canonical ruleset compares to other popular configurations.

<!-- This comparison is created using `./compare` script. -->

|Rule|Canonical|AirBnb|
|---|---|---|
|accessor-pairs|error|"accessor-pairs"|
|array-bracket-newline|"array-bracket-newline"|"array-bracket-newline"|
|array-bracket-spacing|"array-bracket-spacing"|"array-bracket-spacing"|
|array-callback-return|error|"array-callback-return"|
|array-element-newline|"array-element-newline"|"array-element-newline"|
|arrow-body-style|"arrow-body-style"|"arrow-body-style"|
|arrow-parens|"arrow-parens"|"arrow-parens"|
|arrow-spacing|"arrow-spacing"|"arrow-spacing"|
|ava/assertion-arguments|error|N/A|
|ava/max-asserts|"ava/max-asserts"|N/A|
|ava/no-async-fn-without-await|error|N/A|
|ava/no-cb-test|error|N/A|
|ava/no-duplicate-modifiers|error|N/A|
|ava/no-identical-title|error|N/A|
|ava/no-ignored-test-files|error|N/A|
|ava/no-import-test-files|error|N/A|
|ava/no-invalid-end|error|N/A|
|ava/no-nested-tests|error|N/A|
|ava/no-only-test|error|N/A|
|ava/no-skip-assert|error|N/A|
|ava/no-skip-test|error|N/A|
|ava/no-statement-after-end|error|N/A|
|ava/no-todo-implementation|error|N/A|
|ava/no-todo-test|warn|N/A|
|ava/no-unknown-modifiers|error|N/A|
|ava/prefer-async-await|error|N/A|
|ava/prefer-power-assert|error|N/A|
|ava/test-ended|error|N/A|
|ava/test-title|"ava/test-title"|N/A|
|ava/use-t|error|N/A|
|ava/use-t-well|error|N/A|
|ava/use-test|error|N/A|
|ava/use-true-false|error|N/A|
|babel/new-cap|"babel/new-cap"|N/A|
|babel/no-invalid-this|error|N/A|
|babel/object-curly-spacing|"babel/object-curly-spacing"|N/A|
|babel/valid-typeof|error|N/A|
|block-scoped-var|error|"block-scoped-var"|
|block-spacing|"block-spacing"|"block-spacing"|
|brace-style|"brace-style"|"brace-style"|
|callback-return|error|"callback-return"|
|camelcase|"camelcase"|"camelcase"|
|capitalized-comments|"capitalized-comments"|"capitalized-comments"|
|class-methods-use-this|error|"class-methods-use-this"|
|comma-dangle|"comma-dangle"|"comma-dangle"|
|comma-spacing|"comma-spacing"|"comma-spacing"|
|comma-style|"comma-style"|"comma-style"|
|complexity|"complexity"|"complexity"|
|computed-property-spacing|"computed-property-spacing"|"computed-property-spacing"|
|consistent-return|error|"consistent-return"|
|consistent-this|"consistent-this"|"consistent-this"|
|constructor-super|error|"constructor-super"|
|curly|error|"curly"|
|default-case|"default-case"|"default-case"|
|dot-location|"dot-location"|"dot-location"|
|dot-notation|error|"dot-notation"|
|eol-last|error|"eol-last"|
|eqeqeq|error|"eqeqeq"|
|filenames/match-exported|error|N/A|
|filenames/match-regex|"filenames/match-regex"|N/A|
|filenames/no-index|"filenames/no-index"|N/A|
|flowtype/boolean-style|"flowtype/boolean-style"|N/A|
|flowtype/define-flow-type|warn|N/A|
|flowtype/delimiter-dangle|"flowtype/delimiter-dangle"|N/A|
|flowtype/generic-spacing|"flowtype/generic-spacing"|N/A|
|flowtype/newline-after-flow-annotation|error|N/A|
|flowtype/no-existential-type|"flowtype/no-existential-type"|N/A|
|flowtype/no-flow-fix-me-comments|warn|N/A|
|flowtype/no-mutable-array|error|N/A|
|flowtype/no-primitive-constructor-types|error|N/A|
|flowtype/no-types-missing-file-annotation|error|N/A|
|flowtype/no-unused-expressions|"flowtype/no-unused-expressions"|N/A|
|flowtype/no-weak-types|error|N/A|
|flowtype/object-type-delimiter|"flowtype/object-type-delimiter"|N/A|
|flowtype/require-exact-type|warn|N/A|
|flowtype/require-parameter-type|"flowtype/require-parameter-type"|N/A|
|flowtype/require-return-type|"flowtype/require-return-type"|N/A|
|flowtype/require-types-at-top|error|N/A|
|flowtype/require-valid-file-annotation|error|N/A|
|flowtype/require-variable-type|"flowtype/require-variable-type"|N/A|
|flowtype/semi|"flowtype/semi"|N/A|
|flowtype/sort-keys|"flowtype/sort-keys"|N/A|
|flowtype/space-after-type-colon|"flowtype/space-after-type-colon"|N/A|
|flowtype/space-before-generic-bracket|"flowtype/space-before-generic-bracket"|N/A|
|flowtype/space-before-type-colon|"flowtype/space-before-type-colon"|N/A|
|flowtype/type-id-match|"flowtype/type-id-match"|N/A|
|flowtype/type-import-style|"flowtype/type-import-style"|N/A|
|flowtype/union-intersection-spacing|"flowtype/union-intersection-spacing"|N/A|
|flowtype/use-flow-type|warn|N/A|
|for-direction|error|"for-direction"|
|func-call-spacing|"func-call-spacing"|"func-call-spacing"|
|func-name-matching|error|"func-name-matching"|
|func-names|"func-names"|"func-names"|
|func-style|"func-style"|"func-style"|
|function-paren-newline|"function-paren-newline"|"function-paren-newline"|
|generator-star-spacing|"generator-star-spacing"|"generator-star-spacing"|
|getter-return|N/A|"getter-return"|
|global-require|error|"global-require"|
|guard-for-in|error|"guard-for-in"|
|handle-callback-err|error|"handle-callback-err"|
|id-blacklist|N/A|"id-blacklist"|
|id-length|"id-length"|"id-length"|
|id-match|"id-match"|"id-match"|
|implicit-arrow-linebreak|"implicit-arrow-linebreak"|"implicit-arrow-linebreak"|
|import/default|error|"import/default"|
|import/dynamic-import-chunkname|N/A|"import/dynamic-import-chunkname"|
|import/export|error|"import/export"|
|import/exports-last|error|"import/exports-last"|
|import/extensions|"import/extensions"|"import/extensions"|
|import/first|"import/first"|"import/first"|
|import/group-exports|"import/group-exports"|"import/group-exports"|
|import/imports-first|N/A|"import/imports-first"|
|import/max-dependencies|"import/max-dependencies"|"import/max-dependencies"|
|import/named|error|"import/named"|
|import/namespace|error|"import/namespace"|
|import/newline-after-import|error|"import/newline-after-import"|
|import/no-absolute-path|error|"import/no-absolute-path"|
|import/no-amd|error|"import/no-amd"|
|import/no-anonymous-default-export|"import/no-anonymous-default-export"|"import/no-anonymous-default-export"|
|import/no-commonjs|error|"import/no-commonjs"|
|import/no-cycle|error|"import/no-cycle"|
|import/no-default-export|"import/no-default-export"|"import/no-default-export"|
|import/no-deprecated|warn|"import/no-deprecated"|
|import/no-duplicates|"import/no-duplicates"|"import/no-duplicates"|
|import/no-dynamic-require|error|"import/no-dynamic-require"|
|import/no-extraneous-dependencies|"import/no-extraneous-dependencies"|"import/no-extraneous-dependencies"|
|import/no-internal-modules|"import/no-internal-modules"|"import/no-internal-modules"|
|import/no-mutable-exports|error|"import/no-mutable-exports"|
|import/no-named-as-default|error|"import/no-named-as-default"|
|import/no-named-as-default-member|error|"import/no-named-as-default-member"|
|import/no-named-default|error|"import/no-named-default"|
|import/no-namespace|error|"import/no-namespace"|
|import/no-nodejs-modules|"import/no-nodejs-modules"|"import/no-nodejs-modules"|
|import/no-relative-parent-imports|"import/no-relative-parent-imports"|"import/no-relative-parent-imports"|
|import/no-restricted-paths|"import/no-restricted-paths"|"import/no-restricted-paths"|
|import/no-self-import|error|"import/no-self-import"|
|import/no-unassigned-import|error|"import/no-unassigned-import"|
|import/no-unresolved|error|"import/no-unresolved"|
|import/no-useless-path-segments|error|"import/no-useless-path-segments"|
|import/no-webpack-loader-syntax|error|"import/no-webpack-loader-syntax"|
|import/order|"import/order"|"import/order"|
|import/prefer-default-export|warn|"import/prefer-default-export"|
|import/unambiguous|warn|"import/unambiguous"|
|indent|"indent"|"indent"|
|init-declarations|"init-declarations"|"init-declarations"|
|jest/no-disabled-tests|"jest/no-disabled-tests"|N/A|
|jest/no-focused-tests|"jest/no-focused-tests"|N/A|
|jest/no-identical-title|"jest/no-identical-title"|N/A|
|jest/valid-expect|"jest/valid-expect"|N/A|
|jsdoc/check-param-names|warn|N/A|
|jsdoc/check-tag-names|warn|N/A|
|jsdoc/check-types|warn|N/A|
|jsdoc/newline-after-description|"jsdoc/newline-after-description"|N/A|
|jsdoc/require-description-complete-sentence|"jsdoc/require-description-complete-sentence"|N/A|
|jsdoc/require-hyphen-before-param-description|"jsdoc/require-hyphen-before-param-description"|N/A|
|jsdoc/require-param|"jsdoc/require-param"|N/A|
|jsdoc/require-param-description|"jsdoc/require-param-description"|N/A|
|jsdoc/require-param-name|error|N/A|
|jsdoc/require-param-type|"jsdoc/require-param-type"|N/A|
|jsdoc/require-returns-description|"jsdoc/require-returns-description"|N/A|
|jsdoc/require-returns-type|"jsdoc/require-returns-type"|N/A|
|jsx-a11y/accessible-emoji|N/A|"jsx-a11y/accessible-emoji"|
|jsx-a11y/alt-text|N/A|"jsx-a11y/alt-text"|
|jsx-a11y/anchor-has-content|N/A|"jsx-a11y/anchor-has-content"|
|jsx-a11y/anchor-is-valid|N/A|"jsx-a11y/anchor-is-valid"|
|jsx-a11y/aria-activedescendant-has-tabindex|N/A|"jsx-a11y/aria-activedescendant-has-tabindex"|
|jsx-a11y/aria-props|N/A|"jsx-a11y/aria-props"|
|jsx-a11y/aria-proptypes|N/A|"jsx-a11y/aria-proptypes"|
|jsx-a11y/aria-role|N/A|"jsx-a11y/aria-role"|
|jsx-a11y/aria-unsupported-elements|N/A|"jsx-a11y/aria-unsupported-elements"|
|jsx-a11y/click-events-have-key-events|N/A|"jsx-a11y/click-events-have-key-events"|
|jsx-a11y/heading-has-content|N/A|"jsx-a11y/heading-has-content"|
|jsx-a11y/html-has-lang|N/A|"jsx-a11y/html-has-lang"|
|jsx-a11y/iframe-has-title|N/A|"jsx-a11y/iframe-has-title"|
|jsx-a11y/img-redundant-alt|N/A|"jsx-a11y/img-redundant-alt"|
|jsx-a11y/interactive-supports-focus|N/A|"jsx-a11y/interactive-supports-focus"|
|jsx-a11y/label-has-associated-control|N/A|"jsx-a11y/label-has-associated-control"|
|jsx-a11y/label-has-for|N/A|"jsx-a11y/label-has-for"|
|jsx-a11y/lang|N/A|"jsx-a11y/lang"|
|jsx-a11y/media-has-caption|N/A|"jsx-a11y/media-has-caption"|
|jsx-a11y/mouse-events-have-key-events|N/A|"jsx-a11y/mouse-events-have-key-events"|
|jsx-a11y/no-access-key|N/A|"jsx-a11y/no-access-key"|
|jsx-a11y/no-autofocus|N/A|"jsx-a11y/no-autofocus"|
|jsx-a11y/no-distracting-elements|N/A|"jsx-a11y/no-distracting-elements"|
|jsx-a11y/no-interactive-element-to-noninteractive-role|N/A|"jsx-a11y/no-interactive-element-to-noninteractive-role"|
|jsx-a11y/no-noninteractive-element-interactions|N/A|"jsx-a11y/no-noninteractive-element-interactions"|
|jsx-a11y/no-noninteractive-element-to-interactive-role|N/A|"jsx-a11y/no-noninteractive-element-to-interactive-role"|
|jsx-a11y/no-noninteractive-tabindex|N/A|"jsx-a11y/no-noninteractive-tabindex"|
|jsx-a11y/no-onchange|N/A|"jsx-a11y/no-onchange"|
|jsx-a11y/no-redundant-roles|N/A|"jsx-a11y/no-redundant-roles"|
|jsx-a11y/no-static-element-interactions|N/A|"jsx-a11y/no-static-element-interactions"|
|jsx-a11y/role-has-required-aria-props|N/A|"jsx-a11y/role-has-required-aria-props"|
|jsx-a11y/role-supports-aria-props|N/A|"jsx-a11y/role-supports-aria-props"|
|jsx-a11y/scope|N/A|"jsx-a11y/scope"|
|jsx-a11y/tabindex-no-positive|N/A|"jsx-a11y/tabindex-no-positive"|
|jsx-quotes|"jsx-quotes"|"jsx-quotes"|
|key-spacing|"key-spacing"|"key-spacing"|
|keyword-spacing|"keyword-spacing"|"keyword-spacing"|
|line-comment-position|"line-comment-position"|"line-comment-position"|
|linebreak-style|"linebreak-style"|"linebreak-style"|
|lines-around-comment|"lines-around-comment"|"lines-around-comment"|
|lines-around-directive|"lines-around-directive"|"lines-around-directive"|
|lines-between-class-members|"lines-between-class-members"|"lines-between-class-members"|
|lodash/callback-binding|warn|N/A|
|lodash/chain-style|"lodash/chain-style"|N/A|
|lodash/chaining|"lodash/chaining"|N/A|
|lodash/collection-method-value|warn|N/A|
|lodash/collection-return|warn|N/A|
|lodash/consistent-compose|"lodash/consistent-compose"|N/A|
|lodash/identity-shorthand|"lodash/identity-shorthand"|N/A|
|lodash/import-scope|"lodash/import-scope"|N/A|
|lodash/matches-prop-shorthand|warn|N/A|
|lodash/matches-shorthand|"lodash/matches-shorthand"|N/A|
|lodash/no-commit|warn|N/A|
|lodash/no-double-unwrap|warn|N/A|
|lodash/no-extra-args|warn|N/A|
|lodash/path-style|"lodash/path-style"|N/A|
|lodash/prefer-compact|warn|N/A|
|lodash/prefer-constant|"lodash/prefer-constant"|N/A|
|lodash/prefer-filter|"lodash/prefer-filter"|N/A|
|lodash/prefer-find|error|N/A|
|lodash/prefer-get|"lodash/prefer-get"|N/A|
|lodash/prefer-immutable-method|error|N/A|
|lodash/prefer-includes|warn|N/A|
|lodash/prefer-invoke-map|"lodash/prefer-invoke-map"|N/A|
|lodash/prefer-is-nil|warn|N/A|
|lodash/prefer-lodash-chain|warn|N/A|
|lodash/prefer-lodash-method|"lodash/prefer-lodash-method"|N/A|
|lodash/prefer-lodash-typecheck|warn|N/A|
|lodash/prefer-map|warn|N/A|
|lodash/prefer-matches|warn|N/A|
|lodash/prefer-noop|"lodash/prefer-noop"|N/A|
|lodash/prefer-over-quantifier|warn|N/A|
|lodash/prefer-reject|"lodash/prefer-reject"|N/A|
|lodash/prefer-startswith|"lodash/prefer-startswith"|N/A|
|lodash/prefer-thru|warn|N/A|
|lodash/prefer-times|warn|N/A|
|lodash/prefer-wrapper-method|warn|N/A|
|lodash/preferred-alias|warn|N/A|
|lodash/prop-shorthand|warn|N/A|
|lodash/unwrap|warn|N/A|
|max-classes-per-file|N/A|"max-classes-per-file"|
|max-depth|N/A|"max-depth"|
|max-len|"max-len"|"max-len"|
|max-lines|N/A|"max-lines"|
|max-lines-per-function|N/A|"max-lines-per-function"|
|max-nested-callbacks|"max-nested-callbacks"|"max-nested-callbacks"|
|max-params|N/A|"max-params"|
|max-statements|N/A|"max-statements"|
|max-statements-per-line|"max-statements-per-line"|"max-statements-per-line"|
|mocha/max-top-level-suites|"mocha/max-top-level-suites"|N/A|
|mocha/no-exclusive-tests|error|N/A|
|mocha/no-hooks-for-single-case|warn|N/A|
|mocha/no-identical-title|error|N/A|
|mocha/no-nested-tests|error|N/A|
|mocha/no-return-and-callback|error|N/A|
|mocha/no-setup-in-describe|error|N/A|
|mocha/no-top-level-hooks|error|N/A|
|multiline-comment-style|"multiline-comment-style"|"multiline-comment-style"|
|multiline-ternary|"multiline-ternary"|"multiline-ternary"|
|new-cap|"new-cap"|"new-cap"|
|new-parens|error|"new-parens"|
|newline-after-var|"newline-after-var"|"newline-after-var"|
|newline-before-return|error|"newline-before-return"|
|newline-per-chained-call|"newline-per-chained-call"|"newline-per-chained-call"|
|no-alert|error|"no-alert"|
|no-array-constructor|error|"no-array-constructor"|
|no-async-promise-executor|error|"no-async-promise-executor"|
|no-await-in-loop|"no-await-in-loop"|"no-await-in-loop"|
|no-bitwise|N/A|"no-bitwise"|
|no-buffer-constructor|error|"no-buffer-constructor"|
|no-caller|error|"no-caller"|
|no-case-declarations|error|"no-case-declarations"|
|no-catch-shadow|error|"no-catch-shadow"|
|no-class-assign|error|"no-class-assign"|
|no-compare-neg-zero|error|"no-compare-neg-zero"|
|no-cond-assign|error|"no-cond-assign"|
|no-confusing-arrow|error|"no-confusing-arrow"|
|no-console|error|"no-console"|
|no-const-assign|error|"no-const-assign"|
|no-constant-condition|warn|"no-constant-condition"|
|no-continue|error|"no-continue"|
|no-control-regex|error|"no-control-regex"|
|no-debugger|warn|"no-debugger"|
|no-delete-var|error|"no-delete-var"|
|no-div-regex|error|"no-div-regex"|
|no-dupe-args|error|"no-dupe-args"|
|no-dupe-class-members|error|"no-dupe-class-members"|
|no-dupe-keys|error|"no-dupe-keys"|
|no-duplicate-case|error|"no-duplicate-case"|
|no-duplicate-imports|error|"no-duplicate-imports"|
|no-else-return|"no-else-return"|"no-else-return"|
|no-empty|error|"no-empty"|
|no-empty-character-class|error|"no-empty-character-class"|
|no-empty-function|N/A|"no-empty-function"|
|no-empty-pattern|error|"no-empty-pattern"|
|no-eq-null|error|"no-eq-null"|
|no-eval|error|"no-eval"|
|no-ex-assign|error|"no-ex-assign"|
|no-extend-native|error|"no-extend-native"|
|no-extra-bind|error|"no-extra-bind"|
|no-extra-boolean-cast|"no-extra-boolean-cast"|"no-extra-boolean-cast"|
|no-extra-label|N/A|"no-extra-label"|
|no-extra-parens|error|"no-extra-parens"|
|no-extra-semi|error|"no-extra-semi"|
|no-fallthrough|error|"no-fallthrough"|
|no-floating-decimal|error|"no-floating-decimal"|
|no-func-assign|error|"no-func-assign"|
|no-global-assign|error|"no-global-assign"|
|no-implicit-coercion|error|"no-implicit-coercion"|
|no-implicit-globals|"no-implicit-globals"|"no-implicit-globals"|
|no-implied-eval|error|"no-implied-eval"|
|no-inline-comments|error|"no-inline-comments"|
|no-inner-declarations|error|"no-inner-declarations"|
|no-invalid-regexp|error|"no-invalid-regexp"|
|no-invalid-this|"no-invalid-this"|"no-invalid-this"|
|no-irregular-whitespace|error|"no-irregular-whitespace"|
|no-iterator|error|"no-iterator"|
|no-label-var|error|"no-label-var"|
|no-labels|error|"no-labels"|
|no-lone-blocks|error|"no-lone-blocks"|
|no-lonely-if|error|"no-lonely-if"|
|no-loop-func|error|"no-loop-func"|
|no-magic-numbers|"no-magic-numbers"|"no-magic-numbers"|
|no-misleading-character-class|error|"no-misleading-character-class"|
|no-mixed-operators|N/A|"no-mixed-operators"|
|no-mixed-requires|"no-mixed-requires"|"no-mixed-requires"|
|no-mixed-spaces-and-tabs|error|"no-mixed-spaces-and-tabs"|
|no-multi-assign|N/A|"no-multi-assign"|
|no-multi-spaces|error|"no-multi-spaces"|
|no-multi-str|error|"no-multi-str"|
|no-multiple-empty-lines|"no-multiple-empty-lines"|"no-multiple-empty-lines"|
|no-native-reassign|error|"no-native-reassign"|
|no-negated-condition|error|"no-negated-condition"|
|no-negated-in-lhs|error|"no-negated-in-lhs"|
|no-nested-ternary|error|"no-nested-ternary"|
|no-new|error|"no-new"|
|no-new-func|error|"no-new-func"|
|no-new-object|error|"no-new-object"|
|no-new-require|error|"no-new-require"|
|no-new-symbol|error|"no-new-symbol"|
|no-new-wrappers|error|"no-new-wrappers"|
|no-obj-calls|error|"no-obj-calls"|
|no-octal|error|"no-octal"|
|no-octal-escape|error|"no-octal-escape"|
|no-param-reassign|"no-param-reassign"|"no-param-reassign"|
|no-path-concat|error|"no-path-concat"|
|no-plusplus|N/A|"no-plusplus"|
|no-process-env|error|"no-process-env"|
|no-process-exit|error|"no-process-exit"|
|no-proto|error|"no-proto"|
|no-prototype-builtins|N/A|"no-prototype-builtins"|
|no-redeclare|"no-redeclare"|"no-redeclare"|
|no-regex-spaces|error|"no-regex-spaces"|
|no-restricted-globals|"no-restricted-globals"|"no-restricted-globals"|
|no-restricted-imports|N/A|"no-restricted-imports"|
|no-restricted-modules|"no-restricted-modules"|"no-restricted-modules"|
|no-restricted-properties|"no-restricted-properties"|"no-restricted-properties"|
|no-restricted-syntax|"no-restricted-syntax"|"no-restricted-syntax"|
|no-return-assign|error|"no-return-assign"|
|no-return-await|error|"no-return-await"|
|no-script-url|error|"no-script-url"|
|no-self-assign|error|"no-self-assign"|
|no-self-compare|error|"no-self-compare"|
|no-sequences|error|"no-sequences"|
|no-shadow|"no-shadow"|"no-shadow"|
|no-shadow-restricted-names|error|"no-shadow-restricted-names"|
|no-spaced-func|error|"no-spaced-func"|
|no-sparse-arrays|error|"no-sparse-arrays"|
|no-sync|"no-sync"|"no-sync"|
|no-tabs|error|"no-tabs"|
|no-template-curly-in-string|error|"no-template-curly-in-string"|
|no-ternary|"no-ternary"|"no-ternary"|
|no-this-before-super|error|"no-this-before-super"|
|no-throw-literal|error|"no-throw-literal"|
|no-trailing-spaces|error|"no-trailing-spaces"|
|no-undef|error|"no-undef"|
|no-undef-init|error|"no-undef-init"|
|no-undefined|"no-undefined"|"no-undefined"|
|no-underscore-dangle|"no-underscore-dangle"|"no-underscore-dangle"|
|no-unexpected-multiline|error|"no-unexpected-multiline"|
|no-unmodified-loop-condition|error|"no-unmodified-loop-condition"|
|no-unneeded-ternary|error|"no-unneeded-ternary"|
|no-unreachable|warn|"no-unreachable"|
|no-unsafe-finally|error|"no-unsafe-finally"|
|no-unsafe-negation|error|"no-unsafe-negation"|
|no-unused-expressions|error|"no-unused-expressions"|
|no-unused-labels|N/A|"no-unused-labels"|
|no-unused-vars|error|"no-unused-vars"|
|no-use-before-define|error|"no-use-before-define"|
|no-use-extend-native/no-use-extend-native|error|N/A|
|no-useless-call|error|"no-useless-call"|
|no-useless-computed-key|error|"no-useless-computed-key"|
|no-useless-concat|error|"no-useless-concat"|
|no-useless-constructor|error|"no-useless-constructor"|
|no-useless-escape|error|"no-useless-escape"|
|no-useless-rename|"no-useless-rename"|"no-useless-rename"|
|no-useless-return|error|"no-useless-return"|
|no-var|error|"no-var"|
|no-void|error|"no-void"|
|no-warning-comments|"no-warning-comments"|"no-warning-comments"|
|no-whitespace-before-property|error|"no-whitespace-before-property"|
|no-with|error|"no-with"|
|nonblock-statement-body-position|"nonblock-statement-body-position"|"nonblock-statement-body-position"|
|object-curly-newline|N/A|"object-curly-newline"|
|object-curly-spacing|"object-curly-spacing"|"object-curly-spacing"|
|object-property-newline|"object-property-newline"|"object-property-newline"|
|object-shorthand|"object-shorthand"|"object-shorthand"|
|one-var|"one-var"|"one-var"|
|one-var-declaration-per-line|error|"one-var-declaration-per-line"|
|operator-assignment|"operator-assignment"|"operator-assignment"|
|operator-linebreak|"operator-linebreak"|"operator-linebreak"|
|padded-blocks|"padded-blocks"|"padded-blocks"|
|padding-line-between-statements|"padding-line-between-statements"|"padding-line-between-statements"|
|prefer-arrow-callback|error|"prefer-arrow-callback"|
|prefer-const|error|"prefer-const"|
|prefer-destructuring|"prefer-destructuring"|"prefer-destructuring"|
|prefer-numeric-literals|error|"prefer-numeric-literals"|
|prefer-object-spread|N/A|"prefer-object-spread"|
|prefer-promise-reject-errors|error|"prefer-promise-reject-errors"|
|prefer-reflect|"prefer-reflect"|"prefer-reflect"|
|prefer-rest-params|error|"prefer-rest-params"|
|prefer-spread|error|"prefer-spread"|
|prefer-template|"prefer-template"|"prefer-template"|
|promise/always-return|error|N/A|
|promise/avoid-new|"promise/avoid-new"|N/A|
|promise/catch-or-return|error|N/A|
|promise/no-callback-in-promise|"promise/no-callback-in-promise"|N/A|
|promise/no-native|"promise/no-native"|N/A|
|promise/no-nesting|"promise/no-nesting"|N/A|
|promise/no-new-statics|error|N/A|
|promise/no-promise-in-callback|"promise/no-promise-in-callback"|N/A|
|promise/no-return-in-finally|error|N/A|
|promise/no-return-wrap|error|N/A|
|promise/param-names|error|N/A|
|promise/prefer-await-to-callbacks|warn|N/A|
|promise/prefer-await-to-then|warn|N/A|
|promise/valid-params|error|N/A|
|quote-props|"quote-props"|"quote-props"|
|quotes|"quotes"|"quotes"|
|radix|error|"radix"|
|react/boolean-prop-naming|"react/boolean-prop-naming"|"react/boolean-prop-naming"|
|react/button-has-type|error|"react/button-has-type"|
|react/default-props-match-prop-types|error|"react/default-props-match-prop-types"|
|react/destructuring-assignment|"react/destructuring-assignment"|"react/destructuring-assignment"|
|react/display-name|"react/display-name"|"react/display-name"|
|react/forbid-component-props|error|"react/forbid-component-props"|
|react/forbid-dom-props|"react/forbid-dom-props"|"react/forbid-dom-props"|
|react/forbid-elements|"react/forbid-elements"|"react/forbid-elements"|
|react/forbid-foreign-prop-types|"react/forbid-foreign-prop-types"|"react/forbid-foreign-prop-types"|
|react/forbid-prop-types|"react/forbid-prop-types"|"react/forbid-prop-types"|
|react/jsx-boolean-value|"react/jsx-boolean-value"|"react/jsx-boolean-value"|
|react/jsx-child-element-spacing|"react/jsx-child-element-spacing"|"react/jsx-child-element-spacing"|
|react/jsx-closing-bracket-location|"react/jsx-closing-bracket-location"|"react/jsx-closing-bracket-location"|
|react/jsx-closing-tag-location|"react/jsx-closing-tag-location"|"react/jsx-closing-tag-location"|
|react/jsx-curly-brace-presence|"react/jsx-curly-brace-presence"|"react/jsx-curly-brace-presence"|
|react/jsx-curly-spacing|"react/jsx-curly-spacing"|"react/jsx-curly-spacing"|
|react/jsx-equals-spacing|"react/jsx-equals-spacing"|"react/jsx-equals-spacing"|
|react/jsx-filename-extension|N/A|"react/jsx-filename-extension"|
|react/jsx-first-prop-new-line|"react/jsx-first-prop-new-line"|"react/jsx-first-prop-new-line"|
|react/jsx-handler-names|"react/jsx-handler-names"|"react/jsx-handler-names"|
|react/jsx-indent|"react/jsx-indent"|"react/jsx-indent"|
|react/jsx-indent-props|"react/jsx-indent-props"|"react/jsx-indent-props"|
|react/jsx-key|error|"react/jsx-key"|
|react/jsx-max-depth|N/A|"react/jsx-max-depth"|
|react/jsx-max-props-per-line|"react/jsx-max-props-per-line"|"react/jsx-max-props-per-line"|
|react/jsx-no-bind|"react/jsx-no-bind"|"react/jsx-no-bind"|
|react/jsx-no-comment-textnodes|error|"react/jsx-no-comment-textnodes"|
|react/jsx-no-duplicate-props|error|"react/jsx-no-duplicate-props"|
|react/jsx-no-literals|"react/jsx-no-literals"|"react/jsx-no-literals"|
|react/jsx-no-target-blank|error|"react/jsx-no-target-blank"|
|react/jsx-no-undef|error|"react/jsx-no-undef"|
|react/jsx-one-expression-per-line|error|"react/jsx-one-expression-per-line"|
|react/jsx-pascal-case|error|"react/jsx-pascal-case"|
|react/jsx-props-no-multi-spaces|error|"react/jsx-props-no-multi-spaces"|
|react/jsx-sort-default-props|error|"react/jsx-sort-default-props"|
|react/jsx-sort-prop-types|N/A|"react/jsx-sort-prop-types"|
|react/jsx-sort-props|error|"react/jsx-sort-props"|
|react/jsx-space-before-closing|N/A|"react/jsx-space-before-closing"|
|react/jsx-tag-spacing|"react/jsx-tag-spacing"|"react/jsx-tag-spacing"|
|react/jsx-uses-react|warn|"react/jsx-uses-react"|
|react/jsx-uses-vars|warn|"react/jsx-uses-vars"|
|react/jsx-wrap-multilines|"react/jsx-wrap-multilines"|"react/jsx-wrap-multilines"|
|react/no-access-state-in-setstate|error|"react/no-access-state-in-setstate"|
|react/no-array-index-key|error|"react/no-array-index-key"|
|react/no-children-prop|error|"react/no-children-prop"|
|react/no-danger|error|"react/no-danger"|
|react/no-danger-with-children|error|"react/no-danger-with-children"|
|react/no-deprecated|error|"react/no-deprecated"|
|react/no-did-mount-set-state|error|"react/no-did-mount-set-state"|
|react/no-did-update-set-state|error|"react/no-did-update-set-state"|
|react/no-direct-mutation-state|error|"react/no-direct-mutation-state"|
|react/no-find-dom-node|error|"react/no-find-dom-node"|
|react/no-is-mounted|error|"react/no-is-mounted"|
|react/no-multi-comp|error|"react/no-multi-comp"|
|react/no-redundant-should-component-update|error|"react/no-redundant-should-component-update"|
|react/no-render-return-value|N/A|"react/no-render-return-value"|
|react/no-set-state|error|"react/no-set-state"|
|react/no-string-refs|error|"react/no-string-refs"|
|react/no-this-in-sfc|error|"react/no-this-in-sfc"|
|react/no-typos|error|"react/no-typos"|
|react/no-unescaped-entities|error|"react/no-unescaped-entities"|
|react/no-unknown-property|error|"react/no-unknown-property"|
|react/no-unsafe|error|"react/no-unsafe"|
|react/no-unused-prop-types|error|"react/no-unused-prop-types"|
|react/no-unused-state|error|"react/no-unused-state"|
|react/no-will-update-set-state|error|"react/no-will-update-set-state"|
|react/prefer-es6-class|error|"react/prefer-es6-class"|
|react/prefer-stateless-function|"react/prefer-stateless-function"|"react/prefer-stateless-function"|
|react/prop-types|error|"react/prop-types"|
|react/react-in-jsx-scope|error|"react/react-in-jsx-scope"|
|react/require-default-props|error|"react/require-default-props"|
|react/require-optimization|N/A|"react/require-optimization"|
|react/require-render-return|error|"react/require-render-return"|
|react/self-closing-comp|error|"react/self-closing-comp"|
|react/sort-comp|error|"react/sort-comp"|
|react/sort-prop-types|error|"react/sort-prop-types"|
|react/style-prop-object|error|"react/style-prop-object"|
|react/void-dom-elements-no-children|error|"react/void-dom-elements-no-children"|
|require-atomic-updates|N/A|"require-atomic-updates"|
|require-await|warn|"require-await"|
|require-jsdoc|"require-jsdoc"|"require-jsdoc"|
|require-unicode-regexp|N/A|"require-unicode-regexp"|
|require-yield|error|"require-yield"|
|rest-spread-spacing|N/A|"rest-spread-spacing"|
|semi|"semi"|"semi"|
|semi-spacing|"semi-spacing"|"semi-spacing"|
|semi-style|"semi-style"|"semi-style"|
|sort-imports|N/A|"sort-imports"|
|sort-keys|"sort-keys"|"sort-keys"|
|sort-vars|error|"sort-vars"|
|space-before-blocks|"space-before-blocks"|"space-before-blocks"|
|space-before-function-paren|"space-before-function-paren"|"space-before-function-paren"|
|space-in-parens|"space-in-parens"|"space-in-parens"|
|space-infix-ops|error|"space-infix-ops"|
|space-unary-ops|"space-unary-ops"|"space-unary-ops"|
|spaced-comment|"spaced-comment"|"spaced-comment"|
|strict|"strict"|"strict"|
|switch-colon-spacing|"switch-colon-spacing"|"switch-colon-spacing"|
|symbol-description|error|"symbol-description"|
|template-curly-spacing|N/A|"template-curly-spacing"|
|template-tag-spacing|"template-tag-spacing"|"template-tag-spacing"|
|unicode-bom|"unicode-bom"|"unicode-bom"|
|unicorn/catch-error-name|"unicorn/catch-error-name"|N/A|
|unicorn/custom-error-definition|"unicorn/custom-error-definition"|N/A|
|unicorn/error-message|error|N/A|
|unicorn/explicit-length-check|"unicorn/explicit-length-check"|N/A|
|unicorn/filename-case|"unicorn/filename-case"|N/A|
|unicorn/import-index|error|N/A|
|unicorn/new-for-builtins|error|N/A|
|unicorn/no-abusive-eslint-disable|error|N/A|
|unicorn/no-array-instanceof|error|N/A|
|unicorn/no-fn-reference-in-iterator|"unicorn/no-fn-reference-in-iterator"|N/A|
|unicorn/no-hex-escape|error|N/A|
|unicorn/no-new-buffer|error|N/A|
|unicorn/no-process-exit|"unicorn/no-process-exit"|N/A|
|unicorn/number-literal-case|error|N/A|
|unicorn/prefer-add-event-listener|"unicorn/prefer-add-event-listener"|N/A|
|unicorn/prefer-exponentiation-operator|error|N/A|
|unicorn/prefer-spread|"unicorn/prefer-spread"|N/A|
|unicorn/prefer-starts-ends-with|error|N/A|
|unicorn/prefer-type-error|error|N/A|
|unicorn/regex-shorthand|error|N/A|
|unicorn/throw-new-error|error|N/A|
|use-isnan|error|"use-isnan"|
|valid-jsdoc|"valid-jsdoc"|"valid-jsdoc"|
|valid-typeof|N/A|"valid-typeof"|
|vars-on-top|error|"vars-on-top"|
|wrap-iife|"wrap-iife"|"wrap-iife"|
|wrap-regex|"wrap-regex"|"wrap-regex"|
|yield-star-spacing|N/A|"yield-star-spacing"|
|yoda|"yoda"|"yoda"|
