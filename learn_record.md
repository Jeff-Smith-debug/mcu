#Github or personal blog is a good treasure. Just as someone said,you should contribute rather than take always.
#Purspose: It takes 3500yuan,and i want share it to all guys. because the teacher dont guide anyone but teach oneself.
# 1 SoC architerture
the mcu is a low-power chip of dealing with ISP image. It takes RISC-V as processor,built-in ITCM SRAM,DTCM SRAM,inculding MIPI,ISP,USB,QSPI,
UART,I2C,GPIO,ethernet MAC controller_IP. has taken SMIC40 topOut.
* CPU: RISV-V
* ITCM: 64KB
* DTCM:64KB
* Perhips:MIPI/USB/HDMI/UART/I2C/QSPI/GPIO
* sys_clk:100Mhz
* MIPI RX encoder
* ISP image deal 
* HDMI INTF

Should pircture the architeure-image by self for a better understanding.

Now what we care first is the CSI_RX_Block;
Data flow: the data from CMOS sampling will flow into SoC; and the CSI_RX master this thing,which takes MIPI CSI2 Protocal.
# 1 CSI_RX
Steps:
	1.Deserialize:
	2.Word_align:
	3.Data line align
	4.RAW12/RAW10 data take
Data_flow_pic:

