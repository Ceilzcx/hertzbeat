NTP监控的中文文档如下：

# NTP监控

> 收集和监控NTP的常规性能指标。

**协议使用：NTP**

### 配置参数

| 参数名称 | 参数帮助描述                                           |
|------|--------------------------------------------------|
| 监控主机 | 被监控的IPv4、IPv6或域名。注意⚠️不包含协议头（例如：https://，http://） |
| 监控名称 | 标识此监控的名称。名称需要是唯一的                                |
| 采集间隔 | 监控周期性数据采集的时间间隔，单位：秒，最小可设置为30秒                    |
| 是否检测 | 是否在添加监控之前检测和检查监控的可用性。只有在检测成功后，添加和修改操作才会继续进行      |
| 描述备注 | 用于更多关于标识和描述此监控的信息，用户可以在此处添加备注信息                  |

### 采集指标

#### 指标集：概要

| 指标名称 | 指标单位 | 指标帮助描述                   |
|------|------|--------------------------|
| 响应时间 | 毫秒   | NTP服务器响应请求所需的时间。         |
| 时间   | 毫秒   | NTP服务器报告的当前时间。           |
| 日期   |      | 与NTP服务器报告的当前时间对应的日期。     |
| 偏移量  | 毫秒   | NTP服务器的时钟与客户端时钟之间的时间差。   |
| 延迟   | 毫秒   | 请求到达NTP服务器并返回响应所需的时间。    |
| 版本号  |      | 服务器使用的NTP协议的版本号。         |
| 模式   |      | NTP服务器的操作模式，如客户端、服务器或广播。 |
| 层级   |      | NTP服务器的层级，表示其与参考时钟的距离。   |
| 参考ID |      | 指示NTP服务器使用的参考时钟或时间源的标识符。 |
| 精度   |      | NTP服务器时钟的精度，表示其准确性。      |