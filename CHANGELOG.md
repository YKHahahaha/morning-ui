# CHANGELOG

## 0.12.67

#### 新特性

- `ui-carousel`的`emit`事件新增`index`参数
- `ui-counter`新增`controls`配置
- `ui-steps`的`current-type`配置新增`hollow`选项
- `ui-steps`新增`done-type`配置
- `ui-progress`新增`note-position`配置

#### 改进

- 优化`ui-steps`的样式，使其符合设计规范

#### 修复

- 修复`ui-slider`组件的`max`或`min`配置动态变化时可能导致显示不正确的问题
- 修复`ui-select`选中后文本和图标重叠的样式问题

## 0.12.66

#### 新特性

- `ui-upload`组件新增`only-read-file`配置，允许上传组件仅仅读取文件不处理上传
- `ui-video`组件新增`fullscreen`方法

#### 改进

- 完善`ui-mindmap`组件

#### 修复

- 修复`ui-radio`和`ui-checkbox`的选项内容中包含图标时无法展示的问题
- 修复`ui-checkbox`和`ui-radio`在某些特殊的情况下`outline`显示不正确的问题
- 修复`ui-slider`的`mark-range`配置可能导致溢出的问题

#### 更多

- 新增若干图标

## 0.12.65

#### 新特性

- 新增`ui-mindmap`思维导图组件，支持思维导图编辑及导出`xmind`、`json`等格式文件

#### 改进

- 优化`ui-btn`的朴素和幽灵按钮样式，使其符合设计规范
- 现在`ui-multiinput`组件中通过点击删除项目时，不会触发`input-focus`事件
- 优化表单组件的背景色及表单项的背景色，使其在偏暖色的显示器中有更好的呈现

#### 修复

- 修复`ui-progress`文档中的一处错误
- 修复`ui-select`组件中开启`multi-select`配置后，点击删除选项时会弹出下拉框的问题
- 修复`ui-avatar`使用图片作为头像时的一个错位问题
- 修复`ui-form`组件无法通过`set()`方法清空数值的问题
- 修复`ui-form`组件无法通过`set()`方法清空单个表单组件数值的问题

#### 更多

- `ui-select`文档新增`list`为数组的用法示例

## 0.12.64

#### 新特性

- `ui-slider`的`mark-range`配置，现在支持配置颜色
- `ui-form`组件的表单项名称支持`Vue Template`
- `ui-progress`支持`format`配置，可以用来格式化进度文案
- `ui-progress`支持`status`配置，可以用来设置进度条的状态
- `ui-progress`支持`mark-range`配置

#### 改进

- `ui-dialog`弹窗增加圆角，和设计规范保持一致
- 改进`ui-checkbox`和`ui-radio`组件的边距，是其可以更容易布局

#### 修复

- 修复`ui-table`的`vertical-border`配置失效的问题
- 修复`ui-img`预览大图时溢出窗口的问题

#### 更多

- 暂时下线文档搜索功能

__升级注意事项__

- `ui-progress`当进度100%时，不再会显示成功状态，可以通过`status=’success’`配置来替代

## 0.12.63

`2019年10月21日`

#### 修复

- 修复`ui-table`的`fixed-title-col`配置失效的问题

## 0.12.62

`2019年10月14日`

#### 修复

- 修复`ui-uploader`上传失败后，失败信息不显示的问题
- 修复`ui-texteditor`的`uploader`配置无效的问题
- 修复`ui-texteditor`组件插入图片后，图片溢出的问题

#### 更多

- 移除依赖`quill-delta`
- 修复`定制化`文档中错误的部分

## 0.12.61

`2019年10月10日`

#### 改进

- `ui-table`筛选点击确认按钮后，筛选菜单会收起
- 优化`ui-tab`未选中标签页的颜色，使其符合设计规范
- 优化`ui-table`表头和单元格文本颜色，使其符合设计规范

#### 修复

- 修复`ui-texteditor`插入链接时，输入框超出边界被遮挡问题
- 修复`ui-cascader`再未开启`multi-select`配置时，错误的实现了多选框的问题

## 0.12.60

`2019年10月8日`

#### 新特性

- `ui-pagination`的`type`新增`compact`和`block`选项
- `ui-table`的`col-set`配置支持`filters`可以为列设置筛选项
- `ui-btn`新增`min-width`配置

#### 改进

- 优化`ui-pagination`使其符合设计规范
- 优化`ui-btn`的字体大小使其符合设计规范

#### 修复

- 修复`ui-pagination`使用尺寸后页面跳转器高度问题
- 修复`ui-checkbox`和`ui-radio`的`list`配置的Key不能为特殊字符的问题

#### 更多

- 新增图标(`mo-icon-filter-f`)

## 0.12.59

`2019年9月29日`

#### 新特性

- `ui-table`新增`highlight-row-background`和`highlight-row-color`配置，可以用来自定义高亮行的样式
- `ui-table`新增`exportToCsv()`方法
- `ui-texteditor`支持表格
- `ui-texteditor`支持`blur`和`focus`事件

#### 修复

- 修复`ui-sticky`文档中的一处错误
- 修复`ui-select`组件在开启`can-search`后，未搜索到项目时提示没有显示的问题
- 修复`ui-tab`组件使用`position="bottom”`配置后，配合部分组件使用时显示异常的问题
- 修复文档无法打开`codepen`示例的问题(更新至`codepen`最新API)

#### 更多

- Morning UI Roadmap更新
- 依赖库`date-fns`从`2.0.0-alpha.27`升级至`2.2.1`

__升级注意事项__

- Morning UI依赖的`date-fns`从`2.0.0-alpha.27`升级至`2.2.1`，其中存在不兼容升级，Morning UI内已做兼容处理。若在组件库之外使用了`date-fns`请注意安装版本的变化，主要变化为`format`和`parse`方法。(see：`https://date-fns.org`)

## 0.12.58

`2019年9月12日`
    
#### 新特性

- `ui-texteditor`支持`emoji`表情
- `ui-datepicker`和`ui-datetimepicker`新增`hidden-icon`配置
- `ui-texteditor`新增`inline-style`配置
- `ui-texteditor`新增`getHtml()`和`getHtmlWithoutStyle()`方法
- `ui-select`支持`select-btn`配置

#### 改进

- 优化`ui-datepicker`、`ui-datetimepicker`、`ui-timepicker`样式，使其符合设计规范
- 优化`ui-popover`阴影样式

#### 修复

- 修复`ui-anchor`中的一处问题
- 修复`ui-calendar`月份和年份选择时样式问题

## 0.12.57

`2019年8月20日`

#### 新特性

- `ui-btn`新增`ghost`(幽灵按钮)和`fade`(褪色按钮)样式

#### 改进

- 优化`ui-btn`的样式使其符合设计规范
- 优化`ui-dialog`的样式使其符合设计规范
- 优化`info`和`minor`色彩使其符合设计规范
- 所有表单组件统一了默认提示文案

#### 修复

- 修复`ui-datetimepicker`在区间选择时的一个数值清空的问题

## 0.12.56

`2019年8月10日`

#### 新特性

- `ui-select`新增`blur`、`focus`事件
- `ui-timepicker`新增`blur`、`focus`事件

#### 改进

- `ui-table`的表格排序现在支持部分非数字内容的排序 

#### 修复

- 修复`ui-select`组件动态切换`multi-select`配置时的报错
- 修复`ui-form`在同步子表单数值上的一个问题

#### 更多

- `ui-timepicker`、`ui-datepicker`、`ui-datetimepicker`组件现在不会实时校验/修正输入内容，而是在表单失焦后校验/修正输入内容

__升级注意事项__

- 现在`ui-timepicker`、`ui-datepicker`、`ui-datetimepicker`组件不会实时校验/修正输入内容，这可能引起部分即时取值逻辑产生问题，若页面采用了即时性较强的取值逻辑请检查是否正常运行

## 0.12.55

`2019年7月18日`
   
#### 新特性

- `ui-drawer`新增`after-show`和`after-hide`两个事件

#### 改进

- 优化`ui-table`在未使用标题列时的性能

#### 修复

- 修复`ui-table`组件的`custom-sort`配置失效的问题
- 修复安全性漏洞(CVE-2019-10742) 
- 修复底层`TriggerManager`引起的一个报错

## 0.12.54

`2019年7月16日`

#### 修复

- 修复`ui-cascader`一个项目名称显示错误的问题

## 0.12.53

`2019年7月16日`

#### 修复

- 修复`ui-cascader`一个点击区域错误引起的赋值错误的问题
- 修复`ui-cascader`开启`select-leaf-node`配置后，项目名称未显示层级的问题

#### 更多

- 更新对比文档(`element@2.10.0`、`iview@3.4.2`、`antd@3.20.3`)

## 0.12.52

`2019年7月15日`

#### 新特性

- `ui-cascader`新增`multi-select`配置，支持多选的级联选择
- `ui-cascader`新增`select-leaf-node`配置，支持多选非叶子结点
- `ui-multiinput`组件新增`collapse-limit`配置，当项目数量超过此配置时进行折叠
- `ui-select`组件新增`collapse-limit`配置
- `ui-cascader`新增`collapse-limit`配置
- `ui-dialog`新增`white-footer`样式类，可以支持纯白的模拟盒
- `ui-checkbox`新增`checked-state-change`
- 所有表单组件新增`form-width`配置，可以设置五种固定的宽度

