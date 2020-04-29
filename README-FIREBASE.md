# Firebase를 이용한 웹사이트 배포

## firebase 설치 - 각PC에서 한번만
1. [nodejs.org](https://nodejs.org)에 접속하여 **LTS**버전의 프로그램을 다운로드하고 설치한다(기본값)
2. 설치가 완료되면 nodejs프로그램에서 제공하는 **npm**(node package manager)를 사용할 수 있게 된다.
3. npm명령으로 firebase를 설치한다. (vscode의 터미널창을 열고)

```bash
npm i -g firebase-tools
```

4. 설치가 완료되면 firebase 명령을 수행할 수 있다. 그 후 사용자등록을 위해 터미널 창에서 아래의 명령을 수행하고, (Y/n)선택에서 Y를 선택하고 엔터를 하면 브라우저가 뜨면서 본인의 구글계정과 연동하게 된다.

```bash
firebase login
```


## firebase 프로젝트 만들기
### firebase.com에서 할일
1. [firebase.com](https://firebase.com)에 접속하여 구글계정으로 로그인한다.
2. 로그인 이후 우측 상단의 **콘솔로이동** 버튼을 클릭하여, 나의 콘솔로 이동한다.
3. 프로젝트 만들기(+)를 클릭하고 새로운 프로젝트를 생성한다.
- 1P: 사이트 주소 생성(신중하게)
- 2P: 애널리틱스 사용으로 체크
- 3P: 애널리틱스 사용계정(Default Account)로 선택, 혹시 국가선택이 뜨면 '대한민국'을 선택한다.
### vscode에서 할일
