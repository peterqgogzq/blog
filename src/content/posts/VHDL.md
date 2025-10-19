---
title: "VHDL"
description: "超高速硬體描述語言"
published: 2025-10-19
---
# VHDL 是什麼
VHDL全稱超高速積體電路描述語言，從IEEE發表IEEE 1076-198之後，被各大EDA採用。

# VHDL基本語法
 1. 不分大小寫
 2. 標頭檔(?  
`library ieee:` —使用IEEE函式庫  
`use ieee.std_logic_1164`—使用IEEE 1164(基本邏輯閘)包  
3. entity
```entity <name> is
    port(
                A : IN STD_LOGIC;
                B : OUT STD_LOGIC
            )
end [name];
```
4. architecture
```architecture <architecture> of <name> is
begin
    —configuration 
end [architecture] ;
```
 VHDL實例
`待補充`
