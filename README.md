# WAFLIX

![WAFLIX](https://user-images.githubusercontent.com/35910177/60499490-855d9700-9cf3-11e9-9dec-27b5ba6f4376.png)


## WATFLIX 소개
WAFLIX란 **Spring을 이용해서 구현한 영화 스트리밍 사이트**입니다.

사이트 내의 기능으로는 WATCHA, NETFLIX같이 **사이트내에 추천 알고리즘을 구현**하여 고객에게 자신의 성향에 맞는 추천영화들을 제공해주며,  관리자 페이지 내에서도 **해당 사이트 내 현황 판권분석, 수익률 분석 알고리즘을 구현, 고객의 군집화**를 구현하여 관리자페이지에서 확인이 가능할 수 있도록 구현하였습니다.


## 프로젝트 정보

- 프로젝트 기간 : 2019.3.8 ~ 4.2 (근무일수 기준 18일)

- 프로젝트 인원 : 7명

- 프로젝트 기술요소

![OracleQuery](https://img.shields.io/badge/Oracle-Query-red.svg)
![OracleJoin](https://img.shields.io/badge/Oracle-join-red.svg)
![OracleSubQuery](https://img.shields.io/badge/Oracle-SubQuery-red.svg)
![OracleView](https://img.shields.io/badge/Oracle-View-red.svg)
![OracleProceduce](https://img.shields.io/badge/Oracle-Procedure-red.svg)
![OracleFunction](https://img.shields.io/badge/Oracle-Function-red.svg)
![OracleTrigger](https://img.shields.io/badge/Oracle-Trigger-red.svg)
![OracleTransaction](https://img.shields.io/badge/Oracle-Transaction-red.svg)

![SpringFileUpload](https://img.shields.io/badge/Spring-File%20Upload-brightgreen.svg)
![SpringPOI](https://img.shields.io/badge/Spring-POI-brightgreen.svg)
![SpringRestfulAPI](https://img.shields.io/badge/Spring-RestfulAPI-brightgreen.svg)
![SpringInterceptor](https://img.shields.io/badge/Spring-Interceptor-brightgreen.svg)
![SpringChart](https://img.shields.io/badge/Spring-Chart-brightgreen.svg)
![SpringJSOUP](https://img.shields.io/badge/Spring-Jsoup-brightgreen.svg)
![SpringAOP](https://img.shields.io/badge/Spring-AOP-brightgreen.svg)

![MyBatisResultMap](https://img.shields.io/badge/MyBatis-ResultMap-lightgrey.svg)
![MyBatisDynamicQuery](https://img.shields.io/badge/MyBatis-DynamicQuery-lightgrey.svg)

![JavaScriptaJAX](https://img.shields.io/badge/JavaScript-Ajax-yellow.svg)
![JavaScriptJSON](https://img.shields.io/badge/JavaScript-JSON-yellow.svg)
![JavaScriptjstl](https://img.shields.io/badge/JavaScript-jstl-yellow.svg)

## 프로젝트 PPT

[여기에 다 있습니다.](https://github.com/includesorrow/WAFLIX/blob/master/MiddleProject_PPT_A%EC%A1%B0.pptx)

## 프로젝트 중 직접구현한 내용

### 1. 부트스트랩 (![BOOTSTRAP](https://user-images.githubusercontent.com/35910177/60500978-3107e680-9cf6-11e9-9bd7-60fa478ecb1b.png))


![dashio-bootstrap-admin-template](https://user-images.githubusercontent.com/35910177/60500754-d8384e00-9cf5-11e9-8df5-775be13d168a.jpg)
_(사진 : 부트스트랩 UI)_

이번 WAFLIX프로젝트에서 영화페이지 및 관리자페이지 둘 다 적용이 가능한 부트스트랩을 적용시켜 해당 프로젝트 디자인 설정 기간을 단축시키고자 부트스트랩을 적용하였습니다.

또한 부트스트랩을 스프링에 적용한 후 같은 조원에게 부트스트랩 사용법을 알려주어 프로젝트 인원들이 부트스트랩을 사용하는데 불편함이 없도록 하였습니다.






### 2. DB 관리자 (DBA)

프로젝트를 진행하면서 Oracle DB 구축을 필요로 했고, 그에 따라서 DB를 담당할 DB관리자인 DBA가 필요했습니다. 

2017년에 멀티캠퍼스에서 Oracle DB,SQL 수업을 들었던 저는 DBA를 담당하기로 했습니다.

해당 프로젝트에서 DB를 처음에 EXERD로 구성하고 프로젝트 진행 중 필요에 따라서 TABLE Column 수정, Primary Key 설정, Unique 설정, Join 등 DB에 대한 부분을 담당하였습니다.

![DB 구조](https://user-images.githubusercontent.com/35910177/60503887-8e526680-9cfb-11e9-8016-623f56ba3f09.png)
~~(22차 수정본 끝에 완성된 DB구조)~~


### 3. Spring 관리자 페이지 구현
![movielist](https://user-images.githubusercontent.com/35910177/60558025-9e615900-9d82-11e9-9f4e-d22a64edb79b.png)

- 사용 기술
![OracleQuery](https://img.shields.io/badge/Oracle-Query-red.svg)
![OracleView](https://img.shields.io/badge/Oracle-View-red.svg)
![OracleSubQuery](https://img.shields.io/badge/Oracle-SubQuery-red.svg)
![OracleView](https://img.shields.io/badge/Oracle-View-red.svg)
![MyBatisResultMap](https://img.shields.io/badge/MyBatis-ResultMap-lightgrey.svg)
![MyBatisDynamicQuery](https://img.shields.io/badge/MyBatis-DynamicQuery-lightgrey.svg)
![JavaScriptaJAX](https://img.shields.io/badge/JavaScript-Ajax-yellow.svg)
![SpringJSOUP](https://img.shields.io/badge/Spring-Jsoup-brightgreen.svg)
![SpringAOP](https://img.shields.io/badge/Spring-AOP-brightgreen.svg)

- 영화 리스트

 현재 DB에 저장되어 있는 영화 리스트를 출력해주며, 검색기능을 넣어 DB에 있는 영화 검색이 가능하게 구현하였습니다.
 
 또한 영화 가격 수정을 넣어 관리자가 영화의 가격을 실시간으로 수정이 가능하게 해주며, 영화 활성화 상태를 변경하면 페이지에서 출력이 True,False로 전환할 수도 있고 영화 가격을 전체적으로 업데이트하여 관리자가 원하는대로 영화 가격을 업데이트하게 해주는 기능을 넣었습니다.
 
 - 해당 코드 (일부)
 ```
 
	@PostMapping("/blank5")
	public String searchTitle5(String searchType,String search,Model m) {
		Map<String, String> map= new HashMap<String, String>();
		map.put("searchType", searchType);
		map.put("search", search); 
		System.out.println(search);
		m.addAttribute("list",dao.getMovieList3(map)); 
		m.addAttribute("searchType",searchType);
		return "blank5";
	}
	//검색에 값을 받기 위한 Post방식의 Mapping
 ```
 ```
 	public List<MyListsVO> getMyMovieList(String userId){
		return ss.selectList("mymovielist.getMovieList",userId);
	}
 ```
 ```
 <select id="movielist" parameterType="hashmap"
  	resultType="movievo">
  		select * from movie
  	
  			 </select>
  			
  			 <select id="movietitlelist" parameterType="hashmap"
  			 resultType="movievo">
  			 select movie_title from movie
  			 where movie_title like '%' || #{movie_title} || '%'
  			 
  			 </select>
  			 
  			 <!-- 차트를 위한 가격리스트 -->
  			 <select id="price" resultType="int" parameterType="list">
  	select count(*)
         from movie
         group by movie_price
         order by movie_price asc
 
</select>
 ```



### 4. Spring - R - DB  연동

구상도

![image](https://user-images.githubusercontent.com/35910177/60637446-6bd46080-9e55-11e9-8aa4-4bff79ae8433.png)

1. 군집화

머신러닝 기술을 적용하기 위해서 스프링에서 R을 연동하고, R에서는 Oracle DB에 접속하여 데이터를 가지고 온 후, 그 데이터를 군집화인 K-Means를 적용하여 회원의 군집을 정하는 작업을 하였습니다.

- 해당 코드 (일부)
```
R CODE

library(DBI)
library(rJava)
library(RJDBC)
options(java.parameters='-Xmx32g') # rJava의 memory limit default를 512MB->32GB로 확장
connect.drv <- JDBC('oracle.jdbc.driver.OracleDriver', 'C:/bigdata/KOSTA/KOSTA/Oracle/File/lib/ojdbc6.jar') # jdbc 경로
connect.info <- dbConnect(connect.drv, paste('jdbc:oracle:thin:@', connect.db[[1]]$host[connect.db$connect.to], ':', connect.db[[1]]$port[connect.db$connect.to], ':', connect.db[[1]]$sid[connect.db$connect.to], sep=''), connect.db[[1]]$username[connect.db$connect.to], connect.db[[1]]$password[connect.db$connect.to])
# 주의: 쿼리 맨 끝의 세미콜론(;)은 삭제할 것
query.data <- dbGetQuery(connect.info, "SELECT * FROM movie")
#dbDisconnect(connect.info) # DB 접속 종료
head(query.data, n=5)
format(object.size(query.data), units='auto')
gc(verbose=TRUE) # 메모리 Garbage Collection (큰 object 삭제 후 실행하면 메모리를 OS에 돌려주는 역할을 함)
```

2. 댓글을 KoNLP를 통하여 태그화

WAFLIX 페이지에서 댓글을 가져와서 태그화를 해야하는 작업이 필요했습니다.

하지만 


### 5. 기타 요소

Slack을 활용한 자료 및 기술 정보 공유 
![slack](https://user-images.githubusercontent.com/35910177/60557438-7a9d1380-9d80-11e9-884f-0cf24a7cc3ba.PNG)



회의록 작성

