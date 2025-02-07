---
layout: default
title: クラウド帳票 HRBC設定マニュアル
---

# クラウド帳票 HRBC設定マニュアル

## HRBCからクラウド帳票への画面遷移

HRBCからクラウド帳票を利用する場合、HRBCのアクションメニューから遷移します。

![アクションメニュー例](images/hrbc/hrbc_actionmenu_1.png)

### 設定手順

※HRBCにシステム管理者権限でのログインが必要です

1. 設定→カスタマイズの順に選択します
2. アクションメニュー編集を選択
3. アクションメニューを設定するリソースを選択します
   ![アクションメニュー／リソースの選択](images/hrbc/hrbc_actionmenu_2.png)
4. 隣に表示されたリストからアクションメニューを選択します
5. アクションメニューを追加します
   ![アクションメニュー／追加](images/hrbc/hrbc_actionmenu_3.png)
    * 英語：任意の文字列　例：report-output
    * 日本語：任意の文字列　例：帳票出力
    * URL：URL一覧を参照

### URL一覧

#### 利用可能

|リソース|URL|
|-----|-----|
|個人連絡先|https://【利用中のドメイン】.report-cloud.com/report/candidate/\{\{Person.P_Id\}\}?user=\{\{Session.P_UserId\}\}|
|JOB|https://【利用中のドメイン】.report-cloud.com/report/job/\{\{Job.P_Id\}\}?user=\{\{Session.P_UserId\}\}|
|売上|https://【利用中のドメイン】.report-cloud.com/report/sales/\{\{Sales.P_Id\}\}?user=\{\{Session.P_UserId\}\}|
|レジュメ|https://【利用中のドメイン】.report-cloud.com/report/resume/\{\{Resume.P_Id\}\}?user=\{\{Session.P_UserId\}\}|

#### 準備中

|リソース|URL|
|-----|-----|
|企業|https://【利用中のドメイン】.report-cloud.com/report/client/\{\{Client.P_Id\}\}?user=\{\{Session.P_UserId\}\}|
|選考プロセス|https://【利用中のドメイン】.report-cloud.com/report/process/\{\{Process.P_Id\}\}?user=\{\{Session.P_UserId\}\}|
|企業担当者|https://【利用中のドメイン】.report-cloud.com/report/recruiter/\{\{Recruiter.P_Id\}\}?user=\{\{Session.P_UserId\}\}|
|アクティビティ|https://【利用中のドメイン】.report-cloud.com/report/activity/\{\{Activity.P_Id\}\}?user=\{\{Session.P_UserId\}\}|

-----
* 2020年12月25日新規作成

{% include footer.md %}
