
# [KDT] 1st Project : Netflix_그것이 알고싶다.



## 🔍 팀원 소개

| ![KakaoTalk_Photo_2021-07-03-18-43-56-3](image/KakaoTalk_Photo_2021-07-03-18-43-56-3.png) | ![KakaoTalk_Photo_2021-07-03-18-49-22-1](image/KakaoTalk_Photo_2021-07-03-18-49-22-1.png) | ![KakaoTalk_Photo_2021-07-03-18-43-56-2](image/KakaoTalk_Photo_2021-07-03-18-43-56-2.jpeg) | ![KakaoTalk_Photo_2021-07-03-18-43-56-1](image/KakaoTalk_Photo_2021-07-03-18-43-56-1.jpeg) |
| :----------------------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: |
|                             팀장                             |                             팀원                             |                             팀원                             |                             팀원                             |
|           [채길호](https://github.com/chaerui7967)           |            [유화영](https://github.com/cherieuu)             |            [김영성](https://github.com/zerosysk)             |          [천상희](https://github.com/avantgarde-cy)          |

## 🎖수상



![image-20210722105918259](image/image-20210722105918259.png)





## 🔍 업무

|            | 업무                                                         |
| ---------- | ------------------------------------------------------------ |
| **채길호** | 프로젝트 총괄<br /> sns 태그들과 상영시간의 viewPoint간의 상관관계 분석 |
| **유화영** | 데이터 수집 및 분석결과 정리, 회의록 작성<br />상영국가들와 tv 품질의 viewPoint간의 상관관계 분석 |
| **김영성** | 데이터 수집 및 데이터 정제<br />넷플릭스 출시 일자를 통해 월과 년도로 분할하여 viewPoint간의 상관관계 분석 |
| **천상희** | 데이터 수집 및 전처리<br />imdb 점수와 장르의 viewPoint간의 상관관계 분석 |



## 🔍 이용 규칙

### ⚡️ Naming

- 폴더는 자신의 이름으로 된 폴더만 이용합니다.

- 서브 폴더로 변수명을 활용한 이름의 폴더를 생성합니다.

  - **ex.**` 상영국가수-viewpoint-analysis`

-  서브 폴더 안에 파일명은

  ```
  공유날짜_독립변수명_종속변수명__분석__번호 
  ex. 0711_showingOncount_viewpoint_1.ipynb
  ```

  

  로 통일합니다. 띄어쓰기가 있으면 띄어쓰기를 제외하고 작성합니다. 

   

- 자신의 폴더 내 README는 자유롭게 작성하셔도 됩니다.

### ⚡️  Commit message, Pull Request

- Commit message, Pull Request 제목은

   

  ```
  [이름] 날짜_적고싶은내용
  ```

  로 해주세요!

  - 7월 11일 화영 → `[화영]0711_독립변수와종속변수분석1`

- 자신의 닉네임으로 된 브랜치를 딴 후 자신의 이름 폴더에 파일을 추가한 후 commit 하고, Pull Request를 보냅니다.

- Pull Request 양식에 따라 작성해주세요!

- Pull Request를 한 후, 본인의 브랜치는 1회성으로 사용하고 삭제합니다.

### ⚡️ Branch name

| User       | Branch name  |
| ---------- | ------------ |
| **김영성** | **추가예정** |
| **유화영** | **HY**       |
| **채길호** | **추가예정** |
| **천상희** | **추가예정** |



----------------

# PROJECT_Netflix



## 🔍 Title 

- OTT 콘텐츠 viewpoint 예측 모델에 대한 연구 : **넷플릭스 콘텐츠 분석을 중심으로** 
  -  Netflix의 여러 독립변수들을 통해 viewpoint(시청자수)를 예측



## 🔍 가설

	H0 : sns 태그들은 viewPoint에 영향이 없다.
	
	H1 : sns 태그들은 viewPoint에 영향이 있다.



	H0 : 상영시간은 viewPoint에 영향이 없다.
	
	H1 : 상영시간은 viewPoint에 영향이 있다.



	H0 : 사용언어는 viewPoint에 영향이 없다.
	
	H1 : 사용언어은 viewPoint에 영향이 있다.



	H0 : tv품질은 viewPoint에 영향이 없다.
	
	H1 : tv품질은 viewPoint에 영향이 있다.



	H0 : imdb점수는 viewPoint에 영향이 없다.
	
	H1 : imdb점수는 viewPoint에 영향이 있다.



	H0 : 장르들은 viewPoint에 영향이 없다.
	
	H1 : 장르들은 viewPoint에 영향이 있다.



	H0 : Netflix 출시일은 viewPoint에 영향이 없다.
	
	H1 : Netflix 출시일은 viewPoint에 영향이 있다.



p = 0.05

------

## 🔍 사용데이터

###  kaggle 

#### 1. Netflix Original Films & IMDB Scores

 https://www.kaggle.com/luiscorter/netflix-original-films-imdb-scores

- 영화 제목
- 영화 장르
- 최초 최초 공개 날짜
- 몇 분 안에 실행
- IMDB 점수 (21 년 6 월 1 일 기준)
- 현재 사용 가능한 언어 (06/01/21 기준)

#### 2. Latest Netflix data with 26+ joined attributes

https://www.kaggle.com/ashishgup/netflix-rotten-tomatoes-metacritic-imdb



#### 3. Netflix Movie and TV Shows (June 2021)

https://www.kaggle.com/snehaanbhawal/netflix-tv-shows-and-movie-list

- imdb_id : 고유 한 쇼 식별자.
- title : 쇼의 제목.
- popular_rank : 인기도를 기준으로 필터링했을 때 IMDB에서 제공하는 순위입니다.
- certificate : 쇼에서받은 연령 인증을 포함합니다. 많은 null 값.
- startYear : 쇼가 처음 방송 된 때.
- endYear : 쇼 엔딩 연도
- episodes : 프로그램의 에피소드 수입니다. 영화의 경우 1입니다.
- 유형 : 영화 또는 시리즈
- orign_country : 프로그램이 시작된 국가
- 언어 : 쇼의 언어.
- 줄거리 : 쇼의 시놉시스.
- 요약 : 쇼의 이야기 요약.
- rating : 쇼에 주어진 평균 평점.
- numVotes : 쇼에서받은 투표 수.
- genres : 쇼가 속한 장르.
- isAdult : 1 성인용 콘텐츠가있는 경우. 그렇지 않은 경우 0입니다.
- cast : 목록 형식으로 쇼의 메인 캐스트.
- image_url : 포스터 이미지 링크.



#### 4. Netflix Movies and TV Shows

https://www.kaggle.com/adityakadiwal/netflix-movies-and-tv-shows

- 제목 : 영화 / TV 쇼의 이름
- 유형 : 컨텐츠의 종류는
- titlereleased : 년 릴리스의
- 평가 : TV 부모 가이드 라인 평가
- 품질 : 제목의 비디오 품질
- 배우 : 영화 / TV 쇼의 캐스트
- 감독 : 감독 영화 / TV 쇼
- category : 장르 또는 카테고리
- imdb : 영화 / TV 쇼
- 런타임에 대한 IMDb 등급 : 영화 / TV 쇼 런타임 (** 분)



### 넷플릭스 분석 보고서 참조 데이터셋 - 기존 보고서를 이용한 새로운 데이터셋
=======
# [KDT] 1st Project : Netflix_그것이 알고싶다.



## 🔍 팀원 소개

| ![KakaoTalk_Photo_2021-07-03-18-43-56-3](image/KakaoTalk_Photo_2021-07-03-18-43-56-3.png) | ![KakaoTalk_Photo_2021-07-03-18-49-22-1](image/KakaoTalk_Photo_2021-07-03-18-49-22-1.png) | ![KakaoTalk_Photo_2021-07-03-18-43-56-2](image/KakaoTalk_Photo_2021-07-03-18-43-56-2.jpeg) | ![KakaoTalk_Photo_2021-07-03-18-43-56-1](image/KakaoTalk_Photo_2021-07-03-18-43-56-1.jpeg) |
| :----------------------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: |
|                             팀장                             |                             팀원                             |                             팀원                             |                             팀원                             |
|           [채길호](https://github.com/chaerui7967)           |            [유화영](https://github.com/cherieuu)             |            [김영성](https://github.com/zerosysk)             |          [천상희](https://github.com/avantgarde-cy)          |



## 🔍 업무


|            | 업무                                                         |
| ---------- | ------------------------------------------------------------ |
| **채길호** | 프로젝트 총괄<br /> sns 태그들과 상영시간의 viewPoint간의 상관관계 분석 |
| **유화영** | 데이터 수집 및 분석결과 정리, 회의록 작성<br />상영국가들와 tv 품질의 viewPoint간의 상관관계 분석 |
| **김영성** | 데이터 수집 및 데이터 정제<br />넷플릭스 출시 일자를 통해 월과 년도로 분할하여 viewPoint간의 상관관계 분석 |
| **천상희** | 데이터 수집 및 전처리<br />imdb 점수와 장르의 viewPoint간의 상관관계 분석 |



## 🔍 이용 규칙

### ⚡️ Naming

- 폴더는 자신의 이름으로 된 폴더만 이용합니다.

- 서브 폴더로 변수명을 활용한 이름의 폴더를 생성합니다.

  - **ex.**` 상영국가수-viewpoint-analysis`

-  서브 폴더 안에 파일명은

  ```
  공유날짜_독립변수명_종속변수명__분석__번호 
  ex. 0711_showingOncount_viewpoint_1.ipynb
  ```

  

  로 통일합니다. 띄어쓰기가 있으면 띄어쓰기를 제외하고 작성합니다. 

   

- 자신의 폴더 내 README는 자유롭게 작성하셔도 됩니다.

### ⚡️  Commit message, Pull Request

- Commit message, Pull Request 제목은

   

  ```
  [이름] 날짜_적고싶은내용
  ```

  로 해주세요!

  - 7월 11일 화영 → `[화영]0711_독립변수와종속변수분석1`

- 자신의 닉네임으로 된 브랜치를 딴 후 자신의 이름 폴더에 파일을 추가한 후 commit 하고, Pull Request를 보냅니다.

- Pull Request 양식에 따라 작성해주세요!

- Pull Request를 한 후, 본인의 브랜치는 1회성으로 사용하고 삭제합니다.

### ⚡️ Branch name

| User       | Branch name  |
| ---------- | ------------ |
| **김영성** | **ys** |
| **유화영** | **HY**       |
| **채길호** | **chae** |
| **천상희** | **sh** |



----------------

# PROJECT_Netflix (~ing 🚀)



## 🔍 Title 

- OTT 콘텐츠 viewpoint 예측 모델에 대한 연구 : **넷플릭스 콘텐츠 분석을 중심으로** 
  -  Netflix의 여러 독립변수들을 통해 viewpoint(시청자수)를 예측



## 🔍 가설

	H0 : sns 태그들은 viewPoint에 영향이 없다.
	
	H1 : sns 태그들은 viewPoint에 영향이 있다.



	H0 : 상영시간은 viewPoint에 영향이 없다.
	
	H1 : 상영시간은 viewPoint에 영향이 있다.



	H0 : 상영국가는 viewPoint에 영향이 없다.
	
	H1 : 상영국가는 viewPoint에 영향이 있다.



	H0 : tv품질은 viewPoint에 영향이 없다.
	
	H1 : tv품질은 viewPoint에 영향이 있다.



	H0 : imdb점수는 viewPoint에 영향이 없다.
	
	H1 : imdb점수는 viewPoint에 영향이 있다.



	H0 : 장르들은 viewPoint에 영향이 없다.
	
	H1 : 장르들은 viewPoint에 영향이 있다.



	H0 : Netflix 출시일은 viewPoint에 영향이 없다.
	
	H1 : Netflix 출시일은 viewPoint에 영향이 있다.



p = 0.05

------

## 🔍 사용데이터

###  kaggle 

#### 1. Netflix Original Films & IMDB Scores

 https://www.kaggle.com/luiscorter/netflix-original-films-imdb-scores

- 영화 제목
- 영화 장르
- 최초 최초 공개 날짜
- 몇 분 안에 실행
- IMDB 점수 (21 년 6 월 1 일 기준)
- 현재 사용 가능한 언어 (06/01/21 기준)

#### 2. Latest Netflix data with 26+ joined attributes

https://www.kaggle.com/ashishgup/netflix-rotten-tomatoes-metacritic-imdb



#### 3. Netflix Movie and TV Shows (June 2021)

https://www.kaggle.com/snehaanbhawal/netflix-tv-shows-and-movie-list

- imdb_id : 고유 한 쇼 식별자.
- title : 쇼의 제목.
- popular_rank : 인기도를 기준으로 필터링했을 때 IMDB에서 제공하는 순위입니다.
- certificate : 쇼에서받은 연령 인증을 포함합니다. 많은 null 값.
- startYear : 쇼가 처음 방송 된 때.
- endYear : 쇼 엔딩 연도
- episodes : 프로그램의 에피소드 수입니다. 영화의 경우 1입니다.
- 유형 : 영화 또는 시리즈
- orign_country : 프로그램이 시작된 국가
- 언어 : 쇼의 언어.
- 줄거리 : 쇼의 시놉시스.
- 요약 : 쇼의 이야기 요약.
- rating : 쇼에 주어진 평균 평점.
- numVotes : 쇼에서받은 투표 수.
- genres : 쇼가 속한 장르.
- isAdult : 1 성인용 콘텐츠가있는 경우. 그렇지 않은 경우 0입니다.
- cast : 목록 형식으로 쇼의 메인 캐스트.
- image_url : 포스터 이미지 링크.



#### 4. Netflix Movies and TV Shows

https://www.kaggle.com/adityakadiwal/netflix-movies-and-tv-shows

- 제목 : 영화 / TV 쇼의 이름
- 유형 : 컨텐츠의 종류는
- titlereleased : 년 릴리스의
- 평가 : TV 부모 가이드 라인 평가
- 품질 : 제목의 비디오 품질
- 배우 : 영화 / TV 쇼의 캐스트
- 감독 : 감독 영화 / TV 쇼
- category : 장르 또는 카테고리
- imdb : 영화 / TV 쇼
- 런타임에 대한 IMDb 등급 : 영화 / TV 쇼 런타임 (** 분)



### 넷플릭스 분석 보고서 참조 데이터셋 - 기존 보고서를 이용한 새로운 데이터셋

