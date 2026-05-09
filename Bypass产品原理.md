<img width="761" height="991" alt="2466b294f5144e3bb2a4fa4a4f66192" src="https://github.com/user-attachments/assets/6eca8055-b69f-4063-8b19-4ea96d427563" />
<br>

TAP口为分光口（Test Access Point）,分光然后用于监测，分光仅是分光信号强度，数据流量不变<br>
光功率计算公式：10×log（10）（P(mw)/1mw）,在长距离传输过程中可能为负数<br>
分光比为a:b<br>
业务口输出功率为P总+10×log（10）（a/(a+b)）;监控口同理<br>
<br>
分3种模式：<br>
1）k0：直通，不上电也能联通WAN口两端<br>
2）k1：不严格串联，WAN口有流量时复制一份流量到对应LAN口<br>
3）k2：严格串联：从WAN口串联到业务组保护组然后去外部串联设备，再返回保护组从WAN口再发送出去<br>
