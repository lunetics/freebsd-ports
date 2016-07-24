# Created by: Matthias Breddin <mb@lunetics.com>
# $FreeBSD$

PORTNAME=	memcached
PORTVERSION=    3.0.0b1
PORTREVISION=	3
CATEGORIES=	databases
PKGNAMEPREFIX=	pecl-
PKGNAMESUFFIX=	-php7
DIST_SUBDIR=	PECL

USE_GITHUB= yes
GH_ACCOUNT= php-memcached-dev
GH_PROJECT= php-memcached
GH_TAGNAME= a8ed240

MAINTAINER=	mb@lunetics.com
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

USE_PHP=    session:build
USES=       php:ext pkgconfig tar:tgz

IGBINARY_CONFIGURE_ENABLE=  memcached-igbinary
IGBINARY_USE=       PHP=igbinary:build
SASL_CONFIGURE_ENABLE=  memcached-sasl
SASL_LIB_DEPENDS=   libsasl2.so:security/cyrus-sasl2
MSGPACK_CONFIGURE_ENABLE= memcached-msgpack
MSGPACK_USE= PHP=msgpack:build
JSON_CONFIGURE_ENABLE= memcached-json
JSON_USE= PHP=json:build

.include <bsd.port.mk>