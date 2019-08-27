# Node 설치하기
## https://nodejs.org node를 설치한다.
---
### node 프로젝트 설정
1. 폴더를 생성한 후 vscode에서 폴더를 연다.
2. 터미널 창을 열어서 아래의 코드를 실행한다.
```console
npm init -y
```
3. package.json 파일을 생성한 후
4. express.js를 설치한다.
```console
npm i --save express
```
5. 프로젝트 루트에 app.js 파일을 생성한다.
6. app.js에 아래와 같이 코딩한다.
```javascript
const express = require('express');
const app = express();

app.listen(8000, () => {
	log("Server Running");
});
```
7. 터미널 창에서 아래와 같이 실행한다. - *개발중일 때는 8번을 실행한다.*
```
node app
```
8. supervisor를 설치 후 supervisor로 app을 실행한다.
	* supervisor 설치
	```
	npm i -g supervisor
	```
	* supervisor 설치가 되었으면 아래와 같이 실행한다.
	```
	supervisor app
	```