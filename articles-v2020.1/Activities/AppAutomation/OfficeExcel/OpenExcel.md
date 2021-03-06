# 打开/新建

打开一个Office Excel工作簿并为Excel组件操作提供范围。该组件执行结束时，将关闭指定的工作簿和Excel应用程序（如果在属性面板的&quot;输出&quot;提供了变量，则活动结束后不会关闭）。如果指定的文件路径不存在，在勾选&quot;新建文件&quot;属性时则会新建一个新的Excel文件

## 属性
基本
- **显示名称** ：默认为该组件的名称。支持更改，用户自定义此组件的显示名称
- **失败后继续** ：设置当此组件运行失败时，是否忽略此错误继续运行下一个组件。下拉框选择，当选择"是"时，如果该组件运行时遇到错误，该流程也会继续执行下一个组件，并不会停止；当选择"否"时，如果该组件运行时遇到错误，该流程将会停止执行并抛出错误
- **前延时(毫秒)** ：指定在此组件执行前的等待时间。单位为毫秒（ms）,1000ms = 1s。若此处填写1000，意为上一个组件执行完毕后，等待一秒钟后执行此组件
- **后延时(毫秒)** ：指定在此组件执行后的延迟时间。单位为毫秒（ms）,1000ms = 1s。若此处填写1000，意为此组件执行完毕后，等待一秒钟后执行下一个组件


输入

- **文件路径** ：要打开或者新建的Excel文件全路径（同时支持相对路径）。仅支持字符串变量和字符串
- **密码** ：打开受密码保护的工作簿所需的密码。仅支持字符串变量和字符串

可选项

- **另存为** ：将操作后的工作簿另存为。若提供的另存为全路径与原路径相同，则直接覆盖重写原工作簿。仅支持字符串变量和字符串

- **新建文件** ：勾选时，如果在指定路径下找不到工作簿则新建；不勾选时，如果在指定路径下找不到工作簿，则引发异常
- **自动保存** ：勾选时，在组件运行内的每次更改都会自动保存工作簿；不勾选时，在该组件运行结束后将不保存更改
- **只读** ：以只读模式打开指定工作簿
- **可视** ：勾选时，工作簿将在可视化状态下进行操作；不勾选时，所有操作将在后台进行，不可视
- **启用宏** ：勾选后，实现工作簿的&quot;启用宏&quot;效果。
