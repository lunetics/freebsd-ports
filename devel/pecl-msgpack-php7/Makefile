# Created by: Matthias Breddin <mb@lunetics.com>
# $FreeBSD$

PORTNAME=	msgpack
PORTVERSION=	2.0.1

CATEGORIES=	devel
MASTER_SITES=	http://pecl.php.net/get/
PKGNAMEPREFIX=	pecl-
PKGNAMESUFFIX=  -php7
DIST_SUBDIR=	PECL

MAINTAINER=	mb@lunetics.com
COMMENT=	PHP extension for interfacing with MessagePack

LICENSE=	BSD3CLAUSE

USE_PHP=    session:build
USES=   php:ext pkgconfig tar:tgz

PHP_DEFAULT= 7.0
IGNORE_WITH_PHP= 55 56

.include <bsd.port.mk>