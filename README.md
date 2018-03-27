# Material Design Toolkit

Sketch 版本：**Sketch 49.1**

我会在第一时间更新 Sketch 的版本，如果你在使用旧版，可能无法使用最新的版本，我会在每次升级前都打包一次。你可以在这里查看[历史版本](https://github.com/jay1803/Material-Design-Sketch-Library/tags)

Material Design Sketch Library（简称 MDSL）是一套基于 Material Design 规范来设计的 Sketch Library，其目的是为了做快速原型，之所以选择 Material Design 是因为其拥有完整的规范，不需要在规范的细节上在重新设计，可以让我更关注与整体的应用，另外也是因为 Material Design 是目前为止最适合跨多个平台的设计方案。

所有的组件根据 Google 的 Material Design 规范来制作，但并不是完全一样，我会加入一些官方没有组件，以应对更复杂的系统设计，例如列表构造器等。有时候一些组件也会跟官方的有所不同，考虑到纯 CSS 环境下的可用性。例如文本框组件，保留了 MD 旧版本中的一些组建和 MD 中没有的 label 组件。

MDSL 也可以用来做 MD 风格的 UI 设计，但如果你使用 Measure 来导出作为标记，那可能会出问题，一个解决方案是把 Symbol 解锁变成普通的图层，这是 Measure 自身的局限性。

## MDSL 结构说明

Assets.sketch 作为全局变量而存在，其中的组件会用在其他每个组件当中。例如颜色、文本、网格系统以及标注组件。Assets.sketch 通常不会单独使用，除非用于做一些特殊的组件。

其他的组件根据名称来单独设计特定的组件，一些基础的组件例如 Buttons.sketch 也会被用在其他的文件中。

一些数据类的组件，表格、日期，需要配合 generator 文件夹内的 Numbers 文件来生成，具体方法后续补充。

### 示例

![使用手册示例](https://raw.githubusercontent.com/jay1803/Material-Design-Toolkit/master/statics/manual.png?raw=true)

### 文件说明

* Assets.sketch：基本组件，包括一些基本的颜色和文字等，如果要使用其他组建，则该组建也必须一起开启；
* Buttons.sketch：按钮、标签组件，以及下拉菜单的按钮；
* Cards.sketch：卡片组件，以及 Grid List 组件；
* Dialogs.sketch：对话框组件，包括了 Picker 日期选择组件；
* Forms.sketch：表单组件，包括文本框、单项选择和多项选择；
* Lists.sketch：列表组件，包括了常用的列表和列表控制器，以及类似列表的菜单；
* Toolbars.sketch：工具栏组件，包括了应用栏、导航栏和其他导航以及指示性的组件；
* Toolkit.sketch：设计辅助工具，包括 Grid、Layout 以及标记的组件等；