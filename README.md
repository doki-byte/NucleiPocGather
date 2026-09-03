# Nuclei Poc 全网收集
NucleiPocGather，每日更新

这个项目是一个 Python 脚本，用于批量克隆 GitHub 项目，获取 Nuclei POC，并将 POC 按类别分类存放到文件夹中。同时，使用 GitHub Action 每日自动运行脚本。
# POC 详情统计

> **当前项目 POC 更新时间：**`2026-09-03 16:21`

| ID | 标签      | 数量 | 目录       | 数量 | 严重性   | 数量 |
|:---| :-------- | :--- | :--------- | :--- | :------- | :--- |
| 1 | cve | 96695 | other | 56377 | medium | 40214 |
| 2 | wordpress | 90213 | cve | 50079 | low | 34216 |
| 3 | wp-plugin | 83504 | sql | 9093 | high | 28063 |
| 4 | candidate | 32665 | wordpress | 5999 | info | 27445 |
| 5 | low | 31766 | auth | 4615 | critical | 15076 |
| 6 | medium | 30744 | remote_code_execution | 3923 | unknown | 138 |
| 7 | tech | 17504 | detect | 1967 | informative | 17 |
| 8 | detect | 16608 | web | 1443 | hight | 15 |
| 9 | high | 16466 | microsoft | 1306 | meduim | 9 |
| 10 | service | 13832 | api | 1145 | cretical | 4 |

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

