#
# Makefile for Phoenix-RTOS psd (Phoenix Serial Downloader)
#
# Copyright 2018, 2019 Phoenix Systems
#

$(PREFIX_PROG)psd: $(addprefix $(PREFIX_O)core/psd/common/, sdp.o) $(PREFIX_A)libusbclass.a $(PREFIX_A)libusbclient.a


$(PREFIX_PROG)psd: $(addprefix $(PREFIX_O)core/psd/imx6ull/, bch.o bcb.o flashmng.o psd.o) $(PREFIX_A)libflashdrv.a
	$(LINK)


$(PREFIX_PROG)psd-old: $(PREFIX_O)core/psd/imx6ull/psd-old.o $(PREFIX_A)libusbclient.a
	$(LINK)

all: $(PREFIX_PROG_STRIPPED)psd-old $(PREFIX_PROG_STRIPPED)psd
