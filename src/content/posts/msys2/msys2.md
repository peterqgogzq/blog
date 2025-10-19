—-
title: "建置MSYS2環境"
description: "了解如何在Windows 系統上使用GNU編譯器以及其他的Linux程式"
published: 2025-10-19
—-

# msys2
 msys2是個輕量級類Unix shell ，可以安裝MinGW64等編譯器。  
官網&下載鏈結:[msys2](https://www.msys2.org)  
 
# pacman
`pacman`是一種Linux的程式版本控制器，被Arch Linux採用。而msys2也是用`pacman`管理安裝程式的版本。  

# 建置
下載msys2  
安裝好之後應該會有數個Linux 終端，推薦使用urct64  
打開終端，執行更新指令`pacman -Syu`  
待更新完成後再下載編譯器之類的組建  
[package查詢頁面](https://packages.msys2.org/queue)，像是[gcc](https://packages.msys2.org/packages/mingw-w64-ucrt-x86_64-gcc)，基本上安裝時會自動安裝依賴項，但編譯出錯時還是要手動檢查是否有缺少或衝突。  

# 下載好gcc，替換VSCode 的編譯器
1. 將`urct64-gcc`加入系統PATH
2. 編輯`.vscord`的工作區設定
