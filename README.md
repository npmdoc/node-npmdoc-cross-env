# api documentation for  [cross-env (v3.2.4)](https://github.com/kentcdodds/cross-env#readme)  [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-cross-env.svg)](https://travis-ci.org/npmdoc/node-npmdoc-cross-env)
#### Run scripts that set and use environment variables across platforms

[![NPM](https://nodei.co/npm/cross-env.png?downloads=true)](https://www.npmjs.com/package/cross-env)

[![apidoc](https://npmdoc.github.io/node-npmdoc-cross-env/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-cross-env_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-cross-env/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-cross-env/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "Kent C. Dodds",
        "email": "kent@doddsfamily.us",
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
        "shasum": "9e0585f277864ed421ce756f81a980ff0d698aba",
        "tarball": "https://registry.npmjs.org/cross-env/-/cross-env-3.2.4.tgz"
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
    "gitHead": "c1a9ed0764fe1e88f2ba370b43c4ade21d536f60",
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
            "name": "kentcdodds",
            "email": "kent@doddsfamily.us"
        }
    ],
    "name": "cross-env",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
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
    "version": "3.2.4"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module cross-env](#apidoc.module.cross-env)
1.  [function <span class="apidocSignatureSpan">cross-env.</span>default (args)](#apidoc.element.cross-env.default)



# <a name="apidoc.module.cross-env"></a>[module cross-env](#apidoc.module.cross-env)

#### <a name="apidoc.element.cross-env.default"></a>[function <span class="apidocSignatureSpan">cross-env.</span>default (args)](#apidoc.element.cross-env.default)
- description and source-code
```javascript
function crossEnv(args) {
  var _getCommandArgsAndEnv = getCommandArgsAndEnvVars(args),
      _getCommandArgsAndEnv2 = _slicedToArray(_getCommandArgsAndEnv, 3),
      command = _getCommandArgsAndEnv2[0],
      commandArgs = _getCommandArgsAndEnv2[1],
      env = _getCommandArgsAndEnv2[2];

  if (command) {
    var proc = (0, _crossSpawn.spawn)(command, commandArgs, { stdio: 'inherit', env });
    process.on('SIGTERM', function () {
      return proc.kill('SIGTERM');
    });
    process.on('SIGINT', function () {
      return proc.kill('SIGINT');
    });
    process.on('SIGBREAK', function () {
      return proc.kill('SIGBREAK');
    });
    process.on('SIGHUP', function () {
      return proc.kill('SIGHUP');
    });
    proc.on('exit', process.exit);
    return proc;
  }
  return null;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
