# MT-setting-week1

### TypeScript + React + Jest + ESLint + Parcel 개발 환경 세팅

맥북(Mac)기준

작성 중 문제가 생길시 sudo를 활용하자


### Node.js 설치하기

폴더를 하나 만들고 VScode로 폴더열기

```bash
mkdir my-app
cd my-app
code .
```

npm 패키지 생성

```bash
npm init -y
```

'.gitignore' 파일 생성 및 작성 // 최소한  node_modules를 push하지 않도록하자!

```bash
touch .gitignore
```

.gitignore파일에 /node_modules/, /dist/, /.parcel-cache/ 작성하기


### Typescript 설치하기

```bash
npm install -D typescript
npx tsc --init
```

'tsconfig.json' 파일의 jsx속성을 변경한다 ("jsx": "react-jsx")


### ESlint 설정


```bash
npm install -D eslint
npx eslint --init
```

'npx eslint --init'의 선택사항을 적절히 선택해주고, 개발환경을 구축한다. '.eslintrc.js' 파일에 'jest:true'를 잡아준다!
'.eslintignore'파일을 작성한다.

```bash
touch .eslintignore
```

'.eslintignore' 파일에 /node_modules/, /dist/, /.parcel-cache/ 작성하기


### REACT 설치

```bash
npm install react react-dom
npm install -D @types/react @types/react-dom
```

### 테스팅도구 설치 (jest)

```bash
npm i -D jest @types/jest @swc/core @swc/jest \
    jest-environment-jsdom \
    @testing-library/react @testing-library/jest-dom
```

'jest.config.js' 파일생성후 내용 작성

```bash
touch jest.config.js
```

https://github.com/ahastudio/CodingLife/blob/main/20220726/react/jest.config.js 의 내용을 파일에 작성

### Parcel설치 

```bash
npm install -D parcel
```

'package.json'의 scripts, source 부분을 수정한다.

https://github.com/ahastudio/CodingLife/blob/main/20220726/react/package.json 참고!

