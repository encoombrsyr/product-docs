# 保存为CSV文件

将数据表保存为CSV文件

## 属性

输入
- **数据表** ：将此数据表保存为CSV文件
- **文件路径** ：保存的CSV文件路径。支持相对和绝对路径。需提供文件名且带后缀。例如：“E:\DT.csv”。无后缀则视为文件夹，即没有提供文件名，报错。如果有文件夹不存在，则新建。仅支持字符串变量和字符串

可选项
- **分隔符** ：指定CSV文件的分隔符。此属性可不填写，默认使用逗号。仅支持字符变量和字符
- **编码方式** ：文件的编码方式。可以在 [此处](../../Appendix/Encoding.md) 找到每个字符编码的完整代码列表。要指定要使用的编码类型，请使用&quot; 名称&quot;字段中的值。如果未指定编码类型，则默认为UTF-8。仅支持字符串变量和字符串