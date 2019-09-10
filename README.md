# cli-program

## cli 실행
```
$ npm -i g
$ cli
```

## 결과 (디폴트값)
```
? 템플릿 종류를 선택하세요. html
? 파일의 이름을 입력하세요. index
? 파일이 위치할 폴더의 경로를 입력하세요. .
? 생성하시겠습니까? Yes
이미 해당 파일이 존재합니다
터미널을 종료합니다.
```

## public\html\new.html 파일 생성하는 명령어
```
$ cli template html -d public/html -n new
public\html\new.html 생성 완료
```

> 해당 명령어를 통해 public\html 폴더에 new.html 파일을 생성한다. (public\html 폴더가 없을 경우 자동 생성해준다.) new.html 파일의 내용은 command.js에서 선언한 htmlTemplate 변수이다.
```javascript
// htmlTemplate 변수
const htmlTemplate = `<!DOCTYPE html>
<html>
<head>
  <meta chart="utf-8" />
  <title>Template</title>
</head>
<body>
  <h1>Hello</h1>
  <p>CLI</p>
</body>
</html>`;
```