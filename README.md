<!-- 喵呜 -->
# RV32I 批量指令解码器

一个基于 Web 的 RV32I 指令集解码工具，支持将十六进制机器码批量转换为可读的汇编指令。提供文本输入和 COE 文件上传两种模式，支持数千行指令的快速解码，并可将结果导出为 TXT 文件。

## ✨ 功能特性

- **双模式输入**
  - 📝 **文本模式**：直接在文本框中输入多行十六进制代码，每行一条指令
  - 📂 **COE 文件模式**：上传 `.coe` 文件，自动跳过文件头两行，解析逗号分隔的十六进制指令

- **批量解码**
  - 支持超过 2000 行指令的同时解码
  - 左右对照显示：左侧为原始十六进制，右侧为对应的 RV32I 汇编指令

- **完整 RV32I 指令集支持**
  - R-type：ADD, SUB, SLL, SLT, SLTU, XOR, SRL, SRA, OR, AND
  - I-type：ADDI, SLLI, SLTI, SLTIU, XORI, SRLI, SRAI, ORI, ANDI, LB, LH, LW, LBU, LHU, JALR
  - S-type：SB, SH, SW
  - B-type：BEQ, BNE, BLT, BGE, BLTU, BGEU
  - U-type：LUI, AUIPC
  - J-type：JAL
  - 系统指令：ECALL, EBREAK, FENCE, CSR 指令

- **结果导出**
  - 一键将解码结果导出为 TXT 文件，包含行号、十六进制源码和汇编指令

- **实时解码**
  - 文本模式下输入时自动解码，无需手动点击按钮

## 🚀 快速开始

### 在线使用
1. 克隆或下载本仓库
2. 用浏览器打开 `index.html` 文件
3. 选择输入模式，输入或上传十六进制代码
4. 查看右侧解码结果

### 本地运行
```bash
git clone https://github.com/你的用户名/rv32i-decoder.git
cd rv32i-decoder
# 直接用浏览器打开 index.html 即可
