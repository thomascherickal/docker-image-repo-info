## `mariadb:latest`

```console
$ docker pull mariadb@sha256:c467ba9511c91be4aa41726c92cde5a42ad804500c9ccccaf27fca032aaf1966
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:latest` - linux; amd64

```console
$ docker pull mariadb@sha256:15bd5a1891a297e2b1ad33c5fdc40846033e064a152d4cf06841bb19bf8ca46c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.5 MB (123522119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8c340abd40f860ae1a18057efd196c6bdd3d0f55bb5e8829ee7e65165a10757`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 01 Dec 2023 07:49:48 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:49:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:49:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:49:48 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:49:50 GMT
ADD file:36d444e2cede3abe58191dcf28890b874c0908f5259bf7e8855338555701c4c5 in / 
# Fri, 01 Dec 2023 07:49:50 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 02:50:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql --home-dir /var/lib/mysql
# Sat, 02 Dec 2023 02:50:33 GMT
ENV GOSU_VERSION=1.17
# Sat, 02 Dec 2023 02:50:33 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 02 Dec 2023 02:50:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 02 Dec 2023 02:50:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 02 Dec 2023 02:50:57 GMT
ENV LANG=C.UTF-8
# Sat, 02 Dec 2023 02:51:31 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.2.2 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Sat, 02 Dec 2023 02:51:31 GMT
ARG MARIADB_VERSION=1:11.2.2+maria~ubu2204
# Sat, 02 Dec 2023 02:51:31 GMT
ENV MARIADB_VERSION=1:11.2.2+maria~ubu2204
# Sat, 02 Dec 2023 02:51:31 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.2.2/repo/ubuntu/ jammy main main/debug
# Sat, 02 Dec 2023 02:51:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.2.2/repo/ubuntu/ jammy main main/debug
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 02 Dec 2023 02:51:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.2.2/repo/ubuntu/ jammy main main/debug
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql /etc/mysql/mariadb.conf.d/50-mysqld_safe.cnf; 	mkdir -p /var/lib/mysql /run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /run/mysqld; 	chmod 1777 /run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Sat, 02 Dec 2023 02:51:50 GMT
VOLUME [/var/lib/mysql]
# Sat, 02 Dec 2023 02:51:51 GMT
COPY file:9a446c99b3f95c0895b9c81c454dd5f21965ad984eb9becb89690f77b54d08ae in /usr/local/bin/healthcheck.sh 
# Sat, 02 Dec 2023 02:51:51 GMT
COPY file:96ebfe41373ea3f34aed860f1bdf37a922a980d7c3150314988a012b7b1e0ac1 in /usr/local/bin/ 
# Sat, 02 Dec 2023 02:51:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 02 Dec 2023 02:51:51 GMT
EXPOSE 3306
# Sat, 02 Dec 2023 02:51:51 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:cbe3537751ce03ea42788c2fbe2d5d336180dc2e20472c8cdba8b3224191d101`  
		Last Modified: Wed, 29 Nov 2023 19:24:54 GMT  
		Size: 30.4 MB (30446322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bfcd11f87510f9327f74383bb00a0ab670566878722210a9b6962ad00519f73`  
		Last Modified: Sat, 02 Dec 2023 02:55:44 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed018e89b8dbdf4acf90e7d2ed58dc4f73aeeb1658c677c727b8a9de02e71bb1`  
		Last Modified: Sat, 02 Dec 2023 02:55:45 GMT  
		Size: 5.6 MB (5646180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4cf40a46f9d08d8a061e6cd0ab848efba143849f06e850515113c35837947a`  
		Last Modified: Sat, 02 Dec 2023 02:55:42 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:938b1b815dca68dc58c3bcdd4a9a97973122fc1db9ea080ff53c595746184339`  
		Last Modified: Sat, 02 Dec 2023 02:56:07 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07e09e75520d2c8b5c245bb3e5c5683f010188ce747cf9c4040573a205092136`  
		Last Modified: Sat, 02 Dec 2023 02:56:20 GMT  
		Size: 87.4 MB (87415915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82012f0ef36fd7d9f3156916988e18ae2b64cc8de65201d025bca669ea8e407d`  
		Last Modified: Sat, 02 Dec 2023 02:56:07 GMT  
		Size: 3.6 KB (3612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6430910462f435d87bfdcd60ff7392350b9f460e9262a7cd27d4fed2ae5acace`  
		Last Modified: Sat, 02 Dec 2023 02:56:07 GMT  
		Size: 7.9 KB (7863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:c16e82975c27f9606a32123b99bd41a48da66082b6bd75c9ac29743f8c9c6fc5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.0 MB (118024134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:578fc149b5b6cdcc71b11aa867b5e117fe613a6450e43230035723e48d4e2c09`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 05 Oct 2023 07:32:20 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:32:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:32:22 GMT
ADD file:f8594e26831508c318e42c8dfd9942041031087b8de1bf3fec11fd75b8b30fd4 in / 
# Thu, 05 Oct 2023 07:32:22 GMT
CMD ["/bin/bash"]
# Thu, 16 Nov 2023 02:40:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql --home-dir /var/lib/mysql
# Thu, 23 Nov 2023 09:47:16 GMT
ENV GOSU_VERSION=1.17
# Thu, 23 Nov 2023 09:47:16 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 23 Nov 2023 09:48:01 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Nov 2023 09:48:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 23 Nov 2023 09:48:02 GMT
ENV LANG=C.UTF-8
# Thu, 23 Nov 2023 09:48:39 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.2.2 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 23 Nov 2023 09:48:39 GMT
ARG MARIADB_VERSION=1:11.2.2+maria~ubu2204
# Thu, 23 Nov 2023 09:48:39 GMT
ENV MARIADB_VERSION=1:11.2.2+maria~ubu2204
# Thu, 23 Nov 2023 09:48:39 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.2.2/repo/ubuntu/ jammy main main/debug
# Thu, 23 Nov 2023 09:48:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.2.2/repo/ubuntu/ jammy main main/debug
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 23 Nov 2023 09:48:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.2.2/repo/ubuntu/ jammy main main/debug
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql /etc/mysql/mariadb.conf.d/50-mysqld_safe.cnf; 	mkdir -p /var/lib/mysql /run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /run/mysqld; 	chmod 1777 /run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 23 Nov 2023 09:48:58 GMT
VOLUME [/var/lib/mysql]
# Thu, 23 Nov 2023 09:48:58 GMT
COPY file:9a446c99b3f95c0895b9c81c454dd5f21965ad984eb9becb89690f77b54d08ae in /usr/local/bin/healthcheck.sh 
# Thu, 23 Nov 2023 09:48:58 GMT
COPY file:96ebfe41373ea3f34aed860f1bdf37a922a980d7c3150314988a012b7b1e0ac1 in /usr/local/bin/ 
# Thu, 23 Nov 2023 09:48:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Nov 2023 09:48:58 GMT
EXPOSE 3306
# Thu, 23 Nov 2023 09:48:58 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:895d322e8e5957c04af3ab7b3431f2a562182d34167c6e159e02044150a66967`  
		Last Modified: Thu, 05 Oct 2023 08:57:30 GMT  
		Size: 28.4 MB (28391939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1bfd6232aacadb38909692f1216810e5f58bcc333b7736ed1cb7d166f87202c`  
		Last Modified: Thu, 16 Nov 2023 02:46:24 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9635f8643bf05e06695d05adb1ecbf464ae7a5cdf420d10592045759a5f233`  
		Last Modified: Thu, 23 Nov 2023 09:53:23 GMT  
		Size: 5.5 MB (5462238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f18dcba3b402af596079e099146f92758bb602ed4bc4b6f9124a54a642a907a9`  
		Last Modified: Thu, 23 Nov 2023 09:53:21 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be30f636e870500e713f60165fbf5646ac440de6304a6ac5ad89556c11ce89bd`  
		Last Modified: Thu, 23 Nov 2023 09:53:44 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72566af8d2f83213b869e6be321b92ec07161eb0d2324b876aac4514b2955929`  
		Last Modified: Thu, 23 Nov 2023 09:53:53 GMT  
		Size: 84.2 MB (84156255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb99e22385cbe2902094df53ad0721e0e44e2157bac18804daf7cf73744232a`  
		Last Modified: Thu, 23 Nov 2023 09:53:44 GMT  
		Size: 3.6 KB (3614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f36ecf4cdc33fe6d153e4d4f485abccca9a9dde4b11a41104146a573a009d0ab`  
		Last Modified: Thu, 23 Nov 2023 09:53:44 GMT  
		Size: 7.9 KB (7861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; ppc64le

```console
$ docker pull mariadb@sha256:14e610de4f8a80510fa1b54a1b21299f237a5602507f2d40ef577cd0b86c93bf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.9 MB (131870720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdf826d8fc11044b8cde2de042bd9818b249b9462f504c63294d8796c00588cf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 01 Dec 2023 08:12:00 GMT
ARG RELEASE
# Fri, 01 Dec 2023 08:12:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 08:12:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 08:12:00 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 08:12:03 GMT
ADD file:80047e51fa5311c19317ab688acec0517d98f1cbf74fa4c22a7105e80ebaf610 in / 
# Fri, 01 Dec 2023 08:12:04 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 04:52:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql --home-dir /var/lib/mysql
# Sat, 02 Dec 2023 04:52:43 GMT
ENV GOSU_VERSION=1.17
# Sat, 02 Dec 2023 04:52:44 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 02 Dec 2023 04:53:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 02 Dec 2023 04:53:23 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 02 Dec 2023 04:53:25 GMT
ENV LANG=C.UTF-8
# Sat, 02 Dec 2023 04:54:37 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.2.2 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Sat, 02 Dec 2023 04:54:37 GMT
ARG MARIADB_VERSION=1:11.2.2+maria~ubu2204
# Sat, 02 Dec 2023 04:54:37 GMT
ENV MARIADB_VERSION=1:11.2.2+maria~ubu2204
# Sat, 02 Dec 2023 04:54:38 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.2.2/repo/ubuntu/ jammy main main/debug
# Sat, 02 Dec 2023 04:54:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.2.2/repo/ubuntu/ jammy main main/debug
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 02 Dec 2023 04:55:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.2.2/repo/ubuntu/ jammy main main/debug
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql /etc/mysql/mariadb.conf.d/50-mysqld_safe.cnf; 	mkdir -p /var/lib/mysql /run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /run/mysqld; 	chmod 1777 /run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Sat, 02 Dec 2023 04:55:22 GMT
VOLUME [/var/lib/mysql]
# Sat, 02 Dec 2023 04:55:22 GMT
COPY file:9a446c99b3f95c0895b9c81c454dd5f21965ad984eb9becb89690f77b54d08ae in /usr/local/bin/healthcheck.sh 
# Sat, 02 Dec 2023 04:55:23 GMT
COPY file:96ebfe41373ea3f34aed860f1bdf37a922a980d7c3150314988a012b7b1e0ac1 in /usr/local/bin/ 
# Sat, 02 Dec 2023 04:55:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 02 Dec 2023 04:55:23 GMT
EXPOSE 3306
# Sat, 02 Dec 2023 04:55:24 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:c3606768af36fe4984cee7cfc0c9d919a7adf83ac4c1849c30da06916b9ec921`  
		Last Modified: Sat, 02 Dec 2023 04:49:10 GMT  
		Size: 35.7 MB (35662741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e99ccf537f14ade1991be78383a73882f9d47c3439aec5f8ac8ddcc30362a68`  
		Last Modified: Sat, 02 Dec 2023 05:04:29 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e54b82585db45ca54bf2cbc161ff92620e0b1884d28f7bd6d11b6a2fb230312d`  
		Last Modified: Sat, 02 Dec 2023 05:04:30 GMT  
		Size: 6.1 MB (6088430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9244d97f40129435c8540bee0a8086cd4b7634c87215c4f69ebd27e2982ec861`  
		Last Modified: Sat, 02 Dec 2023 05:04:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a26710f6946180c8e28f7decd21e148d4e67e6e3c07641499f1cfbdaf5f87e`  
		Last Modified: Sat, 02 Dec 2023 05:04:57 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:377e2cd10b0f571188144f8050f0d45c098b973463e951e64b2567b8fd79d4e4`  
		Last Modified: Sat, 02 Dec 2023 05:05:12 GMT  
		Size: 90.1 MB (90105852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec36e067b47bf946d758b1d9fa698d268f74aa6cb198cada089784e138bac81`  
		Last Modified: Sat, 02 Dec 2023 05:04:57 GMT  
		Size: 3.6 KB (3611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a16198b062d71815269afd13aa489257e1b4ab47b6ed86aba5539eec4d99250`  
		Last Modified: Sat, 02 Dec 2023 05:04:57 GMT  
		Size: 7.9 KB (7856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; s390x

```console
$ docker pull mariadb@sha256:0337ce54ff5e6437e8a745816931658938cc4fcae020bff2bf9fb7f6ff1a9cf3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.0 MB (122042404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6b68b887dac731330f4c34aec32e26cc0890d9ea705ab2f2ba614a43d575071`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 05 Oct 2023 07:29:34 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:29:34 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:29:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:29:34 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:29:36 GMT
ADD file:d165475f8f027ab758a463da57c8c29f5d302f0a87a475ac68fdfae30005c7ac in / 
# Thu, 05 Oct 2023 07:29:36 GMT
CMD ["/bin/bash"]
# Thu, 16 Nov 2023 02:32:57 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql --home-dir /var/lib/mysql
# Thu, 23 Nov 2023 09:45:36 GMT
ENV GOSU_VERSION=1.17
# Thu, 23 Nov 2023 09:45:36 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 23 Nov 2023 09:46:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Nov 2023 09:46:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 23 Nov 2023 09:46:06 GMT
ENV LANG=C.UTF-8
# Thu, 23 Nov 2023 09:46:48 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.2.2 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 23 Nov 2023 09:46:48 GMT
ARG MARIADB_VERSION=1:11.2.2+maria~ubu2204
# Thu, 23 Nov 2023 09:46:48 GMT
ENV MARIADB_VERSION=1:11.2.2+maria~ubu2204
# Thu, 23 Nov 2023 09:46:48 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.2.2/repo/ubuntu/ jammy main main/debug
# Thu, 23 Nov 2023 09:46:49 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.2.2/repo/ubuntu/ jammy main main/debug
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 23 Nov 2023 09:47:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.2.2/repo/ubuntu/ jammy main main/debug
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql /etc/mysql/mariadb.conf.d/50-mysqld_safe.cnf; 	mkdir -p /var/lib/mysql /run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /run/mysqld; 	chmod 1777 /run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 23 Nov 2023 09:47:12 GMT
VOLUME [/var/lib/mysql]
# Thu, 23 Nov 2023 09:47:12 GMT
COPY file:9a446c99b3f95c0895b9c81c454dd5f21965ad984eb9becb89690f77b54d08ae in /usr/local/bin/healthcheck.sh 
# Thu, 23 Nov 2023 09:47:12 GMT
COPY file:96ebfe41373ea3f34aed860f1bdf37a922a980d7c3150314988a012b7b1e0ac1 in /usr/local/bin/ 
# Thu, 23 Nov 2023 09:47:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Nov 2023 09:47:13 GMT
EXPOSE 3306
# Thu, 23 Nov 2023 09:47:13 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:818e4e246beb9ab026d2b95bf051fe9610b92dbc0a35b45d09b0cf237b6f3c2e`  
		Last Modified: Fri, 13 Oct 2023 10:16:45 GMT  
		Size: 28.7 MB (28650497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eaec34821d8eaa6a095ef6e70345e945d226da7e7f888f35a222e5c83c745d2`  
		Last Modified: Thu, 16 Nov 2023 02:39:29 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:258384f677e518178732cb57eed82b31d899a71c665681a933fde0343583be7d`  
		Last Modified: Thu, 23 Nov 2023 09:51:57 GMT  
		Size: 5.5 MB (5530996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17aca596197aea45dac01473bb026bc2f0cb28a8bb23ce5721a4249cdef098e0`  
		Last Modified: Thu, 23 Nov 2023 09:51:55 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ae56e20f75f059fec5e36a582e08f863546e9cac08cf7c35857edf9fddbc41`  
		Last Modified: Thu, 23 Nov 2023 09:52:16 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c190239ad43d102237f2b7300d0f7f8a25936e288a8f74c6ccba139c0bcdb9e`  
		Last Modified: Thu, 23 Nov 2023 09:52:29 GMT  
		Size: 87.8 MB (87847206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f133c6dadb60999781c4dc650c0537263f4f0dfd3cc9d9c10fb27aa09e016e`  
		Last Modified: Thu, 23 Nov 2023 09:52:16 GMT  
		Size: 3.6 KB (3613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edb5b753949674f7fa412db8478873a68f71a8317de279fbfbd597640c4f241e`  
		Last Modified: Thu, 23 Nov 2023 09:52:16 GMT  
		Size: 7.9 KB (7860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
