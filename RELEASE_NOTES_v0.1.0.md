# 译幕 Yimu Translate v0.1.0

Windows 桌端游戏画面实时翻译：持续捕获屏幕文字 → OCR → 翻译为中文 → 置顶悬浮窗展示。

## 下载与安装

1. 下载 Assets 中的 `Yimu-win64-v0.1.0.zip`
2. **解压整个文件夹**（不要只拷贝 exe）
3. 双击 `Yimu.exe` 运行（无需安装 Python）

## 主要功能

- 邮箱注册 / 登录，未登录不可用翻译
- 「应用 / 用户」双分区界面
- 持续抓屏 + 变化检测 + RapidOCR（中英为主）
- 翻译：Google 免费，或自定义 OpenAI 兼容大模型 API
- 置顶悬浮译文窗 + 历史
- 头像、用户 ID、昵称、主题色等个性化
- 账号数据保存在本机 `%APPDATA%\Yimu`，密码哈希存储

## 系统要求

- Windows 10 / 11（64 位）
- 使用大模型翻译或 Google 时需要联网

## 源码

从本仓库 `main` 分支获取：

```powershell
python -m venv .venv
.venv\Scripts\python.exe -m pip install -r requirements.txt
.venv\Scripts\python.exe -m yimu
```
