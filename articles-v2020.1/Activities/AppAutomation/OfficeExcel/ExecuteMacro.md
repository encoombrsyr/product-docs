# 执行宏

执行外部宏文件或者XLSM格式的内部宏，支持实参传递

## 属性
基本
- **显示名称** ：默认为该组件的名称。支持更改，用户自定义此组件的显示名称
- **失败后继续** ：设置当此组件运行失败时，是否忽略此错误继续运行下一个组件。下拉框选择，当选择"是"时，如果该组件运行时遇到错误，该流程也会继续执行下一个组件，并不会停止；当选择"否"时，如果该组件运行时遇到错误，该流程将会停止执行并抛出错误
- **前延时(毫秒)** ：指定在此组件执行前的等待时间。单位为毫秒（ms）,1000ms = 1s。若此处填写1000，意为上一个组件执行完毕后，等待一秒钟后执行此组件
- **后延时(毫秒)** ：指定在此组件执行后的延迟时间。单位为毫秒（ms）,1000ms = 1s。若此处填写1000，意为此组件执行完毕后，等待一秒钟后执行下一个组件


输入

- **宏文件路径** ：执行此外部宏文件。为空时，默认执行工作表内部宏
- **Sub/Function名** ：执行宏的方法名。内部宏和外部宏均需填充此项。仅支持字符串变量和字符串
- **传入实参** ：传入宏文件的实参

输出

- **返回值** ：将宏执行后返回的值存储在此变量，前提为执行宏后有返回值
