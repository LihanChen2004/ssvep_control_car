# ssvep_control_car

## 1. Overview

基于稳态视觉诱发电位的脑控小车

## 2. Quick Start

### 2.1 Setup Environment

- [uv](https://docs.astral.sh/uv/getting-started/installation/)
- [Microsoft Visual C++](https://visualstudio.microsoft.com/visual-cpp-build-tools/)
  - .NET Framework 4.8 SDK
  - 适用于.NET Framework 4.8 工具包
  - 用于 v142 生成工具(14.29.16.26) 的 C++/CLI 支持

### 2.2 Create Workspace

```shell
git clone git@github.com:LihanChen2004/ssvep_control_car.git
```

### 2.3 Build

```shell
uv sync
```

```shell
uv tool install pyinstaller
```

```shell
pyinstaller -i "resource\cc.ico" -F ssvep_car.py lsl_received_data.py model.py
```

### 2.4 Run

```shell
uv run ssvep_car.py
```
