# Created by: John Chen <johnpupu@gmail.com>
# $FreeBSD: head/devel/pecl-APCu/Makefile 409110 2016-02-18 14:47:05Z miwi $

PORTNAME=       APCu
PORTVERSION=    5.1.5
CATEGORIES=     devel
MASTER_SITES=   http://pecl.php.net/get/
PKGNAMEPREFIX=  pecl-
PKGNAMESUFFIX=  -php7
DISTNAME=       ${PORTNAME:tl}-${PORTVERSION}
DIST_SUBDIR=    PECL

MAINTAINER=     johnpupu@gmail.com
COMMENT=        APC User Caching

LICENSE=        PHP301

CONFLICTS=      pecl-APC-[0-9]*

CFLAGS+=        -I${LOCALBASE}/include

USES=           php php:phpize php:ext tar:tgz

IGNORE_WITH_PHP= 55 56
PHP_MODNAME=    ${PORTNAME:tl}
WRKSRC=         ${WRKDIR}/${PORTNAME:tl}-${PORTVERSION}

.include <bsd.port.mk>
