1. 프로그램 세팅 , git init , git remote , git add . git commit -m "" , git push origin main
2. application-dev.yml, application-test.yml 추가 (각 환경별 설정파일)
3. 정적자원에 접근에 대한 속도향상을 위해서 우선적으로 시큐리티 룰에서 허용, h2-console 접근 할 수 있도록 
4. GET /api/v1/articles : 다건조회
   GET /api/v1/articles/5 : 단건조회
   PUT /api/v1/articles/5 : 수정
   DELETE /api/v1/articles/5 : 삭제
5. API 버저닝을 하는 이유는 API 버전업을 해도 기존 클라이언트가 잘 작동하기 위해서 
6. 타임리프의 결과물은 디자인 + 데이터, JSON 은 순수 데이터로 구성되어있다.
7. FetchType.Lazy 인 녀석을 findBy 로 불러오면 해당객체는 프록시 객체, 잭슨이 해당 프록시를 JSON화 하려다가 실패
8. article.getAuthor().getId() 까지는 쿼리 발생안함. 하지만 username 을 요구하면 쿼리 실행
9. OneToMany는 기본적으로 Lazy 이다. 단 객체가 생성되는 순간은 예외이다. 
10. 엔티티를 API 로 그대로 노출하는 것은 좋지 않다. API 규격에 맞춰진 DTO를 사용하자. 
11. 