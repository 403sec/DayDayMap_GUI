

<p align="center"> <img width="200" height="100" alt="logoLeft" src="https://github.com/user-attachments/assets/fd1ef2e4-4256-4edc-ae8a-3f262d7bd44d" /> </p>


**<p align="center">  DayDayMap官网：https://www.daydaymap.com  </p>**

**<p align="center">  DayDayMap网络安全空间测绘-首款GUI工具  </p>**


# 🛡️ DayDayMap 网络空间资产测绘工具

![Release](https://img.shields.io/badge/RELEASE-V2.0-e74c3c?style=flat-square)
![Language](https://img.shields.io/badge/LANGUAGE-PYTHON_3-3498db?style=flat-square&logo=python&logoColor=white)
![Platform](https://img.shields.io/badge/PLATFORM-WINDOWS-2ecc71?style=flat-square&logo=windows&logoColor=white)
![Focus](https://img.shields.io/badge/FOCUS-ASSET_MAPPING-f39c12?style=flat-square)
![License](https://img.shields.io/badge/LICENSE-MIT-lightgrey?style=flat-square)

> 🚀 **轻量级、高性能网络空间资产测绘图形化工具。**

> 🚀**集成多 API 轮换、智能数据导出、语法自动补全及多线程并发查询，助力安全研究员与红蓝对抗从业者快速发现资产暴露面。**

---

## 🖼️ 工具演示 (Screenshot)

### 1、特色：语法提示

输入语法，web.  会提示以web.开头的所有语法。
点击提示的语法，直接输入到查询框。

<img width="2001" height="1480" alt="PixPin_2026-01-14_16-29-43" src="https://github.com/user-attachments/assets/bc93bf32-760c-4f9c-84f9-20a6853161f1" />

### 2、特色：导出功能

为了不浪费API资源
导出页面分为：当前页、已经查看的页、所有页

<img width="2002" height="1483" alt="PixPin_2026-01-14_16-32-06" src="https://github.com/user-attachments/assets/865b5c90-7339-4f71-9b3c-cea8b6da835a" />

### 3、代理功能

当图标是绿色状态，代理是开启状态，支持http和sockts5两种代理模式。

<img width="2000" height="1137" alt="PixPin_2026-01-14_16-35-54" src="https://github.com/user-attachments/assets/e47dcda4-cc75-4642-8cc6-9ae7ecb6ec86" />

### 4、特色：支持key的轮转

当前key的额度用完时，会切换到下一个key去查询。
可以通过key管理，去添加和删除key

<img width="2000" height="1304" alt="PixPin_2026-01-14_16-41-01" src="https://github.com/user-attachments/assets/3680b4b6-4935-4efc-bf42-6351b4ffe5b8" />

---

## ✨ 核心功能 (Features)

本工具正式版本 (V2.0) 经过作者本地多个版本的深度优化，提升查询效率与数据处理：

### 🔍 深度查询与交互

* **多标签页支持**：支持同时开启多个查询任务，标签页独立管理，互不干扰。
* **智能语法提示**：内置自动补全 (Auto-suggest) 功能，输入关键词（如 `ip`、`port`）自动提示查询语法。
* **语法速查手册**：顶部内置「📖 语法查询」按钮，弹窗展示常用语法并支持滚动查看。
* **交互优化**：支持**右键菜单**（复制/打开链接）、**中键点击关闭标签**，以及底部的全局操作指引栏。

### ⚙️ 高级配置与网络

* **API Key 轮换**：支持添加多个 API Key，遇到限流或积分不足时自动轮换，保障任务不中断。
* **代理支持**：内置 HTTP/SOCKS5 代理配置，支持一键开关，保护隐私并绕过网络限制。
* **配置持久化**：所有的 API Key、代理设置、窗口大小及历史记录均自动保存至本地 JSON 文件。

### 💾 智能导出系统 (Smart Export)

* **自定义列导出**：支持 CSV 和 JSON 格式，可自由勾选需要导出的字段。
* **智能 URL 拼接**：导出时自动生成 **`拼接目标 (URL)`** 列（例如 `https://1.1.1.1:8443` 或 `ssh://192.168.1.1:22`），位于表格首列，方便直接导入漏洞扫描工具（如 Nuclei, Xray）。
* **批量下载**：支持多线程批量导出当前搜索结果的所有分页数据。
