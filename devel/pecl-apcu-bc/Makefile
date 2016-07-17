# Created by: Matthias Breddin <mb@lunetics.com>
# $FreeBSD$

PORTNAME=           apcu_bc
PORTVERSION=        1.0.3
CATEGORIES=         devel
MASTER_SITES=       http://pecl.php.net/get/
PKGNAMEPREFIX=      pecl-
DIST_SUBDIR=        PECL

MAINTAINER=         mb@lunetics.com
COMMENT=            APCu Backwards Compatibility Module for PHP7

LICENSE=            PHP301

BUILD_DEPENDS=      ${LOCALBASE}/lib/php/20151012/apcu.so:devel/pecl-APCu-php7

CONFLICTS=          pecl-APC-[0-9]*

CFLAGS+=            -I${LOCALBASE}/include
USE_PHP=            apcu
USE_PHP_BUILD=      yes
USE_PHPIZE=         yes
USE_PHPEXT=         yes
IGNORE_WITH_PHP=    55 56
USES=               tar:tgz
PHP_MODNAME=        apc
WRKSRC=             ${WRKDIR}/${PORTNAME:tl}-${PORTVERSION}

.include <bsd.port.mk>