#### 改进

- 优化`ui-multiinput`通过按键删除项目的逻辑及交互效果
- 优化`success`、`warning`、`danger`、`primary`四种功能色，与最新的设计规范保持一致

#### 修复

- 修复`ui-table`文档中关于`multi-select`配置的一处描述错误
- 修复`ui-radio`文档中表单基础配置部分缺失的问题
- 修复`ui-checkbox`和`ui-radio`在用户操作时的动效和`color`配置颜色(仅主题色和功能色)不匹配的问题

#### 更多

- `ui-multiinput`文档新增可通过按键删除项目
- `ui-select`的文档新增当开启`multi-select`和`can-search`配置后可以通过按键删除项目

## 0.12.51

`2019年7月11日`

#### 新特性

- `ui-cascader`新增`list-width`配置

## 0.12.50

`2019年7月10日`

#### 改进

- 现在`ui-select`的`list-width`配置可以在未开启`separate-emit`时使用了

#### 修复

- 修复`ui-menu`的展示样式问题

## 0.12.49

`2019年7月9日`

#### 修复

- 修复`ui-menu`的一个样式问题

## 0.12.48

`2019年7月8日`

#### 新特性

- `ui-cascader`、`ui-multiinput`、`ui-multiform`、`ui-timepicker`、`ui-datepicker`、`ui-datetimepicker`支持数值清空按钮
- `ui-datepicker`和`ui-datetimepicker`支持底部插槽`footer`

#### 改进

- 优化组件中下拉箭头和清空按钮的图标展现位置

#### 修复

- 修复`ui-menu`在深色模式下开启`side-expand`配置后，当前所在菜单项的颜色不适配问题

## 0.12.47

`2019年7月6日`

#### 改进

- 优化`ui-calendar`的日期面板，现在更为紧凑
- 优化`ui-datepicker`和`ui-datetimepicker`的日期选择面板
- `ui-table`现在支持在表头中使用Vue组件，详见文档

#### 修复

- 修复`ui-audio`和`ui-video`组件无法通过拖拽调整音量的问题

## 0.12.46

`2019年7月4日`

#### 修复

- 修复`ui-tab`的`append`和`prepend`配置更新后组件未更新的问题
- 修复组件底层配置赋值问题引起的`ui-btn`和`ui-link`在`state`等配置变化时展现错误的问题
- 修复`ui-cascader`在特定的条件下会报错的问题
- 修复`ui-menu`当两个子菜单的`key`一样时，定位当前菜单不准确的问题
- 调整`ui-menu`菜单的`z-index`，解决部分场景下会被其他组件遮挡的问题
    
## 0.12.45

`2019年6月19日`

#### 修复

- 修复`ui-checkbox`的`parent`配置在子组件销毁时父组件的状态无法同步更新的问题

## 0.12.44

`2019年6月17日`

#### 改进

- 优化所有表单组件聚焦状态的视觉效果

#### 修复

- 修复`ui-cascader`组件开启`can-search`配置后的一个样式问题
- 修复`ui-checkbox`的`checked-state`配置的状态同步失效的问题

## 0.12.43

`2019年6月16日`

#### 新特性

- `ui-table`新增`checkedAllRows()`和`uncheckAllRows()`两个方法
- `ui-checkbox`新增`indeterminate`和`checked-state`配置
- `ui-checkbox`新增`getCheckedState()`方法

#### 修复

- 修复部分表单组件在`ui-form`中的宽度无法自适应的问题
- 修复部分具有`align`配置的组件再显示错误提示时文字对齐的问题
- 修复`ui-textarea`组件开启`maxlength`配置后错误提示文字错位的问题
- 修复`ui-pagination`的`total`配置小于`1`时显示异常

## 0.12.42

`2019年6月11日`

#### 修复

- 修复`ui-select`通过`set`方法设置值时的一个问题

## 0.12.41

`2019年6月5日`

#### 新特性

- `ui-multiinput`组件新增`focusInput`方法
- `ui-pagination`组件新增`always-show-nav-arrow`配置，可以设置翻页导航按钮显示逻辑

#### 改进

- `ui-textinput`、`ui-textarea`、`ui-multiinput`组件的`inside-name`配置默认值改为`请输入`
- `ui-select`、`ui-cascader`、`ui-timepicker`、`ui-datepicker`、`ui-datetimepicker`组件的`inside-name`配置默认值改为`请选择`
- 优化`ui-table`组件斑马纹样式
- 现在`ui-select`在多选搜索模式下，鼠标选中项目后搜索框仍然聚焦
- 优化`ui-breadcrumbs`的配色

#### 修复

- 修复`ui-textarea`可以通过`set()`方法设置超过长度字符串的问题

## 0.12.40

`2019年6月5日`
    
#### 改进

- 优化表单组件背景`hover`状态配色
- 优化所有表单组件处于`disabled`和`readonly`状态时的背景色和边框色
- 现在当`ui-select`处于`disabled`和`readonly`状态时，点击不会显示下拉列表
- 现在`ui-rate`处于禁用状态时会显示禁用鼠标样式
- 优化当`ui-checkbox`和`ui-radio`组件处于`disabled`和`readonly`状态时，鼠标`hover`时文本颜色不会改变
- `ui-textarea`组件的最大长度显示位置现在调整到了右下角

#### 修复

- 修复`ui-multiinput`的`backspace`快捷键删除逻辑
- 修复`ui-upload`组件当图片尾缀大写时无法识别的问题

## 0.12.39

`2019年5月30日`
    
#### 新特性

- `ui-table`支持嵌套子内容，详见文档

#### 改进

- 优化`ui-dialog`的标题字体颜色和边距
- 统一`ui-upload`中移除文件的图标
- 优化`ui-checkbox`和`ui-radio`的文案颜色

#### 更多

- 新增`设计/视觉/布局`文档

## 0.12.38

`2019年5月28日`

#### 新特性

-  `ui-table`的`col-set`配置新增`sortmode`可以设置多种排序类型

#### 改进

- 采用了新的字体标准，优先字体从`苹方`切换为`Helvetica`和`Microsoft YaHei`

#### 修复

- 修复`ui-textinput`在使用`append`和`prepend`配置时，清空按钮位置不正确的问题
- 修复`ui-table`排序失效的一个问题

__升级注意事项__

- 由于字体调整可能引起部分场景下文字的位置需要微调

## 0.12.37

`2019年5月24日`

#### 改进

- 优化`ui-table`的`col-set`、`row-set`、`cell-set`中的单元格背景色彩
- 现在当`ui-img`使用`preview`配置后，鼠标移入会显示提示浮层

#### 修复

- 修复`ui-upload`在开启`list-type=“thumbnail”`和`inside-name`配置后文字错位的问题
- 修复`ui-upload`组件`type=“button”`时，按钮色彩不正确的问题

#### 更多
                                                                                                        
- 新增`设计/原则/对比`、`设计/原则/操作定义`文档
- 更新`致谢`文档，新增贡献者
- 更新文档中关于Vue的版本限定

## 0.12.36

`2019年5月21日`

#### 新特性

- `ui-img`从样式组件变更为交互组件，支持`preview`配置预览图片
- `ui-img`新增`show-preview`和`hide-preview`事件
- `ui-img`新增`togglePreview`方法

#### 改进

- `ui-pagination`的`emit`事件新增当前页码参数
- `ui-upload`当上传的文件为图片时，现在可以通过弹窗进行预览

#### 更多

- 新增`设计/原则/间距`、`设计/原则/对齐`文档

## 0.12.35

`2019年5月20日`

#### 新特性

- `ui-calendar`新增`mode`配置，可以设置日历仅显示月份、年份
- `ui-datepicker`新增`month-pick`配置，可以设置月份选择器

#### 修复

- 修复`ui-pagination`分页显示不正确的问题

---

## 0.12.34

`2019年5月20日`

#### 改进

- `辅助色`现在被改进为`中性色`，原有的12种辅助色现在调整为14种中性色，详见文档的`设计/色彩`章节
- 所有组件中使用和支持的`辅助色`现在被调整为`中性色`
- 优化`ui-select`、`ui-multiinput`、`ui-multiform`中的多选项目样式 

#### 修复

- 修复`ui-multiinput`可以输入空数值的问题
- 修复`ui-steps`加载中状态未显示的问题

#### 更多

- 新增`设计/色彩`文档，原有的`形态/色彩`部分内容被调整至此文档
- `ui-menu`移除4种色彩支持：`gray`、`light-gray`、`light-black`、`extra-light-black`

__升级注意事项__

