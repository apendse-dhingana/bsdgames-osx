#	@(#)Makefile	8.1 (Berkeley) 5/31/93
# $FreeBSD: src/games/wump/Makefile,v 1.3.6.3 2002/02/18 16:02:43 ru Exp $
# $DragonFly: src/games/wump/Makefile,v 1.4 2006/10/08 16:22:36 pavalos Exp $

PROG=	wump
FILES=	wump.info
MAN=	wump.6
HIDEGAME=hidegame

beforeinstall:
.if !exists(${BINDIR})
	mkdir -p ${BINDIR}
.endif
.if !exists(${FILESDIR})
	mkdir -p ${FILESDIR}
.endif
.if !exists(${MANDIR}6)
	mkdir -p ${MANDIR}6
.endif

.include <bsd.prog.mk>
