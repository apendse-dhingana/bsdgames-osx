#	$NetBSD: Makefile,v 1.1 1997/10/04 09:11:14 mrg Exp $
#	$OpenBSD: Makefile,v 1.2 1999/01/21 05:47:37 d Exp $
#	$DragonFly: src/games/hunt/Makefile,v 1.1 2008/09/02 21:50:18 dillon Exp $

SUBDIR=	hunt huntd

beforeinstall:
.if !exists(${BINDIR})
	mkdir -p ${BINDIR}
.endif
.if !exists(${MANDIR}6)
	mkdir -p ${MANDIR}6
.endif

.include <bsd.subdir.mk>