- `ui-menu`移除4种色彩支持，请替换为`white`或`black`
- `辅助色`现在被改进为`中性色`，在使用`color`配置以及配色时需要注意以下替换（色值不一致）：
    - `light-black` 替换为 `neutral-11`
    - `extra-light-black` 替换为 `neutral-10`
    - `blue` 替换为 `neutral-9`
    - `light-blue` 替换为 `neutral-8`
    - `extra-light-blue` 替换为 `neutral-7`
    - `silver` 替换为 `neutral-6`
    - `light-silver` 替换为 `neutral-5`
    - `extra-light-silver` 替换为 `neutral-4`
    - `light-gray` 替换为 `neutral-3`
    - `gray` 替换为 `neutral-2`
    - 新增`neutral-1`、`transparent`

## 0.12.33

`2019年5月16日`

#### 新特性

- `ui-timepicker`、`ui-datepicker`、`ui-datetimepicker`组件新增`togglePicker()`方法，可以用来打开/关闭选择器

#### 改进

- `ui-pagination`第一次被设置页码时不会触发`emit`事件

#### 修复

- 修复了`ui-pagination`当`total`配置过少时页码显示不正确的问题

__升级注意事项__

- 现在`ui-pagination`第一次被设置页码时不会触发`emit`事件，如果第一次数据渲染依赖分页组件的`emit`事件场景，需要进行修改

## 0.12.32

`2019年5月13日`
    
#### 改进

- 优化`ui-pagination`分页过多时的性能

## 0.12.31

`2019年5月10日`

#### 改进

- 优化`ui-table`性能

## 0.12.30

`2019年5月6日`

#### 修复

- 回滚`0.12.28`中对于`ui-table`的`list`配置不再需要使用`context`对象进行访问的更新，回滚后在`list`配置中访问`props`、`data`、`methods`等属性或方法需要使用`context`对象

__升级注意事项__

- 在`ui-table`的`list`配置中访问`props`、`data`、`methods`等属性或方法需要使用`context`对象
    
## 0.12.29

`2019年5月6日`

#### 改进

- 分页组件现在会显示第一页和最后一页的页码
- 优化了`ui-table`组件在单元格内使用组件时的性能

## 0.12.28

`2019年4月25日`

#### 改进

- 现在在`ui-table`的`list`配置中用组件时调用`props`、`data`、`methods`等属性或方法不再需要使用`context`对象进行访问
- 优化`ui-table`的`list`配置中使用了组件后，组件事件会重复触发的问题

## 0.12.27

`2019年4月23日`
    
#### 新特性

- `ui-upload`新增`hidden-max-alert`配置

#### 修复

- 修复`ui-select`组件在`multi-select`配置开启和关闭状态时`inside-name`颜色不一致的问题
- 修复`ui-cascader`组件在多选的情况下仍然搜索的问题

## 0.12.26

`2019年4月23日`
    
#### 新特性

- `ui-textinput`和`ui-select`现在在有值的情况下会出现表单内清空按钮

#### 改进

- 优化`ui-upload`在`type` 配置为`box`时可点击上传区域
- 优化所有表单组件当拥有数值时的文本颜色
- 优化`ui-select`选中项的样式
- `ui-select`的`hide-selected`配置默认值由`true`改为`false`
- `ui-form`中的必选表单项标记位置调整到了名字前面

#### 修复

- 修复`ui-cascader`级联组件的禁用状态仍然可以修改数值的问题
- 修复`ui-datetimepicker`组件当点击时间选择时，日期选择弹框会消失的问题

__升级注意事项__

- `ui-select`的`hide-selected`配置默认值由`true`改为`false`

## 0.12.25

`2019年4月21日`
    
#### 新特性

- `ui-cascader`新增`can-search`配置，可以开启搜索功能
- `ui-table`的`row-set`配置新增`readonlySelection`属性，可以在表格多选下禁用某一行
- `ui-calendar`、`ui-datepicker`、`ui-datetimepicker`现在支持按年翻页

#### 改进

- `告示`组件现更名为`警告提示`

#### 修复

- 修复全局事件管理的一个可能导致绑定事件被误解绑的问题

#### 更多

- 新增图标( `mo-icon-left-thin` / `mo-icon-right-thin` / `mo-icon-left-thin-twin` / `mo-icon-right-thin-twin` )

__升级注意事项__

- `告示`组件现更名为`警告提示`

## 0.12.24

`2019年4月20日`
    
#### 新特性

- `ui-textarea`新增`resize`配置，可以通过拖拽调整输入框大小

#### 改进

- `ui-radio`的选中样式默认从`check`调整为`point`

#### 修复

- 修复`ui-upload`在绑定`v-model`后无法批量上传文件的问题
- 修复`ui-upload`的`list-type`配置为`thumbnail`，图片文件缩略图无法等比缩放的问题

__升级注意事项__

- `ui-radio`的`type`配置的默认值由`check`改为`point`

## 0.12.23

`2019年4月19日`

#### 修复

- 修复`ui-table`开启`multi-select`配置后可能导致`col-set`配置失效的问题
- 修复`ui-form`在某些情况下`label-width`无效的情况

## 0.12.22

`2019年4月19日`

#### 新特性

- 新增`ui-form`组件
- 所有表单组件新增`form-note`配置
- `ui-load`新增 `only-hidden`配置
- `ui-upload`新增`list-type`配置
- `ui-table`新增`custom-sort`配置及`col-sort`事件

#### 改进

- 现在`ui-select`的`hide-selected`配置默认改为`false`

#### 修复

- 修复`ui-cascader`组件当`list`配置动态改变时出现显示错误的问题
- 修复`ui-select`组件在特殊情况下可能会无法显示的问题

__升级注意事项__

- `ui-select`组件的`hide-selected`配置默认由`true`变为`false`

## 0.12.21

`2019年4月14日`

#### 新特性

- `ui-upload`组件新增区域和按钮两种风格
- `ui-upload`组件新增`keep-over-limit-file`配置，可以拒绝用户上传超过`max`限制的文件
- `ui-table`支持`checked-row-change`和`highlight-row-change`事件
- `ui-dialog`和`ui-drawer`组件新增`show()`和`hide()`方法

#### 改进

- 统一`ui-dialog`、`ui-popover`、`ui-tip`、`ui-drawer`的`show()`、`hide()`、`toggle()`三个方法

## 0.12.20

`2019年4月12日`

#### 修复

- 修复嵌套使用`ui-row`时的样式问题
- 修复`ui-grid`文档中的一处错误

__升级注意事项__

- 现在使用`ui-grid`时，`ui-row`的父元素必须是`ui-grid`，无法在`ui-col`或`ui-row`中直接嵌套`ui-row`

## 0.12.19

`2019年4月11日`
    
#### 新特性

- `ui-table`新增`setCheckedRows()`方法
- `ui-table`中的栅格间距支持自定义

#### 改进

- 优化`ui-alert`组件中的文本颜色

## 0.12.18

`2019年4月10日`

#### 修复

- 修复`ui-timepicker`、`ui-datepicker`、`ui-datetimepicker`在特定情况下当组件销毁后会报错的问题

## 0.12.17

`2019年4月7日`

#### 新特性

- `ui-radio`支持type配置，可设置小圆点和按钮式样式
- `ui-checkbox`支持按钮式样式
- `ui-texteditor`支持`markdown`配置，可以开启MD编辑模式
- `ui-texteditor`支持`plain-clipboard`配置，可以粘贴纯文本（无样式）
- `ui-textarea`、`ui-switch`、`ui-rate`、`ui-counter`、`ui-cascader`、`ui-transfer`、`ui-multiform`、`ui-slider`、`ui-colorpicker`标准化了`m`尺寸，并支持`s`和`xs`尺寸

#### 改进

- 优化`ui-radio`和`ui-checkbox`不同尺寸的勾选样式
- 现在`ui-switch`的禁用样式统一了
- `ui-multiinput`支持`delete`快捷键
- 优化`ui-breadcrumbs`鼠标移入时的样式
- `ui-tab`禁用标签页现在鼠标移入时会有禁用效果

#### 废弃

- `ui-del`、`ui-u`、`ui-small`、`ui-em`、`ui-strong`已经不再推荐使用

#### 更多

- 文档新增`ui-texteditor`转换为Markdown的示例

<ui-label color="primary">升级注意事项</ui-label>

- `ui-del`、`ui-u`、`ui-small`、`ui-em`、`ui-strong`已经不再推荐使用，替代方案详见组件文档

## 0.12.16

`2019年4月4日`

#### 新特性

- `ui-textinput`、`ui-select`、`ui-checkbox`、`ui-radio`、`ui-multiinput`、`ui-timepicker`、`ui-datepicker`、`ui-datetimepicker`支持`s`和`xs`尺寸

#### 改进

- 优化`ui-tab`选中状态样式
- 优化`ui-menu`菜单项文字对齐方式和字体大小

#### 废弃

- 移除了`ui-textinput`的`l`和`xl`尺寸

<ui-label color="primary">升级注意事项</ui-label>

- `ui-textinput`的`l`和`xl`尺寸被移除了，可以通过覆写样式来支持

## 0.12.15

`2019年4月3日`

#### 新特性

- `ui-table`支持`loading`和`loading-note`配置，可将表格设置为加载中状态
- `ui-menu`支持隐藏某一个菜单项，详见`menu`配置文档

#### 修复

