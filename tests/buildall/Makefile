.POSIX:

all:	buildall

test:	all
	@true

LDADD_POSIX=`export CC="${CC}"; cd ../../POSIX && command -p sh posix-l.sh "$$PATH"`
CFLAGS_POSIX=`export CC="${CC}"; cd ../../POSIX && command -p sh posix-cflags.sh "$$PATH"`

buildall:
	${MAKE} -f Makefile.inc1 CFLAGS_POSIX="${CFLAGS_POSIX}" LDADD_POSIX="${LDADD_POSIX}" CFLAGS="${CFLAGS}" buildall

clean:
	${MAKE} -f Makefile.inc1 clean
