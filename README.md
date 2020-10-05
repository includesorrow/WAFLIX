# WAFLIX

![WAFLIX](https://user-images.githubusercontent.com/35910177/60499490-855d9700-9cf3-11e9-9dec-27b5ba6f4376.png)


## WATFLIX 소개
WAFLIX란 **Spring을 활용한 영화 스트리밍 사이트**입니다.

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

그래서 프로젝트 인원 중 기존에 교육을 들은 경험이 있는 제가 DBA를 담당하기로 했습니다.

해당 프로젝트에서 DB를 EXERD를 통해서 구성 및 생성하고 프로젝트 진행 중 필요에 따라서 TABLE 수정, Primary Key 설정, Unique 설정, Join 등 DB에 대한 부분을 담당하였습니다.

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

- 영화 리스트 및 검색

![g](https://user-images.githubusercontent.com/35910177/61347790-2c683400-a899-11e9-93bc-0e3646b600cb.png)

 현재 DB에 저장되어 있는 영화 리스트를 출력해주며, 검색기능을 넣어 DB에 있는 영화 검색이 가능하게 구현하였습니다.
 
 또한 영화 가격 수정을 넣어 관리자가 영화의 가격을 실시간으로 수정이 가능하게 해주며, 영화 활성화 상태를 변경하면 페이지에서 출력이 True,False로 전환할 수도 있고 영화 가격을 전체적으로 업데이트하여 관리자가 원하는대로 영화 가격을 업데이트하게 해주는 기능을 넣었습니다.
 
 - 해당 코드 (일부)
 ```
 
 동작 순서 : Client -> blank5.jsp  ->  DefaultController  ->  DynamicExampleDao  ->  movieMapper.xml  ->  DefaultController -> blank5.jsp

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
 <!-- 영화 페이지에서 join을 하면서 검색할 때 사용하는 resultmap -->
 <resultMap type="movievo" id="movievo">
 	<result column="movie_number property="movie_number"></result>
		<중간생략>
	<collection property="movietagvo" resultMap="movietagvo">
	</collection>
</resultmap>

<select id="moviehashmap" resultMap="movietagvo" parameterType="hashmap">
		select m.movie_number, m.movie_title, m.movie_price,m.movie_open_date, m.movie_purchase_date, m.movie_rating,m.movie_investment,
		m.active_check_number,  t.tag_table_num,tt.tag_category_num, tt.tag_name
		from movie m, movie_tag t, tag_table tt		
			<where>
				m.movie_number = t.movie_number
				and t.tag_table_num = tt.tag_table_num
				and tt.tag_category_num = 1	
<!-- 				and m.movie_open_date  <![CDATA[ < ]]> ALL (select movie_open_date from movie where movie_open_date <![CDATA[ > ]]> sysdate) -->
				<if test="search != null and search != ''">
				<choose> 
					<when test="searchType == 1">
						and m.movie_title like '%' || #{search} || '%'
					</when>
					<when test="searchType == 2">
						and m.active_check_number like '%' || #{search} || '%'
					</when>
					<otherwise></otherwise>
				</choose>
						</if>
			</where>
		order by 1 asc
	</select> 
</mapper>
```
 

- 영화 가격 수정

![image](https://user-images.githubusercontent.com/35910177/61342436-1badc300-a885-11e9-82d9-f6ac1963ed4b.png)

DB에 접속하지 않아도 관리자 페이지에서 영화 가격을 수정이 가능하게 구현하였습니다.

영화 가격 수정 버튼을 누르고 영화번호와 영화가격을 입력한 후 수정하기 버튼을 누르면 DB에서 해당 영화에 대한 가격이 수정이 되도록 하였습니다.

- 해당 코드 (일부)

```
// 영화 가격 수정 매핑
@RequestMapping(value="update.do", method=RequestMethod.POST)
public String update(@ModelAttribute MovieVO vo) throws Exception {
	dao.updateprice(vo);
	return "redirect:blank5";
	}
```
```
//영화 가격 수정시 사용됨
public void updateprice(MovieVO vo){
	ss.update("movie.update",vo);
	}
```
```
<!-- 영화 페이지에서 가격 수정을 위한 update -->
<update id = "update" parameterType="movievo">
update movie set movie_price =#{movie_price}
where movie_number=#{movie_number}
```

- 영화 활성화상태 변경

![image](https://user-images.githubusercontent.com/35910177/61342786-68de6480-a886-11e9-8397-51c88535aabc.png)

DB에 접속하지 않아도 관리자 페이지에서 영화 활성화 상태를 변경이 가능하게 구현하였습니다.

영화 코드와 상태 코드를 입력한 후, 영화 활성화 상태를 변경하면 영화코드의 상태코드를 DB에서 변경이 가능하도록 구현하였습니다.

- 해당 코드 (일부)

```
//DB의 Active_status_number 수정을 위한 Mapping
@RequestMapping(value="updatestatus.do",method=RequestMethod.POST)
public String updatestatus(@ModelAttribue MovieVO vo) throws Exception{
	dao.updatestatus(vo);
	return "redirect:blank5";
	}
```
```
//영화 active_check_number 수정을 위한 Update
public void updates(MovieVO vo){
	ss.update("movie.updatestatus",vo);
	}
```
```
<update id="updatestatus" parameterType="movievo">
update movie set active_check_number = #{active_check_number}
where movie_number=#{movie_number}
```

- 영화 가격 전체 업데이트

영화 가격 설정을 따로 설정하였습니다. 예시로는 다음과 같습니다.

|개봉일로부터 지난 개월 수 |가격|
|------|---|
|~12개월이내|10000원|
|12~24개월|5000원|
|24~36개월|2500원|
|36개월~|1000원|

영화 가격은 매일 04:00 기준으로 자동으로 db에서 업데이트가 되지만, 만일에 있을 업데이트가 안되는 경우를 대비해 수동으로 업데이트하는 버튼을 따로 만들어 간편하게 영화 가격을 Update하는 방법을 구현하였습니다. 


- 해당 코드 (일부)
```
@RequestMapping(value="moviepriceyearupdate.do",method=RequestMethod.POST)
public String updatemoviepriceyear(@ModelAttribute MovieVO vo) throws Exception{
	dao.updatemoviepriceyear();
	return "redirect:blank5";
	}
```
```
public void updatemoviepriceyear(){
	ss.update("movie.updateyearprice");
	}
```
```
<update id="updateyearprice" parameterType="movievo">
update movie
set movie_price=
case
when (months_between(sysdate,movie_purchase_Date)<![CDATA >=]]>48) then 1
when (months_between(sysdate,movie_purchase_Date)<![CDATA >=]]>36) and months_between(sysdate, movie_purchase_date) <![CDATA[ < ]]>48 then 2
when (months_between(sysdate,movie_purchase_Date)<![CDATA >=]]>24) and months_between(sysdate, movie_purchase_date) <![CDATA[ < ]]>36 then 3
when (months_between(sysdate,movie_purchase_Date)<![CDATA >=]]>12) and months_between(sysdate, movie_purchase_date) <![CDATA[ < ]]>24 then 4
else 5
end
</update>
```

### 4. Spring - R - DB  연동

구상도

![image](https://user-images.githubusercontent.com/35910177/60637446-6bd46080-9e55-11e9-8aa4-4bff79ae8433.png)


머신러닝 기술인 K-Means를 사용하기 위해서 R이 필요했습니다.

그래서 스프링에서 R을 연동하고, R에서는 데이터가 DB에 저장되어 있으므로 R과 DB를 연동하는 것이 필요했습니다.

R과 스프링을 연결하기 위하여 RServe, RJava 를 사용하였고

R과 DB를 연결하기 위하여 DBI, RJDBC, RJava 를 사용하였습니다.

1. 군집화

- 해당 코드 (일부분)

```
public void connectR() throws REXPMismatchException{	 		
			try {
				System.out.println("연결시작");
			RConnection connection =  null;
        	connection = new RConnection();
        	//R과 스프링 연결
        	connection.eval("library(caret)");
        	connection.eval("library('readxl')");
        	//R에서 라이브러리 호출        	
        	connection.parseAndEval("amazon2<-read_xlsx('C:/RTest/amazon.xlsx')");
        	//엑셀파일 불러오기
        	connection.eval("amazonkmeans <- kmeans(amazon2, centers=10, iter.max=10000)");
        	//k_means 알고리즘 적용
        	connection.eval("amazonkmeans$cluster");
        	//데이터리스트 받아오기
        	countlist = connection.eval("amazonkmeans$cluster").asIntegers();
        	        	for(int i=0; i<=29; i++) {
        	System.out.println(countlist[i]); }      	        	
        	connection.close();
			}catch(Exception e) {
				e.getStackTrace();
			}
		return RCommunitylist;
}
```


2. 댓글을 KoNLP를 통하여 태그화

WAFLIX 페이지에서 댓글을 가져와서 태그화를 해야하는 작업이 필요했습니다. 





- 해당 코드 (일부)

```
public class TagListDao {	
	public static String[] namelist;
		public void connectR(String movie_number) throws REXPMismatchException{	 
			InserttagVO vo = new InserttagVO();
			try {
            RConnection connection =  null;
        	connection = new RConnection();
        	connection.eval("library(rJava)");
        	connection.eval("library(DBI)");
        	connection.eval("library(RJDBC)");
        	connection.eval("library(rvest)");
        	connection.eval("library(httr)");
        	connection.eval("library(KoNLP)");
        	connection.eval("library(stringr)");
        	connection.eval("library(tm)");
        	connection.eval("library(qgraph)");
        	connection.eval("library(dplyr)");
        	connection.eval("library(xml2)");
        	// 라이브러리 호출
        	connection.eval("connect.db <- list(data.frame(dbname=c('DB1', 'DB2'), host=c('localhost', '172.188.1.2'),port=c(1521, 9999), sid=c('xe', 'ddbb'), username=c('midproject', 'BDUSER'), password=c('midproject', 'PPWW'),stringsAsFactors=FALSE))");
        	connection.eval("connect.db$connect.to <- 1");
        	connection.eval("options(java.parameters='-Xmx32g')");
        	connection.eval("connect.drv <- JDBC('oracle.jdbc.driver.OracleDriver', 'C:/bigdata/KOSTA/KOSTA/Oracle/File/lib/ojdbc6.jar')");
        	connection.eval("connect.info <- dbConnect(connect.drv, paste('jdbc:oracle:thin:@', connect.db[[1]]$host[connect.db$connect.to], ':', connect.db[[1]]$port[connect.db$connect.to], ':', connect.db[[1]]$sid[connect.db$connect.to], sep=''), connect.db[[1]]$username[connect.db$connect.to], connect.db[[1]]$password[connect.db$connect.to])");
        	// R  <-> DB 연동        	
        	connection.eval("gc(verbose=TRUE)");
        	//메모리 가비지 컬렉션
        	connection.eval("query <- (\"select usedwords_contents as x from review_usedwords where movie_number='"+movie_number+"'\")");
        	connection.eval("query <- (\"select usedwords_contents as x from ( select movie_title, rank() over (order by movie_number_of_audience desc) as rank from movie ), review_usedwords where  rank <= 10 " + ")");
        	connection.eval("query <- (\"select usedwords_contents as x from review_usedwords where movie_number='20129370'\")");
        	connection.eval("result <- dbGetQuery(connect.info,query)");	
        	//오라클로 들어가기 위한 쿼리문
        	connection.eval(hochul);
        	// 명사 / 형용사 추출 함수 생성
        	connection.eval("tdm <- TermDocumentMatrix(cps, control=list(tokenize=ko.words, removePunctuation=T,  stopwords=stopWord, removeNumbers=T,  wordLengths=c(4, 10), weighting=weightBin   )) ");        	
        	connection.eval("cps <- Corpus(VectorSource(result[[\"X\"]]))  ");
        	//cps에 벡터소스 생성
        	connection.eval("dim(tdm)");
        	connection.eval("tdm.matrix <- as.matrix(tdm)");
        	connection.eval("Encoding(rownames(tdm.matrix)) <- 'UTF-8'");
        	connection.eval("word.count <- rowSums(tdm.matrix) ");
        	connection.eval("word.order <- order(word.count, decreasing=T)");
        	connection.eval("freq.words <- tdm.matrix[word.order[1:20], ]");
        	connection.eval("co.matrix <- freq.words %*% t(freq.words)");
        	connection.eval("wordcounttest <- sort(word.count,decreasing = TRUE)");
        	connection.eval("wordlist <- as.list(wordcounttest)");
        	connection.eval("nameslist <- names(wordlist)");
			for(int a=0; a<10; a++) {
			vo.setTag_name(namelist[a]);
        	}
			//태그이름vo로저장
        	connection.close();
    		//연결종료
			}catch(RserveException e) {
				System.out.println("error RserveException");
			}
		}
}
```

- 해당 코드 (일부)
```
R Code
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

query <- ("select usedwords_contents as x from review_usedwords where movie_number='20129370'")
result <- dbGetQuery(connect.info,query)

## 명사/형용사 추출 함수 생성
ko.words <- function(doc){
  d <- as.character(doc)
  pos <- paste(SimplePos22(d))
  extracted <- str_match(pos, '([가-힣]+)/[NC]')
  keyword <- extracted[,2]
  keyword[!is.na(keyword)]}



options(mc.cores=1)    ## 단일 Core 만 활용하도록 변경 (옵션)
cps <- Corpus(VectorSource(result[["X"]]))  


tdm <- TermDocumentMatrix(cps,
                          control=list(tokenize=ko.words,    ## token 분류시 활용할 함수명 지정
                                       removePunctuation=T,  ## 구두점 제거
                                       stopwords=stopWord,   ## 불필요 단어 제거
                                       removeNumbers=T,      ## 숫자 제거
                                       wordLengths=c(4, 10), ## 단어 길이 조정, 한글은 2자
                                       weighting=weightBin   ## 단어가 텍스트에 출현하면 1, 아니면 0을 반환
                          ))  

#최종결과 확인
dim(tdm)
tdm.matrix <- as.matrix(tdm)
Encoding(rownames(tdm.matrix)) <- 'UTF-8'
word.count <- rowSums(tdm.matrix)  ##각 단어별 합계를 구함
word.order <- order(word.count, decreasing=T)  #다음으로 단어들을 쓰인 횟수에 따라 내림차순으로 정렬
freq.words <- tdm.matrix[word.order[1:20], ] #Term Document Matrix에서 자주 쓰인 단어 상위 20개에 해당하는 것만 추출
co.matrix <- freq.words %*% t(freq.words)  #행렬의 곱셈을 이용해 Term Document Matrix를 Co-occurence Matrix로 변경


```


### 4. 프로젝트르 진행하면서 느낀 점

해당 프로젝트르 하면서 느낀건 많지만, 크게 2가지가 있습니다.

먼저 기본기 입니다.

저는 자바 교육을 들으면서 사실 전부 이해했고, 그래서 나는 스프링 할 자격이 있다고 생각하였습니다. IT 교육 과정의 처음을 자바를 먼저 시작하였습니다. 저는 대학교 3학점 전공으로 자바를 먼저 배우 경험이 있어서 쉽게 접근이 가능했고, 매일마다 저녁까지 남아 학습을 하였고, 그만큼 공부했으니 그만큼 기본기가 충실했다고 생각하였습니다. 하지만 그건 아니였습니다. 많이들 강조하는 기초지식이란건 자바의 기초가 아닌 컴퓨터공학, 알고리즘, 자료구조의 기초였습니다. 그 기초가 없이 시작하자보니 자료구조가 안맞는 경우도 많았으며, 프로젝트에서 매번 실수하기 일쑤였습니다. 이러 경험을 통하여 기본기가 필요하다고 생각하였습니다.

두번째로는 단순히 구글링을 해서 나온 내용으 Ctrl c + v를 하는게 아니라, 본질적인 내용을 이해하고 써야한다는 점입니다.

저는 이번 프로젝트에서 수많은 내용을 기본없이 전부 구글링해서 찾을려는 경험을 했습니다. 무엇이 안된다고 싶으면 에러코드르 읽고, 그 에러코드를 복사 + 붙여넣기를 하여 해결할려고 했었습니다. 하지만 매번 복사+붙여넣기를 하면서 제 자신이 업그레이드 하는 것이 아닌 단순히 복사 붙여넣기 하는 기계가 되어버린것 같은 느낌이 들었습니다. 에러가 나면 날수록 그 에러를 읽고 해결하는 능력을 기르지 못하였습니다. 그러한 생각이 든 이후부터 저는 복사 + 붙여넣기가 아닌 에러코드가 어디서 에러났고, 그 에러의 근본을 찾아다닐려고 노력했습니다. 이러한 경험 끝에 저는 단순한 기계가 아닌 생각하고 고칠려는 사람이 되겠다고 생각하였습니다.











### 5. 기타 요소

- Slack을 활용한 자료 및 기술 정보 공유 
 
 ![slack](https://user-images.githubusercontent.com/35910177/60557438-7a9d1380-9d80-11e9-884f-0cf24a7cc3ba.PNG)

- Github를 활용한 백업본 저장

![image](https://user-images.githubusercontent.com/35910177/60640841-118ecc00-9e64-11e9-9ec8-af91b7093b2c.png)

