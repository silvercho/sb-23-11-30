1. 프로그램 세팅 , git init , git remote , git add . git commit -m "" , git push origin main
2. application-dev.yml, application-test.yml 추가 (각 환경별 설정파일)
3. 정적자원에 접근에 대한 속도향상을 위해서 우선적으로 시큐리티 룰에서 허용, h2-console 접근 할 수 있도록 
4. GET /api/v1/articles : 다건조회
   GET /api/v1/articles/5 : 단건조회
   PUT /api/v1/articles/5 : 수정
   DELETE /api/v1/articles/5 : 삭제
5. 