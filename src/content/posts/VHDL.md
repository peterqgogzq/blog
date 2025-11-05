---
title: "VHDL"
description: "超高速積體電路硬體描述語言"
published: 2025-10-19
---
# VHDL 是什麼
VHDL全稱超高速積體電路硬體描述語言，從IEEE發表IEEE 1076-198標準之後，被各大EDA採用。常用於PLD設計模擬或是積體電路設計等場合。  
它可用於：
> - 模擬（Simulation）：驗證邏輯功能是否正確。  
> - 綜合（Synthesis）：由程式碼自動生成邏輯閘與電路（如FPGA或ASIC設計）。  

VHDL 同時具備：  
> - 結構化（Structural）描述：用組件（component）與連線（signal）描述電路。  
> - 行為式（Behavioral）描述：用流程與條件語句描述功能。  
> - 資料流式（Dataflow）描述：用並行的訊號指派描述訊號關係。  

# VHDL基本語法
 1. 不分大小寫
 2. 標頭檔  
`library ieee:` —使用IEEE函式庫  
`use ieee.std_logic_1164`—使用IEEE 1164(基本邏輯閘)包  

常見套件(Package):  
> - `IEEE.STD_LOGIC_1164` : 基本邏輯  
> - `IEEE.NUMERIC_STD` : 定義`SIGNED`、`UNSIGNED`型別與標準化的加減乘除運算  
還有其他電路模擬用的套件

3. entity
```VHDL
entity <name> is
    port(
                A : IN STD_LOGIC;
                B : OUT STD_LOGIC
            )
end [name];
```

4. architecture
```VHDL
architecture <architecture> of <name> is
begin
    —configuration 
end [architecture] ;
```
 VHDL實例
`待補充`
