# GCP

相關套件

pip install google-cloud-bigquery

pip install db-dtypes

pip install protobuf

pip install pandas

pip install google-auth

pip install google-api-core

pip install grpcio

點選Compute Engine-連線-SSH-V箭頭-複製gcloud 指令-貼上Google Cloud SDK shell 成功連線到 VM

✅ 什麼是 gsutil？

gsutil 是 Google 提供的 命令列工具，用來操作 Google Cloud Storage（GCS）裡的 Bucket 和檔案。

你可以把它想成是 GCS 的指令版 Google Drive 工具，像是上傳、下載、刪除、同步、列出檔案等都能做！

它是 Google Cloud SDK 的一部分，只要有安裝 SDK，就有 gsutil 可以用。

🛠 常見 gsutil 指令整理

功能	指令格式	說明

🔍 列出檔案	gsutil ls gs://你的bucket/	顯示 bucket 或路徑下的檔案

📤 上傳檔案	gsutil cp 本地路徑 gs://你的bucket/	把本機的檔案上傳到 GCS

📥 下載檔案	gsutil cp gs://你的bucket/檔案 ./本地/路徑/	從 GCS 下載到本地端

🧽 刪除檔案	gsutil rm gs://你的bucket/檔案	刪除雲端某個檔案

📁 同步資料夾	gsutil rsync -r -d ./local gs://你的bucket/目錄/	本地與 GCS 雙邊同步

📦 建立 bucket	gsutil mb gs://新bucket名稱/	建立一個新的 GCS 儲存空間

🧾 檢查檔案資訊	gsutil stat gs://你的bucket/檔案	看單一檔案的詳細資料
