---
title: "Windows Sandbox"
description: "如何將資料家夾映射進Windows Sandbox"
published: 2025-10-20
---

# Windows Sandbox
Windows 沙箱(Windows Sandbox) 是Windows Pro 版的附加的可選元件。  

# 將資料夾映射進Sandbox
Windows Sandbox的副檔名為`.wsb`，使用XML格式  

> - 範例

```
<Configuration>
  <MappedFolders>
    <MappedFolder>
      <HostFolder>[PATH]</HostFolder>
      <ReadOnly>false</ReadOnly>
    </MappedFolder>
  </MappedFolders>
</Configuration>
```
將要映射進Sandbox的資料夾目錄填入[PATH]，打開`.wsb`檔案設定的目錄就會出現在沙箱桌面