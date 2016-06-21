# Created by: Matthias Breddin <mb@lunetics.com>
# $FreeBSD$

PORTNAME=       check_freebsd_version
PORTVERSION=    1.4.1
CATEGORIES=     net-mgmt
PKGNAMEPREFIX=  nagios-

MAINTAINER= mb@lunetics.com
COMMENT=    Monitor FreeBSD version/ports for updates vulnerabilities

USE_GITHUB= yes
GH_ACCOUNT= frlen
GH_PROJECT= nagios-plugins
GH_TAGNAME= c7cb236

PLIST_FILES= libexec/nagios/check_freebsd_version

NO_BUILD=   yes

.include <bsd.port.options.mk>

.if ${OSVERSION} < 1000000
IGNORE= supported for FreeBSD 10.x only
.endif

do-install:
	@${MKDIR} ${STAGEDIR}${PREFIX}/libexec/nagios
	${INSTALL_SCRIPT} ${WRKSRC}/check_freebsd_version ${STAGEDIR}${PREFIX}/libexec/nagios/

.include <bsd.port.mk>
