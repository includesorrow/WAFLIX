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


해당 프로젝트에서 부트스트랩을 사용한 이유로는
- HTML 디자인 시간 단축
- 관리자페이지 등 차트 자동구현


위해서 부트스트랩을 해당 프로젝트 내에 적용을 하는 작업을 하고 같은 팀프로젝트원들에게 사용법을 설명하였습니다. 







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
 

### 5. 기타 요소

Slack을 활용한 자료 및 기술 정보 공유 
![slack](https://user-images.githubusercontent.com/35910177/60557438-7a9d1380-9d80-11e9-884f-0cf24a7cc3ba.PNG)



회의록 작성

