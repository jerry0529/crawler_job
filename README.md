# ETL爬蟲作業需求規格規劃
## 最終需求(產出) : 
### 找出目前人力需求最ㄏㄤ的IT人員所需的程式語言技能

## 輸入
### 無

## 流程:
### 到各大人力網站爬取相關職缺資料
[104]: https://www.104.com.tw/
[1111]: https://www.1111.com.tw/
[518]: https://www.518.com.tw/

- - -

### 

### 流程設計
 - 以104為例, 以"資訊軟體系統類"找工作, 會看到有19949筆,
   不知道有多少頁, 考量各種因素, 故初步先到各頁抓取各個職缺
   的網址, 存入DataBase

 - 從DataBase存入的網頁開始進入頁內爬取資料
 - 紀錄104網頁資料的table
 Create table src104 (
    href varchar(400) primary key,
    gotIt boolean,
    data text
 );

 - 1111, 518人力銀行的資料表如上
### DataBase規劃
 - 
