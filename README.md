# Nuclei Poc 全网收集
NucleiPocGather，每日更新

这个项目是一个 Python 脚本，用于批量克隆 GitHub 项目，获取 Nuclei POC，并将 POC 按类别分类存放到文件夹中。同时，使用 GitHub Action 每日自动运行脚本。
# POC 详情统计

> **当前项目 POC 更新时间：**`2026-10-04 16:58`

| ID | 标签      | 数量 | 目录       | 数量 | 严重性   | 数量 |
|:---| :-------- | :--- | :--------- | :--- | :------- | :--- |
| 1 | cve | 113115 | cve | 64297 | medium | 45536 |
| 2 | wordpress | 106501 | other | 59012 | low | 39975 |
| 3 | wp-plugin | 98018 | wordpress | 6364 | high | 30209 |
| 4 | low | 37824 | auth | 4837 | info | 27390 |
| 5 | medium | 36319 | sql | 4418 | critical | 17438 |
| 6 | candidate | 35370 | detect | 2683 | unknown | 141 |
| 7 | high | 18840 | microsoft | 2532 | informative | 16 |
| 8 | tech | 17720 | remote_code_execution | 2350 | meduim | 16 |
| 9 | production | 17383 | web | 1437 | hight | 15 |
| 10 | detect | 16869 | social | 1297 | cretical | 4 |

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

