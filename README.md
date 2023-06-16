# micropython_ir
[![MicroPython](https://img.shields.io/badge/MicroPython-v1.20.0-blue.svg)](https://micropython.org/)

MicroPython on esp32  use IR

## 使用方法
- 1.板子刷好MicroPython
- 2.连接好红外传感器 注意区 发射器和接收器的 针脚
- 2.上传ir.py

```python
# 初始化
# gpio 23 为接收针脚  gpio22为发送针脚   如果只有发射或者接收就只传入对应的针脚
# ir_helper = IRHelper(rx_gpio=23, tx_gpio=22)

# 录制信号
# ir_helper.record_cmd()
# 录制的信号默认将保存在 buttomCMD.txt

# 发送信号
# ir_helper.send_cmd('on')
```

## Acknowledgements
We would like to thank the following projects for their contributions to this project:
- [micropython_espX_IR_Transceiver](https://github.com/gamefunc/micropython_espX_IR_Transceiver):micropython_espX_IR_Transceiver
