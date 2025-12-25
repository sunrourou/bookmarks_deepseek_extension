# Bookmarks Smart Organizer - User Guide

<div align="right">
  <a href="#english-version" style="background: #667eea; color: white; border: none; padding: 5px 15px; border-radius: 4px; cursor: pointer; margin-left: 5px; text-decoration: none; display: inline-block;">English</a>
  <a href="#中文版本" style="background: #e0e0e0; color: #333; border: none; padding: 5px 15px; border-radius: 4px; cursor: pointer; text-decoration: none; display: inline-block;">中文</a>
</div>

---

<div id="english-version">

# Bookmarks Smart Organizer - User Guide

Welcome to **Bookmarks Smart Organizer**, a powerful Chrome extension that helps you keep your bookmarks clean, organized, and accessible. This guide will walk you through all the features and how to use them effectively.

## 📋 Table of Contents

- [Overview](#overview)
- [Installation](#installation)
- [Getting Started](#getting-started)
- [Features](#features)
- [Detailed Usage](#detailed-usage)
- [Privacy & Security](#privacy--security)
- [Troubleshooting](#troubleshooting)
- [FAQ](#faq)

## 🎯 Overview

Bookmarks Smart Organizer is designed to solve two common problems:
1. **Invalid Bookmarks**: Over time, many bookmarks become inaccessible due to broken links, moved pages, or deleted websites.
2. **Disorganized Bookmarks**: Without proper organization, finding the right bookmark can be time-consuming.

Our extension provides intelligent solutions for both issues:
- **Smart Detection**: Automatically identifies inaccessible bookmarks
- **AI-Powered Organization**: Uses DeepSeek AI to intelligently categorize your bookmarks
- **One-Click Cleanup**: Easily remove invalid bookmarks or organize them into folders

## 📥 Installation

### Method 1: Chrome Web Store (Recommended)

1. Visit the [Chrome Web Store](https://chrome.google.com/webstore)
2. Search for "Bookmarks Smart Organizer"
3. Click "Add to Chrome"
4. Confirm the installation

### Method 2: Manual Installation

1. Download or clone this repository
2. Open Chrome and navigate to `chrome://extensions/`
3. Enable "Developer mode" (toggle in the top right)
4. Click "Load unpacked"
5. Select the extension folder

## 🚀 Getting Started

### First Launch

1. **Click the extension icon** in your Chrome toolbar
2. You'll see the main interface with two tabs:
   - 🔍 **Detect Invalid Bookmarks** (default)
   - 🤖 **AI Classification**

### Basic Workflow

1. Click **"📖 Load Bookmarks"** to load all your bookmarks
2. Choose your action:
   - **Detect invalid bookmarks** (no setup required)
   - **AI classification** (requires API key setup)

## ✨ Features

### 🔍 Invalid Bookmark Detection

**What it does:**
- Tests each bookmark's accessibility
- Identifies broken links, moved pages, and deleted websites
- Provides a clean list of invalid bookmarks

**Why it's useful:**
- Keeps your bookmark bar clean
- Saves time by removing dead links
- Improves browsing efficiency

### 🤖 AI-Powered Classification

**What it does:**
- Analyzes bookmark titles and URLs
- Groups related bookmarks together
- Creates organized folder structures

**Why it's useful:**
- Saves hours of manual organization
- Creates logical groupings automatically
- Makes finding bookmarks easier

### 📁 Apply Classification

**What it does:**
- Creates bookmark folders based on AI classification
- Moves bookmarks into appropriate folders
- Maintains a record for easy restoration

**Why it's useful:**
- Transforms your bookmark structure instantly
- Keeps everything organized
- Can be undone if needed

### ↩️ Restore Function

**What it does:**
- Restores bookmarks to their original positions
- Removes created folders
- Returns everything to the previous state

**Why it's useful:**
- Safety net for experimentation
- Easy to undo changes
- Peace of mind

## 📖 Detailed Usage

### Detecting Invalid Bookmarks

#### Step-by-Step Guide

1. **Open the Extension**
   - Click the extension icon in your Chrome toolbar
   - The "Detect Invalid Bookmarks" tab is selected by default

2. **Load Your Bookmarks**
   - Click the **"📖 Load Bookmarks"** button
   - Wait for all bookmarks to load
   - You'll see the total count displayed

3. **Start Detection**
   - Click the **"🔍 Check Bookmark Accessibility"** button
   - A progress bar will show the detection progress
   - The status will update as bookmarks are checked

4. **Review Results**
   - Invalid bookmarks are displayed in a list
   - Each bookmark shows:
     - Title
     - URL
     - Delete button (❌)

5. **Take Action**
   - **Delete Individual**: Click the ❌ button next to any bookmark
   - **Delete All**: Click the **"🗑️ Delete All Invalid Bookmarks"** button
   - Confirm the deletion when prompted

#### Tips

- Detection may take time for large bookmark collections
- The extension checks 3 bookmarks simultaneously for efficiency
- You can stop and resume detection if needed

### AI Classification

#### Prerequisites

Before using AI classification, you need to:

1. **Get a DeepSeek API Key**
   - Visit [DeepSeek Platform](https://platform.deepseek.com)
   - Sign up or log in
   - Generate an API key

2. **Configure the Extension**
   - Click the ⚙️ settings button in the extension popup
   - Or right-click the extension icon → Options
   - Enter your API key
   - Click "💾 Save Settings"

#### Step-by-Step Guide

1. **Switch to AI Classification Tab**
   - Click the **"🤖 AI Classification"** tab

2. **Load Your Bookmarks**
   - Click **"📖 Load Bookmarks"**
   - Wait for loading to complete

3. **Start Classification**
   - Click **"🤖 AI Classification"** button
   - The extension will:
     - Process bookmarks in batches (20 per batch)
     - Send data to DeepSeek API
     - Receive classification results
   - Progress is shown in real-time

4. **Review Classification Results**
   - Results are grouped by category
   - Each category shows:
     - Category name
     - Number of bookmarks
     - List of bookmarks in that category

5. **Apply Classification** (Optional)
   - Click **"📁 Apply Classification to Bookmarks"**
   - The extension will:
     - Create folders in your bookmark bar
     - Move bookmarks into appropriate folders
     - Save operation records for restoration
   - Wait for the process to complete

6. **Restore if Needed** (Optional)
   - Click **"↩️ Restore"** to undo changes
   - All bookmarks return to original positions
   - Created folders are removed

#### Tips

- Enable Debug Logs to see detailed classification process
- Classification works best with descriptive bookmark titles
- Large bookmark collections are processed in batches automatically

### Debug Mode

#### Enabling Debug Mode

1. Check the **"Debug Logs"** checkbox
2. A debug log panel will appear
3. All operations will be logged with timestamps

#### What You'll See

- API requests and responses
- Classification progress
- Error messages
- Operation details

#### Using Debug Logs

- Scroll through logs to see the process
- Click **"Clear"** to reset the log
- Useful for troubleshooting

## 🔒 Privacy & Security

### Data Handling

**Local Processing:**
- All bookmark data is processed locally
- No data is uploaded to our servers
- Your bookmarks stay on your device

**API Communication:**
- Only AI classification sends data to DeepSeek API
- Only bookmark titles and URLs are sent
- Data is used solely for classification
- No data is stored by DeepSeek for other purposes

**Storage:**
- API keys stored in Chrome's secure sync storage
- Operation records stored locally
- No personal information collected

### Permissions Explained

- **bookmarks**: Read, create, move, and delete bookmarks
- **storage**: Store API keys and operation records
- **tabs**: Create temporary tabs to test bookmark accessibility

### Privacy Policy

For detailed information, see our [Privacy Policy](privacy.html)

## 🛠️ Troubleshooting

### Common Issues

#### Issue: "Please configure DeepSeek API key"

**Solution:**
- Go to Settings (⚙️ button)
- Enter your DeepSeek API key
- Click Save

#### Issue: Detection is slow

**Solution:**
- This is normal for large bookmark collections
- The extension checks 3 bookmarks at a time
- Be patient, it will complete

#### Issue: Some bookmarks not detected as invalid

**Solution:**
- Some sites may block automated access
- Timeout is set to 3 seconds per bookmark
- Manually verify if needed

#### Issue: Classification results not accurate

**Solution:**
- Ensure bookmark titles are descriptive
- Try re-classifying with different bookmarks
- Check Debug Logs for details

#### Issue: Can't restore bookmarks

**Solution:**
- Ensure you haven't cleared browser data
- Operation records are stored locally
- If cleared, restoration won't be possible

### Getting Help

If you encounter issues:
1. Check Debug Logs for error messages
2. Review this guide
3. Check GitHub Issues
4. Contact support

## ❓ FAQ

### General Questions

**Q: Is this extension free?**
A: Yes, the extension is completely free to use.

**Q: Do I need an API key?**
A: Only for AI classification. Invalid bookmark detection works without any setup.

**Q: Will this slow down my browser?**
A: No, the extension only runs when you actively use it. It doesn't run in the background.

**Q: Can I use this offline?**
A: Invalid bookmark detection works offline. AI classification requires internet connection.

### Technical Questions

**Q: How does bookmark detection work?**
A: The extension creates temporary tabs to test if bookmarks are accessible. It checks for error pages and timeouts.

**Q: How accurate is AI classification?**
A: Classification accuracy depends on bookmark titles and URLs. Descriptive titles yield better results.

**Q: What happens if I delete a bookmark by mistake?**
A: Chrome's bookmark system doesn't have an undo feature. Be careful when deleting. You can restore from Chrome's bookmark backup if available.

**Q: Can I customize classification categories?**
A: Currently, categories are determined by AI. Future versions may include customization options.

### Privacy Questions

**Q: Are my bookmarks sent to any server?**
A: Only for AI classification, and only titles and URLs are sent to DeepSeek API. Detection works entirely locally.

**Q: Is my API key secure?**
A: Yes, API keys are stored in Chrome's encrypted sync storage and never shared.

**Q: Can I use the extension without internet?**
A: Yes, for bookmark detection. AI classification requires internet for API calls.

## 📞 Support

- **GitHub Issues**: [Report Issues](https://github.com/yourusername/bookmarks_deepseek_extension/issues)
- **Email**: your-email@example.com
- **Documentation**: See README.md for technical details

## 📝 Version History

See [CHANGELOG.md](CHANGELOG.md) for version history and updates.

---

**Thank you for using Bookmarks Smart Organizer!** 🎉

We hope this extension helps you maintain a clean and organized bookmark collection. If you have suggestions or feedback, please don't hesitate to reach out.

</div>

---

<div id="中文版本">

# 书签智能整理助手 - 使用手册

欢迎使用**书签智能整理助手**，这是一款强大的Chrome扩展，帮助您保持书签整洁、有序且可访问。本手册将详细介绍所有功能和使用方法。

## 📋 目录

- [概述](#概述)
- [安装](#安装)
- [快速开始](#快速开始)
- [功能特性](#功能特性)
- [详细使用](#详细使用)
- [隐私与安全](#隐私与安全)
- [故障排除](#故障排除)
- [常见问题](#常见问题)

## 🎯 概述

书签智能整理助手旨在解决两个常见问题：
1. **无效书签**：随着时间的推移，许多书签因链接失效、页面移动或网站删除而变得不可访问。
2. **书签混乱**：没有适当的组织，找到正确的书签可能很耗时。

我们的扩展为这两个问题提供了智能解决方案：
- **智能检测**：自动识别不可访问的书签
- **AI驱动整理**：使用DeepSeek AI智能分类您的书签
- **一键清理**：轻松删除无效书签或将其整理到文件夹中

## 📥 安装

### 方法一：Chrome Web Store（推荐）

1. 访问 [Chrome Web Store](https://chrome.google.com/webstore)
2. 搜索"书签智能整理助手"
3. 点击"添加至 Chrome"
4. 确认安装

### 方法二：手动安装

1. 下载或克隆此仓库
2. 打开Chrome并访问 `chrome://extensions/`
3. 启用"开发者模式"（右上角开关）
4. 点击"加载已解压的扩展程序"
5. 选择扩展文件夹

## 🚀 快速开始

### 首次使用

1. **点击扩展图标**（Chrome工具栏中）
2. 您将看到主界面，包含两个标签页：
   - 🔍 **检测无效书签**（默认）
   - 🤖 **AI分类整理**

### 基本流程

1. 点击 **"📖 加载书签"** 加载所有书签
2. 选择您的操作：
   - **检测无效书签**（无需设置）
   - **AI分类整理**（需要API密钥设置）

## ✨ 功能特性

### 🔍 无效书签检测

**功能说明：**
- 测试每个书签的可访问性
- 识别失效链接、移动页面和已删除的网站
- 提供清晰的无效书签列表

**为什么有用：**
- 保持书签栏整洁
- 通过删除死链接节省时间
- 提高浏览效率

### 🤖 AI智能分类

**功能说明：**
- 分析书签标题和URL
- 将相关书签分组
- 创建有序的文件夹结构

**为什么有用：**
- 节省数小时的手动整理时间
- 自动创建逻辑分组
- 使查找书签更容易

### 📁 应用分类

**功能说明：**
- 根据AI分类结果创建书签文件夹
- 将书签移动到相应的文件夹
- 保存操作记录以便轻松恢复

**为什么有用：**
- 即时转换您的书签结构
- 保持一切有序
- 需要时可以撤销

### ↩️ 恢复功能

**功能说明：**
- 将书签恢复到原始位置
- 删除创建的文件夹
- 将所有内容返回到之前的状态

**为什么有用：**
- 实验的安全网
- 轻松撤销更改
- 安心使用

## 📖 详细使用

### 检测无效书签

#### 分步指南

1. **打开扩展**
   - 点击Chrome工具栏中的扩展图标
   - "检测无效书签"标签页默认已选中

2. **加载书签**
   - 点击 **"📖 加载书签"** 按钮
   - 等待所有书签加载完成
   - 您将看到总数显示

3. **开始检测**
   - 点击 **"🔍 检测书签可访问性"** 按钮
   - 进度条将显示检测进度
   - 状态会随着书签检查而更新

4. **查看结果**
   - 无效书签显示在列表中
   - 每个书签显示：
     - 标题
     - URL
     - 删除按钮（❌）

5. **执行操作**
   - **单独删除**：点击任何书签旁边的❌按钮
   - **全部删除**：点击 **"🗑️ 删除所有无效书签"** 按钮
   - 出现提示时确认删除

#### 提示

- 对于大型书签集合，检测可能需要时间
- 扩展同时检查3个书签以提高效率
- 如果需要，可以停止并恢复检测

### AI分类整理

#### 前提条件

在使用AI分类之前，您需要：

1. **获取DeepSeek API密钥**
   - 访问 [DeepSeek平台](https://platform.deepseek.com)
   - 注册或登录
   - 生成API密钥

2. **配置扩展**
   - 点击扩展弹窗中的⚙️设置按钮
   - 或右键扩展图标 → 选项
   - 输入您的API密钥
   - 点击"💾 保存设置"

#### 分步指南

1. **切换到AI分类标签页**
   - 点击 **"🤖 AI分类整理"** 标签页

2. **加载书签**
   - 点击 **"📖 加载书签"**
   - 等待加载完成

3. **开始分类**
   - 点击 **"🤖 AI分类整理"** 按钮
   - 扩展将：
     - 分批处理书签（每批20个）
     - 将数据发送到DeepSeek API
     - 接收分类结果
   - 实时显示进度

4. **查看分类结果**
   - 结果按类别分组
   - 每个类别显示：
     - 类别名称
     - 书签数量
     - 该类别中的书签列表

5. **应用分类**（可选）
   - 点击 **"📁 应用分类到书签"**
   - 扩展将：
     - 在书签栏中创建文件夹
     - 将书签移动到相应的文件夹
     - 保存操作记录以便恢复
   - 等待过程完成

6. **恢复**（如需要）
   - 点击 **"↩️ 恢复原状"** 撤销更改
   - 所有书签返回到原始位置
   - 删除创建的文件夹

#### 提示

- 启用调试日志以查看详细的分类过程
- 分类在书签标题描述性强时效果最佳
- 大型书签集合会自动分批处理

### 调试模式

#### 启用调试模式

1. 勾选 **"Debug日志"** 复选框
2. 将出现调试日志面板
3. 所有操作都会记录时间戳

#### 您将看到的内容

- API请求和响应
- 分类进度
- 错误消息
- 操作详情

#### 使用调试日志

- 滚动查看日志以了解过程
- 点击 **"清除"** 重置日志
- 对故障排除很有用

## 🔒 隐私与安全

### 数据处理

**本地处理：**
- 所有书签数据在本地处理
- 不上传到我们的服务器
- 您的书签保留在您的设备上

**API通信：**
- 只有AI分类会向DeepSeek API发送数据
- 只发送书签标题和URL
- 数据仅用于分类
- DeepSeek不会将数据用于其他目的

**存储：**
- API密钥存储在Chrome的安全同步存储中
- 操作记录本地存储
- 不收集个人信息

### 权限说明

- **bookmarks**：读取、创建、移动和删除书签
- **storage**：存储API密钥和操作记录
- **tabs**：创建临时标签页以测试书签可访问性

### 隐私政策

详细信息请参阅我们的[隐私政策](privacy.html)

## 🛠️ 故障排除

### 常见问题

#### 问题："请配置DeepSeek API密钥"

**解决方案：**
- 转到设置（⚙️按钮）
- 输入您的DeepSeek API密钥
- 点击保存

#### 问题：检测速度慢

**解决方案：**
- 对于大型书签集合这是正常的
- 扩展同时检查3个书签
- 请耐心等待，它会完成

#### 问题：某些书签未检测为无效

**解决方案：**
- 某些网站可能阻止自动访问
- 每个书签的超时设置为3秒
- 如需要，请手动验证

#### 问题：分类结果不准确

**解决方案：**
- 确保书签标题具有描述性
- 尝试使用不同的书签重新分类
- 查看调试日志了解详情

#### 问题：无法恢复书签

**解决方案：**
- 确保您没有清除浏览器数据
- 操作记录存储在本地
- 如果已清除，将无法恢复

### 获取帮助

如果遇到问题：
1. 检查调试日志中的错误消息
2. 查看本手册
3. 查看GitHub Issues
4. 联系支持

## ❓ 常见问题

### 一般问题

**问：这个扩展是免费的吗？**
答：是的，扩展完全免费使用。

**问：我需要API密钥吗？**
答：仅AI分类需要。无效书签检测无需任何设置即可工作。

**问：这会减慢我的浏览器速度吗？**
答：不会，扩展只在您主动使用时运行。它不会在后台运行。

**问：我可以离线使用吗？**
答：无效书签检测可以离线工作。AI分类需要互联网连接。

### 技术问题

**问：书签检测是如何工作的？**
答：扩展创建临时标签页来测试书签是否可访问。它检查错误页面和超时。

**问：AI分类的准确性如何？**
答：分类准确性取决于书签标题和URL。描述性标题会产生更好的结果。

**问：如果我误删了书签怎么办？**
答：Chrome的书签系统没有撤销功能。删除时请小心。如果可用，您可以从Chrome的书签备份中恢复。

**问：我可以自定义分类类别吗？**
答：目前，类别由AI确定。未来版本可能包括自定义选项。

### 隐私问题

**问：我的书签会发送到任何服务器吗？**
答：仅用于AI分类，并且只向DeepSeek API发送标题和URL。检测完全在本地工作。

**问：我的API密钥安全吗？**
答：是的，API密钥存储在Chrome的加密同步存储中，永远不会共享。

**问：我可以在没有互联网的情况下使用扩展吗？**
答：可以，用于书签检测。AI分类需要互联网进行API调用。

## 📞 支持

- **GitHub Issues**：[报告问题](https://github.com/yourusername/bookmarks_deepseek_extension/issues)
- **邮箱**：your-email@example.com
- **文档**：查看README.md了解技术细节

## 📝 版本历史

查看 [CHANGELOG.md](CHANGELOG.md) 了解版本历史和更新。

---

**感谢使用书签智能整理助手！** 🎉

我们希望这个扩展能帮助您维护一个整洁有序的书签集合。如果您有建议或反馈，请随时联系我们。

</div>
