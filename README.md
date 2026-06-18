# Nuclei Poc 全网收集
NucleiPocGather，每日更新

这个项目是一个 Python 脚本，用于批量克隆 GitHub 项目，获取 Nuclei POC，并将 POC 按类别分类存放到文件夹中。同时，使用 GitHub Action 每日自动运行脚本。
# POC 详情统计

> **当前项目 POC 更新时间：**`2026-06-18 16:02`

| ID | 标签      | 数量 | 目录       | 数量 | 严重性   | 数量 |
|:---| :-------- | :--- | :--------- | :--- | :------- | :--- |
| 1 | cve | 100949 | other | 55467 | medium | 41986 |
| 2 | wordpress | 94521 | cve | 54466 | low | 35308 |
| 3 | wp-plugin | 86688 | sql | 10311 | high | 27327 |
| 4 | medium | 33134 | wordpress | 7609 | info | 27149 |
| 5 | low | 33084 | auth | 4379 | critical | 15733 |
| 6 | candidate | 32795 | detect | 1873 | unknown | 134 |
| 7 | tech | 17899 | remote_code_execution | 1699 | informative | 19 |
| 8 | detect | 17135 | microsoft | 1396 | meduim | 19 |
| 9 | high | 16254 | web | 1385 | hight | 15 |
| 10 | service | 13838 | api | 1103 | cretical | 4 |

**81 个目录，44572 个文件**
## 如何使用

### 克隆项目

克隆这个项目到本地：

```bash
git clone https://github.com/lianqingsec/NucleiPocGather.git
```

进入项目目录：

```bash
cd NucleiPocGather
```

### 配置

在 `repo.txt` 文件中配置监控 GitHub 项目信息。

### 运行脚本

运行 Python 脚本：

```bash
python NucleiPocGather.py
```

### GitHub Action

在 GitHub 仓库中设置 Action，以便每日自动运行脚本。

> 需要配置`Workflow permissions`为`Read and write`权限

## 文件结构

- `NucleiPocGather.py`: 收集全网 Nuclei POC 的脚本文件。
- `DeWeight.py`: 对现有的 Nuclei POC 进行进一步去重的脚本文件。
- `WirteREADME.py`: 统计现有的 POC 并更新 README.md 文件。
- `repo.txt`: Nuclei POC 仓库列表。
- `poc.txt`: 已存档 POC 列表。
- `poc/`: 存放分类后的 Nuclei POC 文件夹。

