# Big-Data-Analysis-Practice-Level-2

한국정보인재개발원(www.krdi.co.kr)

[교육안내]
- 교육명 : 빅데이터분석실무 2급
- 교육기관 : 가천대학교
- 교육 일정 : 11월 25일(토) ~ 26일(일) / 09:00~18:00
- 시험 일정 : 11월 26일(일) / 17:30~18:00
- 합격 일자 : 12월 11일(월) 11시~15시 발표예정.

![image](https://github.com/Kyung-Min-Na/Big-Data-Analysis-Practice-Level-2/assets/133650591/e505b182-faf9-4f2c-b868-69b4c20b023f)

------------------------------------------------------------------------------------
## 1. R(4.1.3) 설치

   ![image](https://github.com/Kyung-Min-Na/Big-Data-Analysis-Practice-Level-2/assets/133650591/67ca54cc-121c-4487-ba7f-b4e398004777)

  https://cran.yu.ac.kr/bin/windows/base/old/4.1.3/
  R-4.1.3-win.exe - 관리자 권한으로 실행
  *64-bit or 32-bit중 하나만 선택(64-bit으로 진행)


## 2. JAVA 설치

  ![image](https://github.com/Kyung-Min-Na/Big-Data-Analysis-Practice-Level-2/assets/133650591/c5d57388-737c-4281-a155-b78397bc444c)

  https://www.java.com/ko/download/manual.jsp
  Windows 오프라인 (64비트) - 설치 후 관리자 권한으로 실행


## 3. KoNLP 패키지 설치

  ![image](https://github.com/Kyung-Min-Na/Big-Data-Analysis-Practice-Level-2/assets/133650591/888bae8b-3be0-470f-9dea-2aca4f008d55)

  1번에 설치한 R(4.1.3)을 관리자 권한으로 실행
  
  #Step 1. 의존성 패키지 설치

  install.packages(c("cli","hash", "tau", "Sejong", "RSQLite", "devtools", "bit", "rex", "lazyeval", "htmlwidgets", "crosstalk", "promises", "later", "sessioninfo", "xopen", "bit64", "blob", "DBI", "memoise", "plogr", "covr", "DT", "rcmdcheck", "rversions"), type = "binary")


  #Step 2. github 버전 설치

  install.packages("remotes")


  #Step 3. KoNLP 설치

  remotes::install_github('haven-jeon/KoNLP', upgrade = "never", INSTALL_opts=c("--no-multiarch"))
  library(KoNLP)


  #Step 4. 테스트하기

  ![image](https://github.com/Kyung-Min-Na/Big-Data-Analysis-Practice-Level-2/assets/133650591/49354df8-4088-490f-adf4-ac9e47b5b5f3)

  txt <- '나는 사과와 바나나가 좋아요'
  extractNoun(txt)

  
