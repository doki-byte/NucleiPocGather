# Nuclei Poc 全网收集
NucleiPocGather，每日更新

这个项目是一个 Python 脚本，用于批量克隆 GitHub 项目，获取 Nuclei POC，并将 POC 按类别分类存放到文件夹中。同时，使用 GitHub Action 每日自动运行脚本。
# POC 详情统计

> **当前项目 POC 更新时间：**`2025-07-17 13:34`

| ID | 标签      | 数量 | 目录       | 数量 | 严重性   | 数量 |
|:---| :-------- | :--- | :--------- | :--- | :------- | :--- |
| 1 | cve | 40556 | cve | 33344 | medium | 22098 |
| 2 | wordpress | 36057 | other | 26891 | info | 21458 |
| 3 | wp-plugin | 33503 | sql | 2352 | high | 13609 |
| 4 | tech | 15747 | auth | 2059 | low | 10344 |
| 5 | medium | 15695 | detect | 1408 | critical | 7582 |
| 6 | detect | 14940 | remote_code_execution | 1328 | unknown | 102 |
| 7 | service | 11684 | wordpress | 1112 | informative | 17 |
| 8 | low | 9129 | default | 731 | hight | 16 |
| 9 | high | 6332 | web | 550 | meduim | 4 |
| 10 | http | 4357 | microsoft | 539 | cretical | 2 |

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

