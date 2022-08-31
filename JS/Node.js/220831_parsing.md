  ## 220831


  ### terminal

- 초기화 시

  ```
  npm init
  ```

- 명세서(package.json) 기반 초기화 시

  ```
  npm i
  ```
  
  git hub 업로드 시 node_modules는 파일용량이 커서 제외하기 때문에 package.json을 통해 module init
  
  
  ### node
  
  #### cors 에러
  
  ```
    const result = await axios.get("http://localhost:8080/api/info");
  ```
  node.js
  
같은 IP지만 PORT까지 일치해야 리소스가 공유가능

클라이언트 -> 라이브 서버 (:5500)
백엔드 -> express(:8080)
기본적으로 막아놓는 이유 : 보안 (해커가 요청해서 가져갈 수도 있다.
