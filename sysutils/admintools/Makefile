# Created by: Daniel Morante <daniel@morante.net>
# $FreeBSD$

PORTNAME=	admintools
DISTVERSION=	g20201224
CATEGORIES=	sysutils

MAINTAINER=	daniel@morante.net
COMMENT=	Tools to aid in the DevOps style administration of FreeBSD

LICENSE=	BSD

USE_GITHUB=	yes
GH_TAGNAME=	cc5d4c4
GH_ACCOUNT=	tuaris
GH_PROJECT=	freebsd-${PORTNAME}

NO_ARCH=	yes
NO_BUILD=	yes

PLIST_FILES=	sbin/build-config \
				sbin/iniconfig \
				sbin/setconfig

do-install:
	${INSTALL_SCRIPT} ${WRKSRC}/build-config ${STAGEDIR}${PREFIX}/sbin/
	${INSTALL_SCRIPT} ${WRKSRC}/setconfig ${STAGEDIR}${PREFIX}/sbin/
	${INSTALL_SCRIPT} ${WRKSRC}/iniconfig ${STAGEDIR}${PREFIX}/sbin/

.include <bsd.port.mk>
