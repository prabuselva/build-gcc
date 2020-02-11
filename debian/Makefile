PACKAGES=djgpp-cvs binutils gcc gdb

all: build

build:
	./build-djgpp.sh --batch --no-download --prefix=/usr --destdir=`pwd`/install $(PACKAGES)

install:
	cp -rp install/* $(DESTDIR)/

clean:
	-rm -rf build/ install/
	-find download/*/* ! -wholename '*/.git/*' -delete

.PHONY: all build install clean
