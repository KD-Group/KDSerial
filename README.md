# serial_module:串行接口模块
## 目录结构

* [serial_module](KDSerial)
    * [base](KDSerial/base)
        * [mock_serial.py](KDSerial/base/mock_serial.py)&nbsp;:&nbsp; 模拟通讯串行接口基类<br/>
        * [real_serial.py](KDSerial/base/real_serial.py)&nbsp;:&nbsp; 真实通讯串行接口基类<br/>
        * [serial_controller.py](KDSerial/base/serial_controller.py)&nbsp;:&nbsp; 串行接口控制类, 控制是采用模拟接口还是真实接口以及串行接口通讯日志<br/>
    * [data_type](KDSerial/data_type)
        * [hex_struct.py](KDSerial/data_type/hex_struct.py)&nbsp;:&nbsp; 十六进制结构体<br/>
    * [exception](KDSerial/exception)
        * [connection_exception.py](KDSerial/exception/connection_exception.py)&nbsp;:&nbsp; 连接异常(没有插上专用串行接口或通讯协议错误导致)<br/>
        * [not_connected_exception.py](KDSerial/exception/not_connected_exception.py)&nbsp;:&nbsp; 无连接异常(用户需要自动手动调用函数连接)<br/>
        * [probe_not_down_exception.py](KDSerial/exception/probe_not_down_exception.py)&nbsp;:&nbsp; 探头无下压异常<br/>
        * [respond_parse_exception.py](KDSerial/exception/respond_parse_exception.py)&nbsp;:&nbsp; 单片机的返回数据解析异常(crc8校验失败/与通讯协议不对应)<br/>
        * [timeout_exception.py](KDSerial/exception/timeout_exception.py)&nbsp;:&nbsp; 超时异常(多次尝试请求无回应)<br/>
    * [interface](KDSerial/interface)
       * [serial_interface.py](KDSerial/interface/serial_interface.py)&nbsp;:&nbsp; 串行接口类的通用接口,如有其它接口可放在这<br/>
* [requirements.txt](requirements.txt)

---