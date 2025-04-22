# Verilog AND Gate Project

這是用 Verilog 實作 AND Gate 的專案，包括：

- `and_gate.v`: AND Gate 模組  
- `and_gate_tb.v`: 測試平台  
- `monitor_log.txt`: 模擬輸出的結果紀錄  

---

## 使用工具

- Verilog HDL  
- ModelSim 10.5b  

---

## 模擬步驟（ModelSim 指令）

```shell
vlog src/and_gate.v tb/and_gate_tb.v
vsim work.and_gate_tb
add wave *
run -all
模擬輸出（monitor_log.txt）
ini
複製
編輯
a=0, b=0, y=0 @ 10000 ns  
a=0, b=1, y=0 @ 20000 ns  
a=1, b=0, y=0 @ 30000 ns  
a=1, b=1, y=1 @ 40000 ns 
 
```
---