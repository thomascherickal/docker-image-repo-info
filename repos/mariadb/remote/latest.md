## `mariadb:latest`

```console
$ docker pull mariadb@sha256:c0237db7b596e410e0b9cff9b3bd65227fdf403aa5d050a33eac024fe3455b4b
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
$ docker pull mariadb@sha256:70faf51cf761fe8cc7fae0e9f573682b2110102b97cbb21e6b96f70730e37eba
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.0 MB (118038254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46acb2f21cf934578ed59ba026b8f9154ccce38474f3e23a224d8c6ec9f558e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 01 Dec 2023 07:43:19 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:43:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:43:21 GMT
ADD file:891dcab0c4ce2880c4dca013d326a3efd7601003b6f5076938d678101e301b79 in / 
# Fri, 01 Dec 2023 07:43:22 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 05:59:53 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql --home-dir /var/lib/mysql
# Sat, 02 Dec 2023 05:59:53 GMT
ENV GOSU_VERSION=1.17
# Sat, 02 Dec 2023 05:59:53 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 02 Dec 2023 06:00:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 02 Dec 2023 06:00:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 02 Dec 2023 06:00:09 GMT
ENV LANG=C.UTF-8
# Sat, 02 Dec 2023 06:00:40 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.2.2 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Sat, 02 Dec 2023 06:00:41 GMT
ARG MARIADB_VERSION=1:11.2.2+maria~ubu2204
# Sat, 02 Dec 2023 06:00:41 GMT
ENV MARIADB_VERSION=1:11.2.2+maria~ubu2204
# Sat, 02 Dec 2023 06:00:41 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.2.2/repo/ubuntu/ jammy main main/debug
# Sat, 02 Dec 2023 06:00:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.2.2/repo/ubuntu/ jammy main main/debug
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 02 Dec 2023 06:00:58 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.2.2/repo/ubuntu/ jammy main main/debug
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql /etc/mysql/mariadb.conf.d/50-mysqld_safe.cnf; 	mkdir -p /var/lib/mysql /run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /run/mysqld; 	chmod 1777 /run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Sat, 02 Dec 2023 06:00:59 GMT
VOLUME [/var/lib/mysql]
# Sat, 02 Dec 2023 06:01:00 GMT
COPY file:9a446c99b3f95c0895b9c81c454dd5f21965ad984eb9becb89690f77b54d08ae in /usr/local/bin/healthcheck.sh 
# Sat, 02 Dec 2023 06:01:00 GMT
COPY file:96ebfe41373ea3f34aed860f1bdf37a922a980d7c3150314988a012b7b1e0ac1 in /usr/local/bin/ 
# Sat, 02 Dec 2023 06:01:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 02 Dec 2023 06:01:00 GMT
EXPOSE 3306
# Sat, 02 Dec 2023 06:01:00 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:aeb9f260d781cd1e09daf0d0a9e5bcb581efce5b33b221f2f4a27de8db66e463`  
		Last Modified: Thu, 30 Nov 2023 02:35:43 GMT  
		Size: 28.4 MB (28399939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19eb1c6c20e389a6e3fea35c96b2a8801193051d9ffb433a17e83ec029eba2e2`  
		Last Modified: Sat, 02 Dec 2023 06:04:37 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1641b3e16fca1feca4d6eda617e0d7878527061e9b1e366e6bcc96a0daa05f0`  
		Last Modified: Sat, 02 Dec 2023 06:04:38 GMT  
		Size: 5.5 MB (5462092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e35664529bc1c82fd82d422237d16c3774da01d364a59bcf55fe54156ae22e1`  
		Last Modified: Sat, 02 Dec 2023 06:04:35 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3198602b044f6d28c9cb91aa751605dc60b424ceeb41fe097e64f2a2ef3a7548`  
		Last Modified: Sat, 02 Dec 2023 06:04:59 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa22afb0a54bbfd324d9b31a262c69cf2ce7836b0caaa750e2cdbfcdad0b7542`  
		Last Modified: Sat, 02 Dec 2023 06:05:09 GMT  
		Size: 84.2 MB (84162522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aedfcb2d397eff1da0be85ec5f93384d62048999acf83e2c4b0f09ea8c223ee6`  
		Last Modified: Sat, 02 Dec 2023 06:04:59 GMT  
		Size: 3.6 KB (3611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a621690fb9ca26b374e3044d9c9864fe86e714de13df12e5ee0a1179debfb6`  
		Last Modified: Sat, 02 Dec 2023 06:04:59 GMT  
		Size: 7.9 KB (7859 bytes)  
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
$ docker pull mariadb@sha256:3d449eba9535ab200d5639874d81257fecc69368506f9a3ad3fee9581513dec8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.0 MB (122047469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d76307ef2d3feacbedf5587c070a7e480432c6dbb78f48ec82af0158e69cd30`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 12 Dec 2023 11:44:57 GMT
ARG RELEASE
# Tue, 12 Dec 2023 11:44:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Dec 2023 11:44:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Dec 2023 11:44:57 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 12 Dec 2023 11:44:59 GMT
ADD file:1729e720d10023da7d783040cefa8f30d3c61772a5e1ae577182a1fcba69aff1 in / 
# Tue, 12 Dec 2023 11:44:59 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 08:18:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql --home-dir /var/lib/mysql
# Sat, 16 Dec 2023 08:18:12 GMT
ENV GOSU_VERSION=1.17
# Sat, 16 Dec 2023 08:18:12 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 16 Dec 2023 08:18:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 16 Dec 2023 08:18:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 16 Dec 2023 08:18:26 GMT
ENV LANG=C.UTF-8
# Sat, 16 Dec 2023 08:19:04 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.2.2 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Sat, 16 Dec 2023 08:19:05 GMT
ARG MARIADB_VERSION=1:11.2.2+maria~ubu2204
# Sat, 16 Dec 2023 08:19:05 GMT
ENV MARIADB_VERSION=1:11.2.2+maria~ubu2204
# Sat, 16 Dec 2023 08:19:06 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.2.2/repo/ubuntu/ jammy main main/debug
# Sat, 16 Dec 2023 08:19:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.2.2/repo/ubuntu/ jammy main main/debug
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 16 Dec 2023 08:19:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.2.2/repo/ubuntu/ jammy main main/debug
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql /etc/mysql/mariadb.conf.d/50-mysqld_safe.cnf; 	mkdir -p /var/lib/mysql /run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /run/mysqld; 	chmod 1777 /run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Sat, 16 Dec 2023 08:19:31 GMT
VOLUME [/var/lib/mysql]
# Sat, 16 Dec 2023 08:19:31 GMT
COPY file:9a446c99b3f95c0895b9c81c454dd5f21965ad984eb9becb89690f77b54d08ae in /usr/local/bin/healthcheck.sh 
# Sat, 16 Dec 2023 08:19:31 GMT
COPY file:96ebfe41373ea3f34aed860f1bdf37a922a980d7c3150314988a012b7b1e0ac1 in /usr/local/bin/ 
# Sat, 16 Dec 2023 08:19:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Dec 2023 08:19:31 GMT
EXPOSE 3306
# Sat, 16 Dec 2023 08:19:31 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:6949655473f9a6801351bc2ee9bef80a58f5ac2dd31547e0d4f473c53d282400`  
		Last Modified: Sat, 16 Dec 2023 07:42:42 GMT  
		Size: 28.7 MB (28654553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26bffac4ffb9f1e2051b95325c4281211af1167d8d31bdc7e8ba1b4fe661a364`  
		Last Modified: Sat, 16 Dec 2023 08:23:47 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8101e5d090baa9bb28394022e958f8cef0991ffc876a70752b27891099f9691`  
		Last Modified: Sat, 16 Dec 2023 08:23:47 GMT  
		Size: 5.5 MB (5531087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317c773017fe3812dc31ed33010542de0512d79313be835675ad9d5d66b846f0`  
		Last Modified: Sat, 16 Dec 2023 08:23:45 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f7a3a0348189fa3fdf04857afd8338b896853512ae378dbbb298a7b3547e891`  
		Last Modified: Sat, 16 Dec 2023 08:24:06 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4ac2ae6206dcf742ee628a65622f1762b51ea9420df76ce3c2ec5cc2ab9e3fd`  
		Last Modified: Sat, 16 Dec 2023 08:24:20 GMT  
		Size: 87.8 MB (87848125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf90172daf4092039d1ecccc4ad4a1cbcb362dde0466b37ec942d2da74682562`  
		Last Modified: Sat, 16 Dec 2023 08:24:06 GMT  
		Size: 3.6 KB (3615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a6da844b5f9671176820f692cb3a2fab15ba1b3d8fc8a44ad18a8fd5c99527c`  
		Last Modified: Sat, 16 Dec 2023 08:24:06 GMT  
		Size: 7.9 KB (7862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
