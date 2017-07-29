# 2017-104Hackathon Mobile App / Web Service

104首次開放海量職缺工作細節內容，及珍貴求職者行為資料，請參賽者發揮創意，打造職場媒合相關創新服務。
## 活動網址
+ https://www.104.com.tw/2017hackathon/
+ Leader Board：https://hackathon2017.events.104.com.tw
## 主題說明
最佳人性化的設計，來自於傾聽user insight，利用主辦單位特定時間區間內去識別化的行為記錄（user Log），達到觀測真實行為目的。參賽者歡迎使用主辦單位所提供之資料集，設計製作徵才或求職相關的 App、Web Service。
## 範例 - 我要活下去之何處是我家
使用 __政府統計資訊網的家庭收支-平均每戶全年經常性支出__，與 __104職務資料集中有提供薪水資訊的職務資料__，加上一個簡單的職務名稱推薦職缺類別的分類器，接上line-bot的api後，就可以完成一個在哪裡工作CP值最高的line機器人。  

[詳細說明](https://github.com/104corp/2017-104Hackathon-AppWebService/tree/master/linebot-example)  

<img src="https://github.com/104corp/2017-104Hackathon-AppWebService/blob/master/linebot-example/line_screenshot.png"  width="50%">

## 資料集說明
* 104 Job Search API
    + 透過104的Job Search API取得職務和公司資訊
    + [Link](http://www.104.com.tw/i/api_doc/jobsearch/)
* 104求職者去識別化行為記錄
    + File: user_log.csv
    + Description：求職者在104網站上瀏覽應徵職務時的行為log
    + Date: 2016-04 ~ 2017-03
    + [Schema](https://github.com/104corp/2017-104Hackathon-AppWebService/blob/master/data-schema/user_log_schema.md)
    + [Sample](https://github.com/104corp/2017-104Hackathon-AppWebService/blob/master/sample-data/user_log_sample.csv) 
    + 訓練資料集將在賽前以Email通知參賽者
* 公司與職務資料
    + 上市櫃公司與五百大企業
        - File: companies.csv 
        - Decription: 台灣所有上市櫃公司與資本額前五百大企業，共有1147間公司
        - [Schema](https://github.com/104corp/2017-104Hackathon-AppWebService/blob/master/data-schema/companies_schema.md)
        - [Sample](https://github.com/104corp/2017-104Hackathon-AppWebService/blob/master/sample-data/companies_sample.csv)
        - 訓練資料集將在賽前以Email通知參賽者
    + 職務資料
        - File: job_structured_info.csv, job_description.csv
        - Description: 對每一筆職務結構化的欄位資料與該職務的文字描述
        - Date: 2017/03/29
        - [Job Description Schema](https://github.com/104corp/2017-104Hackathon-AppWebService/blob/master/data-schema/job_description_schema.md)
        - [Job Structured Info Schema](https://github.com/104corp/2017-104Hackathon-AppWebService/blob/master/data-schema/job_structured_info_schema.md)
        - [Job Description Sample](https://github.com/104corp/2017-104Hackathon-AppWebService/blob/master/sample-data/job_description_sample.csv)
        - [Job Structured Info Sample](https://github.com/104corp/2017-104Hackathon-AppWebService/blob/master/sample-data/job_structured_info_sample.csv)
        - 訓練資料集將在賽前以Email通知參賽者
    + 職務異動歷史資料
        - File: job_structured_info_{yyyymm}.csv, job_description_{yyyymm}.csv
        - Description: 對每一筆職務結構化的欄位資料與該職務文字描述的修改歷程
        - Date: 2014/03 - 2017/03/31 
        - [Job Description History Schema](https://github.com/104corp/2017-104Hackathon-AppWebService/blob/master/data-schema/job_description_history_schema.md)
        - [Job Structured Info History Schema](https://github.com/104corp/2017-104Hackathon-AppWebService/blob/master/data-schema/job_structured_info_history_schema.md)
        - [Job Description History Sample](https://github.com/104corp/2017-104Hackathon-AppWebService/blob/master/sample-data/job_description_2014_sample.csv)
        - [Job Structured Info History Sample](https://github.com/104corp/2017-104Hackathon-AppWebService/blob/master/sample-data/job_structured_info_2014_sample.csv)
        - 訓練資料集將在賽前以Email通知參賽者
    + 類目資料
        - File:
            - 科系類目: department.csv [Sample](https://github.com/104corp/2017-104Hackathon-AppWebService/blob/master/sample-data/department_sample.csv)
            - 地區類目: district.csv [Sample](https://github.com/104corp/2017-104Hackathon-AppWebService/blob/master/sample-data/district_sample.csv)
            - 產業類目: industry.csv [Sample](https://github.com/104corp/2017-104Hackathon-AppWebService/blob/master/sample-data/industry_sample.csv)
            - 職務類目: job_category.csv [Sample](https://github.com/104corp/2017-104Hackathon-AppWebService/blob/master/sample-data/job_category_sample.csv)
        - Description: 在職務結構化欄位中的類目對照
        - 訓練資料集將在賽前以Email通知參賽者

## 評分標準
* 創新70%
* 作品效益20%
* 價值10%（包含資料應用狀況、創意綜合評估、價值效益等）

## 104開放資料授權條款 
【2017-104-hackathon-dataset】是 2017年104資訊科技Hackathon活動中開放的資料集。當您使用104提供之【2017-104-hackathon-dataset】資料集時，即表示您已閱讀、瞭解並同意接受本授權條款所訂定之所有內容。本授權條款得隨時修訂並公告於本頁面上，修訂後之內容自公告時起生效，授權說明如下：

* 使用者權利：
    + 使用者得自由應用104提供的資料集，產生新的程式、文件、圖表等著作，使用者亦可自由修改104提供的資料集，衍生新的資料集，使用者基於本活動目的範圍的任何使用方式，無須104再為授權。
* 使用者義務：
    + 使用者必須在您的著作或衍生資料集明確標示【2017年104資訊科技Hackathon】為資料來源，與此份說明文件的連結。
    + 使用者違反前項標示義務，視為自始未取得104開放資料之授權，須負擔所有相關之法律責任。
* 使用者規範：
    1. 使用者不可使用可能造成104會員混淆或困擾的商標或名稱，或為任何違反104會員服務條款或本活動授權規範之行為。
    2. 使用者不可違反中華民國法令，或造成第三人發生違反中華民國法令的行為。
    3. 使用者保證不可另為提供他人資料集下載，意即，使用者不得複製一份資料集到您自己的網路服務上供他人下載，但您可以提供他人此份說明文件的連結。使用者同意且了解，若您利用104提供的資料集，開發任何妨礙善良風俗之違法服務或程式工具，104並不為此負擔任何法律連帶責任。
    4. 使用者不得意圖或為任何可能損害104商譽或侵害104資料之任何行為或聲明。
    5. 謝絕競業使用，作任何商業營利或非商業研究分析之用。
    6. 本條款之解釋、效力、履行及其他未盡事宜，以中華民國法律為準據法。
