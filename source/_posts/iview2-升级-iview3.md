---
title: iview2 升级 iview3
date: 2018-08-24 14:54:29
categories: VUE
tags: [vue,iview]
---
<link rel="stylesheet" href="https://at.alicdn.com/t/font_798158_wn4udd6bx9.css">

# 版本升级背景
## <icon class='iconfont gy-sound'></icon> iview 版本迭代 （截至 `2018-08-24`）
>* V 3.0.1 `2018-08-22`
>* V 3.0.0 `2018-07-28`  
> V 3.0.1 主要修复了 V 3.0.0 的一些 bug，不影响版本正常升级。

# 版本升级要素
## [Button](https://www.iviewui.com/components/button)

>* 废弃 type ghost，原先的 default 样式有改变。 `不兼容`
>* 新增属性 custom-icon，支持自定义图标。
>* 新增属性 to、replace、target，支持点击直接跳转。
>* 新增幽灵属性 ghost，可以使按钮背景透明，常用于有色背景上。

## [Icon](https://www.iviewui.com/components/icon)
>* Icon 的图标升级至 ionicons 3.0 图标，图标名称有改变。`不兼容`
>* 新增属性 custom，支持自定义图标。

## [Breadcrumb](https://www.iviewui.com/components/breadcrumb )
>* 新增属性 target。
>* Breadcrumb 废弃 href 属性。`不兼容`
>* 在链接上会显示 a 标签的 href 值。

## [Badge](https://www.iviewui.com/components/badge )
>* Badge 的 count 属性只支持 Number 类型。`不兼容`
>* 新增属性 show-zero。
>* 新增属性 text，可以自定义内容。
>* 新增属性 status，可以设置徽标为状态点。
>* 新增属性 offset，可以设置偏移量。
>* 新增属性 type，可以设置预设的颜色

## [Tag](https://www.iviewui.com/components/tag )
>* Tag 的 color 属性将原先的 blur、green、yellow、red 更名为了 primary、success、warning、error。`不兼容`
>* color 属性新增了 13 种预设。

## [Input](https://www.iviewui.com/components/input )
>* 新增属性 prefix 和 suffix 以及同名 slot，支持设置前缀和后缀图标。
>* 新增属性 search 和 enterButton，支持搜索类型的输入框。
>* 新增事件 @on-search，使用搜索类型输入框时，点击搜索或按下回车键时触发。

## [Modal 对话框](https://www.iviewui.com/components/modal  )
>* 新增全屏属性 fullscreen。
>* 新增隐藏遮罩层属性 mask。
>* 新增拖拽属性 draggable。

## [Table ](https://www.iviewui.com/components/table  )
>* Column 新增属性 indexMethod， 可以自定义 type="index" 时的序号。
>* Column 新增属性 tooltip，开启后，当单元格文本超过一行，会以…显示，并在 Tooltip 中显示完整内容。
>* 优化 type="selection" 时，Checkbox 为居中。

## [Menu ](https://www.iviewui.com/components/menu   )
>* 新增属性 to、replace、target，支持点击直接跳转。

## [Badge 徽章](https://www.iviewui.com/components/badge   )
>* 新增属性 show-zero。
>* 新增属性 text，可以自定义内容。
>* 新增属性 status，可以设置徽标为状态点。
>* 新增属性 offset，可以设置偏移量。
>* 新增属性 type，可以设置预设的颜色。

## [Page 分页](https://www.iviewui.com/components/page   )
>* 新增属性 prev-text 和 next-text，可以自定义上下页的文案。
>* 优化快进和快退的逻辑

## [Upload 上传](https://www.iviewui.com/components/upload   )
>* 新增属性 paste，开启后可以上传复制在剪贴板的文件。


## [Tooltip 文字提示](https://www.iviewui.com/components/tooltip   )
>* 新增属性 theme，可以设置 dark（默认）或 light 两种主题。
>* 新增属性 max-width，超出最大值后，文本将自动换行，并两端对齐。


## [Poptip 气泡提示](https://www.iviewui.com/components/poptip   )
>* 新增属性 word-wrap，开启后，超出指定宽度文本将自动换行，并两端对齐。
>* 新增属性 padding，可以自定义间距值。


## [Rate 评分](https://www.iviewui.com/components/rate   )
>* 新增属性 character、icon 和 custom-icon，支持自定义字符或图标。

## [Collapse 折叠面板](https://www.iviewui.com/components/collapse   )
>* 新增属性 hide-arrow，可以隐藏箭头。
>* 新增属性 simple，可以显示为无边框的简洁模式。


## [Switch 开关](https://www.iviewui.com/components/switch   )
>* 新增属性 loading，可表示开关仍在执行中


## [Dropdown ](https://www.iviewui.com/components/dropdown   )
>* 触发方式 trigger 新增 contextMenu，可以通过点击右键触发。

## [Circle 进度环](https://www.iviewui.com/components/circle  )
>* 新增仪表盘属性 dashboard。

## [Progress 进度条 ](https://www.iviewui.com/components/progress   )
>* 新增分段进度属性 success-percent。

## [Avatar 头像 ](https://www.iviewui.com/components/avatar   )
>* 新增自定义图标属性 custom-icon。

## [Progress 进度条 ](https://www.iviewui.com/components/progress   )
>* 新增分段进度属性 success-percent。

## [Progress 进度条 ](https://www.iviewui.com/components/progress   )
>* 新增分段进度属性 success-percent。