-  修复`ui-datepicker`等日期时间选择组件的边界溢出错位问题
-  修复`ui-datetimepicker`组件在区间选择时开启`date-selectable-range`配置无效的问题
-  修复部分组件使用了未定义的属性
-  修复`ui-popover`组件的属性校验问题
-  修复`ui-select`是部分情况下错误的展示了为空的提示

## 0.12.14

`2019年3月29日`

#### 修复

- 修复`ui-table`头部排序按钮无法显示的问题

## 0.12.13

`2019年3月28日`

#### 改进

- `ui-table`表头支持自定义色彩

## 0.12.12

`2019年3月25日`

#### 新特性

- `ui-grid`支持`ui-row`和`ui-col`写法，详见文档

#### 修复

- 修复日期组件在区间选择模式下，清空表单数据引起的一个问题
- 修复日期组件在区间选择模式下，仅选择一个日期时`getDate()`方法取值错误的问题

#### 更多

- 文档优化关于表单组件获取/设置数值的内容

## 0.12.11

`2019年3月22日`

#### 新特性

- `ui-table`新增`hover-effect`配置，可以设置鼠标`hover`效果

#### 修复

- 修复`ui-table`的`multi-select`配置的一个问题

## 0.12.10

`2019年3月21日`

#### 新特性

- 所有表单的`value-change`事件支持`value`参数，可用于获取表单值
- `ui-tree`新增`block-leaf`配置，可用于展示块状的子节点

#### 改进

- 现在`ui-breadcrumbs`的`emit`事件不会在组件初始化时被触发

#### 修复

- 修复`ui-tree`的一个图标对齐的问题

## 0.12.9

`2019年3月17日`

#### 新特性

- `ui-tree`的`node-emit`、`node-fold`、`node-unfold`事件新增`nodes`参数
- `ui-select`新增`done-hidden`配置
- `ui-pagination`新增`type`配置，支持简洁和迷你模式的分页组件

#### 改进

-  优化文档中对于`form-key`、`group`配置及`setKey()`、`getKey()`、`setGroup()`、`getGroup()`方法的说明

#### 修复

- 修复`ui-tree`文档中的一处错误
- 修复`ui-colorpicker`透明度选择器背景显示问题
- 修复`ui-colorpicker`在HALS和RGBA模式下拷贝透明度不正确的问题
- 修复`ui-datepicker`和`ui-datetimepicker`在靠近左右边界时，弹出框错位的问题

## 0.12.8

`2019年3月15日`

#### 新特性

- `ui-table`新增`highlight-last-click`配置，开启后会高亮最后点击的行
- `ui-table`新增`multi-select`配置，支持多选行
- `ui-table`新增`fixed-title-row`配置，可固定标题行
- `ui-table`新增`getHighlightRow()`、`setHighlightRow()`、`cleanLastClickRow()`方法，可分别用于获取/设置最后一次点击行号及清空
- `ui-table`新增`getCheckedRow()`方法，可获取选中的行号
- `ui-table`新增`cell-click`、`cell-enter`、`cell-leave`事件，分别在点击单元格、鼠标移入/移出单元格触发
- `ui-table`新增`xl`、`l`、`s`、`xs`四种尺寸
- `ui-table`支持通过`slot=“header”`来自定义表头内容
- `ui-tab`的`switch`事件的回调函数新增一个`name`参数，可用于获取当前所在的标签页名字
- `ui-datetimepicker`新增`input-blur`、`input-focus`、`blur`、`focus`事件
- `ui-datepicker`和`ui-datetimepicker`新增`pick-done`事件

#### 改进

- 优化`ui-table`的固定标题列的样式
- `ui-checkbox`的`parent`配置现在支持多个复选框组件关联一个父选项

#### 修复

- 修复`ui-datepicker`的`blur`和`focus`事件在开启`is-range`配置且在两个输入框间切换时会触发两次的问题
- 修复`ui-menu`的在`color=black`且使用`.block`的情况下，选中样式错误的问题
- 修复`ui-menu`动态切换`side-collapse`时的一个样式问题

## 0.12.7

`2019年3月12日`

#### 新特性

- 新增`ui-avatar`头像组件
- 徽章组件更名为徽标，同时从样式组件变更为交互组件，支持作为角标使用，新增计数模式、小圆点模式、图标模式，新增`plain`样式

#### 修复

- 修复`ui-colorpicker`的色板选择层关闭按钮错位的问题

#### 更多

- `ui-dropdown`组件的`auto-close`配置改名为`done-hidden`，使得语意更准确（`done-hidden`为完成后消失，`auto-close`为点击外部区域关闭）
- `ui-lowercase`、`ui-uppercase`、`ui-capitalize`已经不再推荐使用
- 新增图标( `mo-icon-user-o` )

__升级注意事项__

- `ui-lowercase`、`ui-uppercase`、`ui-capitalize`已经不再推荐使用，替代方案详见组件文档
- `ui-dropdown`组件的`auto-close`配置改名为`done-hidden`，请注意替换
- `徽章`更名为`徽标`

## 0.12.6

`2019年3月10日`

#### 新特性

- 新增`ui-backtop`回到顶部组件
- `ui-datetimepicker`新增`getDate()`方法
- `ui-timepicker`、`ui-datepicker`、`ui-datetimepicker`组件新增`relative`配置，支持通过相对日期时间表达式选择日期和时间
- `ui-tip`和`ui-popover`的`trigger`配置新增`rclick`选项，可用于鼠标右键触发

#### 改进

- 优化`ui-grid`的样式文件大小
- `ui-sticky`组件现在有了默认的`z-index`值(为组件库全局初始`z-index`值减1)
- 移除了`ui-tip`组件的最大宽度限制

#### 修复

- 修复`ui-calendar`组件的`getDate`方法取值不正确的问题
- 修复`ui-grid`中的一个样式问题
- 修复`ui-calendar`、`ui-timepicker`、`ui-datepicker`文档中的一些问题
- 修复`ui-checkbox`、`ui-radio`文档中`形态`部分内容无法显示的问题
- 修复`ui-multiinput`组件当处于禁用状态且没有值时，高度错误的问题

#### 更多

- `ui-textleft`、`ui-textcenter`、`ui-textright`已经不再推荐使用
- 依赖库`tether`替换为`popper`，因为`tether`已经不再维护
- `date-fns`升级至`2.0.0-alpha.27`
- `css-loader`升级至`2.1.0`
- `github-markdown-css`升级至`3.0.1`
- `less`升级至`3.9.0`
- `postcss-les`升级至`3.1.1`
- `postcss-loader`升级至`3.0.0`

__升级注意事项__

