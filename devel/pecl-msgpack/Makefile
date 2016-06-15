# Created by: John Chen <johnpupu@gmail.com>
# $FreeBSD: head/devel/pecl-msgpack/Makefile 413746 2016-04-21 16:43:14Z swills $

PORTNAME=	msgpack
PORTVERSION=	2.0.1
CATEGORIES=	devel
MASTER_SITES=	http://pecl.php.net/get/
PKGNAMEPREFIX=	pecl-
DIST_SUBDIR=	PECL

MAINTAINER=	johnpupu@gmail.com
COMMENT=	Provides API for communicating with MessagePack serialization

LICENSE=	BSD3CLAUSE

BROKEN_powerpc64=	Does not build

USES=		tar:tgz
USE_PHP=	session
USE_PHPEXT=	yes
USE_PHP_BUILD=	yes

.include <bsd.port.mk>

