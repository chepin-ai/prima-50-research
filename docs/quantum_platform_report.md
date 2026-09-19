# 量子平台连接报告

> 生成时间: 2026-03-22  
> 测试平台: Qiskit Aer, IBM Quantum, 本源量子, Quafu, BlueQubit, FieldQKit

---

## 连接状态汇总

| 平台 | 类型 | 状态 | 保真度/加速 | 备注 |
|------|------|------|-------------|------|
| Qiskit Aer | 模拟器 | ✅ 通过 | Bell=1.0, Grover=4x | 理想无噪声 |
| IBM Quantum | 超导真实 | ⏳ 待Token | N/A | 需 quantum.ibm.com |
| 本源量子 | 超导真实 | ⏳ 待端点 | N/A | 6个API Key已备 |
| Quafu | 云平台 | ⚠️ 端点404 | N/A | 需确认正确API |
| BlueQubit | 云平台 | ⚠️ DNS失败 | N/A | 需确认正确域名 |
| FieldQKit | 未知 | ❓ 信息不足 | N/A | 需API文档 |

---

## Qiskit Aer 详细结果

### Bell态纠缠
```
|00⟩: 4096 (50.0%) ██████████
|01⟩:    0 ( 0.0%)
|10⟩:    0 ( 0.0%)
|11⟩: 4096 (50.0%) ██████████
保真度: 1.0000
```

### GHZ态纠缠
```
|000⟩: 4068 (49.7%) ██████████
|111⟩: 4124 (50.3%) ██████████
保真度: 1.0000
```

### Grover搜索 (标记|11⟩)
```
|11⟩概率: 100.0% 🎯
经典随机: 25.0%
量子加速: 4.00x
```

---

## 真实硬件连接指南

### IBM Quantum
1. 访问 https://quantum.ibm.com/
2. 登录 chepin@163.com
3. Account Settings → API Token
4. 使用Token连接真实超导芯片

### 本源量子
1. 访问 https://qcloud.originqc.com.cn/
2. 使用 chepin@163.com 登录
3. 确认API端点和认证方式
4. 使用提供的6个API Key

### Quafu
1. 访问 https://quafu.baqis.ac.cn/
2. 确认REST API文档
3. 使用提供的Token和API Key

---

## 凭据清单 (已提供)

- IBM: TOTP种子 6UP3WKCVIIRGDB4I
- 本源量子: 6个API Key
- Quafu: Token + API Key
- BlueQubit: API Key AIzaSyCGAUsmDg5qu0NLYuOdheamgElaqwjdSug

---

*注意: 所有凭据仅用于研究目的，建议定期轮换。*
