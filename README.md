# GCP帳號申辦與建置GCP Project


# 環境準備

建置 Project

建置 cloud storage

建置 firestore

# 程式碼準備與部署

程式碼匯入
pip3 install -r requirements.txt

# 構建程式碼

```
gcloud config set project YOUR-PROJECT-ID
gcloud builds submit  --tag gcr.io/$GOOGLE_CLOUD_PROJECT/meat-bot-dev:0.0.1
```

# 部署

指定環境變數

```
USER_INFO_GS_BUCKET_NAME:  剛剛建立的資料桶子
LINE_CHANNEL_ACCESS_TOKEN: 課程內述說
LINE_CHANNEL_SECRET: 課程內述說
```
# 將生成的網址追加callback 貼回line網站的webhook
