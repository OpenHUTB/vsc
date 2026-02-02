# 打包

将 vscode 和相关包打包为一个 hutb.zip 。


## 自定义快捷键

先后按`Ctrl+K` 和 `Ctrl+S`。然后搜索，比如搜索：`Python: Run Python File in Terminal`，双击并输入`Ctrl+F10`，回车保存。


## 问题

* vscode 运行Python脚本(激活conda环境)报错：不应有&
    > 按 `Ctrl+Shift+P`，选择`Terminal: Configure Terminal Settings`
    > 
    > 在弹出的配置页面选择`Terminal > Integrated > Env: Windows` 下的 `Edit in settings.json`
    > 
    > 在`"Command Prompt"`下配置 3 个参数：
    > ```
    >    "Command Prompt": {
    >        "path": "C:\\Windows\\System32\\cmd.exe",
    >        "args": [
    >            "/K",
    >            "D:\\hutb\\Build\\dependencies\\prerequisites\\miniconda3\\Scripts\\activate.bat",
    >            "D:\\hutb\\Build\\dependencies\\prerequisites\\miniconda3"
    >        ]
    > ```