.PHONY: libxml2

libxml2/Makefile:
	# prevent LDFLAGS inheritance from rebar.config
	# cd libxml2; ./configure CFLAGS="$(CFLAGS)" LDFLAGS=
	cd libxml2; ./configure

libxml2: libxml2/Makefile
	cd libxml2; make -j4

compile: libxml2

clean:
	cd libxml; make clean

