# express-web-app

## Command

### workspace config 
```
mkdir workspace
cd workspace
```

### git config
```
git init
echo "# <git-repository>" >> README.md
git add .
git commit -m "express-web-app first"
git remote add origin https://github.com/<git-user>/<git-repository>.git
git push --set-upstream origin master
```

### express config

#### npm init 명령을 이용하여 애플리케이션에 대한 package.json 파일을 작성
```
npm init
```

#### npm config
```
package name: workspace
version: (1.0.0)
description:
entry point: (index.js)
test command:
git repository: (https://github.com/<git-user>/.git)
keywords:
author:
license: (ISC)
About to write to <workspace-path>/package.json:
{
  "name": "<workspace>",
  "version": "1.0.0",
  "description": "",
  "main": "index.js",
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1"
  },
  "repository": {
    "type": "git",
    "url": "git+https://github.com/<git-user>/<git-repository>.git"
  },
  "author": "",
  "license": "ISC",
  "bugs": {
    "url": "https://github.com/<git-user>/<git-repository>/issues"
  },
  "homepage": "https://github.com/<git-user>/<git-repository>#readme"
}

Is this OK? (yes) 
```

#### express config

```
npm install express --save
```

##### --save 옵션을 통해 설치된 Node 모듈은 package.json 파일 내의 dependencies 목록에 추가됩니다. 이후 app 디렉토리에서 npm install을 실행하면 종속 항목 목록 내의 모듈이 자동으로 설치됩니다.
