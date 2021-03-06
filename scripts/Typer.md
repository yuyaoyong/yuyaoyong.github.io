## **Typer** 是一个可以给Photoshop提供文字类扩展功能的插件，包括 *文字识别*、*翻译* 和 *文字消除*等。
**Typer** is a plug-in that provides Photoshop with text-related extensions, including text recognition 、elimination and translation.  

```**注：原 PS-OCR 已合并到此插件中```

---

## 支持的Photoshop版本：
Photoshop CC 2015.5及以上；

## 一、安装：
1. **下载**：下载最新版本 `Typer`: [https://yuyaoyong.com/Typer.zip](https://yuyaoyong.com/Typer.zip), 解压此文件；

2. **安装**：右键单击`install.jsx`，选择打开方式为Photoshop，按提示将 `Typer-package` 文件夹放入插件文件夹中：
>- WINDOWS : `\Program Files\Adobe\Adobe Photoshop 版本号\Plug-ins\Generator`
>- MAC : `/Applications/Adobe\ Photoshop\ CC\ 版本号/Plug-ins/Generator/`

![安装演示](imgs/Typer-安装演示.gif)

3. **配置**：在Photoshop中，依次打开菜单: `编辑 > 首选项 > 增效工具`，或者使用快捷键 `CTRL+K` 打开受选项对话框，选择 `增效工具` 项。勾选 `启动生成器` ,确定后重新启动Photoshop；
![配置演示](imgs/Typer-配置演示.gif)

## 二、使用：
### Typer_文字识别
> 1. **全图识别**：打开一个需要识别文字的文件，依次打开菜单：`文件 > 生成 > Typer_文字识别` ，插件会识别画面中的文字，并在对应的位置创建对应大小的文字对象。
> 2. **局部识别：** 如果你只想识别图像中部分文字，只需要用任意选区工具，选取目标区域，再使用`Typer_文字识别`；

![文字识别演示](imgs/Typer-文字识别演示.gif)
### Typer_翻译
> 1. 在 `Typer_首选项` 中选择翻译的目标语言；
> 2. 选中需要识别的文字图层，执行 `Typer_翻译`。

![文字翻译演示](imgs/Typer-文字翻译演示.gif)
### Typer_文字消除（BETA）
> 1. 打开一个需要识别文字的图片文件，依次打开菜单：`文件 > 生成 > Typer_文字消除（BETA）`。

![文字消除演示](imgs/Typer-文字消除演示.gif)

## 三、定义快捷键：
依次打开菜单: `编辑 > 键盘快捷键（Alt + Ctrl + Shift + K）` ，在对话框中依次找到 `文件 > 生成 > Typer_文字识别`，为其指定快捷键既可，比如 `Ctrl + Shift + O`；

---
Translated from Google

---
## 1、Install：
1. **Download:**  Download the lastest version `Typer`: [https://yuyaoyong.com/Typer.zip](https://yuyaoyong.com/Typer.zip), Unzip it；
2. **Install:** Right-click `install.jsx`, select open with Photoshop, and follow the prompts to put the `Typer-package` folder into the plugin folder:
> - WINDOWS : `\Program Files\Adobe\Adobe Photoshop {{version}} \Plug-ins\Generator`;
> - MAC : `/Applications/Adobe\ Photoshop\ CC\ {{version}} /Plug-ins/Generator/`
3. **Config:**  Click the menus in turn: `Edit > Preferences > Plug-ins`, or use the shortcut `CTRL+K` to open the Options dialog and select the 'Plug-ins' item. Check the 'Enable Generator' , restart Photoshop after confirming;
## 2、Use：
### Typer_OCR
> 1. **Whole picture OCR:**：Open a target file，click the menus in turn：`file > Generator > Typer` ，The plugin recognizes the text in the image and creates a text object of the corresponding size at the corresponding location.
> 2. **Partial OCR：** If you only want to identify some of the text in the image, just use any selection tool, select the target area, and use the `Typer_OCR` plugin.
### Typer_Translator
> 1. Select the target language for translation in `Typer_Preferences`；
> 2. Select the text layers you want to recognize and execute the `Typer_Translator`.
### Typer_RemoveText（BETA）
> 1. Open a target file，click the menus in turn：`file > Generator > Typer_RemoveText（BETA）`。

## 3、shortcuts:：
Click the menus in turn: `Edit > Keyboard Shortcuts（Alt + Ctrl + Shift + K）` ，In the dialog box, go to `File > Generator > Typer_OCR` and specify a shortcut key for it, such as `Ctrl + Shift + O`;
