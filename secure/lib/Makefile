# $FreeBSD: releng/11.0/secure/lib/Makefile 265420 2014-05-06 04:22:01Z imp $

.include <src.opts.mk>

SUBDIR= 
.if ${MK_OPENSSL} != "no"
SUBDIR+=libcrypto libssl
.if ${MK_OPENSSH} != "no"
SUBDIR+=libssh
.endif
.if ${MK_LIBRESSL} != "no"
SUBDIR+=libtls
.endif
.endif

.if ${MK_TESTS} != "no"
SUBDIR+=tests
.endif

.include <bsd.subdir.mk>
