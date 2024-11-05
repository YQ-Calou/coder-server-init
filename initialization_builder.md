# 平台初始化工具使用方式

你應當會於資料夾中看到 initialization_builder.sh 之檔案

通常此刻暫時無法執行，需授予chmod權限

因此請打開console (Windows 為 ctrl + ~ / MacOS 為 control + ~)

於根目錄(~/workspace)執行以下指令
```bash
chmod 777 ./initialization_builder.sh
```

好了，此刻你已經完成chmod權限

接下來該啟動腳本

```bash
./initialization_builder.sh
```

然後選擇你要安裝的檔案即可

# 關於zip

你要打包東西的話，就是在跟目錄下(~/workspace)使用
```bash
zip -r 你要的檔案名稱.zip 資料夾
```

等他跑完後
然後在左側對要下載的檔案 右鍵 > 下載

# 關於 rclone

rclone一率建議使用sudo權限
創建config
```bash
sudo rclone config
```

接下來
```bash
sudo rclone mount 伺服器名稱:路徑 本地路徑 --vfs-cache-mode writes --allow-other
```

# 備註

開發者 : Calou Zhou