---
title: "yt-dlp教學"
description: "yt-dlp教學"
pubDate: 2025-10-19
published: 2025-10-19
---

# yt-dlp教學

# 注意事項
本文僅作為學術分享 請勿用於非法用途

# 開始
[yt-dlp](https://github.com/yt-dlp/yt-dlp) 是款開源的Youtube下載工具，可以導入cookit來模仿使用者

將程式目錄加入system PATH就可以整合進CMD
在Windows搜索`檢視進階系統設定`<br>
![alt text](.\image1.png)<br>
找到環境變數<br>
![alt text](.\image2.png)<br>
在系統變數的Paht選項按編輯<br>
![alt text](.\image3.png)<br>
點選新增，將yt-dlp.exe的路徑貼上並保存<br>
![alt text](.\image4.png)<br>

# 指令與參數
`yt-dlp --version`列出版本號

參數:<br>
`--list-formats` 列出所有格式<br>
`-f [options] <URL>` 下載指定格式<br>
*下載指定格式的影片和音訊是分開的，必須同時下載並合成<br>
`-U` 更新套件

指定畫質<br>
`yt-dlp -f "bv[height<=<pixel>]+ba" <URL>`

下載影片<br>
`yt-dlp <URL>` 預設1080p

下載影片+字幕<br>
`yt-dlp --write-subs --embed-subs --sub-lang <language> <URL>`

# 使用cookies

`yt-dlp --cookies ["cookies PATH"] <URL>` <ba>
`yt-dlp --cookies-from-browser chrome <URL>`

# ffempg

[ffmpeg](https://www.ffmpeg.org/download.html)是一款輕量強大的軟體，本文用來合併視訊與音訊<br>
`ffmpeg -i <video> -i <audio> -c copy <output.mkv>`<br>
將下載的視訊和音訊檔按路徑貼在`<video>`和`<Audio>`的欄位裡，即可合併視訊和音訊檔案