- `ui-datepicker`、`ui-datetimepicker`、`ui-time`组件的`format`配置格式改变：
    - `YYYY`由`yyyy`替代，`DD`由`dd`替代，因为`YYYY`和`DD`是一个不佳的用法（详见[date-fns: Popular mistakes](https://github.com/date-fns/date-fns/blob/master/docs/unicodeTokens.md#popular-mistakes)）
    - `d`由`i`替代，`do`由`io`替代，`dd`由`iiiiii`替代，`ddd`由`iii`替代，`dddd`由`iiii`，且开始日期从周一开始
    - `DDD`由`D`替代，`DDDo`由`Do`替代，`DDDD`由`DDD`替代
    - `A`由`a`替代，`DDDo`由`Do`替代，`DDDD`由`DDD`替代
- `ui-grid`中的`.col-[n]`元素现在从`display:flex`变为了`display:block`，这会导致子元素的排列方式改变(从横向排列变为垂直)
- `ui-textleft`、`ui-textcenter`、`ui-textright`已经不再推荐使用，替代方案详见组件文档
- `ui-tip`的默认最大宽度限制被移除，现在如果内容过宽，需要在`slot`中的元素上设置额外的样式来解决
- `ui-tip`、`ui-popover`组件`offset`配置现在通过`,`(逗号)来分割两个偏移量，同时第一位改为左右偏移量，第二位改为上下偏移量

## 0.12.5

`2019年3月4日`

#### 新特性

- 新增`ui-time`组件
- `ui-grid`支持设置栅格列的位移，支持等宽栅格，支持水平和垂直对齐方式，支持设置栅格空隙尺寸

#### 改进

- 统一`ui-message`和`ui-load`组件中含义类似的配置名(`time`及`close-time`现在统一为`done-time`)

__升级注意事项__

- `ui-message`组件的`close-time`配置改名为`done-time`
- `ui-load`组件的`time` 配置改名为`done-time`
- 现在`ui-grid`中的`.c-[n]`改名为`.col-[n]`，且必须在`.row`中使用
- `ui-grid`组件的`avggap`样式类改名为`space-around`
- `ui-grid`组件的`nogap`样式类改名为`gutter-none`

## 0.12.4

`2019年3月1日`

#### 新特性

- 新增`ui-drawer`抽屉组件
- `ui-tab`组件的`position`配置新增`right`和`bottom`两个值，可以分别设置位于右侧和底部的标签页
- Morning UI全局配置新增`zIndex`可用来配置组件初始`z-index`值，并以此递增
- Morning UI现在支持圆角定制化

#### 修复

- 修复所有使用`ui-dialog`的组件的弹窗尾部样式问题，以及内容更新会导致头部和尾部消失的问题
- 修复在线演示中Morning UI版本可能不正确的问题

## 0.12.3

`2019年2月26日`

#### 新特性

- `ui-colorpicker`支持`palettes`和`only-palettes`配置，可使用调色板选取色彩及仅使用调色板选取色彩
- `ui-card`支持通过`slot="header"`和`slot="footer"`来设置卡片的头部和尾部，且支持HTML内容
- `ui-card`新增`inside-padding`样式类，用来设置具有内部留白的卡片
- `ui-textinput`新增五种尺寸：`xs`、`s`、`m`、`l`、`xl`
- `ui-textinput`新增`prepend-type`配置，可以区分前缀和后缀的展现类型

#### 改进

- `ui-cascader`组件的滚动条现在符合组件库整体风格
- 现在`ui-dialog`的头部和尾部设置只需通过`slot="header"`或`slot="footer"`来指定，不再要求必须使用`<header>`或`<footer>`标签，和其他组件的用法保持一致

#### 修复

- 修复`ui-textinput`组件在使用`prepend`/`append`和`append-type`配置时的一个样式问题
- 修复`ui-textinput`在使用`prepend`和`append`配置时，同时使用表单的禁用和只读状态时，表单样式错误的问题
- 修复`ui-formgroup`组件会影响子组件中`.item`元素的样式的问题
- 修复表单组件在设置纯数字字符串(比如：`"99"`)时，在转换过程中字符串会被转换成数字类型，若字符串中为较长数字或小数，最终导致输入数据不正确的问题

#### 更多

- 现在所有组件的演示也可以在`CodePen`中在线预览

__升级注意事项__

- `ui-card`不再支持`slot`传入`header`和`div`来设置卡片的头部和主体，现在需要通过`slot="header"`来设置卡片头部，其余内容会默认为卡片的主体
- `ui-textinput`的`append-type`配置不再应用于前缀和后缀的样式控制，现在需要通过`prepend-type`来控制前缀样式，`append-type`来控制后缀样式
- `ui-dialog`中的`<header slot="header">`和`<footer slot="footer">`现在不再需要使用`<header>`或`<footer>`标签，像`<div slot="header">`或`<div slot="footer">`这样的写法也被支持
- `ui-dialog`中`footer`部分，在之前的版本中如果要添加操作区需要在`<footer slot="footer">`标签中增加子级`<div>`来实现，现在可以在任意的标签中使用`.operate`元素来实现一个操作区，比如`<div slot="footer"><div class="operate"></div></div>`这样的写法

## 0.12.2

`2019年2月22日`

#### 新特性

- 支持自定义主题色

#### 改进

- 现在`ui-dropdown`、`ui-tip`、`ui-popover`在鼠标右键点击时不会触发弹出框的显示及隐藏

#### 修复

- 修复`ui-dropdown`当`trigger`配置不为`click`时，点击展示下拉列表的逻辑问题
- 修复`ui-table`文档中的一些问题
- 修复`ui-calendar`文档中的一处问题及部分文档日期格式在`Safari`浏览器中错误的问题
- 修复`ui-tip`组件当`trigger`配置设为`hover click`时的触发行为不正确的问题
- 修复`ui-carousel`文档中的一处错误
- 修复`ui-menu`在使用`side-collapse`配置及`block`样式时的交互样式错误问题

#### 更多

- 所有交互组件可兼容`Firefox`及`Safari`浏览器
- 组件库中所有的`childs`字段均改为`children`

__升级注意事项__

- 所有组件配置中的`childs`字段已改为`children`，涉及：`ui-cascader`的`list`配置、`ui-menu`的`menu`配置、`ui-tree`的`tree`配置


## 0.12.1

`2019年2月19日`

#### 新特性

- 新增`ui-empty`空状态组件
- `ui-transfer`新增`source-to-target-text`和`target-to-source-text`配置，可以自定义按钮文案
- `ui-transfer`新增`source-footer`和`target-footer`两个`slot`，可以自定义两侧底部内容

#### 修复

- 修复`ui-tree`的`can-click`配置设为`false`时，子节点仍然可以点击的问题
- 修复`ui-tree`的连接线(`cable`配置)的样式问题
- 修复一些文档错误

#### 更多

- 新增图标( `mo-icon-tag-f` / `mo-icon-drawer-full` / `mo-icon-drawer-empty`)

## 0.12.0

`2019年2月8日`

#### 新特性

- 新增`ui-tree`树状控件组件
- 新增`ui-rate`评分组件
- 新增`ui-anchor`锚点导航组件
- 新增`ui-transfer`穿梭框组件
- 新增`ui-popover`弹出框组件
- 新增`ui-cascader`级联选择组件
- `ui-carousel`新增`direction`配置，可设置竖向的轮播
- `ui-menu`支持暗色系配色
- `ui-menu`支持`side-collapse`配置，可以折叠侧边栏
- `ui-counter`新增`controls-position`配置，可调按钮位置
- `ui-dropdown`新增`auto-reverse`配置，可在下拉菜单超出可视区域时自动反转出现方向
- `ui-checkbox`和`ui-radio`新增`hidden-options`配置，可以隐藏指定的选项
- `ui-tip`新增`align`配置，可以设置小提示对齐

#### 改进

- 现在`ui-link`和`ui-btn`中使用`js`来执行代码时，可以通过`this`访问正确的视图模型上下文
- 优化文档中示例的展示，使示例更清晰
- 优化文档中配置的展示
- 优化部分组件的示例
- 现在文档中的示例可以在jsfiddle中浏览
- 组件的事件文档增加参数说明
- 组件的方法文档增加返回值说明
- 优化Webpack构建性能

#### 修复

- 修复`ui-itemlist`的一个样式问题
- 修复`ui-grid`的一些样式问题
- 修复`ui-block`文档中的一处错误
- 修复`ui-tab`嵌套使用时，父组件会影响子组件的问题
- 修复`ui-pagination`使用`total`配置时的一个问题
- 修复`ui-pagination`的一个样式问题
- 修复`ui-multiinput`的`add`方法在某些情况下返回`undefined`的问题
- 修复`ui-imagemap`在某些情况下热区编辑区缩放会变为0%的问题
- 修复`ui-tip`当`trigger-in-delay`配置大于0且`trigger`配置为`hover`时，会导致鼠标从触发元素移动到提示内容时，小提示消失的问题
- 修复`ui-tip`中当`trigger`配置为`click`时，点击显示，然后使用`toggle()`方法关闭小提示后，点击无法再次打开的问题

#### 废弃

- 移除所有表单组件`default-value`配置

#### 更多

- Morning UI 网站更新
- Morning UI Roadmap更新
- 推荐Vue版本升级至`2.5.22`
- 优化单元测试写法
- `v-model`在表单组件初始化时会同步数值到表单，行为与`default-value`保持一致
- 修正部分文档中的错误
- 新增Vue版本兼容性测试
- 新增三个图标(`mo-icon-folder-close-o`/`mo-icon-folder-open-o`/`mo-icon-file-o`)

__升级注意事项__

- 请注意本地Vue版本，推荐版本升级至`2.5.22`
- 现在所有表单组件的`default-value`配置被废弃了，可以通过`v-model`来替代。若只想为表单单次设值，也可以通过`set()`或`setGroup()`方法来替代。
- 现在`v-model`的行为有略微改变，将会在表单初始化时对表单进行首次赋值。在早前的版本中若表单处于`disabled`状态，只有`default-value`会进行首次赋值，`v-model`不会首次赋值。在新的版本中表单处于`disabled`状态，`v-model`也会进行首次赋值。

## 0.11.17

`2018年1月3日`

#### 改进

- 现在`ui-table`在导出csv文件时会过滤HTML标签，并将`<br>`转换为换行符

#### 修复

- 修复`ui-dialog`使用时可能导致内部元素高宽获取错误的问题
- 修复`ui-table`导出csv文件时，特殊字符引起的csv错乱
- 修复`ui-table`导出的csv文件中包含中文字符时，在excel中打开乱码的问题

## 0.11.16

`2018年11月14日`

#### 新特性

- `ui-grid`支持响应式布局

#### 修复

- 修复`ui-select`组件设置一个数组的值且数组中包含数字时，值会被过滤的问题
- 修复`ui-pagination`页码输入框的样式问题
- 修复`ui-pagination`组件报错的问题

#### 更多

- LESS升级至`3.8.1`

## 0.11.15

`2018年8月28日`

#### 修复

- 修复`ui-video`和`ui-audio`组件进度条的样式问题
- 修复`ui-imagemap`在某些情况下缩放值会调整为`0%`的问题

#### 更多

- README新增BrowserStack的信息

## 0.11.14

`2018年8月25日`

#### 改进

- 在`ui-table`的单元格中使用Vue组件可以通过`context`对象获取到正确的上下文了(不需要通过`window`代理)
- 使用Vue Lint检查并通过`Priority A: Essential(Error Prevention)`规则

#### 修复

- 修复表单组件的`value-change`会多次触发的问题，并增加对应的单元测试
- 修复边框和背景配色类无效的问题
- 修复部分表单组件禁用状态下的样式问题
- 修复`ui-texteditor`组件在设置特殊数值(对象)时可能出错的问题
- 修复`ui-select`使用`separate-emit`配置后一个样式问题

#### 废弃

-  `ui-select`的选项内容现在仅支持HTML

__升级注意事项__

- 现在表单组件的`value-change`事件不会在组件初始化时触发一次，重复触发次数也减少了，这符合`value-change`事件预期的行为。但是由于之前和触发行为不同，可能导致某些问题。请在升级版本的时候对使用此事件的场景进行检查
- `ui-select`的选项内容现在仅支持HTML，需要排查是否使用了Vue组件，并替换成HTML

## 0.11.13

`2018年8月22日`

#### 新特性

- 新增`ui-carousel`轮播组件
- `ui-formgroup`支持设置表单项标题的对齐方式

#### 改进

- 统一表单组件的`form-name`配置的行为和表现
- 当`form-name`为空时，不需要设置`hide-name`表单名称也会隐藏
- `ui-switch`的`form-name`文字色彩不会随着组件的色彩配置改变

#### 修复

- 修复`ui-counter`的一个样式问题
- 修复`ui-menu`的一些问题

#### 废弃

- `ui-texteditor`组件移除`placeholder`配置
- `ui-switch`组件移除`auto-hide-name`配置

__升级注意事项__

- `form-name`配置现在在所有的表单组件中有了一致的行为和表现，部分表单组件原有显示`form-name`的行为采用新的`inside-name`配置替代，具体使用见组件文档
- `ui-texteditor`组件的`placeholder`配置被移除，可用`inside-name`替代
- `ui-switch`组件移除`auto-hide-name`配置，现在表单名(`form-name`)为空时会自动隐藏
- 现在`ui-switch`的`form-name`文字色彩不会随着组件的色彩配置改变，如需调整色彩，可以通过CSS覆写

## 0.11.12

`2018年8月19日`

#### 新特性

- `ui-menu`新增三种尺寸：`s`、`xs`、`xxs`
- `ui-menu`新增`position-current`配置，可定位到所在菜单项
- `ui-menu`新增`side-expand`配置，可设置不可收缩的菜单
- `ui-menu`新增`line`和`block`两个样式类，支持极简、线条、区块三种风格
- `ui-menu`新增`fill`样式类，可以使菜单自适应父级元素高度（仅在`position`配置为`top`时可用）

#### 改进

- 改进表单组件在`Firefox`及`Safari`浏览器中的兼容性

#### 修复

- 修复`ui-counter`在某些情况下鼠标键放开后仍会计数的错误
- 修复`ui-menu`的一些样式问题

__升级注意事项__

- `ui-menu`的默认样式变为极简，若要使用之前版本的样式，需要添加`line`的样式类

## 0.11.11

`2018年8月15日`

#### 新特性

- 新增`ui-menu`导航菜单组件
- 新增`ui-steps`步骤条组件
- `ui-table`的`col-set`配置支持`pos`，可用于设置列的位置

#### 改进

- `ui-select`支持快捷键(方向上/下键和回车键)选择选项

#### 修复

- 修复`ui-datepicker`和`ui-datetimepicker`在某些情况下弹窗位置会超出可视区边界(位置修正失效)的情况
- 修复`Guide/基础/形态`文档中的一处链接错误

#### 更多

- 推荐Vue版本升级至`2.5.17`

__升级注意事项__

- 请注意本地Vue版本，推荐版本升级至`2.5.17`

## 0.11.10

`2018年7月26日`

#### 新特性

- 新增`ui-alert`告示组件
- `ui-slider`新增`show-counter`配置，可以显示在滑块输入旁显示计数器

#### 改进

- 优化`ui-counter`组件的尺寸，使其与其他表单组件更协调

#### 修复

- 修复`ui-message`组件的`show-type`配置为`topleft`时，消息不会显示的问题
- 修复在浏览器缓存(from disk cache及from memory cache)情况下`ui-upload`组件通过URL获取图片失败的问题

## 0.11.9

`2018年7月23日`

#### 新特性

- 新增`ui-progress`进度条组件
- `ui-textinput`和`ui-textarea`组件新增`maxlength`配置

#### 改进

- 现在`ui-select`的下拉框超过视窗边界时，会自动反转方向

#### 修复

- 修复`ui-dialog`的`z-index`不按打开顺序递增的问题

## 0.11.8

`2018年7月16日`

#### 新特性

- `ui-dropdown`组件新增`trigger-in-delay`配置

#### 改进

- `ui-tip`和`ui-dropdown`组件默认开启`trigger-in-delay`配置
- `ui-colorpicker`在用户输入非法色值时会自动校正

#### 修复

- 修复`ui-dialog`同步调用`toggle(true)`和`toggle(false)`时，窗口不会关闭的问题
- 修复`ui-table`中包含`ui-link`或`ui-btn`时，在开启`fixed-title-col`时滚动列覆盖标题列的问题
- 修复`ui-colorpicker`的`set()`方法在某些情况下设值失败的问题
- 修复`ui-colorpicker`在某些情况下在色板上无法单击选中颜色
- 修复`ui-colorpicker`输入色值后颜色不变的问题

__升级注意事项__

- 现在`ui-tip`和`ui-dropdown`组件的`trigger`配置为`hover`时，不会立即触发，会有200毫秒的延迟。可以通过将`trigger-in-delay`配置设为0，来达到立即触发的效果。

## 0.11.7

`2018年7月10日`

#### 新特性

- 新增`ui-counter`计数器组件
- `ui-tip`新增`trigger-in-delay`配置，可以延迟触发小提示

#### 修复

- 修复`ui-colorpicker`组件的Vue警告

#### 更多

- 更新贡献者指南文档

## 0.11.6

`2018年7月4日`

#### 改进

- 规范了`ui-btn`和`ui-link`的样式行为
- 优化了`ui-dialog`非首次打开的性能

#### 修复

- 修复`ui-select`高性能模式下拉列表高度计算错误的问题
- 修复`ui-texteditor`图片上传弹窗无法主动关闭的问题

## 0.11.5

`2018年7月3日`

#### 新特性

- `ui-datepicker`和`ui-datetimepicker`新增`range-input-direction`配置，可以在区间选择时竖向排列输入框

#### 修复

- 修复`ui-select`文档中的一处错误
- 修复`ui-collapse`开启`max-show`配置无效的问题
- 修复`ui-collapse`的`line`样式类样式错误问题

## 0.11.4

`2018年7月1日`

#### 新特性

- 新增`ui-collapse`折叠面板组件
- `ui-upload`支持显示真实的上传进度
- `ui-colorpicker`新增`show-picker`、`hide-picker`、`hue-slider-change`、`alpha-slider-change`、`input-type-change`事件和`togglePicker`方法
- `ui-tab`新增`disabled-options`配置，支持禁用指定标签

#### 改进

- 使用Parallelism优化CircleCI持续集成性能

#### 修复

- 修复`ui-btn`和`ui-link`的一些样式问题
- 修复`ui-datepicker`和`ui-datetimepicker`在选中特定日期范围时显示区间错误的问题
- 修复`ui-dropdown`点击触发元素无法关闭下拉菜单的问题

## 0.11.3

`2018年6月28日`

#### 新特性

- `ui-texteditor`组件新增图片工具，同时支持图片定位及缩放

#### 改进

-  优化`ui-select`在处理大量可选项时的性能
- `ui-btn`和`ui-link`采用`<a>`标签实现，可支持浏览器中链接的功能

#### 修复

- 修复`ui-video`组件的一个样式问题
- 修复`ui-datepicker`和`ui-datetimepicker`的`done-hidden`配置在开启`quick-pick`时不生效的问题

## 0.11.2

`2018年6月25日`

#### 新特性

- `ui-multiform`组件新增`show-type`配置
- `ui-texteditor`组件`tools`工具配置新增`divider`(横划线)

#### 修复

- 修复`ui-table`在设置标题列并且数据为空时的样式错误
- 修复`ui-imagemap`缩放时光标状态可能与缩放状态不一致的情况
- 修复 `ui-imagemap`在缩放放大模式下新建区域最小高宽错误的问题
- 修复`ui-select`使用`dynamic-list`配置后的一些问题
- 修复`ui-datetimepicker`和`ui-datepicker`在开启`is-range`配置后无法删除选中日期的问题

## 0.11.1

`2018年6月24日`

#### 新特性

- `ui-table`新增title-col-width`配置，可以设置标题列的绝对宽度

#### 修复

- 修复`ui-colorpicker`透明度不能拖动调整的问题
- 修复`ui-select`使用`separate-emit`配置时可能报错的问题(`'removeEventListener' of null`)
- 修复`ui-datetimepicker`和`ui-datepicker`开启`is-range`配置后弹窗错位的问题

#### 更多

- 文档新增富文本编辑器`tools`配置的演示

## 0.11.0

`2018年6月23日`

#### 新特性

- 新增字体图标库
- 新增`ui-sticky`吸附组件
- 新增`ui-audio`音频组件
- 新增`ui-video`视频组件
- 新增`ui-slider`滑块输入组件
- 新增`ui-colorpicker`颜色选择器组件
- `ui-select`新增`list`配置，用来设置可选项目
- `ui-select`新增`dynamic-list`和`validate`配置，开启后支持动态调整可选项目及过滤项目
- `ui-select`新增`max-show-height`配置，用来替代原有的`max-show`，原有的`max-show`配置现在用来控制最多显示项目
- `ui-select`新增`search`事件
- `ui-select`选中项标识更明显
- `ui-textinput`新增`append-type`配置，前置和附加内容支持行内样式
- `ui-textarea`新增`auto-size`配置，可设置段落输入框自动调整高度
- `ui-textarea`新增`max-rows`配置，可设置最大高度
- `ui-btn`新增`plain`、`round`、`circle`样式类，以及可配合`ui-img`实现图片按钮
- `ui-breadcrumbs`新增`separator`配置，可修改层级分隔符
- `ui-tab`新增`position`配置，可调整标签页位置
- `ui-tab`新增`btn`样式类，可设置按钮式标签页
- `ui-checkbox`新增`disabled-options`配置，可禁用部分选项
- `ui-checkbox`新增`max`配置，可设置对多可选项目数
- `ui-checkbox`新增`parent`配置，支持多个`ui-checkbox`选择联动
- `ui-checkbox`新增`border`和`vertical`样式类，为组件增加带边框和垂直样式布局
- `ui-radio`新增`disabled-options`配置，可禁用部分选项
- `ui-radio`新增`border`和`vertical`样式类，为组件增加带边框和垂直样式布局
- `ui-tip`新增`position`方法，配置`trigger`新增`method`选项
- `ui-switch`新增`open-note`和`close-note`配置，可为开关添加备注
- `ui-switch`新增`open-mark`和`close-mark`配置，可为开关添加内部标记
- `ui-datepicker`和`ui-datetimepicker`新增`done-hidden`配置

#### 改进

- 新的文档
- 优化加载动画效果
- 全局事件管理支持`hashchange`事件
- `ui-tab`组件样式优化
- `morning-co-font-*`、`morning-co-border-*`、`morning-co-bg-*`配色类缩短为`mo-co-font-*`、`mo-co-border-*`、`mo-co-bg-*`
- `ui-tip`的`underline`样式类改名为`line`
- `ui-img`的`rounded`样式类改名为`round`
- `ui-switch`组件样式优化
- 优化`ui-formgroup`中的部分字体大小，使其更具可读性
- `ui-multiinput`在删除项目时不会清空输入框已输入的内容

#### 修复

- 修复`ui-dropdown`组件`auto-close`的一个问题

#### 废弃

- `ui-textarea`的`setRows(num)`方法被废弃

#### 更多

- 新的更新日志规范
- 更新对比文档，新增与iView的对比

__升级注意事项__

- `ui-select`的选项定义方式改变，现在需要使用`list`配置来定义选项
- `ui-select`的`max-show`配置改名为`max-show-height`
- `ui-multiinput`在删除项目时不会清空输入框已输入的内容
- `ui-textarea`的`setRows(num)`方法被废弃，采用`rows`配置来替代
- `ui-tab`的`underline`样式类改名为`line`
- `ui-img`的`rounded`样式类改名为`round`
- `ui-downdrop`组件的内置icon从`<i class="morningicon">&#xe6b1;</i>`变为`<i class="mo-icon mo-icon-dropdown"></i>`
- `morning-co-font-*`、`morning-co-border-*`、`morning-co-bg-*`配色类缩短为`mo-co-font-*`、`mo-co-border-*`、`mo-co-bg-*`

## 0.10.32

`2018年6月5日`

- `ui-upload`组件新增`keep-origin-name`配置，可以保留文件原始名
- 修复`ui-table`组件的`empty-cell-value`配置判断问题
- 修复`ui-table`的一些样式问题
- 修复`ui-table`行高计算错误的问题

## 0.10.31

`2018年5月28日`

- `ui-calendar`组件区分高亮当天和高亮日期的样式
- `ui-datepicker`和`ui-datetimepicker`现在会高亮当前日期
- 修复`ui-tip`判断内容是否为空的一个逻辑错误
- 修复`ui-tab`再锚点错误的情况下会报错的问题

## 0.10.30

`2018年5月24日`

- `ui-upload`的`validate`配置新增参数，可用于获取图片的高度和宽度
- 优化 `ui-select`切换下拉列表的性能
- 修复`ui-select`的`z-index`计算错误导致部分场景无法展示的问题
- 修复`ui-imagemap`的值用`getGroup`方式取值时可能出现错误的问题

## 0.10.29

`2018年5月22日`

- `ui-select`新增`list-width`配置用来设置下拉列表的宽度
- 修复`ui-select`组件使用`separate-emit`配置后下拉选项不可见的问题

## 0.10.28

`2018年5月22日`

- `ui-tab`新增`no-padding`样式类
- 优化`ui-select`在渲染大列表时的性能
- 修复`ui-datepick`、`ui-datetimepick`中的快速选择区域消失的问题

__Upgrade Precautions__

- 现在`ui-tab`默认具有内边距，可以通过`no-padding`样式类来取消内边距

## 0.10.27

`2018年5月20日`

- `ui-tab`新增`anchor-target`配置，支持锚点定位
- `ui-select`新增`separate-emit`配置
- 完善组件的基础单元和端点测试
- 修复`ui-imagemap`新增的热区自定义数据为`undefined`
- 修复动态更新`ui-select`可选项时导致选项的Tip错乱的问题
- 修复`ui-tip`和`ui-select`组件文本溢出的一个问题
- 修复Vue警告(Do not use built-in or reserved HTML elements as component id)
- 修复文档中的一些错误

## 0.10.26

`2018年5月18日`

- 新增Vue版本检测并要求大于`2.5.2`
- `ui-timepicker`、`ui-datepicker`、`ui-datetimepicker`新增`separator-type`配置
- 修复`ui-dropdown`和`ui-select`等有弹框的组件导致父容器出现竖向滚动条
- 修复`ui-select`导致父容器出现横向滚动条
- 修复`ui-radio`样式错乱的问题
- 更新Vue文档链接
- 为GitHub增加Contributing Guidelines和Code of conduct

## 0.10.25

`2018年5月17日`

- 优化`ui-select`、`ui-timepicker`、`ui-datepicker`、`ui-datetimepicker`组件的弹框，若超出窗口位置会自动调整位置
- 优化CSS大小(从 240.57kb 减少至 186.257kb)
- 修复日期组件文档中`quick-pick`配置中的一个错误
- 修复`ui-imagemap`的一个问题(`custom validator check failed for prop "color"`)
- 修复`ui-datepicker`中的一个样式问题
- 修复`ui-datepicker`中一个数值类型错误的问题
- 修复`ui-datepicker`中启用`quick-pick`会报错(Uncaught TypeError: Cannot read property '0' of undefined)的问题
- 修复`ui-datepicker`及`ui-datetimepicker`在开启`is-range`的配置时`default-value`超过可选范围时报错的问题
- 修复`ui-timepicker`、`ui-datepicker`、`ui-datetimepicker`中获取相近日期及时间的一个问题
- 修复`ui-select`选中项后，搜索功能显示错误的问题
- 修复`ui-tip`在某些情况下会闪烁的问题
- 新增Morning UI CSS Analysis工具帮助开发者分析各个组件的CSS大小(npm run css-analysis)

__Upgrade Precautions__

- `ui-grid`的`averagegap`被废弃，采用`avggap`替代
- `ui-timepicker`、`ui-datepicker`的`align`配置不再对弹出的时间选择框位置生效，选择框位置仅会居中

## 0.10.24

`2018年5月14日`

- 表单组件新增`readonly`状态
- 新增CHANGELOG
- 为GitHub新增Issue templates及Pull request template
- `ui-dropdown`支持右键触发
- `ui-dropdown`和`ui-tip`的弹出框遇到边界会自动调整位置，使内容在窗口内
- `ui-tip`新增`auto-reverse`配置，当小提示超出窗口时允许反转方向
- 修复`ui-select`在禁用状态下开启`multi-select`配置后仍可输入的问题 
- 修复`ui-select`文档中形态部分的错误
- 修复`ui-imagemap`上传图片后高宽计算错误

## 0.10.23

`2018年5月12日`

- `ui-table`的`col-set`、`row-set`、`cell-set`支持更多的颜色
- `ui-dropdown`支持配合链接使用，并新增`trigger`配置
- 修复`ui-dropdown`下拉弹框可能被遮挡的问题
- 更新README

## 0.10.22

`2018年5月9日`

- `ui-datetimepicker`和`ui-datepicker`支持快速选择 
- 增加主流UI库对比文档
- 修复项目首次运行测试无法通过的问题
- CDN增加unpkg.com

## 0.10.21

`2018年4月22日`

- webpack升级至4.6.0
- 优化工程构建性能
- 优化图片热区组件并增加编辑区缩放功能
- 修复`ui-timepicker`内部滚动会引起外部滚动的问题

## 0.10.20

`2018年4月18日`

- `ui-imagemap`新增`clean-allzone-btn`配置，开启后显示清空所有热区按钮
- 修复`ui-timepicker`在选择时间时，如果禁用了某段时间会有闪烁的问题
- 修复`ui-tip`鼠标无法移动到内容区域的问题
- 修复`ui-datepicker`中`is-range`和`selectable-range`无法同时使用的问题

## 0.10.19

`2018年4月15日`

- `ui-select`组件新增`auto-reset-search`配置，开启后在多选模式下选中项目后会重置搜索内容
- `ui-select`组件新增`hide-selected`配置，关闭后选中的项目不会消失
- 修复`ui-select`组件在多选时，项目值和名称不一致的问题

__Upgrade Precautions__

- `ui-select`移除`clean-btn`配置，采用`clearable`配置代替

## 0.10.18

`2018年4月13日`

- 新增`ui-datetimepicker`日期时间选择器
- 优化`ui-datepicker`的区间选择功能
- `ui-calendar`新增`date-enter`和`date-leave`事件
- `ui-datepicker`新增`input-focus`、`input-blur`、`focus`、`blur`事件
- `ui-timepicker`新增`getDate`方法
- 修复`ui-tab`的标签页不能动态修改的问题
- 修复在Vue版本2.5.14之后`ui-table`会导致内存溢出的问题
- 适配Vue版本至2.5.16

## 0.10.17

`2018年2月26日`

- 新增`ui-datepicker`日期选择器组件
- 修复`ui-select`在同时使用`multi-select`配置和`v-for`生成列表时无法选择的问题
- `ui-calendar`新增`highlight-hover`/`background-mark`/`point-mark`配置以及`click-date`事件

## 0.10.16

`2018年1月31日`

- 新增`ui-timepicker`时间选择器组件
- `ui-imagemap`支持`max-spot`配置

## 0.10.15

`2018年1月16日`

- 标准化组件的clearable行为
- 修复使用`v-model`时组件数值初始化不正确的问题
- 修复`ui-imagemap`组件无法清空数值
    
## 0.10.14

`2018年1月15日`

- `ui-multiform`新增`item-validator`配置
- `ui-textinput`的`append`和`prepend`配置支持HTML
- `ui-textinput`和`ui-select`新增`align`配置
- `ui-select`新增`clearable`配置，可以清空表单数据
- `ui-select`新增`prepend`配置
- 修复`ui-imagemap`组件的`hide-name`配置无效的问题
- 修复`ui-select`的一个取值错误问题
- 修复`ui-message`的z-index问题
- 修复`ui-imagemap`无法删除值的问题

## 0.10.13

`2017年12月7日`

- 配置文档中的key可直接跳转到对应的demo
- 增加许可证扫描([fossa](https://fossa.io/))
- 修复`ui-imagemap`组件的一些问题
- 修复文档的一些问题
- 更新全局命名

## 0.10.12

`2017年12月5日`

- 新增`ui-imagemap`图片热区组件
- 新增`cleanGroup()`方法
- `ui-upload`组件新增`isUploading()`方法，用来判断组件是否仍然上传图片
- 修复`ui-upload`触发最大上传限制后，删除文件仍然显示无法上传的问题
- 修复文档中的一些问题

## 0.10.11

`2017年11月29日`

- 新增`ui-calendar`日历组件
- `ui-table`组件支持单列/多列排序，支持导出`.csv`文件时排除指定列
- `ui-table`支持隐藏特定列
- `ui-table`在没有数据时会显示"无数据"
- 新增`findAllVM`方法用来查找所有匹配`ref`的组件vm
- `ui-message`组件的`close-time`配置新增`false`值，设置后消息不会定时关闭
- 修复`ui-pagination`可能出现无法跳转页码的问题
- 修复`ui-message`组件关闭按钮错误的问题
- 修复`ui-multiform`在使用批量输入后，无法点击修改项目内容的问题
- 修复文档的一些问题

## 0.10.10

`2017年11月27日`

- 新增`ui-message`消息组件
- 组件生成的HTML标签的前缀改为`mor-`
- 符合Vue风格指南中优先级D的规则
- `ui-dialog`组件新增`show-mask`配置

__Upgrade Precautions__

- 组件生成的HTML标签前缀由`i-`变为`mor-`，如JS、CSS有使用请修改

## 0.10.9

`2017年11月23日`

- 新增`ui-upload`文件上传组件
- 修复`morning.getGroupJson`方法无法使用的问题
- 修复`ui-textinput`和`ui-textarea`设置某些值(对象或数组的JSON字符串)得到的结果不符合预期的问题
- 符合Vue风格指南中优先级A的规则

## 0.10.8

`2017年11月20日`

- 组件的配置支持单向数据流(与父组件属性绑定)
- `ui-table`支持HTML内容和Vue组件
- 增加配色CSS类，为组件外元素提供颜色
- 文档章节增加锚点
- 修复`ui-table`配置的一些问题
- 修复文档的一些错误

__Upgrade Precautions__

- `声明`被移除，通过`形态`来替代，使用方法也发生变化，详见`形态`文档
- `声明`的`style`现在通过`形态`的`color`替代
- `声明`中状态的`loading`和`processing`被移除
- `布局组件`更名为`样式组件`
- 组件的`配置`及`形态`支持单向绑定
- `setConf`方法被移除
- `ui-table`的`setList`方法被移除，通过配置`list`替代

## 0.10.7

`2017年11月13日`

- 新增`ui-table`表格组件
- `ui-grid`栅格组件列数从16变为24

__Upgrade Precautions__

- `ui-grid`栅格组件一行列数更新至24列

## 0.10.6

`2017年11月20日`

- 组件的配置支持单向数据流(与父组件属性绑定)
- `ui-table`支持HTML内容和Vue组件
- 增加配色CSS类，为组件外元素提供颜色
- 文档章节增加锚点
- 修复`ui-table`配置的一些问题
- 修复文档的一些错误

__Upgrade Precautions__

- `声明`被移除，通过`形态`来替代，使用方法也发生变化，详见`形态`文档
- `声明`的`style`现在通过`形态`的`color`替代
- `声明`中状态的`loading`和`processing`被移除
- `布局组件`更名为`样式组件`
- 组件的`配置`及`形态`支持单向绑定
- `setConf`方法被移除
- `ui-table`的`setList`方法被移除，通过配置`list`替代

## 0.10.7

`2017年11月13日`

- 新增`ui-table`表格组件
- `ui-grid`栅格组件列数从16变为24

__Upgrade Precautions__

- `ui-grid`栅格组件一行列数更新至24列

## 0.10.6

`2017年11月10日`

- `ui-multiinput`组件新增`update`方法
- `ui-multiform`组件新增`item-filler`和`clean-btn`配置
- 完善样式组件的端点(E2E)测试
- 项目构建工具升级至Webpack3

__Upgrade Precautions__

- `ui-multiform`的`item-title-key`配置被移除，使用`item-filler`替代

## 0.10.5

`2017年11月6日`

- `ui-multiform`组件支持批量输入
- 表单组件数据支持通过`v-model`指令双向绑定
- 网站支持HTTPS，增加Google Analytics

## 0.10.4

`2017年11月5日`

- 新增`ui-multiform`多项表单输入组件
- 支持文档搜索([DocSearch](https://community.algolia.com/docsearch/))
- 支持使用模块管理器(Webpack/Rollup等)
- 支持CDN引用(cdn.jsdelivr.net)

__Upgrade Precautions__

- 通过模块方式引入，不会在全局注册window.morning变量
- 初始化方法从`morning.init([options])`变为`Vue.use(morning, [options])`

## 0.10.3

`2017年11月2日`

- `ui-formgroup`支持内联布局
- 现在表单方法`.get()`返回原始值，`.getJson()`返回JSON值
- 新增样式组件的单元测试
- 更新开发者规范
- 优化CI流程中的测试覆盖率部分，避免重复的测试
- 优化文档构建方式，减小文档体积
- 修复`ui-select`在搜索模式下不会出现`无项目`提示的问题

__Upgrade Precautions__

- 表单组件的`.get()`方法变更，请查询最新文档
- 组件样式中以驼峰法命名的`class`现在换成了中划线法命名
- 所有之前返回`undeifned`的组件方法，现在都会返回组件的Vue实例(取值方法除外)
- `ui-tab`的`switchNext()`和`switchPrev()`方法换成了`next()`和`prev()`方法

## 0.10.2

`2017年11月1日`

- 增加`ui-pagination`分页组件
- 增加codecov.io统计测试覆盖率
- 更新文档
- 修复`ui-select`组件的`list`通过模板渲染，会导致默认值被过滤的问题

## 0.10.1

`2017年10月31日`

- 增加codacy代码质量检测
- 增加Lint、Build、Test、Coverage等CI流程
- 更新README
- 优化功能色彩
- 移除`.npmignore`
- 修复ESLint和StyleLint检测到的问题
- 修复表单组的中表单销毁了，但值还可以通过`getGroup`取到的问题

## 0.10.0

`2017年10月31日`

MorningUI第一个版本，基于HMP UI，规范了定义，实现部分组件。
