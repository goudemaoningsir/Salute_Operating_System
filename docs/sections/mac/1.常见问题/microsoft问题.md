## 关闭Microsoft AutoUpdate弹窗

Microsoft AutoUpdate 用于自动更新 Microsoft 产品，比如 Office。然而，有些用户可能希望停用或关闭这个功能，以免弹窗干扰。下面的步骤说明了如何关闭 Microsoft AutoUpdate 的弹窗：

**步骤1： 软件内关闭**

1. 打开任一 Office 应用，例如 Word、Excel 或 PowerPoint。
2. 点击菜单栏上的 "帮助" 选项，然后选择 "检查更新"。这会打开 Microsoft AutoUpdate 窗口。
3. 在 Microsoft AutoUpdate 窗口中，你会看到 "如何检查更新" 部分。选择 "手动" 或 "关闭"。

注意，关闭自动更新后，你需要手动检查和安装更新。这是因为更新通常包括新功能和重要的安全修复，所以定期检查更新仍然很重要。

**步骤2： 设置权限不可访问**

如果步骤1不能解决，请执行以下操作

打开终端，输入以下代码

```bash
cd /Library/Application Support/Microsoft/MAU2.0
sudo chmod 000 Microsoft\ AutoUpdate.app
```

然后输入密码，这样Microsoft AutoUpdate.app就没有执行权限了。

**步骤3： 删除**

如果步骤2不能解决，请执行以下操作

使用快捷键：`command（⌘）+⇧+G`，或者顶部菜单，选择`前往`——`前往文件夹`

在弹出的对话框中输入以下路径，点击`前往`

```cobol
/Library/Application Support/Microsoft/ 
```

删除文件夹`MAU2.0`，大功告成

也可以进入此文件夹删除`Microsoft AutoUpdate.app`就可以了。
