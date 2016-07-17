# Created by: Matthias Breddin <mb@lunetics.com>
# $FreeBSD$

PORTNAME=	msgpack
PORTVERSION=	0.5.7
PORTREVISION?=	1

CATEGORIES=	devel
MASTER_SITES=	http://pecl.php.net/get/
PKGNAMEPREFIX=	pecl-
PKGNAMESUFFIX=  -php5
DIST_SUBDIR=	PECL

MAINTAINER=	mb@lunetics.com
COMMENT=	PHP extension for interfacing with MessagePack

LICENSE=	BSD3CLAUSE

USE_PHP=    session:build
USES=   php:ext pkgconfig tar:tgz

IGNORE_WITH_PHP=	70

.include <bsd.port.mk>