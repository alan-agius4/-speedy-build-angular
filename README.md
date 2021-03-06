
# Angular CLI Stylelint builder

[![CircleCI](https://circleci.com/gh/alan-agius4/speedy-build-angular/tree/master.svg?style=svg)](https://circleci.com/gh/alan-agius4/speedy-build-angular/tree/master)
[![Build status](https://ci.appveyor.com/api/projects/status/opl22djxtn8vep9q?svg=true)](https://ci.appveyor.com/project/alan-agius4/speedy-build-angular)
[![npm version](https://img.shields.io/npm/v/@speedy/build-angular.svg)](https://www.npmjs.com/package/@speedy/build-angular)
[![Dependency Status](https://img.shields.io/david/alan-agius4/speedy-build-angular.svg?style=flat-square)](https://david-dm.org/alan-agius4/speedy-build-angular)
[![devDependency Status](https://img.shields.io/david/dev/alan-agius4/speedy-build-angular.svg?style=flat-square)](https://david-dm.org/alan-agius4/speedy-build-angular?type=dev)

Angular CLI third party builder (not officially supported by Angular), for [Stylelint](https://github.com/stylelint/stylelint).

## Get started

```bash
npm install @speedy/build-angular stylelint --save-dev
```

Open your `angular.json` and add the new builder example;

```json
"lint-styles": {
    "builder": "@speedy/build-angular:stylelint",
    "options": {
        "stylelintConfig": ".stylelintrc",
        "exclude": [
            "**/node_modules/**"
        ]
    }
}
```

For a full list of options that can be provided to this builder check the [schema](https://github.com/alan-agius4/speedy-build-angular/blob/master/src/schema.json).

More details about angular workspace can be found in the [Angular CLI docs](https://github.com/angular/angular-cli/wiki/angular-workspace).

To run the new builder use the following command;

```bash
ng run <project>:lint-styles
```
