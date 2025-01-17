# IPv4 报文格式

Version（版本）
- 4 bit
- 0100 代表 IPv4 版本
- 0110 代表 IPv6 版本

Header Length（头部长度）
- 4 bit
- 4 bit，二进制为 0000 ~ 1111，即 0 ~ 15，单位为 4 Byte。因此 IP 头部的固定长度 20 Byte 用 0101 来表示，最大长度为 60 Byte（4 bit 的最大值 1111（15） * 4 = 60 Byte）。

Type of Service（服务类型）
- 8 bit
- 只有在有QoS差分服务要求时，这个字段才起作用。

Total Length（总长度）：
- 16 bit
- 代表整个 ip 包的总长度，报文最大为 2^16 - 1 = 65535 Byte
- 数据是通过识别出每个报文的长度字段去进行封装和解封装的。

Identification：


Flags：


Fragment：

TTL（生存时间）

Protocol（协议）

Header Checksum（头部校验和）

Source IP（源 IP）

Destination IP（目标 IP）

Options（选项）

Padding（）
