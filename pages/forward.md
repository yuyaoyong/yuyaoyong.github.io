## Photoshop的自动化
Photoshop为提高用户的工作效率，在软件中提供了多种自动化工具：[动作](httPhotoshop://helpx.adobe.com/cn/photoshop/using/creating-actions.html)、[数据驱动](httPhotoshop://helpx.adobe.com/cn/photoshop/using/creating-data-driven-graphics.html)、[脚本](httPhotoshop://helpx.adobe.com/cn/photoshop/using/scripting.html)；
- **动作** : 是指在单个文件或一批文件上执行的一系列任务，如菜单命令、面板选项、工具动作等；
- **数据驱动** : 利用数据驱动图形，可以以模板为基础快速准确地生成图像的多个版本；
- **脚本** : 通过脚本程序驱动Photoshop，弥补动作和数据驱动的局限，具有更自由和强大的功能；

## Photoshop的功能扩展
开放的Photoshop提供了多种扩展方式，让广大开发者可以尽情地挥洒创意：
- **脚本** : 通过脚本程序驱动Photoshop；
- **CEP** : Photoshop内部的基于H5和node的WEB应用；
- **plug-in** : 使用C系列语言编写的插件：滤镜、导入导出等；

## Photoshop脚本
> Photoshop 通过脚本支持外部自动化。在 Windows 中，可以使用支持 COM 自动化的脚本语言，例如 VB Script。在 Mac OS 中，可以使用允许发送 Apple 事件的语言，例如 AppleScript。这些语言不是跨平台的，但可以控制多个应用程序，例如 Adobe Photoshop、Adobe Illustrator 和 Microsoft Office。也可以在这两种平台上使用 Javascript。您可以利用 Javascript 支持编写可以在 Windows 或 Mac OS 上运行的 Photoshop 脚本。  
> 
> （说明 : 文中的Javascript具体来说其实是 [ExtendScript](pages/extendScript)，本站所有脚本均使用 ExtendScript 编写。）

打个比方，**Photoshop脚本就像给Photoshop用户配的一个机器人助理，它会帮助我们快速的完成那些不想做的琐碎的、机械性的工作，我们只需要完成那些艺术或技术性的工作部分。**当然，机器人助理之所以能为我们工作，就需要我们告诉它怎么去工作，这就是大家在这个教程中需要学习的知识，编写Photoshop脚本。

## 文件格式和使用方法
通常，Photoshop脚本是文件名以.jsx结尾的纯文本文件。更多内容，参考下表。

|文件后缀|文件类型|
|:---:|:---:|
|.jsx|脚本执行文件|
|.jsxinc|脚本引用文件|
|.jsxbin|二进制脚本文件|

### 编写第一个Photoshop脚本
```javascript
app.documents.add(500,500);
```
1. 新建一个空白文档，将上面的代码复制进去，然后将文件存储为`newDocument.jsx`；
2. 将脚本文件复制到Photoshop的脚本文件夹下`"……\Adobe Photoshop CC 2018\Presets\Scripts\"`（文件夹位置可能会有差别）；
3. 重新打开Photoshop，**从菜单打开**: 文件 > 脚本 > newDocument,  
   或者: 文件 > 脚本 > 浏览 > 找到newDocument.jsx;
4. GOOD! 你已经成功的编写了一个Photoshop脚本，并且成功的用脚本新建了一个尺寸为500-500的文档；

脚本文件还支持**在任何位置双击执行**，你只需要在代码开头加上一个预处理指令：
```javascript
#target photoshop
//注释：这个预处理指令告诉系统,这个文件用photoshop打开
app.documents.add(500,500);
```

## 准备工作
### 编程工具
上文提到脚本是纯文本文件，理所当然，您可以用任何文本编辑工具来编写。但是我还是推荐使用Adobe为我们提供的脚本开发工具 ExtendScript Toolkit。

#### ExtendScript Toolkit (ESTK)
> ESTK为所有支持ExtendScript的Adobe应用程序中的ExtendScript提供了交互式开发和测试环境。它包括一个功能齐全，语法高亮的文本编辑器，具有Unicode功能和多个撤消/重做支持。ESTK是ExtendScript文件的默认编辑器，它使用扩展名.jsx。

### 语言基础
标题中的语言指的是编程语言。本站中的所有脚本均是用JavaScript编写。它是一种比较容易上手的语言。教程中有单独的一章来快速的学习ExtendScript。另外，凡是涉及到ExtendScript语法的地方，都会有注释讲解。所以，尽管放心，即使你一点基础也没有。

### 参考文档
下面这些文档，大家需要保存在电脑里，因为在编写脚本的时候，你会经常用到他们。