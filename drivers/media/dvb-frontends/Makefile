# SPDX-License-Identifier: GPL-2.0
#
# Makefile for the kernel DVB frontend device drivers.
#

ccflags-y += -I$(srctree)/drivers/media/tuners/

# FIXME: RTL2832 SDR driver uses power management directly from USB IF driver
ifdef CONFIG_DVB_RTL2832_SDR
	ccflags-y += -I$(srctree)/drivers/media/usb/dvb-usb-v2
endif

cxd2820r-objs := cxd2820r_core.o cxd2820r_c.o cxd2820r_t.o cxd2820r_t2.o
drxd-objs := drxd_firm.o drxd_hard.o
drxk-objs := drxk_hard.o
stb0899-objs := stb0899_drv.o stb0899_algo.o
stv0900-objs := stv0900_core.o stv0900_sw.o

# Please keep it alphabetically sorted by Kconfig name
# (e. g. LC_ALL=C sort Makefile)

obj-$(CONFIG_DVB_A8290) += a8290.o
obj-$(CONFIG_DVB_A8293) += a8293.o
obj-$(CONFIG_DVB_AF9013) += af9013.o
obj-$(CONFIG_DVB_AF9033) += af9033.o
obj-$(CONFIG_DVB_AS102_FE) += as102_fe.o
obj-$(CONFIG_DVB_ASCOT2E) += ascot2e.o
obj-$(CONFIG_DVB_ATBM8830) += atbm8830.o
obj-$(CONFIG_DVB_AU8522) += au8522_common.o
obj-$(CONFIG_DVB_AU8522_DTV) += au8522_dig.o
obj-$(CONFIG_DVB_AU8522_V4L) += au8522_decoder.o
obj-$(CONFIG_DVB_BCM3510) += bcm3510.o
obj-$(CONFIG_DVB_CX22700) += cx22700.o
obj-$(CONFIG_DVB_CX22702) += cx22702.o
obj-$(CONFIG_DVB_CX24110) += cx24110.o
obj-$(CONFIG_DVB_CX24116) += cx24116.o
obj-$(CONFIG_DVB_CX24117) += cx24117.o
obj-$(CONFIG_DVB_CX24120) += cx24120.o
obj-$(CONFIG_DVB_CX24123) += cx24123.o
obj-$(CONFIG_DVB_CXD2099) += cxd2099.o
obj-$(CONFIG_DVB_CXD2820R) += cxd2820r.o
obj-$(CONFIG_DVB_CXD2841ER) += cxd2841er.o
obj-$(CONFIG_DVB_CXD2880) += cxd2880/
obj-$(CONFIG_DVB_DIB3000MB) += dib3000mb.o
obj-$(CONFIG_DVB_DIB3000MC) += dib3000mc.o dibx000_common.o
obj-$(CONFIG_DVB_DIB7000M) += dib7000m.o dibx000_common.o
obj-$(CONFIG_DVB_DIB7000P) += dib7000p.o dibx000_common.o
obj-$(CONFIG_DVB_DIB8000) += dib8000.o dibx000_common.o
obj-$(CONFIG_DVB_DIB9000) += dib9000.o dibx000_common.o
obj-$(CONFIG_DVB_DRX39XYJ) += drx39xyj/
obj-$(CONFIG_DVB_DRXD) += drxd.o
obj-$(CONFIG_DVB_DRXK) += drxk.o
obj-$(CONFIG_DVB_DS3000) += ds3000.o
obj-$(CONFIG_DVB_DUMMY_FE) += dvb_dummy_fe.o
obj-$(CONFIG_DVB_EC100) += ec100.o
obj-$(CONFIG_DVB_GP8PSK_FE) += gp8psk-fe.o
obj-$(CONFIG_DVB_HELENE) += helene.o
obj-$(CONFIG_DVB_HORUS3A) += horus3a.o
obj-$(CONFIG_DVB_ISL6405) += isl6405.o
obj-$(CONFIG_DVB_ISL6421) += isl6421.o
obj-$(CONFIG_DVB_ISL6423) += isl6423.o
obj-$(CONFIG_DVB_IX2505V) += ix2505v.o
obj-$(CONFIG_DVB_L64781) += l64781.o
obj-$(CONFIG_DVB_LG2160) += lg2160.o
obj-$(CONFIG_DVB_LGDT3305) += lgdt3305.o
obj-$(CONFIG_DVB_LGDT3306A) += lgdt3306a.o
obj-$(CONFIG_DVB_LGDT330X) += lgdt330x.o
obj-$(CONFIG_DVB_LGS8GL5) += lgs8gl5.o
obj-$(CONFIG_DVB_LGS8GXX) += lgs8gxx.o
obj-$(CONFIG_DVB_LNBH25) += lnbh25.o
obj-$(CONFIG_DVB_LNBH29) += lnbh29.o
obj-$(CONFIG_DVB_LNBP21) += lnbp21.o
obj-$(CONFIG_DVB_LNBP22) += lnbp22.o
obj-$(CONFIG_DVB_M88DS3103) += m88ds3103.o
obj-$(CONFIG_DVB_M88RS2000) += m88rs2000.o
obj-$(CONFIG_DVB_MB86A16) += mb86a16.o
obj-$(CONFIG_DVB_MB86A20S) += mb86a20s.o
obj-$(CONFIG_DVB_MN88443X) += mn88443x.o
obj-$(CONFIG_DVB_MN88472) += mn88472.o
obj-$(CONFIG_DVB_MN88473) += mn88473.o
obj-$(CONFIG_DVB_MT312) += mt312.o
obj-$(CONFIG_DVB_MT352) += mt352.o
obj-$(CONFIG_DVB_MXL5XX) += mxl5xx.o
obj-$(CONFIG_DVB_MXL692) += mxl692.o
obj-$(CONFIG_DVB_NXT200X) += nxt200x.o
obj-$(CONFIG_DVB_NXT6000) += nxt6000.o
obj-$(CONFIG_DVB_OR51132) += or51132.o
obj-$(CONFIG_DVB_OR51211) += or51211.o
obj-$(CONFIG_DVB_PLL) += dvb-pll.o
obj-$(CONFIG_DVB_RTL2830) += rtl2830.o
obj-$(CONFIG_DVB_RTL2832) += rtl2832.o
obj-$(CONFIG_DVB_RTL2832_SDR) += rtl2832_sdr.o
obj-$(CONFIG_DVB_S5H1409) += s5h1409.o
obj-$(CONFIG_DVB_S5H1411) += s5h1411.o
obj-$(CONFIG_DVB_S5H1420) += s5h1420.o
obj-$(CONFIG_DVB_S5H1432) += s5h1432.o
obj-$(CONFIG_DVB_S921) += s921.o
obj-$(CONFIG_DVB_SI2165) += si2165.o
obj-$(CONFIG_DVB_SI2168) += si2168.o
obj-$(CONFIG_DVB_SI21XX) += si21xx.o
obj-$(CONFIG_DVB_SP2) += sp2.o
obj-$(CONFIG_DVB_SP887X) += sp887x.o
obj-$(CONFIG_DVB_STB0899) += stb0899.o
obj-$(CONFIG_DVB_STB6000) += stb6000.o
obj-$(CONFIG_DVB_STB6100) += stb6100.o
obj-$(CONFIG_DVB_STV0288) += stv0288.o
obj-$(CONFIG_DVB_STV0297) += stv0297.o
obj-$(CONFIG_DVB_STV0299) += stv0299.o
obj-$(CONFIG_DVB_STV0367) += stv0367.o
obj-$(CONFIG_DVB_STV0900) += stv0900.o
obj-$(CONFIG_DVB_STV090x) += stv090x.o
obj-$(CONFIG_DVB_STV0910) += stv0910.o
obj-$(CONFIG_DVB_STV6110) += stv6110.o
obj-$(CONFIG_DVB_STV6110x) += stv6110x.o
obj-$(CONFIG_DVB_STV6111) += stv6111.o
obj-$(CONFIG_DVB_TC90522) += tc90522.o
obj-$(CONFIG_DVB_TDA10021) += tda10021.o
obj-$(CONFIG_DVB_TDA10023) += tda10023.o
obj-$(CONFIG_DVB_TDA10048) += tda10048.o
obj-$(CONFIG_DVB_TDA1004X) += tda1004x.o
obj-$(CONFIG_DVB_TDA10071) += tda10071.o
obj-$(CONFIG_DVB_TDA10086) += tda10086.o
obj-$(CONFIG_DVB_TDA18271C2DD) += tda18271c2dd.o
obj-$(CONFIG_DVB_TDA665x) += tda665x.o
obj-$(CONFIG_DVB_TDA8083) += tda8083.o
obj-$(CONFIG_DVB_TDA8261) += tda8261.o
obj-$(CONFIG_DVB_TDA826X) += tda826x.o
obj-$(CONFIG_DVB_TS2020) += ts2020.o
obj-$(CONFIG_DVB_TUA6100) += tua6100.o
obj-$(CONFIG_DVB_TUNER_CX24113) += cx24113.o
obj-$(CONFIG_DVB_TUNER_DIB0070) += dib0070.o
obj-$(CONFIG_DVB_TUNER_DIB0090) += dib0090.o
obj-$(CONFIG_DVB_TUNER_ITD1000) += itd1000.o
obj-$(CONFIG_DVB_VES1820) += ves1820.o
obj-$(CONFIG_DVB_VES1X93) += ves1x93.o
obj-$(CONFIG_DVB_ZD1301_DEMOD) += zd1301_demod.o
obj-$(CONFIG_DVB_ZL10036) += zl10036.o
obj-$(CONFIG_DVB_ZL10039) += zl10039.o
obj-$(CONFIG_DVB_ZL10353) += zl10353.o

obj-$(CONFIG_DVB_CXD2817) += cxd2817.o
obj-$(CONFIG_DVB_CXD2850) += cxd2850.o
obj-$(CONFIG_DVB_DS3K) += ds3k.o
obj-$(CONFIG_DVB_TAS2101) += tas2101.o
obj-$(CONFIG_DVB_AVL6882) += avl6882.o
obj-$(CONFIG_DVB_STV091X) += stv091x.o
obj-$(CONFIG_DVB_MXL58X) += mxl58x.o
obj-$(CONFIG_DVB_SI2183) += si2183.o
obj-$(CONFIG_DVB_STID135) += stid135/
