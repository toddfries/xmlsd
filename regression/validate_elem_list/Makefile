
PROG=validate_elem_list
NOMAN=

.if ${.CURDIR} == ${.OBJDIR}
LDADD+= -L${.CURDIR}/../../
.elif ${.CURDIR}/obj == ${.OBJDIR}
LDADD+= -L${.CURDIR}/../../obj
.else
LDADD+= -L${.OBJDIR}/../../
.endif

SRCS= validate_elem_list.c
DEBUG+= -g
CFLAGS+= -Wall
CFLAGS+= -I../../
CFLAGS+=-I${.CURDIR}/../../
LDADD+= -lexpat -lxmlsd

.include <bsd.prog.mk>
