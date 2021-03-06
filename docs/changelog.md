## changelog

### 2021.1.31
* **支持同时设置多个元素选择器，并安装自定义消息模板发送提醒消息**
* 修复规则 increase 和 decrease 在首次抓取时的错误
* 添加新监控规则：-without

### 2020.8.14
* 正则表达式，规则和元素选择器最大长度设为500
* 支持多规则

### 2020.8.7
* header 字段不限长度
* 任务频率可以设置为大于0的任意数
* 元素选择器支持修改

### 2019.4.27
* 增加数据导入导出功能
* fix bugs

### 2019.4.18
***此版本改动较大，旧版本备份在 flask 分支***

* django 重构，样式更美观
* 仅保留 sqlite 数据库连接方式
* 通知方式可以预先设置无限多，不再限制各种方式各一个

### 2019.3.31
* 修复 RSS 监控无法正常运行 bug
* 添加规则：equal, less, more

### 2019.3.28
* xpath 支持非正式函数 string() 以获取元素及其子元素的所有文本信息

### 2019.3.16
* 支持 JsonPath 提取 json 数据
* 支持 pushover 通知

### 2019.3.13
* 修正规则匹配逻辑
* 修复多种通知方式下, 某一个出错导致的重复发送连锁反应。现在只要用一种方式通知成功, 系统将保存更新后的监控对象, 从而不会在下一次执行时重复发送
* 展现更详细的任务执行状态