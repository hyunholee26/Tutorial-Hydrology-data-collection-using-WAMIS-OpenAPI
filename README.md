# [Tutorial] WAMIS OpenAPI를 이용한 수문관측데이터 수집


## 1. 국가수자원관리종합정보시스템(WAMIS)
 - 환경부 산하 한강홍수통제소에서 관리중인 시스템으로 환경부, 기상청, 한국수자원공사, 한국농어촌공사 등을 통해 수집된 **강수량, 수위, 기상 등 수문데이터를 통합하여 OpenAPI 방식으로 제공**
   - URL : [http://www.wamis.go.kr/](http://www.wamis.go.kr/)
   - 본 튜토리얼에서는 WAMIS에서 제공하는 OpenAPI를 이용함에 따라, 미리 **WAMIS의 OpenAPI 인증키를 발급받아야 합니다.**
```
**[OpenAPI 발급절차]**
1. [http://www.wamis.go.kr/](http://www.wamis.go.kr/) 접속
2. OpenAPI 메뉴 클릭
3. 로그인
4. OpenAPI활용 신청 및 키 확인
```

## 2. OpenAPI
  - OpenAPI란 S/W개발에 사용가능한 **공개된 API를 의미**하며, 본 튜토리얼에서는 WAMIS에서 제공하는 OpenAPI를 이용하여 수문데이터를 수집하는 예제를 제공하고자 합니다.

## 3. Tutoral 주요 내용
  - WAMIS OpenAPI 호출하여 단기간(6개월 미만) 시단위 강우데이터 수집하기
  - 반복적으로 OpenAPI를 호출하여 장기간(6개월 이상) 시단위 강우데이터 수집하기
