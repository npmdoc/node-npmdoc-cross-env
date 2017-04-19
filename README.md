# npmdoc-cross-env

#### api documentation for  [cross-env (v4.0.0)](https://github.com/kentcdodds/cross-env#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-cross-env.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-cross-env) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-cross-env.svg)](https://travis-ci.org/npmdoc/node-npmdoc-cross-env)

#### Run scripts that set and use environment variables across platforms

[![NPM](https://nodei.co/npm/cross-env.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/cross-env)

- [https://npmdoc.github.io/node-npmdoc-cross-env/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-cross-env/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-cross-env/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-cross-env/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-cross-env/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-cross-env/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Kent C. Dodds",
        "url": "http://kentcdodds.com/"
    },
    "bin": {
        "cross-env": "dist/bin/cross-env.js"
    },
    "bugs": {
        "url": "https://github.com/kentcdodds/cross-env/issues"
    },
    "config": {
        "commitizen": {
            "path": "node_modules/cz-conventional-changelog"
        }
    },
    "dependencies": {
        "cross-spawn": "^5.1.0",
        "is-windows": "^1.0.0"
    },
    "description": "Run scripts that set and use environment variables across platforms",
    "devDependencies": {
        "all-contributors-cli": "^4.0.1",
        "babel-cli": "^6.23.0",
        "babel-core": "^6.23.1",
        "babel-jest": "^19.0.0",
        "babel-preset-env": "^1.2.0",
        "babel-preset-stage-2": "^6.22.0",
        "babel-register": "^6.23.0",
        "codecov": "^1.0.1",
        "commitizen": "^2.9.6",
        "cz-conventional-changelog": "^2.0.0",
        "eslint": "^3.17.0",
        "eslint-config-kentcdodds": "^12.0.0",
        "husky": "^0.13.2",
        "jest-cli": "^19.0.2",
        "lint-staged": "^3.3.1",
        "nps": "^5.0.3",
        "nps-utils": "^1.1.2",
        "opt-cli": "^1.5.1",
        "prettier-eslint-cli": "^3.1.2",
        "semantic-release": "^6.3.6",
        "validate-commit-msg": "^2.11.1"
    },
    "directories": {},
    "dist": {
        "shasum": "16083862d08275a4628b0b243b121bedaa55dd80",
        "tarball": "https://registry.npmjs.org/cross-env/-/cross-env-4.0.0.tgz"
    },
    "engines": {
        "node": ">=4.0"
    },
    "eslintConfig": {
        "extends": [
            "kentcdodds",
            "kentcdodds/jest"
        ],
        "rules": {
            "max-len": [
                "error",
                80
            ]
        }
    },
    "files": [
        "dist"
    ],
    "gitHead": "e8a1614683fad01b2927ac8a4be308a21aa7df98",
    "homepage": "https://github.com/kentcdodds/cross-env#readme",
    "jest": {
        "testEnvironment": "node",
        "coverageThreshold": {
            "global": {
                "branches": 100,
                "functions": 100,
                "lines": 100,
                "statements": 100
            }
        }
    },
    "keywords": [],
    "license": "MIT",
    "lint-staged": {
        "*.js": [
            "prettier-eslint --write",
            "git add"
        ]
    },
    "main": "dist/index.js",
    "maintainers": [
        {
            "name": "kentcdodds"
        }
    ],
    "name": "cross-env",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/kentcdodds/cross-env.git"
    },
    "scripts": {
        "commitmsg": "opt --in commit-msg --exec \"validate-commit-msg\"",
        "precommit": "lint-staged && opt --in pre-commit --exec \"npm start validate\"",
        "start": "nps",
        "test": "nps test"
    },
    "version": "4.0.0"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
