#	@(#)Makefile	8.1 (Berkeley) 5/31/93
# $FreeBSD: src/games/robots/Makefile,v 1.5.2.3 2002/08/07 16:31:42 ru Exp $
# $DragonFly: src/games/robots/Makefile,v 1.4 2006/10/08 16:22:36 pavalos Exp $

PROG=	robots
CFLAGS+=-DMAX_PER_UID=5
SRCS=	extern.c init_field.c main.c make_level.c move.c move_robs.c \
	play_level.c query.c rnd_pos.c score.c flush_in.c
MAN=	robots.6
DPADD=	${LIBCURSES}
LDADD=	-lcurses
HIDEGAME=hidegame

beforeinstall:
.if !exists(${BINDIR})
	mkdir -p ${BINDIR}
.endif
.if !exists(${VARDIR})
	mkdir -p ${VARDIR}
.endif
.if !exists(${VARDIR}/robots_roll)
	${INSTALL} -o ${BINOWN} -g ${BINGRP} -m 664 /dev/null \
	    ${VARDIR}/robots_roll
.endif
.if !exists(${MANDIR}6)
	mkdir -p ${MANDIR}6
.endif

.include <bsd.prog.mk>
