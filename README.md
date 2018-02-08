# BlogSrc

## 실행

1. hexo-cli 설치
```
npm install -g hexo-cli
```
or
```
yarn global add hexo-cli
```

2. 로컬 환경에서 실행

```
cd blog
hexo server
```

## 배포
```
hexo deploy
```

## 빌드

1. 테마 파일 빌드 (해당 테마 폴더 위치)
```
$ npm run-script build
```

2. 퍼블릭 폴더 빌드 (해당 Hexo 폴더 위치)

```
$ hexo generate
```
