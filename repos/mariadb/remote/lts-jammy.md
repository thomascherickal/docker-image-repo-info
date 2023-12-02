## `mariadb:lts-jammy`

```console
$ docker pull mariadb@sha256:00d3b4988e063d70e1df46993536ab10282967096415b9abd52e84743ea1258d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:lts-jammy` - linux; amd64

```console
$ docker pull mariadb@sha256:36cd50777da463bd3250df14be1e089d54bdd6f9d61f37dec05415496611575b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.3 MB (123292901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc28c72eefe7b971b7ff7e6543eb22a377ac9d234ee0b80529a540dbea4fdce4`
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
# Sat, 02 Dec 2023 02:52:44 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.6 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Sat, 02 Dec 2023 02:52:44 GMT
ARG MARIADB_VERSION=1:10.11.6+maria~ubu2204
# Sat, 02 Dec 2023 02:52:44 GMT
ENV MARIADB_VERSION=1:10.11.6+maria~ubu2204
# Sat, 02 Dec 2023 02:52:44 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.6/repo/ubuntu/ jammy main main/debug
# Sat, 02 Dec 2023 02:52:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.6/repo/ubuntu/ jammy main main/debug
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 02 Dec 2023 02:53:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.6/repo/ubuntu/ jammy main main/debug
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql /etc/mysql/mariadb.conf.d/50-mysqld_safe.cnf; 	mkdir -p /var/lib/mysql /run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /run/mysqld; 	chmod 1777 /run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Sat, 02 Dec 2023 02:53:03 GMT
VOLUME [/var/lib/mysql]
# Sat, 02 Dec 2023 02:53:03 GMT
COPY file:d6a6fe0f5ccf1ff426ecfbbf36fe07bb3e2dee038ff0d2921a15feb1a93838fd in /usr/local/bin/healthcheck.sh 
# Sat, 02 Dec 2023 02:53:03 GMT
COPY file:44f2518cf36698179914a53c24c51ee15f77765915d6dc53baf697230efd95c2 in /usr/local/bin/ 
# Sat, 02 Dec 2023 02:53:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 02 Dec 2023 02:53:03 GMT
EXPOSE 3306
# Sat, 02 Dec 2023 02:53:04 GMT
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
	-	`sha256:8299b80a2e0f97acc0487941c2c5650893ce38a4cc4ea06003bbdcc619ac12e5`  
		Last Modified: Sat, 02 Dec 2023 02:57:40 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a18ec7c9a375c66a1ce9179231d0381cf6a531c4eab7168891005c9ee479ac79`  
		Last Modified: Sat, 02 Dec 2023 02:57:53 GMT  
		Size: 87.2 MB (87186691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669b36336460dcfb7b102cbc633315a295aa889129fdf634ddaef62ab6ee8f3f`  
		Last Modified: Sat, 02 Dec 2023 02:57:40 GMT  
		Size: 3.6 KB (3617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83f908a31ef49e2e1eb080e86bb7bb7268cacedf47e49909ff6ccea0a4401461`  
		Last Modified: Sat, 02 Dec 2023 02:57:40 GMT  
		Size: 7.9 KB (7864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:lts-jammy` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:e4b6d2094c6a4ca98419490989b51ca45b759b77f92cfeb53597bfb44c62e2c4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.8 MB (117803066 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0afa72dd90c6b6a903e31ef6ac13e7dd1bdc2941e32a3928286aab4b0b4a974f`
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
# Thu, 23 Nov 2023 09:49:49 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.6 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 23 Nov 2023 09:49:49 GMT
ARG MARIADB_VERSION=1:10.11.6+maria~ubu2204
# Thu, 23 Nov 2023 09:49:49 GMT
ENV MARIADB_VERSION=1:10.11.6+maria~ubu2204
# Thu, 23 Nov 2023 09:49:49 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.6/repo/ubuntu/ jammy main main/debug
# Thu, 23 Nov 2023 09:49:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.6/repo/ubuntu/ jammy main main/debug
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 23 Nov 2023 09:50:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.6/repo/ubuntu/ jammy main main/debug
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql /etc/mysql/mariadb.conf.d/50-mysqld_safe.cnf; 	mkdir -p /var/lib/mysql /run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /run/mysqld; 	chmod 1777 /run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 23 Nov 2023 09:50:07 GMT
VOLUME [/var/lib/mysql]
# Thu, 23 Nov 2023 09:50:07 GMT
COPY file:d6a6fe0f5ccf1ff426ecfbbf36fe07bb3e2dee038ff0d2921a15feb1a93838fd in /usr/local/bin/healthcheck.sh 
# Thu, 23 Nov 2023 09:50:07 GMT
COPY file:44f2518cf36698179914a53c24c51ee15f77765915d6dc53baf697230efd95c2 in /usr/local/bin/ 
# Thu, 23 Nov 2023 09:50:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Nov 2023 09:50:08 GMT
EXPOSE 3306
# Thu, 23 Nov 2023 09:50:08 GMT
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
	-	`sha256:1709466fea1dcf1b68023e70352e5b90a4ff4c4512092c4866b7c6d6d8d4e51c`  
		Last Modified: Thu, 23 Nov 2023 09:55:04 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5895dea043c00a584a4cb0d984ce1d746e73ebe04803b96dba7895190eaf9018`  
		Last Modified: Thu, 23 Nov 2023 09:55:13 GMT  
		Size: 83.9 MB (83935190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:295bdadc16b9abae56be97c7d1dd3ee0d7ccf1ac6dae9be879295431c73db877`  
		Last Modified: Thu, 23 Nov 2023 09:55:04 GMT  
		Size: 3.6 KB (3611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae899290c1cbec873602c73cdd4f78c9ed7c99fae4adefcab23d0b4ee2fc020a`  
		Last Modified: Thu, 23 Nov 2023 09:55:04 GMT  
		Size: 7.9 KB (7858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:lts-jammy` - linux; ppc64le

```console
$ docker pull mariadb@sha256:85f87392dfe53fde5faf0ae576e52c4c3597e945f405f50e508f41d8bf7f7951
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.7 MB (131674811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d829c9e4cae8572535c074c22caf381298f7631e607b4fa4255cb80147382ee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 05 Oct 2023 07:34:18 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:34:19 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:34:19 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:34:19 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:34:22 GMT
ADD file:595ff761b2778bdc6bb59cbe8ce51c4a247e0f279ccd59a17b5be6cdeac0b4d2 in / 
# Thu, 05 Oct 2023 07:34:22 GMT
CMD ["/bin/bash"]
# Thu, 16 Nov 2023 05:57:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql --home-dir /var/lib/mysql
# Thu, 23 Nov 2023 10:19:42 GMT
ENV GOSU_VERSION=1.17
# Thu, 23 Nov 2023 10:19:42 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 23 Nov 2023 10:20:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Nov 2023 10:20:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 23 Nov 2023 10:20:34 GMT
ENV LANG=C.UTF-8
# Thu, 23 Nov 2023 10:23:39 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.6 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 23 Nov 2023 10:23:40 GMT
ARG MARIADB_VERSION=1:10.11.6+maria~ubu2204
# Thu, 23 Nov 2023 10:23:40 GMT
ENV MARIADB_VERSION=1:10.11.6+maria~ubu2204
# Thu, 23 Nov 2023 10:23:40 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.6/repo/ubuntu/ jammy main main/debug
# Thu, 23 Nov 2023 10:23:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.6/repo/ubuntu/ jammy main main/debug
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 23 Nov 2023 10:24:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.6/repo/ubuntu/ jammy main main/debug
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql /etc/mysql/mariadb.conf.d/50-mysqld_safe.cnf; 	mkdir -p /var/lib/mysql /run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /run/mysqld; 	chmod 1777 /run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 23 Nov 2023 10:24:11 GMT
VOLUME [/var/lib/mysql]
# Thu, 23 Nov 2023 10:24:12 GMT
COPY file:d6a6fe0f5ccf1ff426ecfbbf36fe07bb3e2dee038ff0d2921a15feb1a93838fd in /usr/local/bin/healthcheck.sh 
# Thu, 23 Nov 2023 10:24:12 GMT
COPY file:44f2518cf36698179914a53c24c51ee15f77765915d6dc53baf697230efd95c2 in /usr/local/bin/ 
# Thu, 23 Nov 2023 10:24:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Nov 2023 10:24:13 GMT
EXPOSE 3306
# Thu, 23 Nov 2023 10:24:13 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:589c4cce1daa100afadbdbeda96025d02f85c117e0e60b70801af41b4e618668`  
		Last Modified: Fri, 13 Oct 2023 06:13:20 GMT  
		Size: 35.7 MB (35682793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe0560a699c960cbb34e0a04f1977b7d4eacb4bf39a969f4799f4186e0d0190a`  
		Last Modified: Thu, 16 Nov 2023 06:05:23 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c01b388668e97223cd3dc0a7d95ed325016f75bb732f258a9e93c5815388d04f`  
		Last Modified: Thu, 23 Nov 2023 10:29:17 GMT  
		Size: 6.1 MB (6088371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d3bdc5b7ed022319ef2adaa075c1dd0333b03f801b7f4cf376e204e1b75f011`  
		Last Modified: Thu, 23 Nov 2023 10:29:13 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf90cae265ebf748fc3be78dd197173a7b2d63a6be157e06b9fde797cc34384`  
		Last Modified: Thu, 23 Nov 2023 10:31:27 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd213a1e0faf128877486a7b9c20718e9067187a1c5ed6b89a2c088074522ae6`  
		Last Modified: Thu, 23 Nov 2023 10:31:42 GMT  
		Size: 89.9 MB (89889938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c3c1956a74ce30c684b4dc2ac5ff1b0e51cb414fcdf44124e281ac8643d5289`  
		Last Modified: Thu, 23 Nov 2023 10:31:27 GMT  
		Size: 3.6 KB (3616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0827d865e17c8771586e9669a6a2256bb07c898da3cb82ecb739d2161250f7a`  
		Last Modified: Thu, 23 Nov 2023 10:31:27 GMT  
		Size: 7.9 KB (7863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:lts-jammy` - linux; s390x

```console
$ docker pull mariadb@sha256:56b278d79970a52e19284d849ac305c1c1fd46f36a6b19099d1bf129991a6fcc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.8 MB (121822495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff2d59df2c0f5b65009fe12201f6f9bd27e9c53bf0607f337d34e9ffc790688e`
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
# Thu, 23 Nov 2023 09:48:32 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.6 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 23 Nov 2023 09:48:32 GMT
ARG MARIADB_VERSION=1:10.11.6+maria~ubu2204
# Thu, 23 Nov 2023 09:48:32 GMT
ENV MARIADB_VERSION=1:10.11.6+maria~ubu2204
# Thu, 23 Nov 2023 09:48:32 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.6/repo/ubuntu/ jammy main main/debug
# Thu, 23 Nov 2023 09:48:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.6/repo/ubuntu/ jammy main main/debug
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 23 Nov 2023 09:48:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.6/repo/ubuntu/ jammy main main/debug
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql /etc/mysql/mariadb.conf.d/50-mysqld_safe.cnf; 	mkdir -p /var/lib/mysql /run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /run/mysqld; 	chmod 1777 /run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 23 Nov 2023 09:48:53 GMT
VOLUME [/var/lib/mysql]
# Thu, 23 Nov 2023 09:48:53 GMT
COPY file:d6a6fe0f5ccf1ff426ecfbbf36fe07bb3e2dee038ff0d2921a15feb1a93838fd in /usr/local/bin/healthcheck.sh 
# Thu, 23 Nov 2023 09:48:53 GMT
COPY file:44f2518cf36698179914a53c24c51ee15f77765915d6dc53baf697230efd95c2 in /usr/local/bin/ 
# Thu, 23 Nov 2023 09:48:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Nov 2023 09:48:53 GMT
EXPOSE 3306
# Thu, 23 Nov 2023 09:48:54 GMT
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
	-	`sha256:1a69a9a2775c9ad0f984c4dfa96a5dff11d819835844298d826c3bb51c84d11b`  
		Last Modified: Thu, 23 Nov 2023 09:53:25 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0af844974833e9b0985677e7242013b51d653d781c7a84933b1bd70dc7cb151a`  
		Last Modified: Thu, 23 Nov 2023 09:53:38 GMT  
		Size: 87.6 MB (87627295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dfd54d79d473552b53dad65ec68baecce92281ee52439adb046c172aee948ba`  
		Last Modified: Thu, 23 Nov 2023 09:53:24 GMT  
		Size: 3.6 KB (3616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80f337804eee3f1b8bdb526bfcdfd379afcb56c00422cf694e2c4413057c9dc7`  
		Last Modified: Thu, 23 Nov 2023 09:53:25 GMT  
		Size: 7.9 KB (7860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
