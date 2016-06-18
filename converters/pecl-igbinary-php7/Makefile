# Created by: Matthias Breddin <mb@lunetics.com>
# $FreeBSD$

PORTNAME=	igbinary
PORTVERSION= 1.2.2
CATEGORIES=	converters
PKGNAMEPREFIX=	pecl-
PKGNAMESUFFIX= -php7
DIST_SUBDIR=	PECL

USE_GITHUB= yes
GH_ACCOUNT= igbinary
GH_PROJECT= igbinary7
GH_TAGNAME= 2b7c703


MAINTAINER=	mb@lunetics.com
COMMENT=	Replacement for the standard PHP serializer

LICENSE=	BSD3CLAUSE
LICENSE_FILE=	${WRKSRC}/COPYING

PHP_DEFAULT= 7.0 
IGNORE_WITH_PHP= 55 56
USE_PHP=	session
USE_PHP_BUILD=	yes
USE_PHPEXT=	yes
USE_PHPIZE=	yes
USES=		tar:tgz

.include <bsd.port.mk>
