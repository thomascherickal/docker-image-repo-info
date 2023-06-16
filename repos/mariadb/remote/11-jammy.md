## `mariadb:11-jammy`

```console
$ docker pull mariadb@sha256:212f24e652594f68a4549052b06396cb89f77b50ae29b99b30e679b0f285131d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:11-jammy` - linux; amd64

```console
$ docker pull mariadb@sha256:63f4ae82d147dddf4e8f206c71cd58ae0c035f2a9e213206f87320e4a1832b49
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.4 MB (125411497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b54e74c9be392b0cfa2c5c5eb4e14be88ab4c11565e220927c7bc0f2536e79f0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Mon, 22 May 2023 17:45:50 GMT
ARG RELEASE
# Mon, 22 May 2023 17:45:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 22 May 2023 17:45:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 22 May 2023 17:45:50 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 22 May 2023 17:45:52 GMT
ADD file:2fd2684e989d275c95e18b6f6e9ccf57ca1382ecd8faf4a66961ede28102dedf in / 
# Mon, 22 May 2023 17:45:52 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 01:21:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Jun 2023 01:21:14 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Jun 2023 01:21:14 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Jun 2023 01:21:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Jun 2023 01:21:35 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Jun 2023 01:21:35 GMT
ENV LANG=C.UTF-8
# Fri, 09 Jun 2023 21:29:52 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.0.2 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 09 Jun 2023 21:29:52 GMT
ARG MARIADB_VERSION=1:11.0.2+maria~ubu2204
# Fri, 09 Jun 2023 21:29:52 GMT
ENV MARIADB_VERSION=1:11.0.2+maria~ubu2204
# Fri, 09 Jun 2023 21:29:52 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
# Fri, 09 Jun 2023 21:29:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 09 Jun 2023 21:30:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 09 Jun 2023 21:30:15 GMT
VOLUME [/var/lib/mysql]
# Fri, 09 Jun 2023 21:30:15 GMT
COPY file:835b387376a8b7e7292ae71352abf1c02fc75f579bcc76af370b0497b20be068 in /usr/local/bin/healthcheck.sh 
# Fri, 09 Jun 2023 21:30:16 GMT
COPY file:8a4258a11da28308d0b9b254da95e930f850bcec67d37cfb12bc00f5a37939bd in /usr/local/bin/ 
# Fri, 09 Jun 2023 21:30:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 09 Jun 2023 21:30:16 GMT
EXPOSE 3306
# Fri, 09 Jun 2023 21:30:16 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d1669123f28121211977ed38e663dca1a397c0c001e5386598b96c89b1b1cd51`  
		Last Modified: Mon, 22 May 2023 20:49:59 GMT  
		Size: 30.4 MB (30430275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7942299fe584ae926671d6e010bc59c3ea5e651742cfc7af2488c50fa2daa05f`  
		Last Modified: Fri, 02 Jun 2023 01:24:14 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca116927bbe123aec204718cb63664b2dc19d357b1b6dd7958a354c4b5b3879c`  
		Last Modified: Fri, 02 Jun 2023 01:24:15 GMT  
		Size: 5.6 MB (5592249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0f0b5293ed6194c5d04bf423e3222e39553df6db49e7f775ff6af7c44b92e6`  
		Last Modified: Fri, 02 Jun 2023 01:24:12 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a3772c1823cfea4e158667284bd95f66c2299b54a0a8898ebb14068a9e294c`  
		Last Modified: Fri, 09 Jun 2023 21:34:21 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65ed9178c2cd530336ec2a27ba5e8ec6662acf75bf6f842b27e30597ee6d6c14`  
		Last Modified: Fri, 09 Jun 2023 21:34:35 GMT  
		Size: 89.4 MB (89375914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1917f5a0ac83237c041775808c325c158b848a4abf37ddd44ba501d1108978d`  
		Last Modified: Fri, 09 Jun 2023 21:34:21 GMT  
		Size: 3.5 KB (3526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2003d5da743c6ffb3cb20fdb454e867bbbe910b962a0344223112db40e1880cb`  
		Last Modified: Fri, 09 Jun 2023 21:34:21 GMT  
		Size: 7.3 KB (7307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:11-jammy` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:a7c76f3c09cf523de88524416df422a4c1f1a8388062cc974ad0c1373e2a6126
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.9 MB (119904860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a907bf7d29128542074359db61c4409b6dcb104ed5d9e98b6152f4671ca85beb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Mon, 22 May 2023 17:53:00 GMT
ARG RELEASE
# Mon, 22 May 2023 17:53:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 22 May 2023 17:53:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 22 May 2023 17:53:01 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 22 May 2023 17:53:07 GMT
ADD file:f0435ed8dcf91cc69ec63b6b16d9efac56e5a6a7ec518e1fcc3df7457d3113ed in / 
# Mon, 22 May 2023 17:53:08 GMT
CMD ["/bin/bash"]
# Thu, 01 Jun 2023 23:40:52 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 01 Jun 2023 23:40:52 GMT
ENV GOSU_VERSION=1.14
# Thu, 01 Jun 2023 23:40:52 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 01 Jun 2023 23:41:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 01 Jun 2023 23:41:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 01 Jun 2023 23:41:08 GMT
ENV LANG=C.UTF-8
# Fri, 09 Jun 2023 20:23:04 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.0.2 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 09 Jun 2023 20:23:05 GMT
ARG MARIADB_VERSION=1:11.0.2+maria~ubu2204
# Fri, 09 Jun 2023 20:23:05 GMT
ENV MARIADB_VERSION=1:11.0.2+maria~ubu2204
# Fri, 09 Jun 2023 20:23:05 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
# Fri, 09 Jun 2023 20:23:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 09 Jun 2023 20:23:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 09 Jun 2023 20:23:27 GMT
VOLUME [/var/lib/mysql]
# Fri, 09 Jun 2023 20:23:27 GMT
COPY file:835b387376a8b7e7292ae71352abf1c02fc75f579bcc76af370b0497b20be068 in /usr/local/bin/healthcheck.sh 
# Fri, 09 Jun 2023 20:23:27 GMT
COPY file:8a4258a11da28308d0b9b254da95e930f850bcec67d37cfb12bc00f5a37939bd in /usr/local/bin/ 
# Fri, 09 Jun 2023 20:23:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 09 Jun 2023 20:23:27 GMT
EXPOSE 3306
# Fri, 09 Jun 2023 20:23:27 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:6c7698a779f6d8c45a39a6721fb5cce267d66ff8ab5181c55aa6d02c8ddacd01`  
		Last Modified: Tue, 23 May 2023 02:05:13 GMT  
		Size: 28.4 MB (28389044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3beef926275df9bcc0f302dcc80b1df1778597e3762c0bcba4aba7cb6640680`  
		Last Modified: Thu, 01 Jun 2023 23:43:36 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd40ffbb6cb3906cf4feaa019e5002505b5aa18f7fc6fc78552fe0499d3b56b0`  
		Last Modified: Thu, 01 Jun 2023 23:43:37 GMT  
		Size: 5.4 MB (5405164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31691bc52e3b474eb0509035feef6f06782d2807ad942714f4d3830b8c5aa1b0`  
		Last Modified: Thu, 01 Jun 2023 23:43:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b4de91620aa77d5917e1a6299f85a2c9e37bde196a18518058ac5e8851e79b9`  
		Last Modified: Fri, 09 Jun 2023 20:27:22 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ecbfd4a00bdfaf588cf4ee94c90f43e3b83d1b02df80ae6c3b41b449934030b`  
		Last Modified: Fri, 09 Jun 2023 20:27:32 GMT  
		Size: 86.1 MB (86097592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91656c5c74a81203924fe4ec4eaa72c8e1dc8a89fcb5bc4d155aad7f12aa110d`  
		Last Modified: Fri, 09 Jun 2023 20:27:22 GMT  
		Size: 3.5 KB (3526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbc99aa6f42639a2798a12f0e1836d462e943f555bde80f2436d90e9b2f82df9`  
		Last Modified: Fri, 09 Jun 2023 20:27:22 GMT  
		Size: 7.3 KB (7308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:11-jammy` - linux; ppc64le

```console
$ docker pull mariadb@sha256:f0e7e504ead6939309c5dd20dba8076bf42c31a9b4d3fd99eae0dc19b3e60d51
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.7 MB (131747941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70088daa965e901d2bba38c8854778cec8a57e8c14d083adff2de853a9cf2e88`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Mon, 05 Jun 2023 17:01:00 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:01:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:01:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:01:01 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:01:03 GMT
ADD file:00c4f44b35b683caef54d5b8b0e0b1e68872f45eae17dd7543adaf6c54512447 in / 
# Mon, 05 Jun 2023 17:01:04 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:42:09 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 16 Jun 2023 01:42:09 GMT
ENV GOSU_VERSION=1.14
# Fri, 16 Jun 2023 01:42:10 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 16 Jun 2023 01:42:49 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 16 Jun 2023 01:42:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 16 Jun 2023 01:42:51 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 01:44:02 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.0.2 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 16 Jun 2023 01:44:03 GMT
ARG MARIADB_VERSION=1:11.0.2+maria~ubu2204
# Fri, 16 Jun 2023 01:44:03 GMT
ENV MARIADB_VERSION=1:11.0.2+maria~ubu2204
# Fri, 16 Jun 2023 01:44:03 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
# Fri, 16 Jun 2023 01:44:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 16 Jun 2023 01:44:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 16 Jun 2023 01:45:00 GMT
VOLUME [/var/lib/mysql]
# Fri, 16 Jun 2023 01:45:01 GMT
COPY file:835b387376a8b7e7292ae71352abf1c02fc75f579bcc76af370b0497b20be068 in /usr/local/bin/healthcheck.sh 
# Fri, 16 Jun 2023 01:45:01 GMT
COPY file:8a4258a11da28308d0b9b254da95e930f850bcec67d37cfb12bc00f5a37939bd in /usr/local/bin/ 
# Fri, 16 Jun 2023 01:45:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 01:45:02 GMT
EXPOSE 3306
# Fri, 16 Jun 2023 01:45:02 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:a02dd69d9a8a1e6f4fc2ccb509fb8efd6014b00ff932a757d23b4b012a2bec49`  
		Last Modified: Fri, 16 Jun 2023 00:44:52 GMT  
		Size: 35.7 MB (35711397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ef2f0de58dc6b86ab230fc24fdea7663e7c4036eaecb5cfaa5ca13d0538e76`  
		Last Modified: Fri, 16 Jun 2023 01:55:23 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:527730925c9b9eea7a40aa0f642c5ecb732e3ffe1537b1481481e867ece7fc5b`  
		Last Modified: Fri, 16 Jun 2023 01:55:25 GMT  
		Size: 6.0 MB (6017949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68b6ffe59959eb8b4ce9b862df0bc5e9542904c81ae9b29b3bb640e9df667043`  
		Last Modified: Fri, 16 Jun 2023 01:55:21 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9e369030e1c24e18f39ad5b106945f62c15ea2fa2704e4e03e15f29afb897a`  
		Last Modified: Fri, 16 Jun 2023 01:55:59 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe19c7358a2d6a49e881d1019a1237ed1e6c3247292b8c77c8b81e987a93d9f0`  
		Last Modified: Fri, 16 Jun 2023 01:56:23 GMT  
		Size: 90.0 MB (90005535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c42c78ecc428450f9f26050239aeddeb72a4d32afbc8aee2ebde7a72013248ba`  
		Last Modified: Fri, 16 Jun 2023 01:55:58 GMT  
		Size: 3.5 KB (3529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b74b82f034006b0ea4acf28cee9ef77d234f28418eb46a7615e727b5fac530`  
		Last Modified: Fri, 16 Jun 2023 01:55:59 GMT  
		Size: 7.3 KB (7311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
