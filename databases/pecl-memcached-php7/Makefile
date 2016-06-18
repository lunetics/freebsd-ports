# Created by: Gea-Suan Lin <gslin@gslin.org>
# $FreeBSD: head/databases/pecl-memcached/Makefile 413836 2016-04-23 06:48:42Z sunpoet $

PORTNAME=	memcached
PORTVERSION=    a8ed240
PORTREVISION=	3
CATEGORIES=	databases
#MASTER_SITES=	https://github.com/php-memcached-dev/php-memcached/archive/
PKGNAMEPREFIX=	pecl-
PKGNAMESUFFIX=	-php7
DIST_SUBDIR=	PECL

USE_GITHUB= yes
GH_ACCOUNT= php-memcached-dev
GH_PROJECT= php-memcached
GH_TAGNAME= a8ed240

MAINTAINER=	sunpoet@FreeBSD.org
COMMENT=	PHP extension for interfacing with memcached via libmemcached library

LICENSE=	PHP30
LICENSE_FILE=	${WRKSRC}/LICENSE

LIB_DEPENDS=	libmemcached.so:databases/libmemcached

BROKEN_powerpc64=	does not build

OPTIONS_DEFINE= IGBINARY \
                SASL \
                MSGPACK \
                JSON

OPTIONS_DEFAULT=JSON

IGBINARY_DESC=  Binary serializer support
MSGPACK_DESC= Msgpack support

CONFIGURE_ARGS= --with-libmemcached-dir=${LOCALBASE}
USE_PHP= session
USE_PHPEXT= yes
USE_PHPIZE= yes
USE_PHP_BUILD=  yes
USES=       pkgconfig tar:tgz

IGBINARY_CONFIGURE_ENABLE=  memcached-igbinary
IGBINARY_USE=       PHP=igbinary
SASL_CONFIGURE_ENABLE=  memcached-sasl
SASL_LIB_DEPENDS=   libsasl2.so:security/cyrus-sasl2
MGSPACK_CONFIGURE_ENABLE= memcached-msgpack
MSGPACK_USE= PHP=msgpack

JSON_CONFIGURE_ENABLE= memcached-json
JSON_USE= PHP=json

.include <bsd.port.mk>