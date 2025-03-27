# RISC-V 指令集

## Arithmetic Operations
- **ADD**: 加法 (`ADD rd, rs1, rs2`)
- **ADDI**: 立即數加法 (`ADDI rd, rs1, imm`)
- **SUB**: 減法 (`SUB rd, rs1, rs2`)
- **SLL**: 邏輯左移 (`SLL rd, rs1, rs2`)
- **SLLI**: 立即數邏輯左移 (`SLLI rd, rs1, imm`)
- **SLT**: 設置小於 (`SLT rd, rs1, rs2`)
- **SLTI**: 設置小於立即數 (`SLTI rd, rs1, imm`)
- **SLTU**: 無符號小於 (`SLTU rd, rs1, rs2`)
- **SLTIU**: 無符號小於立即數 (`SLTIU rd, rs1, imm`)
- **XOR**: 異或 (`XOR rd, rs1, rs2`)
- **XORI**: 異或立即數 (`XORI rd, rs1, imm`)
- **OR**: 位或 (`OR rd, rs1, rs2`)
- **ORI**: 位或立即數 (`ORI rd, rs1, imm`)
- **AND**: 位與 (`AND rd, rs1, rs2`)
- **ANDI**: 位與立即數 (`ANDI rd, rs1, imm`)

## Extended
- **MUL**: 乘法 (`MUL rd, rs1, rs2`)
- **MULH**: 高位乘法 (`MULH rd, rs1, rs2`)
- **MULHSU**: 高位有符號乘法 (`MULHSU rd, rs1, rs2`)
- **MULHU**: 高位無符號乘法 (`MULHU rd, rs1, rs2`)
- **DIV**: 除法 (`DIV rd, rs1, rs2`)
- **DIVU**: 無符號除法 (`DIVU rd, rs1, rs2`)
- **REM**: 餘數 (`REM rd, rs1, rs2`)
- **REMU**: 無符號餘數 (`REMU rd, rs1, rs2`)

## Control Flow Instructions
- **BEQ**: 相等跳轉 (`BEQ rs1, rs2, offset`)
- **BNE**: 不相等跳轉 (`BNE rs1, rs2, offset`)
- **BLT**: 小於跳轉 (`BLT rs1, rs2, offset`)
- **BGE**: 大於等於跳轉 (`BGE rs1, rs2, offset`)
- **BLTU**: 無符號小於跳轉 (`BLTU rs1, rs2, offset`)
- **BGEU**: 無符號大於等於跳轉 (`BGEU rs1, rs2, offset`)
- **JAL**: 跳躍並鏈接 (`JAL rd, offset`)
- **JALR**: 跳躍並鏈接 (`JALR rd, rs1, offset`)

## Memory Access Instructions
- **LW**: 加載字 (`LW rd, offset(rs1)`)
- **LH**: 加載半字 (`LH rd, offset(rs1)`)
- **LB**: 加載字節 (`LB rd, offset(rs1)`)
- **LBU**: 加載無符號字節 (`LBU rd, offset(rs1)`)
- **LHU**: 加載無符號半字 (`LHU rd, offset(rs1)`)
- **SW**: 儲存字 (`SW rs2, offset(rs1)`)
- **SH**: 儲存半字 (`SH rs2, offset(rs1)`)
- **SB**: 儲存字節 (`SB rs2, offset(rs1)`)

## Atomic Operations
- **LR.W**: 加載保留 (`LR.W rd, (rs1)`)
- **SC.W**: 儲存條件 (`SC.W rd, rs2, (rs1)`)

## System Instructions
- **ECALL**: 系統呼叫 (`ECALL`)
- **EBREAK**: 中斷指令 (`EBREAK`)

## Shift Instructions
- **SRA**: 算術右移 (`SRA rd, rs1, rs2`)
- **SRAI**: 立即數算術右移 (`SRAI rd, rs1, imm`)
- **SRL**: 邏輯右移 (`SRL rd, rs1, rs2`)
- **SRLI**: 立即數邏輯右移 (`SRLI rd, rs1, imm`)

## Comparison and Branching Instructions
- **BEQZ**: 比較是否為零 (`BEQZ rs1, offset`)
- **BNEZ**: 比較是否不為零 (`BNEZ rs1, offset`)

## Immediate Instructions
- **LUI**: 加載高位立即數 (`LUI rd, imm`)
- **AUIPC**: 加載高位PC並加法 (`AUIPC rd, imm`)

## Floating Point
- **FMADD.S**: 單精度浮點數乘加 (`FMADD.S rd, rs1, rs2, rs3`)
- **FADD.S**: 單精度浮點加法 (`FADD.S rd, rs1, rs2`)
- **FSUB.S**: 單精度浮點減法 (`FSUB.S rd, rs1, rs2`)

## 其他
- **NOP**: 空操作 (`NOP`，無操作指令)
- **FENCE**: 記憶體屏障 (`FENCE`)
