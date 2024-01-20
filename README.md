# React State Management

### npm workspace 모노레포 설정
1. 루트 디렉토리 초기화
   ```
   npm init -y
   ```
2. package.json 설정
   ```json
  {
      ...
      "private": true,
      "workspaces": [
          "react-context-workspace",
          "react-redux-workspace",
          "react-query-workspace"
      ]
  }
  ```
3. 디렉토리 생성
  ```
  mkdir react-context-workspace
  mkdir react-redux-workspace
  mkdir react-query-workspace
  ```
4. 워크스페이스 초기화
  ```
  npm init -w ./react-context-workspace
  npm init -w ./react-redux-workspace
  npm init -w ./react-query-workspace
  ```
5. 워크스페이스 npm install
  ```
  cd react-context-workspace 
  npm install
  cd react-redux-workspace 
  npm install
  cd react-query-workspace 
  npm install
  ```
6. 워크스페이스별 패키지 설치
  ```
  npm install <PACKAGE> -w <WORKSPACE>
  ```
7. 워크스페이스별 script 실행
  ```
  npm run <SCRIPT> -w <WORKSPACE>
  ```
