<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mariadb`

-	[`mariadb:10`](#mariadb10)
-	[`mariadb:10-focal`](#mariadb10-focal)
-	[`mariadb:10.2`](#mariadb102)
-	[`mariadb:10.2-bionic`](#mariadb102-bionic)
-	[`mariadb:10.2.40`](#mariadb10240)
-	[`mariadb:10.2.40-bionic`](#mariadb10240-bionic)
-	[`mariadb:10.3`](#mariadb103)
-	[`mariadb:10.3-focal`](#mariadb103-focal)
-	[`mariadb:10.3.31`](#mariadb10331)
-	[`mariadb:10.3.31-focal`](#mariadb10331-focal)
-	[`mariadb:10.4`](#mariadb104)
-	[`mariadb:10.4-focal`](#mariadb104-focal)
-	[`mariadb:10.4.21`](#mariadb10421)
-	[`mariadb:10.4.21-focal`](#mariadb10421-focal)
-	[`mariadb:10.5`](#mariadb105)
-	[`mariadb:10.5-focal`](#mariadb105-focal)
-	[`mariadb:10.5.12`](#mariadb10512)
-	[`mariadb:10.5.12-focal`](#mariadb10512-focal)
-	[`mariadb:10.6`](#mariadb106)
-	[`mariadb:10.6-focal`](#mariadb106-focal)
-	[`mariadb:10.6.4`](#mariadb1064)
-	[`mariadb:10.6.4-focal`](#mariadb1064-focal)
-	[`mariadb:focal`](#mariadbfocal)
-	[`mariadb:latest`](#mariadblatest)

## `mariadb:10`

```console
$ docker pull mariadb@sha256:b95f3b88e2880bf1191712c122a4c5998b380c4f1afb87ab9fc1415c0ea0b9ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10` - linux; amd64

```console
$ docker pull mariadb@sha256:2e955f90e3af94a992b3e63d34c93e875706d0ec672b18202630ded0706dde71
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.0 MB (127012840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45eaeedf03deed202dade660cbfe44ae17cac512cfd23ca2becab1cd20b5a6f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:05:00 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 27 Jul 2021 00:05:14 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:05:15 GMT
ENV GOSU_VERSION=1.13
# Tue, 27 Jul 2021 00:05:26 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 27 Jul 2021 00:05:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 27 Jul 2021 00:05:34 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:05:35 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 27 Jul 2021 00:05:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 27 Jul 2021 00:05:37 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 27 Jul 2021 00:05:37 GMT
ENV MARIADB_MAJOR=10.6
# Mon, 09 Aug 2021 19:24:13 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Mon, 09 Aug 2021 19:24:14 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Mon, 09 Aug 2021 19:24:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Mon, 09 Aug 2021 19:24:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 09 Aug 2021 19:24:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 09 Aug 2021 19:24:55 GMT
VOLUME [/var/lib/mysql]
# Mon, 09 Aug 2021 19:24:55 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Mon, 09 Aug 2021 19:24:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Aug 2021 19:24:55 GMT
EXPOSE 3306
# Mon, 09 Aug 2021 19:24:56 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf20e69555c2118df81cd7906473b0bbef5210f014d45113251b1298fb1c996`  
		Last Modified: Tue, 27 Jul 2021 00:10:02 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69afd1ffc85b8fe385e48d00e89467a4e080c81b2447ce86ebf964f3e43efb9`  
		Last Modified: Tue, 27 Jul 2021 00:10:04 GMT  
		Size: 5.5 MB (5488764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e720dc7fcd8609016e69543f354117290ffee7c9ea1bdd97d7ca84bcc06d616`  
		Last Modified: Tue, 27 Jul 2021 00:10:03 GMT  
		Size: 3.6 MB (3582379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a81d177e410065c8eec2b5c018ab6ac60b2a5161184890bc3bf7627e78fb2dd`  
		Last Modified: Tue, 27 Jul 2021 00:10:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827c8c103c898d23db5f0cfc69b6faa45038d27b1ec3c15cb5d5b29ee60fca0b`  
		Last Modified: Tue, 27 Jul 2021 00:09:59 GMT  
		Size: 2.3 MB (2274133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2108ccd013748c7fce6a19a3f7434b860401f78326ac7373c486eafa3c719354`  
		Last Modified: Tue, 27 Jul 2021 00:09:59 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05414cb5e8f4dcf16b70640f3bcf904bafddd184d3971881c10b194fb74e8a0`  
		Last Modified: Mon, 09 Aug 2021 19:27:56 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6981930106c6d6380293a728b1bda2840d2392194e1b19649b7a863e1174054`  
		Last Modified: Mon, 09 Aug 2021 19:28:09 GMT  
		Size: 87.1 MB (87089293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009b7e8d11861e3f00504f9b3ff616177ec6f4e7f14f2e0162b0f92811c73bca`  
		Last Modified: Mon, 09 Aug 2021 19:27:56 GMT  
		Size: 5.6 KB (5613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:d6a5e003eae42397f7ee4589e9f21e231d3721ac131970d2286bd616e7f55bb4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124308266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63449ffc5ac65f64a30f340aa4db0c8d502f74c51962eb9b969f08999b20604e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:44 GMT
ADD file:cec21619ecbd37b4cf8da15153b8957a343cd25c6f714e3ac3969b6003704a58 in / 
# Tue, 31 Aug 2021 01:40:45 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:04:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 31 Aug 2021 03:04:38 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:04:38 GMT
ENV GOSU_VERSION=1.13
# Tue, 31 Aug 2021 03:04:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 31 Aug 2021 03:04:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 31 Aug 2021 03:04:57 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:04:57 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 31 Aug 2021 03:05:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 31 Aug 2021 03:05:05 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 31 Aug 2021 03:05:05 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 31 Aug 2021 03:05:05 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Tue, 31 Aug 2021 03:05:05 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Tue, 31 Aug 2021 03:05:05 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Tue, 31 Aug 2021 03:05:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 31 Aug 2021 03:05:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 31 Aug 2021 03:05:28 GMT
VOLUME [/var/lib/mysql]
# Tue, 31 Aug 2021 03:05:29 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Tue, 31 Aug 2021 03:05:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Aug 2021 03:05:29 GMT
EXPOSE 3306
# Tue, 31 Aug 2021 03:05:29 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ab2d02b1ec420fdb84c9f52abda403b6aef20f5de904a2ecda5ae4f5cd6e4d46`  
		Last Modified: Tue, 31 Aug 2021 01:42:34 GMT  
		Size: 27.2 MB (27173099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d16f1b8a1bc9060d0c98a0e09c73ceab3d694a99f57672d6e44f2f5dcf09eae`  
		Last Modified: Tue, 31 Aug 2021 03:09:41 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16d8285f3be08ea7340eaf6dced5161164096c3fb3345fe8c5d6d64496bc143`  
		Last Modified: Tue, 31 Aug 2021 03:09:40 GMT  
		Size: 5.5 MB (5455084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ffd6c9eed67b115939ab5f6d4bb8ffd2f0f152fe9a61024122b558e83ce912e`  
		Last Modified: Tue, 31 Aug 2021 03:09:39 GMT  
		Size: 3.4 MB (3368457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdbc2935c20fd14d96044dcdb65fb79a0f676bcdf334058da282716411d3ff9b`  
		Last Modified: Tue, 31 Aug 2021 03:09:39 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b302bb5f11cae70b4c8ec1079e6de6c62dacfdce3e8f3ccdfabd6ce44b63d2`  
		Last Modified: Tue, 31 Aug 2021 03:09:37 GMT  
		Size: 2.2 MB (2203569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21de8a622698dffd65e882759b0b6e4fe0e56b60d892f2e4446f94439a1270f`  
		Last Modified: Tue, 31 Aug 2021 03:09:36 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9389e144f5d4ea04b6dc1760537798680338137683d9e509ac7072a5c7282d9`  
		Last Modified: Tue, 31 Aug 2021 03:09:36 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed66c3adfe54028b15ff801e6142c6ae4f65eb2bfd313aed2281deb53c447a1a`  
		Last Modified: Tue, 31 Aug 2021 03:09:51 GMT  
		Size: 86.1 MB (86097727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440559db5c8c5208fa4fd147135bce07d75b0f4a04cc838207b125cb6e4cfcbe`  
		Last Modified: Tue, 31 Aug 2021 03:09:38 GMT  
		Size: 5.6 KB (5609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10` - linux; ppc64le

```console
$ docker pull mariadb@sha256:0cf82c9d58ae3326749b0fe0ed1f094d02516dba9c3e6fdf9d2c193f2fa48b4a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137540073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20c817c255cdeba976f7d5a97418f28626785a200c99e223a6450298661f4b64`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 26 Jul 2021 23:12:46 GMT
ADD file:68eb628c2202763afa91d554dde9668d8a468fe53fdbd2fe98627a5f91d224b4 in / 
# Mon, 26 Jul 2021 23:12:49 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 02:05:55 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 27 Jul 2021 02:06:47 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:06:50 GMT
ENV GOSU_VERSION=1.13
# Tue, 27 Jul 2021 02:07:32 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 27 Jul 2021 02:07:42 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 27 Jul 2021 02:08:11 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:08:14 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 27 Jul 2021 02:08:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 27 Jul 2021 02:08:24 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 27 Jul 2021 02:08:25 GMT
ENV MARIADB_MAJOR=10.6
# Mon, 09 Aug 2021 19:17:05 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Mon, 09 Aug 2021 19:17:08 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Mon, 09 Aug 2021 19:17:10 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Mon, 09 Aug 2021 19:17:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 09 Aug 2021 19:22:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 09 Aug 2021 19:22:56 GMT
VOLUME [/var/lib/mysql]
# Mon, 09 Aug 2021 19:23:00 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Mon, 09 Aug 2021 19:23:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Aug 2021 19:23:12 GMT
EXPOSE 3306
# Mon, 09 Aug 2021 19:23:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:1a396eed835b3b7b4101a9863d174e145ddbb1de1502a63bae726b0f81e7ca93`  
		Last Modified: Mon, 26 Jul 2021 23:15:51 GMT  
		Size: 33.3 MB (33290427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65be85b12a63573ebccb059357c5c0db6046f4a074454eea617c402e3bf99c1f`  
		Last Modified: Tue, 27 Jul 2021 02:26:16 GMT  
		Size: 1.8 KB (1760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:803c8e5bf0c59b9b01b70cac07bb24bc696bc577d8e74c79ff15bcbd480874b4`  
		Last Modified: Tue, 27 Jul 2021 02:26:17 GMT  
		Size: 6.7 MB (6667884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62bd7bf9c00152c4fb338b2c1a01d5b241ceda5c58d9e700a353072ab80fb4b9`  
		Last Modified: Tue, 27 Jul 2021 02:26:17 GMT  
		Size: 3.7 MB (3670853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:372602ac4ce9a3a693cb97ec9b3e71b449fdafbaded2ce2937fec39cec9c9b6e`  
		Last Modified: Tue, 27 Jul 2021 02:26:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a80c4de70a1ded78cf0175b1f5fda38b3119857dd2d8d9f1fafcdc39eafef0e`  
		Last Modified: Tue, 27 Jul 2021 02:26:13 GMT  
		Size: 2.6 MB (2569871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc8dec87672a96e86220faa6c3e98577b2a9090fc81d81efb4681fe59e732b7`  
		Last Modified: Tue, 27 Jul 2021 02:26:12 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce893fcc2e86ea1fb70c9730683306fb99ed9b96529607badefbeb824f32081`  
		Last Modified: Mon, 09 Aug 2021 19:45:06 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea2b83ad4dfbaa9a9aa432f398880354589538421ef773a7bdc59bf41856282`  
		Last Modified: Mon, 09 Aug 2021 19:45:24 GMT  
		Size: 91.3 MB (91330692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e301a165b39ae64033fe826324cbfdf9f8e0e01fd8d20d7e69f7a8b771aa41`  
		Last Modified: Mon, 09 Aug 2021 19:45:06 GMT  
		Size: 5.6 KB (5617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10` - linux; s390x

```console
$ docker pull mariadb@sha256:f338e06fc65ca71eda1ac48527970da30cd5b3f1316fbb5974cd2ea2ffa87152
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.0 MB (126020736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12c9756f3b2fe668579749a2963c372a54db873f6e054bbf6f6ca8702b5d6d1f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:23 GMT
ADD file:979855f79ebaca36cc7878f71b2326f1cd189970fdb223b37cd64ee12d1c9a2b in / 
# Tue, 31 Aug 2021 01:42:27 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:49:44 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 31 Aug 2021 02:49:51 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:49:51 GMT
ENV GOSU_VERSION=1.13
# Tue, 31 Aug 2021 02:50:04 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 31 Aug 2021 02:50:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 31 Aug 2021 02:50:12 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:50:12 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 31 Aug 2021 02:50:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 31 Aug 2021 02:50:18 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 31 Aug 2021 02:50:18 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 31 Aug 2021 02:50:19 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Tue, 31 Aug 2021 02:50:19 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Tue, 31 Aug 2021 02:50:19 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Tue, 31 Aug 2021 02:50:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 31 Aug 2021 02:50:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 31 Aug 2021 02:50:49 GMT
VOLUME [/var/lib/mysql]
# Tue, 31 Aug 2021 02:50:49 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Tue, 31 Aug 2021 02:50:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Aug 2021 02:50:49 GMT
EXPOSE 3306
# Tue, 31 Aug 2021 02:50:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:9fbf86d355c92d30b8de4c0360b0d79e1100e392d0885b6b5b302a1c3781dbf1`  
		Last Modified: Tue, 31 Aug 2021 01:44:13 GMT  
		Size: 27.1 MB (27127470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5652d937cd93c6c333210a7c5783a5defbac72c096a74537a0e99da179e69e15`  
		Last Modified: Tue, 31 Aug 2021 02:52:15 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1b48caf1d89a34f08f8ee38f48260ccfd25cfdc0e5425a1f7e2e1c3bc1c8cf0`  
		Last Modified: Tue, 31 Aug 2021 02:52:16 GMT  
		Size: 5.4 MB (5380989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352b2892aadbd934d1a0415ca24f71baf53ef4b324fe9f8772a37405d8607dba`  
		Last Modified: Tue, 31 Aug 2021 02:52:16 GMT  
		Size: 3.2 MB (3241880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354edb6860dbb419b59714606f392488735bc5e9adc7496059e98f51de24d84a`  
		Last Modified: Tue, 31 Aug 2021 02:52:15 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9934bdf22d9a668fcaab9695424d4074294aef89d849a8c8ba80b0bb31ab2ab9`  
		Last Modified: Tue, 31 Aug 2021 02:52:13 GMT  
		Size: 2.2 MB (2186296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a940a6a2154f17326f40b9d4619aa517978b7eed0f68a8a68738928defef66`  
		Last Modified: Tue, 31 Aug 2021 02:52:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6840dfebdaf0d0162e783790b87c1c9eff72aca9dc017163baa2059ac974ec21`  
		Last Modified: Tue, 31 Aug 2021 02:52:13 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:badfbe5adb85e7a406e6d7af361229a125b295cec1d104f15f0334488fb8e38d`  
		Last Modified: Tue, 31 Aug 2021 02:52:26 GMT  
		Size: 88.1 MB (88073778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa96305d4f85828482207efa32cb56c1fcbf6bf32d41e5f7ca27f479f57acec9`  
		Last Modified: Tue, 31 Aug 2021 02:52:13 GMT  
		Size: 5.6 KB (5608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10-focal`

```console
$ docker pull mariadb@sha256:b95f3b88e2880bf1191712c122a4c5998b380c4f1afb87ab9fc1415c0ea0b9ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:2e955f90e3af94a992b3e63d34c93e875706d0ec672b18202630ded0706dde71
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.0 MB (127012840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45eaeedf03deed202dade660cbfe44ae17cac512cfd23ca2becab1cd20b5a6f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:05:00 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 27 Jul 2021 00:05:14 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:05:15 GMT
ENV GOSU_VERSION=1.13
# Tue, 27 Jul 2021 00:05:26 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 27 Jul 2021 00:05:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 27 Jul 2021 00:05:34 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:05:35 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 27 Jul 2021 00:05:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 27 Jul 2021 00:05:37 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 27 Jul 2021 00:05:37 GMT
ENV MARIADB_MAJOR=10.6
# Mon, 09 Aug 2021 19:24:13 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Mon, 09 Aug 2021 19:24:14 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Mon, 09 Aug 2021 19:24:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Mon, 09 Aug 2021 19:24:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 09 Aug 2021 19:24:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 09 Aug 2021 19:24:55 GMT
VOLUME [/var/lib/mysql]
# Mon, 09 Aug 2021 19:24:55 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Mon, 09 Aug 2021 19:24:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Aug 2021 19:24:55 GMT
EXPOSE 3306
# Mon, 09 Aug 2021 19:24:56 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf20e69555c2118df81cd7906473b0bbef5210f014d45113251b1298fb1c996`  
		Last Modified: Tue, 27 Jul 2021 00:10:02 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69afd1ffc85b8fe385e48d00e89467a4e080c81b2447ce86ebf964f3e43efb9`  
		Last Modified: Tue, 27 Jul 2021 00:10:04 GMT  
		Size: 5.5 MB (5488764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e720dc7fcd8609016e69543f354117290ffee7c9ea1bdd97d7ca84bcc06d616`  
		Last Modified: Tue, 27 Jul 2021 00:10:03 GMT  
		Size: 3.6 MB (3582379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a81d177e410065c8eec2b5c018ab6ac60b2a5161184890bc3bf7627e78fb2dd`  
		Last Modified: Tue, 27 Jul 2021 00:10:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827c8c103c898d23db5f0cfc69b6faa45038d27b1ec3c15cb5d5b29ee60fca0b`  
		Last Modified: Tue, 27 Jul 2021 00:09:59 GMT  
		Size: 2.3 MB (2274133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2108ccd013748c7fce6a19a3f7434b860401f78326ac7373c486eafa3c719354`  
		Last Modified: Tue, 27 Jul 2021 00:09:59 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05414cb5e8f4dcf16b70640f3bcf904bafddd184d3971881c10b194fb74e8a0`  
		Last Modified: Mon, 09 Aug 2021 19:27:56 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6981930106c6d6380293a728b1bda2840d2392194e1b19649b7a863e1174054`  
		Last Modified: Mon, 09 Aug 2021 19:28:09 GMT  
		Size: 87.1 MB (87089293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009b7e8d11861e3f00504f9b3ff616177ec6f4e7f14f2e0162b0f92811c73bca`  
		Last Modified: Mon, 09 Aug 2021 19:27:56 GMT  
		Size: 5.6 KB (5613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:d6a5e003eae42397f7ee4589e9f21e231d3721ac131970d2286bd616e7f55bb4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124308266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63449ffc5ac65f64a30f340aa4db0c8d502f74c51962eb9b969f08999b20604e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:44 GMT
ADD file:cec21619ecbd37b4cf8da15153b8957a343cd25c6f714e3ac3969b6003704a58 in / 
# Tue, 31 Aug 2021 01:40:45 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:04:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 31 Aug 2021 03:04:38 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:04:38 GMT
ENV GOSU_VERSION=1.13
# Tue, 31 Aug 2021 03:04:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 31 Aug 2021 03:04:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 31 Aug 2021 03:04:57 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:04:57 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 31 Aug 2021 03:05:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 31 Aug 2021 03:05:05 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 31 Aug 2021 03:05:05 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 31 Aug 2021 03:05:05 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Tue, 31 Aug 2021 03:05:05 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Tue, 31 Aug 2021 03:05:05 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Tue, 31 Aug 2021 03:05:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 31 Aug 2021 03:05:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 31 Aug 2021 03:05:28 GMT
VOLUME [/var/lib/mysql]
# Tue, 31 Aug 2021 03:05:29 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Tue, 31 Aug 2021 03:05:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Aug 2021 03:05:29 GMT
EXPOSE 3306
# Tue, 31 Aug 2021 03:05:29 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ab2d02b1ec420fdb84c9f52abda403b6aef20f5de904a2ecda5ae4f5cd6e4d46`  
		Last Modified: Tue, 31 Aug 2021 01:42:34 GMT  
		Size: 27.2 MB (27173099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d16f1b8a1bc9060d0c98a0e09c73ceab3d694a99f57672d6e44f2f5dcf09eae`  
		Last Modified: Tue, 31 Aug 2021 03:09:41 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16d8285f3be08ea7340eaf6dced5161164096c3fb3345fe8c5d6d64496bc143`  
		Last Modified: Tue, 31 Aug 2021 03:09:40 GMT  
		Size: 5.5 MB (5455084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ffd6c9eed67b115939ab5f6d4bb8ffd2f0f152fe9a61024122b558e83ce912e`  
		Last Modified: Tue, 31 Aug 2021 03:09:39 GMT  
		Size: 3.4 MB (3368457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdbc2935c20fd14d96044dcdb65fb79a0f676bcdf334058da282716411d3ff9b`  
		Last Modified: Tue, 31 Aug 2021 03:09:39 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b302bb5f11cae70b4c8ec1079e6de6c62dacfdce3e8f3ccdfabd6ce44b63d2`  
		Last Modified: Tue, 31 Aug 2021 03:09:37 GMT  
		Size: 2.2 MB (2203569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21de8a622698dffd65e882759b0b6e4fe0e56b60d892f2e4446f94439a1270f`  
		Last Modified: Tue, 31 Aug 2021 03:09:36 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9389e144f5d4ea04b6dc1760537798680338137683d9e509ac7072a5c7282d9`  
		Last Modified: Tue, 31 Aug 2021 03:09:36 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed66c3adfe54028b15ff801e6142c6ae4f65eb2bfd313aed2281deb53c447a1a`  
		Last Modified: Tue, 31 Aug 2021 03:09:51 GMT  
		Size: 86.1 MB (86097727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440559db5c8c5208fa4fd147135bce07d75b0f4a04cc838207b125cb6e4cfcbe`  
		Last Modified: Tue, 31 Aug 2021 03:09:38 GMT  
		Size: 5.6 KB (5609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:0cf82c9d58ae3326749b0fe0ed1f094d02516dba9c3e6fdf9d2c193f2fa48b4a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137540073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20c817c255cdeba976f7d5a97418f28626785a200c99e223a6450298661f4b64`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 26 Jul 2021 23:12:46 GMT
ADD file:68eb628c2202763afa91d554dde9668d8a468fe53fdbd2fe98627a5f91d224b4 in / 
# Mon, 26 Jul 2021 23:12:49 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 02:05:55 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 27 Jul 2021 02:06:47 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:06:50 GMT
ENV GOSU_VERSION=1.13
# Tue, 27 Jul 2021 02:07:32 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 27 Jul 2021 02:07:42 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 27 Jul 2021 02:08:11 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:08:14 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 27 Jul 2021 02:08:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 27 Jul 2021 02:08:24 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 27 Jul 2021 02:08:25 GMT
ENV MARIADB_MAJOR=10.6
# Mon, 09 Aug 2021 19:17:05 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Mon, 09 Aug 2021 19:17:08 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Mon, 09 Aug 2021 19:17:10 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Mon, 09 Aug 2021 19:17:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 09 Aug 2021 19:22:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 09 Aug 2021 19:22:56 GMT
VOLUME [/var/lib/mysql]
# Mon, 09 Aug 2021 19:23:00 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Mon, 09 Aug 2021 19:23:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Aug 2021 19:23:12 GMT
EXPOSE 3306
# Mon, 09 Aug 2021 19:23:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:1a396eed835b3b7b4101a9863d174e145ddbb1de1502a63bae726b0f81e7ca93`  
		Last Modified: Mon, 26 Jul 2021 23:15:51 GMT  
		Size: 33.3 MB (33290427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65be85b12a63573ebccb059357c5c0db6046f4a074454eea617c402e3bf99c1f`  
		Last Modified: Tue, 27 Jul 2021 02:26:16 GMT  
		Size: 1.8 KB (1760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:803c8e5bf0c59b9b01b70cac07bb24bc696bc577d8e74c79ff15bcbd480874b4`  
		Last Modified: Tue, 27 Jul 2021 02:26:17 GMT  
		Size: 6.7 MB (6667884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62bd7bf9c00152c4fb338b2c1a01d5b241ceda5c58d9e700a353072ab80fb4b9`  
		Last Modified: Tue, 27 Jul 2021 02:26:17 GMT  
		Size: 3.7 MB (3670853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:372602ac4ce9a3a693cb97ec9b3e71b449fdafbaded2ce2937fec39cec9c9b6e`  
		Last Modified: Tue, 27 Jul 2021 02:26:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a80c4de70a1ded78cf0175b1f5fda38b3119857dd2d8d9f1fafcdc39eafef0e`  
		Last Modified: Tue, 27 Jul 2021 02:26:13 GMT  
		Size: 2.6 MB (2569871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc8dec87672a96e86220faa6c3e98577b2a9090fc81d81efb4681fe59e732b7`  
		Last Modified: Tue, 27 Jul 2021 02:26:12 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce893fcc2e86ea1fb70c9730683306fb99ed9b96529607badefbeb824f32081`  
		Last Modified: Mon, 09 Aug 2021 19:45:06 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea2b83ad4dfbaa9a9aa432f398880354589538421ef773a7bdc59bf41856282`  
		Last Modified: Mon, 09 Aug 2021 19:45:24 GMT  
		Size: 91.3 MB (91330692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e301a165b39ae64033fe826324cbfdf9f8e0e01fd8d20d7e69f7a8b771aa41`  
		Last Modified: Mon, 09 Aug 2021 19:45:06 GMT  
		Size: 5.6 KB (5617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:f338e06fc65ca71eda1ac48527970da30cd5b3f1316fbb5974cd2ea2ffa87152
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.0 MB (126020736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12c9756f3b2fe668579749a2963c372a54db873f6e054bbf6f6ca8702b5d6d1f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:23 GMT
ADD file:979855f79ebaca36cc7878f71b2326f1cd189970fdb223b37cd64ee12d1c9a2b in / 
# Tue, 31 Aug 2021 01:42:27 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:49:44 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 31 Aug 2021 02:49:51 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:49:51 GMT
ENV GOSU_VERSION=1.13
# Tue, 31 Aug 2021 02:50:04 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 31 Aug 2021 02:50:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 31 Aug 2021 02:50:12 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:50:12 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 31 Aug 2021 02:50:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 31 Aug 2021 02:50:18 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 31 Aug 2021 02:50:18 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 31 Aug 2021 02:50:19 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Tue, 31 Aug 2021 02:50:19 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Tue, 31 Aug 2021 02:50:19 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Tue, 31 Aug 2021 02:50:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 31 Aug 2021 02:50:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 31 Aug 2021 02:50:49 GMT
VOLUME [/var/lib/mysql]
# Tue, 31 Aug 2021 02:50:49 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Tue, 31 Aug 2021 02:50:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Aug 2021 02:50:49 GMT
EXPOSE 3306
# Tue, 31 Aug 2021 02:50:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:9fbf86d355c92d30b8de4c0360b0d79e1100e392d0885b6b5b302a1c3781dbf1`  
		Last Modified: Tue, 31 Aug 2021 01:44:13 GMT  
		Size: 27.1 MB (27127470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5652d937cd93c6c333210a7c5783a5defbac72c096a74537a0e99da179e69e15`  
		Last Modified: Tue, 31 Aug 2021 02:52:15 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1b48caf1d89a34f08f8ee38f48260ccfd25cfdc0e5425a1f7e2e1c3bc1c8cf0`  
		Last Modified: Tue, 31 Aug 2021 02:52:16 GMT  
		Size: 5.4 MB (5380989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352b2892aadbd934d1a0415ca24f71baf53ef4b324fe9f8772a37405d8607dba`  
		Last Modified: Tue, 31 Aug 2021 02:52:16 GMT  
		Size: 3.2 MB (3241880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354edb6860dbb419b59714606f392488735bc5e9adc7496059e98f51de24d84a`  
		Last Modified: Tue, 31 Aug 2021 02:52:15 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9934bdf22d9a668fcaab9695424d4074294aef89d849a8c8ba80b0bb31ab2ab9`  
		Last Modified: Tue, 31 Aug 2021 02:52:13 GMT  
		Size: 2.2 MB (2186296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a940a6a2154f17326f40b9d4619aa517978b7eed0f68a8a68738928defef66`  
		Last Modified: Tue, 31 Aug 2021 02:52:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6840dfebdaf0d0162e783790b87c1c9eff72aca9dc017163baa2059ac974ec21`  
		Last Modified: Tue, 31 Aug 2021 02:52:13 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:badfbe5adb85e7a406e6d7af361229a125b295cec1d104f15f0334488fb8e38d`  
		Last Modified: Tue, 31 Aug 2021 02:52:26 GMT  
		Size: 88.1 MB (88073778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa96305d4f85828482207efa32cb56c1fcbf6bf32d41e5f7ca27f479f57acec9`  
		Last Modified: Tue, 31 Aug 2021 02:52:13 GMT  
		Size: 5.6 KB (5608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2`

```console
$ docker pull mariadb@sha256:fb98cf26c3463c6c560b4f7ac6b52cc86b4beb81d0d523a0d163387e22681907
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2` - linux; amd64

```console
$ docker pull mariadb@sha256:abd7c7416fd1b62bb216504f43a33921516dd527b36664b62355588deca9117c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.3 MB (109277614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee1f276f080220ce22db6e607f464e042570515b1b3d3ae03361db1ccef08b46`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:30 GMT
ADD file:e729fb032bd2f7cde20fb343da0cd358447e8b23028422c123944e8d0be660fa in / 
# Mon, 26 Jul 2021 21:21:31 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:08:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 27 Jul 2021 00:08:23 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:08:23 GMT
ENV GOSU_VERSION=1.13
# Tue, 27 Jul 2021 00:08:36 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 27 Jul 2021 00:08:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 27 Jul 2021 00:08:44 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:08:45 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 27 Jul 2021 00:08:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 27 Jul 2021 00:08:46 GMT
ARG MARIADB_MAJOR=10.2
# Tue, 27 Jul 2021 00:08:46 GMT
ENV MARIADB_MAJOR=10.2
# Mon, 09 Aug 2021 19:26:39 GMT
ARG MARIADB_VERSION=1:10.2.40+maria~bionic
# Mon, 09 Aug 2021 19:26:40 GMT
ENV MARIADB_VERSION=1:10.2.40+maria~bionic
# Mon, 09 Aug 2021 19:26:40 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
# Mon, 09 Aug 2021 19:26:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 09 Aug 2021 19:27:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 09 Aug 2021 19:27:25 GMT
VOLUME [/var/lib/mysql]
# Mon, 09 Aug 2021 19:27:25 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Mon, 09 Aug 2021 19:27:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 09 Aug 2021 19:27:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Aug 2021 19:27:26 GMT
EXPOSE 3306
# Mon, 09 Aug 2021 19:27:27 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:feac5306138255e28a9862d3f3d29025d0a4d0648855afe1acd6131af07138ac`  
		Last Modified: Mon, 26 Jul 2021 21:22:52 GMT  
		Size: 26.7 MB (26709039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb140a0551352f5156c6a13b36727ad0aae313be276fab6bd318c2cba256a9f0`  
		Last Modified: Tue, 27 Jul 2021 00:12:20 GMT  
		Size: 1.9 KB (1873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30512fa1a94cc2482eeaf059f79ce38aa4f603c2defe33998d85c2d2e956002b`  
		Last Modified: Tue, 27 Jul 2021 00:12:18 GMT  
		Size: 4.8 MB (4813162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e8fcc2d063d7408470485f3a8fbf38c139104bd68e1c5335c576764a8fc7ee2`  
		Last Modified: Tue, 27 Jul 2021 00:12:18 GMT  
		Size: 3.5 MB (3547372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f11911c2ef7d32010088cdd2dc674473579ec4ee07fadbd86b3590a90f284d7`  
		Last Modified: Tue, 27 Jul 2021 00:12:18 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322065849b37adce4f4b199b1fcba599346d0b3c11542c0e7e25755b25c60fbe`  
		Last Modified: Tue, 27 Jul 2021 00:12:18 GMT  
		Size: 1.6 MB (1585615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a2eef23ce3eea0a95b77bbc7682dadfc5fc39f6bcd71f22d9aba781c899b99`  
		Last Modified: Tue, 27 Jul 2021 00:12:14 GMT  
		Size: 5.0 KB (5029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac773a01d910467cf70bb984e236ad126e708ec3519e4b586812293ae08d4ae6`  
		Last Modified: Mon, 09 Aug 2021 19:30:10 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d65f8eed5d5b225f36a8055ea118e8e07196ea927073eaa6b1d60e528a2f449a`  
		Last Modified: Mon, 09 Aug 2021 19:30:21 GMT  
		Size: 72.6 MB (72609316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b998c0995447a11364efdaf1e75eeedb063453ebfcfa32bedbf59aa5cad5202`  
		Last Modified: Mon, 09 Aug 2021 19:30:10 GMT  
		Size: 5.6 KB (5612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a04801e8caea4413206f26fa6cf8b0e481fa927362eea3c834e025b36ef9fb`  
		Last Modified: Mon, 09 Aug 2021 19:30:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:3a5859934b486b3cbfd139191e3b285911d9a0e77bc4e36e7b529f261beeffa9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.4 MB (104366865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed958704c7d4e6a2fd8d3620e6204875222ffc2e86ea227cbe4b62a040405cc3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:36 GMT
ADD file:27e3c8f7785fef80f6172954da7c3c73734c02b933dc19847e888542897d568f in / 
# Tue, 31 Aug 2021 01:40:36 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:07:21 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 31 Aug 2021 03:07:31 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:07:31 GMT
ENV GOSU_VERSION=1.13
# Tue, 31 Aug 2021 03:07:45 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 31 Aug 2021 03:07:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 31 Aug 2021 03:07:53 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:07:53 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 31 Aug 2021 03:08:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 31 Aug 2021 03:08:03 GMT
ARG MARIADB_MAJOR=10.2
# Tue, 31 Aug 2021 03:08:03 GMT
ENV MARIADB_MAJOR=10.2
# Tue, 31 Aug 2021 03:08:03 GMT
ARG MARIADB_VERSION=1:10.2.40+maria~bionic
# Tue, 31 Aug 2021 03:08:03 GMT
ENV MARIADB_VERSION=1:10.2.40+maria~bionic
# Tue, 31 Aug 2021 03:08:04 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
# Tue, 31 Aug 2021 03:08:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 31 Aug 2021 03:08:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 31 Aug 2021 03:08:29 GMT
VOLUME [/var/lib/mysql]
# Tue, 31 Aug 2021 03:08:29 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Tue, 31 Aug 2021 03:08:30 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 31 Aug 2021 03:08:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Aug 2021 03:08:30 GMT
EXPOSE 3306
# Tue, 31 Aug 2021 03:08:30 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:4028d4a2ab035ee99388f4aa429a83fbaf8022de67206e9a5b69615c71069135`  
		Last Modified: Tue, 31 Aug 2021 01:42:16 GMT  
		Size: 23.7 MB (23730599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4276840cdb584f45ad146fa037b43e752db5f0c493ba463f52cb70e782f21681`  
		Last Modified: Tue, 31 Aug 2021 03:12:13 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:110e731b29a9b68e0dcf229f482358c01543f41d293b8d69244ad9127576653c`  
		Last Modified: Tue, 31 Aug 2021 03:12:12 GMT  
		Size: 4.4 MB (4395589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecd220c548aaab56b376af549595fd4687a831ee0f15b413ff7d944ca3e6bbf8`  
		Last Modified: Tue, 31 Aug 2021 03:12:11 GMT  
		Size: 3.2 MB (3206019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68bfa6ed6e88d3faebf9551531c332c38b6b1e4d36e2be424caf152f40bfd93e`  
		Last Modified: Tue, 31 Aug 2021 03:12:10 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99231b4672b58f8b6513a03608798af633a01823474c28095d2a99bc739bba36`  
		Last Modified: Tue, 31 Aug 2021 03:12:11 GMT  
		Size: 1.5 MB (1532460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf3c868b66173349cfdc8fc2523266c44235743993bd7d11ec9326727f81f7ff`  
		Last Modified: Tue, 31 Aug 2021 03:12:08 GMT  
		Size: 5.0 KB (5030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d2c818246a9e13f7bc486b03a93c21c70d3fe72aed3baba8676ddf0b12ec35`  
		Last Modified: Tue, 31 Aug 2021 03:12:08 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7ce295f342350817c1376956171c94234b7fd0829411152d15e2663a4e4e46`  
		Last Modified: Tue, 31 Aug 2021 03:12:20 GMT  
		Size: 71.5 MB (71489081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566bf65da1c571d7324602b836b4764cf6eeea3bcf350172f13dec6666904c51`  
		Last Modified: Tue, 31 Aug 2021 03:12:08 GMT  
		Size: 5.6 KB (5610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe0bab5feaf0b83a82d6b9ee7ae1095b313bed2d17ce304ffd840381f4102dbe`  
		Last Modified: Tue, 31 Aug 2021 03:12:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2` - linux; ppc64le

```console
$ docker pull mariadb@sha256:1542e68b1d26e59100b74755bff5e1f5605eb88d0315991d09906d883325aa27
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117677946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5c38b272f8f58ecaf1030ea8496fffec224ab8ee12dc2313de5c13497245459`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 26 Jul 2021 23:12:31 GMT
ADD file:2e6f05bbffb47b3ea8e5e4127452e80debc89fb9e22af2dc5c735ea579adad64 in / 
# Mon, 26 Jul 2021 23:12:34 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 02:21:01 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 27 Jul 2021 02:21:42 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:21:44 GMT
ENV GOSU_VERSION=1.13
# Tue, 27 Jul 2021 02:22:24 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 27 Jul 2021 02:22:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 27 Jul 2021 02:22:52 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:22:55 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 27 Jul 2021 02:23:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 27 Jul 2021 02:23:05 GMT
ARG MARIADB_MAJOR=10.2
# Tue, 27 Jul 2021 02:23:07 GMT
ENV MARIADB_MAJOR=10.2
# Mon, 09 Aug 2021 19:39:32 GMT
ARG MARIADB_VERSION=1:10.2.40+maria~bionic
# Mon, 09 Aug 2021 19:39:37 GMT
ENV MARIADB_VERSION=1:10.2.40+maria~bionic
# Mon, 09 Aug 2021 19:39:44 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
# Mon, 09 Aug 2021 19:40:00 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 09 Aug 2021 19:43:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 09 Aug 2021 19:43:33 GMT
VOLUME [/var/lib/mysql]
# Mon, 09 Aug 2021 19:43:36 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Mon, 09 Aug 2021 19:43:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 09 Aug 2021 19:43:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Aug 2021 19:43:54 GMT
EXPOSE 3306
# Mon, 09 Aug 2021 19:43:59 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3c742a0b2a0025420dcf1bc91d81de2ffb292328fad483ce715521d725503b66`  
		Last Modified: Mon, 26 Jul 2021 23:15:30 GMT  
		Size: 30.4 MB (30437958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:369dd90b95d5e9e1f7299ee72bcc98c621a479bdd448995a21b7d2e18ca75c6f`  
		Last Modified: Tue, 27 Jul 2021 02:29:00 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250de9da182a63a714f54597dc6306ac894ef11aaf8df9201705a0fd59942b7f`  
		Last Modified: Tue, 27 Jul 2021 02:28:59 GMT  
		Size: 5.6 MB (5630466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317de8985ff8af48122ff1378537bc7fbf84fa3bcf6d458e6a75cea28d0a1e24`  
		Last Modified: Tue, 27 Jul 2021 02:28:58 GMT  
		Size: 3.5 MB (3528921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c5ce4ef345c6df4ad4307ef718016906f4b26c1acb7357ca63c501a730c5d7`  
		Last Modified: Tue, 27 Jul 2021 02:28:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97f397676522b618a417470f1aa2e15c07db16aa22c6c549e08841baec3bc25a`  
		Last Modified: Tue, 27 Jul 2021 02:28:57 GMT  
		Size: 1.9 MB (1938720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a70d1088ca86bed51db4882db9013cc70c2d60f9008aa42e63347af965891f`  
		Last Modified: Tue, 27 Jul 2021 02:28:54 GMT  
		Size: 5.0 KB (5028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bb5820ea221765dc720a8619dc4aaf79b35eaf2861cca2a79ecb50f9d28fbbb`  
		Last Modified: Mon, 09 Aug 2021 19:47:46 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af2313bc2270fb370255337e749783b4a28f305644a4a387e28271ab6121b374`  
		Last Modified: Mon, 09 Aug 2021 19:48:01 GMT  
		Size: 76.1 MB (76128758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0546e8b3fb31277222b26c8a72f570f103b4a9a224b0df18fa18e0ecf0927ef`  
		Last Modified: Mon, 09 Aug 2021 19:47:46 GMT  
		Size: 5.6 KB (5614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c761f0aac1a9a03d5195b6aea2ccbb20186ef3fc51c6b88d534a48135be4d589`  
		Last Modified: Mon, 09 Aug 2021 19:47:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2-bionic`

```console
$ docker pull mariadb@sha256:fb98cf26c3463c6c560b4f7ac6b52cc86b4beb81d0d523a0d163387e22681907
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2-bionic` - linux; amd64

```console
$ docker pull mariadb@sha256:abd7c7416fd1b62bb216504f43a33921516dd527b36664b62355588deca9117c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.3 MB (109277614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee1f276f080220ce22db6e607f464e042570515b1b3d3ae03361db1ccef08b46`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:30 GMT
ADD file:e729fb032bd2f7cde20fb343da0cd358447e8b23028422c123944e8d0be660fa in / 
# Mon, 26 Jul 2021 21:21:31 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:08:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 27 Jul 2021 00:08:23 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:08:23 GMT
ENV GOSU_VERSION=1.13
# Tue, 27 Jul 2021 00:08:36 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 27 Jul 2021 00:08:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 27 Jul 2021 00:08:44 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:08:45 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 27 Jul 2021 00:08:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 27 Jul 2021 00:08:46 GMT
ARG MARIADB_MAJOR=10.2
# Tue, 27 Jul 2021 00:08:46 GMT
ENV MARIADB_MAJOR=10.2
# Mon, 09 Aug 2021 19:26:39 GMT
ARG MARIADB_VERSION=1:10.2.40+maria~bionic
# Mon, 09 Aug 2021 19:26:40 GMT
ENV MARIADB_VERSION=1:10.2.40+maria~bionic
# Mon, 09 Aug 2021 19:26:40 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
# Mon, 09 Aug 2021 19:26:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 09 Aug 2021 19:27:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 09 Aug 2021 19:27:25 GMT
VOLUME [/var/lib/mysql]
# Mon, 09 Aug 2021 19:27:25 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Mon, 09 Aug 2021 19:27:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 09 Aug 2021 19:27:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Aug 2021 19:27:26 GMT
EXPOSE 3306
# Mon, 09 Aug 2021 19:27:27 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:feac5306138255e28a9862d3f3d29025d0a4d0648855afe1acd6131af07138ac`  
		Last Modified: Mon, 26 Jul 2021 21:22:52 GMT  
		Size: 26.7 MB (26709039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb140a0551352f5156c6a13b36727ad0aae313be276fab6bd318c2cba256a9f0`  
		Last Modified: Tue, 27 Jul 2021 00:12:20 GMT  
		Size: 1.9 KB (1873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30512fa1a94cc2482eeaf059f79ce38aa4f603c2defe33998d85c2d2e956002b`  
		Last Modified: Tue, 27 Jul 2021 00:12:18 GMT  
		Size: 4.8 MB (4813162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e8fcc2d063d7408470485f3a8fbf38c139104bd68e1c5335c576764a8fc7ee2`  
		Last Modified: Tue, 27 Jul 2021 00:12:18 GMT  
		Size: 3.5 MB (3547372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f11911c2ef7d32010088cdd2dc674473579ec4ee07fadbd86b3590a90f284d7`  
		Last Modified: Tue, 27 Jul 2021 00:12:18 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322065849b37adce4f4b199b1fcba599346d0b3c11542c0e7e25755b25c60fbe`  
		Last Modified: Tue, 27 Jul 2021 00:12:18 GMT  
		Size: 1.6 MB (1585615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a2eef23ce3eea0a95b77bbc7682dadfc5fc39f6bcd71f22d9aba781c899b99`  
		Last Modified: Tue, 27 Jul 2021 00:12:14 GMT  
		Size: 5.0 KB (5029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac773a01d910467cf70bb984e236ad126e708ec3519e4b586812293ae08d4ae6`  
		Last Modified: Mon, 09 Aug 2021 19:30:10 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d65f8eed5d5b225f36a8055ea118e8e07196ea927073eaa6b1d60e528a2f449a`  
		Last Modified: Mon, 09 Aug 2021 19:30:21 GMT  
		Size: 72.6 MB (72609316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b998c0995447a11364efdaf1e75eeedb063453ebfcfa32bedbf59aa5cad5202`  
		Last Modified: Mon, 09 Aug 2021 19:30:10 GMT  
		Size: 5.6 KB (5612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a04801e8caea4413206f26fa6cf8b0e481fa927362eea3c834e025b36ef9fb`  
		Last Modified: Mon, 09 Aug 2021 19:30:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2-bionic` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:3a5859934b486b3cbfd139191e3b285911d9a0e77bc4e36e7b529f261beeffa9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.4 MB (104366865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed958704c7d4e6a2fd8d3620e6204875222ffc2e86ea227cbe4b62a040405cc3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:36 GMT
ADD file:27e3c8f7785fef80f6172954da7c3c73734c02b933dc19847e888542897d568f in / 
# Tue, 31 Aug 2021 01:40:36 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:07:21 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 31 Aug 2021 03:07:31 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:07:31 GMT
ENV GOSU_VERSION=1.13
# Tue, 31 Aug 2021 03:07:45 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 31 Aug 2021 03:07:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 31 Aug 2021 03:07:53 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:07:53 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 31 Aug 2021 03:08:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 31 Aug 2021 03:08:03 GMT
ARG MARIADB_MAJOR=10.2
# Tue, 31 Aug 2021 03:08:03 GMT
ENV MARIADB_MAJOR=10.2
# Tue, 31 Aug 2021 03:08:03 GMT
ARG MARIADB_VERSION=1:10.2.40+maria~bionic
# Tue, 31 Aug 2021 03:08:03 GMT
ENV MARIADB_VERSION=1:10.2.40+maria~bionic
# Tue, 31 Aug 2021 03:08:04 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
# Tue, 31 Aug 2021 03:08:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 31 Aug 2021 03:08:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 31 Aug 2021 03:08:29 GMT
VOLUME [/var/lib/mysql]
# Tue, 31 Aug 2021 03:08:29 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Tue, 31 Aug 2021 03:08:30 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 31 Aug 2021 03:08:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Aug 2021 03:08:30 GMT
EXPOSE 3306
# Tue, 31 Aug 2021 03:08:30 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:4028d4a2ab035ee99388f4aa429a83fbaf8022de67206e9a5b69615c71069135`  
		Last Modified: Tue, 31 Aug 2021 01:42:16 GMT  
		Size: 23.7 MB (23730599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4276840cdb584f45ad146fa037b43e752db5f0c493ba463f52cb70e782f21681`  
		Last Modified: Tue, 31 Aug 2021 03:12:13 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:110e731b29a9b68e0dcf229f482358c01543f41d293b8d69244ad9127576653c`  
		Last Modified: Tue, 31 Aug 2021 03:12:12 GMT  
		Size: 4.4 MB (4395589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecd220c548aaab56b376af549595fd4687a831ee0f15b413ff7d944ca3e6bbf8`  
		Last Modified: Tue, 31 Aug 2021 03:12:11 GMT  
		Size: 3.2 MB (3206019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68bfa6ed6e88d3faebf9551531c332c38b6b1e4d36e2be424caf152f40bfd93e`  
		Last Modified: Tue, 31 Aug 2021 03:12:10 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99231b4672b58f8b6513a03608798af633a01823474c28095d2a99bc739bba36`  
		Last Modified: Tue, 31 Aug 2021 03:12:11 GMT  
		Size: 1.5 MB (1532460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf3c868b66173349cfdc8fc2523266c44235743993bd7d11ec9326727f81f7ff`  
		Last Modified: Tue, 31 Aug 2021 03:12:08 GMT  
		Size: 5.0 KB (5030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d2c818246a9e13f7bc486b03a93c21c70d3fe72aed3baba8676ddf0b12ec35`  
		Last Modified: Tue, 31 Aug 2021 03:12:08 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7ce295f342350817c1376956171c94234b7fd0829411152d15e2663a4e4e46`  
		Last Modified: Tue, 31 Aug 2021 03:12:20 GMT  
		Size: 71.5 MB (71489081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566bf65da1c571d7324602b836b4764cf6eeea3bcf350172f13dec6666904c51`  
		Last Modified: Tue, 31 Aug 2021 03:12:08 GMT  
		Size: 5.6 KB (5610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe0bab5feaf0b83a82d6b9ee7ae1095b313bed2d17ce304ffd840381f4102dbe`  
		Last Modified: Tue, 31 Aug 2021 03:12:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2-bionic` - linux; ppc64le

```console
$ docker pull mariadb@sha256:1542e68b1d26e59100b74755bff5e1f5605eb88d0315991d09906d883325aa27
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117677946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5c38b272f8f58ecaf1030ea8496fffec224ab8ee12dc2313de5c13497245459`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 26 Jul 2021 23:12:31 GMT
ADD file:2e6f05bbffb47b3ea8e5e4127452e80debc89fb9e22af2dc5c735ea579adad64 in / 
# Mon, 26 Jul 2021 23:12:34 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 02:21:01 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 27 Jul 2021 02:21:42 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:21:44 GMT
ENV GOSU_VERSION=1.13
# Tue, 27 Jul 2021 02:22:24 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 27 Jul 2021 02:22:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 27 Jul 2021 02:22:52 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:22:55 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 27 Jul 2021 02:23:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 27 Jul 2021 02:23:05 GMT
ARG MARIADB_MAJOR=10.2
# Tue, 27 Jul 2021 02:23:07 GMT
ENV MARIADB_MAJOR=10.2
# Mon, 09 Aug 2021 19:39:32 GMT
ARG MARIADB_VERSION=1:10.2.40+maria~bionic
# Mon, 09 Aug 2021 19:39:37 GMT
ENV MARIADB_VERSION=1:10.2.40+maria~bionic
# Mon, 09 Aug 2021 19:39:44 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
# Mon, 09 Aug 2021 19:40:00 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 09 Aug 2021 19:43:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 09 Aug 2021 19:43:33 GMT
VOLUME [/var/lib/mysql]
# Mon, 09 Aug 2021 19:43:36 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Mon, 09 Aug 2021 19:43:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 09 Aug 2021 19:43:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Aug 2021 19:43:54 GMT
EXPOSE 3306
# Mon, 09 Aug 2021 19:43:59 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3c742a0b2a0025420dcf1bc91d81de2ffb292328fad483ce715521d725503b66`  
		Last Modified: Mon, 26 Jul 2021 23:15:30 GMT  
		Size: 30.4 MB (30437958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:369dd90b95d5e9e1f7299ee72bcc98c621a479bdd448995a21b7d2e18ca75c6f`  
		Last Modified: Tue, 27 Jul 2021 02:29:00 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250de9da182a63a714f54597dc6306ac894ef11aaf8df9201705a0fd59942b7f`  
		Last Modified: Tue, 27 Jul 2021 02:28:59 GMT  
		Size: 5.6 MB (5630466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317de8985ff8af48122ff1378537bc7fbf84fa3bcf6d458e6a75cea28d0a1e24`  
		Last Modified: Tue, 27 Jul 2021 02:28:58 GMT  
		Size: 3.5 MB (3528921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c5ce4ef345c6df4ad4307ef718016906f4b26c1acb7357ca63c501a730c5d7`  
		Last Modified: Tue, 27 Jul 2021 02:28:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97f397676522b618a417470f1aa2e15c07db16aa22c6c549e08841baec3bc25a`  
		Last Modified: Tue, 27 Jul 2021 02:28:57 GMT  
		Size: 1.9 MB (1938720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a70d1088ca86bed51db4882db9013cc70c2d60f9008aa42e63347af965891f`  
		Last Modified: Tue, 27 Jul 2021 02:28:54 GMT  
		Size: 5.0 KB (5028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bb5820ea221765dc720a8619dc4aaf79b35eaf2861cca2a79ecb50f9d28fbbb`  
		Last Modified: Mon, 09 Aug 2021 19:47:46 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af2313bc2270fb370255337e749783b4a28f305644a4a387e28271ab6121b374`  
		Last Modified: Mon, 09 Aug 2021 19:48:01 GMT  
		Size: 76.1 MB (76128758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0546e8b3fb31277222b26c8a72f570f103b4a9a224b0df18fa18e0ecf0927ef`  
		Last Modified: Mon, 09 Aug 2021 19:47:46 GMT  
		Size: 5.6 KB (5614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c761f0aac1a9a03d5195b6aea2ccbb20186ef3fc51c6b88d534a48135be4d589`  
		Last Modified: Mon, 09 Aug 2021 19:47:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2.40`

```console
$ docker pull mariadb@sha256:fb98cf26c3463c6c560b4f7ac6b52cc86b4beb81d0d523a0d163387e22681907
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2.40` - linux; amd64

```console
$ docker pull mariadb@sha256:abd7c7416fd1b62bb216504f43a33921516dd527b36664b62355588deca9117c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.3 MB (109277614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee1f276f080220ce22db6e607f464e042570515b1b3d3ae03361db1ccef08b46`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:30 GMT
ADD file:e729fb032bd2f7cde20fb343da0cd358447e8b23028422c123944e8d0be660fa in / 
# Mon, 26 Jul 2021 21:21:31 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:08:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 27 Jul 2021 00:08:23 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:08:23 GMT
ENV GOSU_VERSION=1.13
# Tue, 27 Jul 2021 00:08:36 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 27 Jul 2021 00:08:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 27 Jul 2021 00:08:44 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:08:45 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 27 Jul 2021 00:08:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 27 Jul 2021 00:08:46 GMT
ARG MARIADB_MAJOR=10.2
# Tue, 27 Jul 2021 00:08:46 GMT
ENV MARIADB_MAJOR=10.2
# Mon, 09 Aug 2021 19:26:39 GMT
ARG MARIADB_VERSION=1:10.2.40+maria~bionic
# Mon, 09 Aug 2021 19:26:40 GMT
ENV MARIADB_VERSION=1:10.2.40+maria~bionic
# Mon, 09 Aug 2021 19:26:40 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
# Mon, 09 Aug 2021 19:26:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 09 Aug 2021 19:27:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 09 Aug 2021 19:27:25 GMT
VOLUME [/var/lib/mysql]
# Mon, 09 Aug 2021 19:27:25 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Mon, 09 Aug 2021 19:27:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 09 Aug 2021 19:27:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Aug 2021 19:27:26 GMT
EXPOSE 3306
# Mon, 09 Aug 2021 19:27:27 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:feac5306138255e28a9862d3f3d29025d0a4d0648855afe1acd6131af07138ac`  
		Last Modified: Mon, 26 Jul 2021 21:22:52 GMT  
		Size: 26.7 MB (26709039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb140a0551352f5156c6a13b36727ad0aae313be276fab6bd318c2cba256a9f0`  
		Last Modified: Tue, 27 Jul 2021 00:12:20 GMT  
		Size: 1.9 KB (1873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30512fa1a94cc2482eeaf059f79ce38aa4f603c2defe33998d85c2d2e956002b`  
		Last Modified: Tue, 27 Jul 2021 00:12:18 GMT  
		Size: 4.8 MB (4813162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e8fcc2d063d7408470485f3a8fbf38c139104bd68e1c5335c576764a8fc7ee2`  
		Last Modified: Tue, 27 Jul 2021 00:12:18 GMT  
		Size: 3.5 MB (3547372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f11911c2ef7d32010088cdd2dc674473579ec4ee07fadbd86b3590a90f284d7`  
		Last Modified: Tue, 27 Jul 2021 00:12:18 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322065849b37adce4f4b199b1fcba599346d0b3c11542c0e7e25755b25c60fbe`  
		Last Modified: Tue, 27 Jul 2021 00:12:18 GMT  
		Size: 1.6 MB (1585615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a2eef23ce3eea0a95b77bbc7682dadfc5fc39f6bcd71f22d9aba781c899b99`  
		Last Modified: Tue, 27 Jul 2021 00:12:14 GMT  
		Size: 5.0 KB (5029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac773a01d910467cf70bb984e236ad126e708ec3519e4b586812293ae08d4ae6`  
		Last Modified: Mon, 09 Aug 2021 19:30:10 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d65f8eed5d5b225f36a8055ea118e8e07196ea927073eaa6b1d60e528a2f449a`  
		Last Modified: Mon, 09 Aug 2021 19:30:21 GMT  
		Size: 72.6 MB (72609316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b998c0995447a11364efdaf1e75eeedb063453ebfcfa32bedbf59aa5cad5202`  
		Last Modified: Mon, 09 Aug 2021 19:30:10 GMT  
		Size: 5.6 KB (5612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a04801e8caea4413206f26fa6cf8b0e481fa927362eea3c834e025b36ef9fb`  
		Last Modified: Mon, 09 Aug 2021 19:30:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2.40` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:3a5859934b486b3cbfd139191e3b285911d9a0e77bc4e36e7b529f261beeffa9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.4 MB (104366865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed958704c7d4e6a2fd8d3620e6204875222ffc2e86ea227cbe4b62a040405cc3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:36 GMT
ADD file:27e3c8f7785fef80f6172954da7c3c73734c02b933dc19847e888542897d568f in / 
# Tue, 31 Aug 2021 01:40:36 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:07:21 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 31 Aug 2021 03:07:31 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:07:31 GMT
ENV GOSU_VERSION=1.13
# Tue, 31 Aug 2021 03:07:45 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 31 Aug 2021 03:07:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 31 Aug 2021 03:07:53 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:07:53 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 31 Aug 2021 03:08:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 31 Aug 2021 03:08:03 GMT
ARG MARIADB_MAJOR=10.2
# Tue, 31 Aug 2021 03:08:03 GMT
ENV MARIADB_MAJOR=10.2
# Tue, 31 Aug 2021 03:08:03 GMT
ARG MARIADB_VERSION=1:10.2.40+maria~bionic
# Tue, 31 Aug 2021 03:08:03 GMT
ENV MARIADB_VERSION=1:10.2.40+maria~bionic
# Tue, 31 Aug 2021 03:08:04 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
# Tue, 31 Aug 2021 03:08:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 31 Aug 2021 03:08:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 31 Aug 2021 03:08:29 GMT
VOLUME [/var/lib/mysql]
# Tue, 31 Aug 2021 03:08:29 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Tue, 31 Aug 2021 03:08:30 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 31 Aug 2021 03:08:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Aug 2021 03:08:30 GMT
EXPOSE 3306
# Tue, 31 Aug 2021 03:08:30 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:4028d4a2ab035ee99388f4aa429a83fbaf8022de67206e9a5b69615c71069135`  
		Last Modified: Tue, 31 Aug 2021 01:42:16 GMT  
		Size: 23.7 MB (23730599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4276840cdb584f45ad146fa037b43e752db5f0c493ba463f52cb70e782f21681`  
		Last Modified: Tue, 31 Aug 2021 03:12:13 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:110e731b29a9b68e0dcf229f482358c01543f41d293b8d69244ad9127576653c`  
		Last Modified: Tue, 31 Aug 2021 03:12:12 GMT  
		Size: 4.4 MB (4395589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecd220c548aaab56b376af549595fd4687a831ee0f15b413ff7d944ca3e6bbf8`  
		Last Modified: Tue, 31 Aug 2021 03:12:11 GMT  
		Size: 3.2 MB (3206019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68bfa6ed6e88d3faebf9551531c332c38b6b1e4d36e2be424caf152f40bfd93e`  
		Last Modified: Tue, 31 Aug 2021 03:12:10 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99231b4672b58f8b6513a03608798af633a01823474c28095d2a99bc739bba36`  
		Last Modified: Tue, 31 Aug 2021 03:12:11 GMT  
		Size: 1.5 MB (1532460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf3c868b66173349cfdc8fc2523266c44235743993bd7d11ec9326727f81f7ff`  
		Last Modified: Tue, 31 Aug 2021 03:12:08 GMT  
		Size: 5.0 KB (5030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d2c818246a9e13f7bc486b03a93c21c70d3fe72aed3baba8676ddf0b12ec35`  
		Last Modified: Tue, 31 Aug 2021 03:12:08 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7ce295f342350817c1376956171c94234b7fd0829411152d15e2663a4e4e46`  
		Last Modified: Tue, 31 Aug 2021 03:12:20 GMT  
		Size: 71.5 MB (71489081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566bf65da1c571d7324602b836b4764cf6eeea3bcf350172f13dec6666904c51`  
		Last Modified: Tue, 31 Aug 2021 03:12:08 GMT  
		Size: 5.6 KB (5610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe0bab5feaf0b83a82d6b9ee7ae1095b313bed2d17ce304ffd840381f4102dbe`  
		Last Modified: Tue, 31 Aug 2021 03:12:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2.40` - linux; ppc64le

```console
$ docker pull mariadb@sha256:1542e68b1d26e59100b74755bff5e1f5605eb88d0315991d09906d883325aa27
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117677946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5c38b272f8f58ecaf1030ea8496fffec224ab8ee12dc2313de5c13497245459`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 26 Jul 2021 23:12:31 GMT
ADD file:2e6f05bbffb47b3ea8e5e4127452e80debc89fb9e22af2dc5c735ea579adad64 in / 
# Mon, 26 Jul 2021 23:12:34 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 02:21:01 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 27 Jul 2021 02:21:42 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:21:44 GMT
ENV GOSU_VERSION=1.13
# Tue, 27 Jul 2021 02:22:24 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 27 Jul 2021 02:22:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 27 Jul 2021 02:22:52 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:22:55 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 27 Jul 2021 02:23:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 27 Jul 2021 02:23:05 GMT
ARG MARIADB_MAJOR=10.2
# Tue, 27 Jul 2021 02:23:07 GMT
ENV MARIADB_MAJOR=10.2
# Mon, 09 Aug 2021 19:39:32 GMT
ARG MARIADB_VERSION=1:10.2.40+maria~bionic
# Mon, 09 Aug 2021 19:39:37 GMT
ENV MARIADB_VERSION=1:10.2.40+maria~bionic
# Mon, 09 Aug 2021 19:39:44 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
# Mon, 09 Aug 2021 19:40:00 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 09 Aug 2021 19:43:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 09 Aug 2021 19:43:33 GMT
VOLUME [/var/lib/mysql]
# Mon, 09 Aug 2021 19:43:36 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Mon, 09 Aug 2021 19:43:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 09 Aug 2021 19:43:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Aug 2021 19:43:54 GMT
EXPOSE 3306
# Mon, 09 Aug 2021 19:43:59 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3c742a0b2a0025420dcf1bc91d81de2ffb292328fad483ce715521d725503b66`  
		Last Modified: Mon, 26 Jul 2021 23:15:30 GMT  
		Size: 30.4 MB (30437958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:369dd90b95d5e9e1f7299ee72bcc98c621a479bdd448995a21b7d2e18ca75c6f`  
		Last Modified: Tue, 27 Jul 2021 02:29:00 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250de9da182a63a714f54597dc6306ac894ef11aaf8df9201705a0fd59942b7f`  
		Last Modified: Tue, 27 Jul 2021 02:28:59 GMT  
		Size: 5.6 MB (5630466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317de8985ff8af48122ff1378537bc7fbf84fa3bcf6d458e6a75cea28d0a1e24`  
		Last Modified: Tue, 27 Jul 2021 02:28:58 GMT  
		Size: 3.5 MB (3528921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c5ce4ef345c6df4ad4307ef718016906f4b26c1acb7357ca63c501a730c5d7`  
		Last Modified: Tue, 27 Jul 2021 02:28:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97f397676522b618a417470f1aa2e15c07db16aa22c6c549e08841baec3bc25a`  
		Last Modified: Tue, 27 Jul 2021 02:28:57 GMT  
		Size: 1.9 MB (1938720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a70d1088ca86bed51db4882db9013cc70c2d60f9008aa42e63347af965891f`  
		Last Modified: Tue, 27 Jul 2021 02:28:54 GMT  
		Size: 5.0 KB (5028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bb5820ea221765dc720a8619dc4aaf79b35eaf2861cca2a79ecb50f9d28fbbb`  
		Last Modified: Mon, 09 Aug 2021 19:47:46 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af2313bc2270fb370255337e749783b4a28f305644a4a387e28271ab6121b374`  
		Last Modified: Mon, 09 Aug 2021 19:48:01 GMT  
		Size: 76.1 MB (76128758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0546e8b3fb31277222b26c8a72f570f103b4a9a224b0df18fa18e0ecf0927ef`  
		Last Modified: Mon, 09 Aug 2021 19:47:46 GMT  
		Size: 5.6 KB (5614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c761f0aac1a9a03d5195b6aea2ccbb20186ef3fc51c6b88d534a48135be4d589`  
		Last Modified: Mon, 09 Aug 2021 19:47:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2.40-bionic`

```console
$ docker pull mariadb@sha256:fb98cf26c3463c6c560b4f7ac6b52cc86b4beb81d0d523a0d163387e22681907
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2.40-bionic` - linux; amd64

```console
$ docker pull mariadb@sha256:abd7c7416fd1b62bb216504f43a33921516dd527b36664b62355588deca9117c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.3 MB (109277614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee1f276f080220ce22db6e607f464e042570515b1b3d3ae03361db1ccef08b46`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:30 GMT
ADD file:e729fb032bd2f7cde20fb343da0cd358447e8b23028422c123944e8d0be660fa in / 
# Mon, 26 Jul 2021 21:21:31 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:08:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 27 Jul 2021 00:08:23 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:08:23 GMT
ENV GOSU_VERSION=1.13
# Tue, 27 Jul 2021 00:08:36 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 27 Jul 2021 00:08:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 27 Jul 2021 00:08:44 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:08:45 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 27 Jul 2021 00:08:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 27 Jul 2021 00:08:46 GMT
ARG MARIADB_MAJOR=10.2
# Tue, 27 Jul 2021 00:08:46 GMT
ENV MARIADB_MAJOR=10.2
# Mon, 09 Aug 2021 19:26:39 GMT
ARG MARIADB_VERSION=1:10.2.40+maria~bionic
# Mon, 09 Aug 2021 19:26:40 GMT
ENV MARIADB_VERSION=1:10.2.40+maria~bionic
# Mon, 09 Aug 2021 19:26:40 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
# Mon, 09 Aug 2021 19:26:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 09 Aug 2021 19:27:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 09 Aug 2021 19:27:25 GMT
VOLUME [/var/lib/mysql]
# Mon, 09 Aug 2021 19:27:25 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Mon, 09 Aug 2021 19:27:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 09 Aug 2021 19:27:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Aug 2021 19:27:26 GMT
EXPOSE 3306
# Mon, 09 Aug 2021 19:27:27 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:feac5306138255e28a9862d3f3d29025d0a4d0648855afe1acd6131af07138ac`  
		Last Modified: Mon, 26 Jul 2021 21:22:52 GMT  
		Size: 26.7 MB (26709039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb140a0551352f5156c6a13b36727ad0aae313be276fab6bd318c2cba256a9f0`  
		Last Modified: Tue, 27 Jul 2021 00:12:20 GMT  
		Size: 1.9 KB (1873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30512fa1a94cc2482eeaf059f79ce38aa4f603c2defe33998d85c2d2e956002b`  
		Last Modified: Tue, 27 Jul 2021 00:12:18 GMT  
		Size: 4.8 MB (4813162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e8fcc2d063d7408470485f3a8fbf38c139104bd68e1c5335c576764a8fc7ee2`  
		Last Modified: Tue, 27 Jul 2021 00:12:18 GMT  
		Size: 3.5 MB (3547372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f11911c2ef7d32010088cdd2dc674473579ec4ee07fadbd86b3590a90f284d7`  
		Last Modified: Tue, 27 Jul 2021 00:12:18 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322065849b37adce4f4b199b1fcba599346d0b3c11542c0e7e25755b25c60fbe`  
		Last Modified: Tue, 27 Jul 2021 00:12:18 GMT  
		Size: 1.6 MB (1585615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a2eef23ce3eea0a95b77bbc7682dadfc5fc39f6bcd71f22d9aba781c899b99`  
		Last Modified: Tue, 27 Jul 2021 00:12:14 GMT  
		Size: 5.0 KB (5029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac773a01d910467cf70bb984e236ad126e708ec3519e4b586812293ae08d4ae6`  
		Last Modified: Mon, 09 Aug 2021 19:30:10 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d65f8eed5d5b225f36a8055ea118e8e07196ea927073eaa6b1d60e528a2f449a`  
		Last Modified: Mon, 09 Aug 2021 19:30:21 GMT  
		Size: 72.6 MB (72609316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b998c0995447a11364efdaf1e75eeedb063453ebfcfa32bedbf59aa5cad5202`  
		Last Modified: Mon, 09 Aug 2021 19:30:10 GMT  
		Size: 5.6 KB (5612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a04801e8caea4413206f26fa6cf8b0e481fa927362eea3c834e025b36ef9fb`  
		Last Modified: Mon, 09 Aug 2021 19:30:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2.40-bionic` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:3a5859934b486b3cbfd139191e3b285911d9a0e77bc4e36e7b529f261beeffa9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.4 MB (104366865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed958704c7d4e6a2fd8d3620e6204875222ffc2e86ea227cbe4b62a040405cc3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:36 GMT
ADD file:27e3c8f7785fef80f6172954da7c3c73734c02b933dc19847e888542897d568f in / 
# Tue, 31 Aug 2021 01:40:36 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:07:21 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 31 Aug 2021 03:07:31 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:07:31 GMT
ENV GOSU_VERSION=1.13
# Tue, 31 Aug 2021 03:07:45 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 31 Aug 2021 03:07:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 31 Aug 2021 03:07:53 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:07:53 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 31 Aug 2021 03:08:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 31 Aug 2021 03:08:03 GMT
ARG MARIADB_MAJOR=10.2
# Tue, 31 Aug 2021 03:08:03 GMT
ENV MARIADB_MAJOR=10.2
# Tue, 31 Aug 2021 03:08:03 GMT
ARG MARIADB_VERSION=1:10.2.40+maria~bionic
# Tue, 31 Aug 2021 03:08:03 GMT
ENV MARIADB_VERSION=1:10.2.40+maria~bionic
# Tue, 31 Aug 2021 03:08:04 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
# Tue, 31 Aug 2021 03:08:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 31 Aug 2021 03:08:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 31 Aug 2021 03:08:29 GMT
VOLUME [/var/lib/mysql]
# Tue, 31 Aug 2021 03:08:29 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Tue, 31 Aug 2021 03:08:30 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 31 Aug 2021 03:08:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Aug 2021 03:08:30 GMT
EXPOSE 3306
# Tue, 31 Aug 2021 03:08:30 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:4028d4a2ab035ee99388f4aa429a83fbaf8022de67206e9a5b69615c71069135`  
		Last Modified: Tue, 31 Aug 2021 01:42:16 GMT  
		Size: 23.7 MB (23730599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4276840cdb584f45ad146fa037b43e752db5f0c493ba463f52cb70e782f21681`  
		Last Modified: Tue, 31 Aug 2021 03:12:13 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:110e731b29a9b68e0dcf229f482358c01543f41d293b8d69244ad9127576653c`  
		Last Modified: Tue, 31 Aug 2021 03:12:12 GMT  
		Size: 4.4 MB (4395589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecd220c548aaab56b376af549595fd4687a831ee0f15b413ff7d944ca3e6bbf8`  
		Last Modified: Tue, 31 Aug 2021 03:12:11 GMT  
		Size: 3.2 MB (3206019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68bfa6ed6e88d3faebf9551531c332c38b6b1e4d36e2be424caf152f40bfd93e`  
		Last Modified: Tue, 31 Aug 2021 03:12:10 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99231b4672b58f8b6513a03608798af633a01823474c28095d2a99bc739bba36`  
		Last Modified: Tue, 31 Aug 2021 03:12:11 GMT  
		Size: 1.5 MB (1532460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf3c868b66173349cfdc8fc2523266c44235743993bd7d11ec9326727f81f7ff`  
		Last Modified: Tue, 31 Aug 2021 03:12:08 GMT  
		Size: 5.0 KB (5030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d2c818246a9e13f7bc486b03a93c21c70d3fe72aed3baba8676ddf0b12ec35`  
		Last Modified: Tue, 31 Aug 2021 03:12:08 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7ce295f342350817c1376956171c94234b7fd0829411152d15e2663a4e4e46`  
		Last Modified: Tue, 31 Aug 2021 03:12:20 GMT  
		Size: 71.5 MB (71489081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566bf65da1c571d7324602b836b4764cf6eeea3bcf350172f13dec6666904c51`  
		Last Modified: Tue, 31 Aug 2021 03:12:08 GMT  
		Size: 5.6 KB (5610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe0bab5feaf0b83a82d6b9ee7ae1095b313bed2d17ce304ffd840381f4102dbe`  
		Last Modified: Tue, 31 Aug 2021 03:12:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2.40-bionic` - linux; ppc64le

```console
$ docker pull mariadb@sha256:1542e68b1d26e59100b74755bff5e1f5605eb88d0315991d09906d883325aa27
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117677946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5c38b272f8f58ecaf1030ea8496fffec224ab8ee12dc2313de5c13497245459`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 26 Jul 2021 23:12:31 GMT
ADD file:2e6f05bbffb47b3ea8e5e4127452e80debc89fb9e22af2dc5c735ea579adad64 in / 
# Mon, 26 Jul 2021 23:12:34 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 02:21:01 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 27 Jul 2021 02:21:42 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:21:44 GMT
ENV GOSU_VERSION=1.13
# Tue, 27 Jul 2021 02:22:24 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 27 Jul 2021 02:22:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 27 Jul 2021 02:22:52 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:22:55 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 27 Jul 2021 02:23:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 27 Jul 2021 02:23:05 GMT
ARG MARIADB_MAJOR=10.2
# Tue, 27 Jul 2021 02:23:07 GMT
ENV MARIADB_MAJOR=10.2
# Mon, 09 Aug 2021 19:39:32 GMT
ARG MARIADB_VERSION=1:10.2.40+maria~bionic
# Mon, 09 Aug 2021 19:39:37 GMT
ENV MARIADB_VERSION=1:10.2.40+maria~bionic
# Mon, 09 Aug 2021 19:39:44 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
# Mon, 09 Aug 2021 19:40:00 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 09 Aug 2021 19:43:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 09 Aug 2021 19:43:33 GMT
VOLUME [/var/lib/mysql]
# Mon, 09 Aug 2021 19:43:36 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Mon, 09 Aug 2021 19:43:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 09 Aug 2021 19:43:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Aug 2021 19:43:54 GMT
EXPOSE 3306
# Mon, 09 Aug 2021 19:43:59 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3c742a0b2a0025420dcf1bc91d81de2ffb292328fad483ce715521d725503b66`  
		Last Modified: Mon, 26 Jul 2021 23:15:30 GMT  
		Size: 30.4 MB (30437958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:369dd90b95d5e9e1f7299ee72bcc98c621a479bdd448995a21b7d2e18ca75c6f`  
		Last Modified: Tue, 27 Jul 2021 02:29:00 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250de9da182a63a714f54597dc6306ac894ef11aaf8df9201705a0fd59942b7f`  
		Last Modified: Tue, 27 Jul 2021 02:28:59 GMT  
		Size: 5.6 MB (5630466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317de8985ff8af48122ff1378537bc7fbf84fa3bcf6d458e6a75cea28d0a1e24`  
		Last Modified: Tue, 27 Jul 2021 02:28:58 GMT  
		Size: 3.5 MB (3528921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c5ce4ef345c6df4ad4307ef718016906f4b26c1acb7357ca63c501a730c5d7`  
		Last Modified: Tue, 27 Jul 2021 02:28:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97f397676522b618a417470f1aa2e15c07db16aa22c6c549e08841baec3bc25a`  
		Last Modified: Tue, 27 Jul 2021 02:28:57 GMT  
		Size: 1.9 MB (1938720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a70d1088ca86bed51db4882db9013cc70c2d60f9008aa42e63347af965891f`  
		Last Modified: Tue, 27 Jul 2021 02:28:54 GMT  
		Size: 5.0 KB (5028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bb5820ea221765dc720a8619dc4aaf79b35eaf2861cca2a79ecb50f9d28fbbb`  
		Last Modified: Mon, 09 Aug 2021 19:47:46 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af2313bc2270fb370255337e749783b4a28f305644a4a387e28271ab6121b374`  
		Last Modified: Mon, 09 Aug 2021 19:48:01 GMT  
		Size: 76.1 MB (76128758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0546e8b3fb31277222b26c8a72f570f103b4a9a224b0df18fa18e0ecf0927ef`  
		Last Modified: Mon, 09 Aug 2021 19:47:46 GMT  
		Size: 5.6 KB (5614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c761f0aac1a9a03d5195b6aea2ccbb20186ef3fc51c6b88d534a48135be4d589`  
		Last Modified: Mon, 09 Aug 2021 19:47:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3`

```console
$ docker pull mariadb@sha256:6cd37e22c049027eb83c8070cdc6f3df8c769aab00af40bcf1679c8391c095ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3` - linux; amd64

```console
$ docker pull mariadb@sha256:1ab45fcbf5231f9f3527e2c57e0c6a57e0ee0e12dc37373f2b57aece0d9e0807
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.0 MB (120014376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2c8dae1f6f5606d625fe0e3aaa1f8791e4d00674bf05c0cd907e7565d3c5403`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:05:00 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 27 Jul 2021 00:05:14 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:05:15 GMT
ENV GOSU_VERSION=1.13
# Tue, 27 Jul 2021 00:05:26 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 27 Jul 2021 00:05:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 27 Jul 2021 00:05:34 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:05:35 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 27 Jul 2021 00:05:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 27 Jul 2021 00:07:32 GMT
ARG MARIADB_MAJOR=10.3
# Tue, 27 Jul 2021 00:07:32 GMT
ENV MARIADB_MAJOR=10.3
# Mon, 09 Aug 2021 19:26:04 GMT
ARG MARIADB_VERSION=1:10.3.31+maria~focal
# Mon, 09 Aug 2021 19:26:04 GMT
ENV MARIADB_VERSION=1:10.3.31+maria~focal
# Mon, 09 Aug 2021 19:26:04 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
# Mon, 09 Aug 2021 19:26:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 09 Aug 2021 19:26:31 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 09 Aug 2021 19:26:31 GMT
VOLUME [/var/lib/mysql]
# Mon, 09 Aug 2021 19:26:31 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Mon, 09 Aug 2021 19:26:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 09 Aug 2021 19:26:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Aug 2021 19:26:32 GMT
EXPOSE 3306
# Mon, 09 Aug 2021 19:26:32 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf20e69555c2118df81cd7906473b0bbef5210f014d45113251b1298fb1c996`  
		Last Modified: Tue, 27 Jul 2021 00:10:02 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69afd1ffc85b8fe385e48d00e89467a4e080c81b2447ce86ebf964f3e43efb9`  
		Last Modified: Tue, 27 Jul 2021 00:10:04 GMT  
		Size: 5.5 MB (5488764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e720dc7fcd8609016e69543f354117290ffee7c9ea1bdd97d7ca84bcc06d616`  
		Last Modified: Tue, 27 Jul 2021 00:10:03 GMT  
		Size: 3.6 MB (3582379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a81d177e410065c8eec2b5c018ab6ac60b2a5161184890bc3bf7627e78fb2dd`  
		Last Modified: Tue, 27 Jul 2021 00:10:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827c8c103c898d23db5f0cfc69b6faa45038d27b1ec3c15cb5d5b29ee60fca0b`  
		Last Modified: Tue, 27 Jul 2021 00:09:59 GMT  
		Size: 2.3 MB (2274133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2108ccd013748c7fce6a19a3f7434b860401f78326ac7373c486eafa3c719354`  
		Last Modified: Tue, 27 Jul 2021 00:09:59 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8900c3d54d69bc9fab7b747feb0a470376a1a346e1ba78752ead65506d06f33f`  
		Last Modified: Mon, 09 Aug 2021 19:29:42 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496d3f780dd791eb10b78b4b0376c3afed298ac67dc52262a1278dabfc1d318f`  
		Last Modified: Mon, 09 Aug 2021 19:29:54 GMT  
		Size: 80.1 MB (80090705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77805c057f07ba4de9b922b741a8b078369c3e440e1fa4b80d1c645510e6df66`  
		Last Modified: Mon, 09 Aug 2021 19:29:42 GMT  
		Size: 5.6 KB (5613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3fa47ecdca663b37feca04369ec700446cb994ecc1d7d09c6436613e0c34ce9`  
		Last Modified: Mon, 09 Aug 2021 19:29:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:86cb5b855f40bbdbc56f3e4e9a207f8e7be3c0020d8facad8b781b2288767132
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117624368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23b1ae977ba9883f9e1eabf5adb70757edf5179897714cf603dc7dcbd31fbf13`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:44 GMT
ADD file:cec21619ecbd37b4cf8da15153b8957a343cd25c6f714e3ac3969b6003704a58 in / 
# Tue, 31 Aug 2021 01:40:45 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:04:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 31 Aug 2021 03:04:38 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:04:38 GMT
ENV GOSU_VERSION=1.13
# Tue, 31 Aug 2021 03:04:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 31 Aug 2021 03:04:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 31 Aug 2021 03:04:57 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:04:57 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 31 Aug 2021 03:05:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 31 Aug 2021 03:06:44 GMT
ARG MARIADB_MAJOR=10.3
# Tue, 31 Aug 2021 03:06:44 GMT
ENV MARIADB_MAJOR=10.3
# Tue, 31 Aug 2021 03:06:44 GMT
ARG MARIADB_VERSION=1:10.3.31+maria~focal
# Tue, 31 Aug 2021 03:06:44 GMT
ENV MARIADB_VERSION=1:10.3.31+maria~focal
# Tue, 31 Aug 2021 03:06:45 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
# Tue, 31 Aug 2021 03:06:45 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 31 Aug 2021 03:07:10 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 31 Aug 2021 03:07:11 GMT
VOLUME [/var/lib/mysql]
# Tue, 31 Aug 2021 03:07:11 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Tue, 31 Aug 2021 03:07:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 31 Aug 2021 03:07:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Aug 2021 03:07:12 GMT
EXPOSE 3306
# Tue, 31 Aug 2021 03:07:12 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ab2d02b1ec420fdb84c9f52abda403b6aef20f5de904a2ecda5ae4f5cd6e4d46`  
		Last Modified: Tue, 31 Aug 2021 01:42:34 GMT  
		Size: 27.2 MB (27173099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d16f1b8a1bc9060d0c98a0e09c73ceab3d694a99f57672d6e44f2f5dcf09eae`  
		Last Modified: Tue, 31 Aug 2021 03:09:41 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16d8285f3be08ea7340eaf6dced5161164096c3fb3345fe8c5d6d64496bc143`  
		Last Modified: Tue, 31 Aug 2021 03:09:40 GMT  
		Size: 5.5 MB (5455084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ffd6c9eed67b115939ab5f6d4bb8ffd2f0f152fe9a61024122b558e83ce912e`  
		Last Modified: Tue, 31 Aug 2021 03:09:39 GMT  
		Size: 3.4 MB (3368457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdbc2935c20fd14d96044dcdb65fb79a0f676bcdf334058da282716411d3ff9b`  
		Last Modified: Tue, 31 Aug 2021 03:09:39 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b302bb5f11cae70b4c8ec1079e6de6c62dacfdce3e8f3ccdfabd6ce44b63d2`  
		Last Modified: Tue, 31 Aug 2021 03:09:37 GMT  
		Size: 2.2 MB (2203569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21de8a622698dffd65e882759b0b6e4fe0e56b60d892f2e4446f94439a1270f`  
		Last Modified: Tue, 31 Aug 2021 03:09:36 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06baf7b3e62e04d357bc19a03d9eef62d4e2e56d174f435674c61b5a62c3040e`  
		Last Modified: Tue, 31 Aug 2021 03:11:34 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f36d11e8b12a687bb22ae80bd9efdf894a7ab2aa15ce371f9ebed4b5e9eeea9`  
		Last Modified: Tue, 31 Aug 2021 03:11:47 GMT  
		Size: 79.4 MB (79413709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35884153062497a3274b9fe8217cf811b74e887e60e4b0391ab9f4a00c97bda9`  
		Last Modified: Tue, 31 Aug 2021 03:11:34 GMT  
		Size: 5.6 KB (5610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae1550e290c604c88c7286305167ec6ca5ce8ae62cf657e726e53e21d6abee00`  
		Last Modified: Tue, 31 Aug 2021 03:11:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3` - linux; ppc64le

```console
$ docker pull mariadb@sha256:ee3e3a13e267f025f2f76988ac95eff3e8771e80bdd6a19a4dfe4191baaaa2f8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.9 MB (130878367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0ee69d70a05d108b91f57174ad144788a86814c14f746ed448af3b789e11c55`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 26 Jul 2021 23:12:46 GMT
ADD file:68eb628c2202763afa91d554dde9668d8a468fe53fdbd2fe98627a5f91d224b4 in / 
# Mon, 26 Jul 2021 23:12:49 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 02:05:55 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 27 Jul 2021 02:06:47 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:06:50 GMT
ENV GOSU_VERSION=1.13
# Tue, 27 Jul 2021 02:07:32 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 27 Jul 2021 02:07:42 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 27 Jul 2021 02:08:11 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:08:14 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 27 Jul 2021 02:08:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 27 Jul 2021 02:18:29 GMT
ARG MARIADB_MAJOR=10.3
# Tue, 27 Jul 2021 02:18:30 GMT
ENV MARIADB_MAJOR=10.3
# Mon, 09 Aug 2021 19:33:17 GMT
ARG MARIADB_VERSION=1:10.3.31+maria~focal
# Mon, 09 Aug 2021 19:33:24 GMT
ENV MARIADB_VERSION=1:10.3.31+maria~focal
# Mon, 09 Aug 2021 19:33:42 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
# Mon, 09 Aug 2021 19:34:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 09 Aug 2021 19:38:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 09 Aug 2021 19:38:30 GMT
VOLUME [/var/lib/mysql]
# Mon, 09 Aug 2021 19:38:33 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Mon, 09 Aug 2021 19:38:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 09 Aug 2021 19:38:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Aug 2021 19:39:08 GMT
EXPOSE 3306
# Mon, 09 Aug 2021 19:39:16 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:1a396eed835b3b7b4101a9863d174e145ddbb1de1502a63bae726b0f81e7ca93`  
		Last Modified: Mon, 26 Jul 2021 23:15:51 GMT  
		Size: 33.3 MB (33290427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65be85b12a63573ebccb059357c5c0db6046f4a074454eea617c402e3bf99c1f`  
		Last Modified: Tue, 27 Jul 2021 02:26:16 GMT  
		Size: 1.8 KB (1760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:803c8e5bf0c59b9b01b70cac07bb24bc696bc577d8e74c79ff15bcbd480874b4`  
		Last Modified: Tue, 27 Jul 2021 02:26:17 GMT  
		Size: 6.7 MB (6667884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62bd7bf9c00152c4fb338b2c1a01d5b241ceda5c58d9e700a353072ab80fb4b9`  
		Last Modified: Tue, 27 Jul 2021 02:26:17 GMT  
		Size: 3.7 MB (3670853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:372602ac4ce9a3a693cb97ec9b3e71b449fdafbaded2ce2937fec39cec9c9b6e`  
		Last Modified: Tue, 27 Jul 2021 02:26:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a80c4de70a1ded78cf0175b1f5fda38b3119857dd2d8d9f1fafcdc39eafef0e`  
		Last Modified: Tue, 27 Jul 2021 02:26:13 GMT  
		Size: 2.6 MB (2569871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc8dec87672a96e86220faa6c3e98577b2a9090fc81d81efb4681fe59e732b7`  
		Last Modified: Tue, 27 Jul 2021 02:26:12 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d4c44c1594096752ada6ed92604830640dfb30532bb4bef9286d87106641171`  
		Last Modified: Mon, 09 Aug 2021 19:47:10 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2768461faac96a25d8dda5bb9ca72d8f376094a119254fec9101de609a6b5d99`  
		Last Modified: Mon, 09 Aug 2021 19:47:27 GMT  
		Size: 84.7 MB (84668868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea5921594fde1ae68d8eb7c9e67dc38772e2d8bb4afc3fade4f6dc4484146ffd`  
		Last Modified: Mon, 09 Aug 2021 19:47:10 GMT  
		Size: 5.6 KB (5614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bdcee0fbec51cf829dd268049dbc5fbd6ff4b409fac5d1df8cfa0a3895787cd`  
		Last Modified: Mon, 09 Aug 2021 19:47:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3-focal`

```console
$ docker pull mariadb@sha256:6cd37e22c049027eb83c8070cdc6f3df8c769aab00af40bcf1679c8391c095ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:1ab45fcbf5231f9f3527e2c57e0c6a57e0ee0e12dc37373f2b57aece0d9e0807
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.0 MB (120014376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2c8dae1f6f5606d625fe0e3aaa1f8791e4d00674bf05c0cd907e7565d3c5403`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:05:00 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 27 Jul 2021 00:05:14 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:05:15 GMT
ENV GOSU_VERSION=1.13
# Tue, 27 Jul 2021 00:05:26 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 27 Jul 2021 00:05:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 27 Jul 2021 00:05:34 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:05:35 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 27 Jul 2021 00:05:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 27 Jul 2021 00:07:32 GMT
ARG MARIADB_MAJOR=10.3
# Tue, 27 Jul 2021 00:07:32 GMT
ENV MARIADB_MAJOR=10.3
# Mon, 09 Aug 2021 19:26:04 GMT
ARG MARIADB_VERSION=1:10.3.31+maria~focal
# Mon, 09 Aug 2021 19:26:04 GMT
ENV MARIADB_VERSION=1:10.3.31+maria~focal
# Mon, 09 Aug 2021 19:26:04 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
# Mon, 09 Aug 2021 19:26:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 09 Aug 2021 19:26:31 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 09 Aug 2021 19:26:31 GMT
VOLUME [/var/lib/mysql]
# Mon, 09 Aug 2021 19:26:31 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Mon, 09 Aug 2021 19:26:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 09 Aug 2021 19:26:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Aug 2021 19:26:32 GMT
EXPOSE 3306
# Mon, 09 Aug 2021 19:26:32 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf20e69555c2118df81cd7906473b0bbef5210f014d45113251b1298fb1c996`  
		Last Modified: Tue, 27 Jul 2021 00:10:02 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69afd1ffc85b8fe385e48d00e89467a4e080c81b2447ce86ebf964f3e43efb9`  
		Last Modified: Tue, 27 Jul 2021 00:10:04 GMT  
		Size: 5.5 MB (5488764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e720dc7fcd8609016e69543f354117290ffee7c9ea1bdd97d7ca84bcc06d616`  
		Last Modified: Tue, 27 Jul 2021 00:10:03 GMT  
		Size: 3.6 MB (3582379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a81d177e410065c8eec2b5c018ab6ac60b2a5161184890bc3bf7627e78fb2dd`  
		Last Modified: Tue, 27 Jul 2021 00:10:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827c8c103c898d23db5f0cfc69b6faa45038d27b1ec3c15cb5d5b29ee60fca0b`  
		Last Modified: Tue, 27 Jul 2021 00:09:59 GMT  
		Size: 2.3 MB (2274133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2108ccd013748c7fce6a19a3f7434b860401f78326ac7373c486eafa3c719354`  
		Last Modified: Tue, 27 Jul 2021 00:09:59 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8900c3d54d69bc9fab7b747feb0a470376a1a346e1ba78752ead65506d06f33f`  
		Last Modified: Mon, 09 Aug 2021 19:29:42 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496d3f780dd791eb10b78b4b0376c3afed298ac67dc52262a1278dabfc1d318f`  
		Last Modified: Mon, 09 Aug 2021 19:29:54 GMT  
		Size: 80.1 MB (80090705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77805c057f07ba4de9b922b741a8b078369c3e440e1fa4b80d1c645510e6df66`  
		Last Modified: Mon, 09 Aug 2021 19:29:42 GMT  
		Size: 5.6 KB (5613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3fa47ecdca663b37feca04369ec700446cb994ecc1d7d09c6436613e0c34ce9`  
		Last Modified: Mon, 09 Aug 2021 19:29:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:86cb5b855f40bbdbc56f3e4e9a207f8e7be3c0020d8facad8b781b2288767132
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117624368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23b1ae977ba9883f9e1eabf5adb70757edf5179897714cf603dc7dcbd31fbf13`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:44 GMT
ADD file:cec21619ecbd37b4cf8da15153b8957a343cd25c6f714e3ac3969b6003704a58 in / 
# Tue, 31 Aug 2021 01:40:45 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:04:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 31 Aug 2021 03:04:38 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:04:38 GMT
ENV GOSU_VERSION=1.13
# Tue, 31 Aug 2021 03:04:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 31 Aug 2021 03:04:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 31 Aug 2021 03:04:57 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:04:57 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 31 Aug 2021 03:05:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 31 Aug 2021 03:06:44 GMT
ARG MARIADB_MAJOR=10.3
# Tue, 31 Aug 2021 03:06:44 GMT
ENV MARIADB_MAJOR=10.3
# Tue, 31 Aug 2021 03:06:44 GMT
ARG MARIADB_VERSION=1:10.3.31+maria~focal
# Tue, 31 Aug 2021 03:06:44 GMT
ENV MARIADB_VERSION=1:10.3.31+maria~focal
# Tue, 31 Aug 2021 03:06:45 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
# Tue, 31 Aug 2021 03:06:45 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 31 Aug 2021 03:07:10 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 31 Aug 2021 03:07:11 GMT
VOLUME [/var/lib/mysql]
# Tue, 31 Aug 2021 03:07:11 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Tue, 31 Aug 2021 03:07:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 31 Aug 2021 03:07:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Aug 2021 03:07:12 GMT
EXPOSE 3306
# Tue, 31 Aug 2021 03:07:12 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ab2d02b1ec420fdb84c9f52abda403b6aef20f5de904a2ecda5ae4f5cd6e4d46`  
		Last Modified: Tue, 31 Aug 2021 01:42:34 GMT  
		Size: 27.2 MB (27173099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d16f1b8a1bc9060d0c98a0e09c73ceab3d694a99f57672d6e44f2f5dcf09eae`  
		Last Modified: Tue, 31 Aug 2021 03:09:41 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16d8285f3be08ea7340eaf6dced5161164096c3fb3345fe8c5d6d64496bc143`  
		Last Modified: Tue, 31 Aug 2021 03:09:40 GMT  
		Size: 5.5 MB (5455084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ffd6c9eed67b115939ab5f6d4bb8ffd2f0f152fe9a61024122b558e83ce912e`  
		Last Modified: Tue, 31 Aug 2021 03:09:39 GMT  
		Size: 3.4 MB (3368457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdbc2935c20fd14d96044dcdb65fb79a0f676bcdf334058da282716411d3ff9b`  
		Last Modified: Tue, 31 Aug 2021 03:09:39 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b302bb5f11cae70b4c8ec1079e6de6c62dacfdce3e8f3ccdfabd6ce44b63d2`  
		Last Modified: Tue, 31 Aug 2021 03:09:37 GMT  
		Size: 2.2 MB (2203569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21de8a622698dffd65e882759b0b6e4fe0e56b60d892f2e4446f94439a1270f`  
		Last Modified: Tue, 31 Aug 2021 03:09:36 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06baf7b3e62e04d357bc19a03d9eef62d4e2e56d174f435674c61b5a62c3040e`  
		Last Modified: Tue, 31 Aug 2021 03:11:34 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f36d11e8b12a687bb22ae80bd9efdf894a7ab2aa15ce371f9ebed4b5e9eeea9`  
		Last Modified: Tue, 31 Aug 2021 03:11:47 GMT  
		Size: 79.4 MB (79413709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35884153062497a3274b9fe8217cf811b74e887e60e4b0391ab9f4a00c97bda9`  
		Last Modified: Tue, 31 Aug 2021 03:11:34 GMT  
		Size: 5.6 KB (5610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae1550e290c604c88c7286305167ec6ca5ce8ae62cf657e726e53e21d6abee00`  
		Last Modified: Tue, 31 Aug 2021 03:11:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:ee3e3a13e267f025f2f76988ac95eff3e8771e80bdd6a19a4dfe4191baaaa2f8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.9 MB (130878367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0ee69d70a05d108b91f57174ad144788a86814c14f746ed448af3b789e11c55`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 26 Jul 2021 23:12:46 GMT
ADD file:68eb628c2202763afa91d554dde9668d8a468fe53fdbd2fe98627a5f91d224b4 in / 
# Mon, 26 Jul 2021 23:12:49 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 02:05:55 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 27 Jul 2021 02:06:47 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:06:50 GMT
ENV GOSU_VERSION=1.13
# Tue, 27 Jul 2021 02:07:32 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 27 Jul 2021 02:07:42 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 27 Jul 2021 02:08:11 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:08:14 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 27 Jul 2021 02:08:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 27 Jul 2021 02:18:29 GMT
ARG MARIADB_MAJOR=10.3
# Tue, 27 Jul 2021 02:18:30 GMT
ENV MARIADB_MAJOR=10.3
# Mon, 09 Aug 2021 19:33:17 GMT
ARG MARIADB_VERSION=1:10.3.31+maria~focal
# Mon, 09 Aug 2021 19:33:24 GMT
ENV MARIADB_VERSION=1:10.3.31+maria~focal
# Mon, 09 Aug 2021 19:33:42 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
# Mon, 09 Aug 2021 19:34:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 09 Aug 2021 19:38:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 09 Aug 2021 19:38:30 GMT
VOLUME [/var/lib/mysql]
# Mon, 09 Aug 2021 19:38:33 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Mon, 09 Aug 2021 19:38:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 09 Aug 2021 19:38:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Aug 2021 19:39:08 GMT
EXPOSE 3306
# Mon, 09 Aug 2021 19:39:16 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:1a396eed835b3b7b4101a9863d174e145ddbb1de1502a63bae726b0f81e7ca93`  
		Last Modified: Mon, 26 Jul 2021 23:15:51 GMT  
		Size: 33.3 MB (33290427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65be85b12a63573ebccb059357c5c0db6046f4a074454eea617c402e3bf99c1f`  
		Last Modified: Tue, 27 Jul 2021 02:26:16 GMT  
		Size: 1.8 KB (1760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:803c8e5bf0c59b9b01b70cac07bb24bc696bc577d8e74c79ff15bcbd480874b4`  
		Last Modified: Tue, 27 Jul 2021 02:26:17 GMT  
		Size: 6.7 MB (6667884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62bd7bf9c00152c4fb338b2c1a01d5b241ceda5c58d9e700a353072ab80fb4b9`  
		Last Modified: Tue, 27 Jul 2021 02:26:17 GMT  
		Size: 3.7 MB (3670853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:372602ac4ce9a3a693cb97ec9b3e71b449fdafbaded2ce2937fec39cec9c9b6e`  
		Last Modified: Tue, 27 Jul 2021 02:26:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a80c4de70a1ded78cf0175b1f5fda38b3119857dd2d8d9f1fafcdc39eafef0e`  
		Last Modified: Tue, 27 Jul 2021 02:26:13 GMT  
		Size: 2.6 MB (2569871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc8dec87672a96e86220faa6c3e98577b2a9090fc81d81efb4681fe59e732b7`  
		Last Modified: Tue, 27 Jul 2021 02:26:12 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d4c44c1594096752ada6ed92604830640dfb30532bb4bef9286d87106641171`  
		Last Modified: Mon, 09 Aug 2021 19:47:10 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2768461faac96a25d8dda5bb9ca72d8f376094a119254fec9101de609a6b5d99`  
		Last Modified: Mon, 09 Aug 2021 19:47:27 GMT  
		Size: 84.7 MB (84668868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea5921594fde1ae68d8eb7c9e67dc38772e2d8bb4afc3fade4f6dc4484146ffd`  
		Last Modified: Mon, 09 Aug 2021 19:47:10 GMT  
		Size: 5.6 KB (5614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bdcee0fbec51cf829dd268049dbc5fbd6ff4b409fac5d1df8cfa0a3895787cd`  
		Last Modified: Mon, 09 Aug 2021 19:47:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3.31`

```console
$ docker pull mariadb@sha256:6cd37e22c049027eb83c8070cdc6f3df8c769aab00af40bcf1679c8391c095ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3.31` - linux; amd64

```console
$ docker pull mariadb@sha256:1ab45fcbf5231f9f3527e2c57e0c6a57e0ee0e12dc37373f2b57aece0d9e0807
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.0 MB (120014376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2c8dae1f6f5606d625fe0e3aaa1f8791e4d00674bf05c0cd907e7565d3c5403`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:05:00 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 27 Jul 2021 00:05:14 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:05:15 GMT
ENV GOSU_VERSION=1.13
# Tue, 27 Jul 2021 00:05:26 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 27 Jul 2021 00:05:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 27 Jul 2021 00:05:34 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:05:35 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 27 Jul 2021 00:05:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 27 Jul 2021 00:07:32 GMT
ARG MARIADB_MAJOR=10.3
# Tue, 27 Jul 2021 00:07:32 GMT
ENV MARIADB_MAJOR=10.3
# Mon, 09 Aug 2021 19:26:04 GMT
ARG MARIADB_VERSION=1:10.3.31+maria~focal
# Mon, 09 Aug 2021 19:26:04 GMT
ENV MARIADB_VERSION=1:10.3.31+maria~focal
# Mon, 09 Aug 2021 19:26:04 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
# Mon, 09 Aug 2021 19:26:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 09 Aug 2021 19:26:31 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 09 Aug 2021 19:26:31 GMT
VOLUME [/var/lib/mysql]
# Mon, 09 Aug 2021 19:26:31 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Mon, 09 Aug 2021 19:26:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 09 Aug 2021 19:26:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Aug 2021 19:26:32 GMT
EXPOSE 3306
# Mon, 09 Aug 2021 19:26:32 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf20e69555c2118df81cd7906473b0bbef5210f014d45113251b1298fb1c996`  
		Last Modified: Tue, 27 Jul 2021 00:10:02 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69afd1ffc85b8fe385e48d00e89467a4e080c81b2447ce86ebf964f3e43efb9`  
		Last Modified: Tue, 27 Jul 2021 00:10:04 GMT  
		Size: 5.5 MB (5488764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e720dc7fcd8609016e69543f354117290ffee7c9ea1bdd97d7ca84bcc06d616`  
		Last Modified: Tue, 27 Jul 2021 00:10:03 GMT  
		Size: 3.6 MB (3582379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a81d177e410065c8eec2b5c018ab6ac60b2a5161184890bc3bf7627e78fb2dd`  
		Last Modified: Tue, 27 Jul 2021 00:10:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827c8c103c898d23db5f0cfc69b6faa45038d27b1ec3c15cb5d5b29ee60fca0b`  
		Last Modified: Tue, 27 Jul 2021 00:09:59 GMT  
		Size: 2.3 MB (2274133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2108ccd013748c7fce6a19a3f7434b860401f78326ac7373c486eafa3c719354`  
		Last Modified: Tue, 27 Jul 2021 00:09:59 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8900c3d54d69bc9fab7b747feb0a470376a1a346e1ba78752ead65506d06f33f`  
		Last Modified: Mon, 09 Aug 2021 19:29:42 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496d3f780dd791eb10b78b4b0376c3afed298ac67dc52262a1278dabfc1d318f`  
		Last Modified: Mon, 09 Aug 2021 19:29:54 GMT  
		Size: 80.1 MB (80090705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77805c057f07ba4de9b922b741a8b078369c3e440e1fa4b80d1c645510e6df66`  
		Last Modified: Mon, 09 Aug 2021 19:29:42 GMT  
		Size: 5.6 KB (5613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3fa47ecdca663b37feca04369ec700446cb994ecc1d7d09c6436613e0c34ce9`  
		Last Modified: Mon, 09 Aug 2021 19:29:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.31` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:86cb5b855f40bbdbc56f3e4e9a207f8e7be3c0020d8facad8b781b2288767132
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117624368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23b1ae977ba9883f9e1eabf5adb70757edf5179897714cf603dc7dcbd31fbf13`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:44 GMT
ADD file:cec21619ecbd37b4cf8da15153b8957a343cd25c6f714e3ac3969b6003704a58 in / 
# Tue, 31 Aug 2021 01:40:45 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:04:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 31 Aug 2021 03:04:38 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:04:38 GMT
ENV GOSU_VERSION=1.13
# Tue, 31 Aug 2021 03:04:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 31 Aug 2021 03:04:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 31 Aug 2021 03:04:57 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:04:57 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 31 Aug 2021 03:05:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 31 Aug 2021 03:06:44 GMT
ARG MARIADB_MAJOR=10.3
# Tue, 31 Aug 2021 03:06:44 GMT
ENV MARIADB_MAJOR=10.3
# Tue, 31 Aug 2021 03:06:44 GMT
ARG MARIADB_VERSION=1:10.3.31+maria~focal
# Tue, 31 Aug 2021 03:06:44 GMT
ENV MARIADB_VERSION=1:10.3.31+maria~focal
# Tue, 31 Aug 2021 03:06:45 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
# Tue, 31 Aug 2021 03:06:45 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 31 Aug 2021 03:07:10 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 31 Aug 2021 03:07:11 GMT
VOLUME [/var/lib/mysql]
# Tue, 31 Aug 2021 03:07:11 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Tue, 31 Aug 2021 03:07:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 31 Aug 2021 03:07:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Aug 2021 03:07:12 GMT
EXPOSE 3306
# Tue, 31 Aug 2021 03:07:12 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ab2d02b1ec420fdb84c9f52abda403b6aef20f5de904a2ecda5ae4f5cd6e4d46`  
		Last Modified: Tue, 31 Aug 2021 01:42:34 GMT  
		Size: 27.2 MB (27173099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d16f1b8a1bc9060d0c98a0e09c73ceab3d694a99f57672d6e44f2f5dcf09eae`  
		Last Modified: Tue, 31 Aug 2021 03:09:41 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16d8285f3be08ea7340eaf6dced5161164096c3fb3345fe8c5d6d64496bc143`  
		Last Modified: Tue, 31 Aug 2021 03:09:40 GMT  
		Size: 5.5 MB (5455084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ffd6c9eed67b115939ab5f6d4bb8ffd2f0f152fe9a61024122b558e83ce912e`  
		Last Modified: Tue, 31 Aug 2021 03:09:39 GMT  
		Size: 3.4 MB (3368457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdbc2935c20fd14d96044dcdb65fb79a0f676bcdf334058da282716411d3ff9b`  
		Last Modified: Tue, 31 Aug 2021 03:09:39 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b302bb5f11cae70b4c8ec1079e6de6c62dacfdce3e8f3ccdfabd6ce44b63d2`  
		Last Modified: Tue, 31 Aug 2021 03:09:37 GMT  
		Size: 2.2 MB (2203569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21de8a622698dffd65e882759b0b6e4fe0e56b60d892f2e4446f94439a1270f`  
		Last Modified: Tue, 31 Aug 2021 03:09:36 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06baf7b3e62e04d357bc19a03d9eef62d4e2e56d174f435674c61b5a62c3040e`  
		Last Modified: Tue, 31 Aug 2021 03:11:34 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f36d11e8b12a687bb22ae80bd9efdf894a7ab2aa15ce371f9ebed4b5e9eeea9`  
		Last Modified: Tue, 31 Aug 2021 03:11:47 GMT  
		Size: 79.4 MB (79413709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35884153062497a3274b9fe8217cf811b74e887e60e4b0391ab9f4a00c97bda9`  
		Last Modified: Tue, 31 Aug 2021 03:11:34 GMT  
		Size: 5.6 KB (5610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae1550e290c604c88c7286305167ec6ca5ce8ae62cf657e726e53e21d6abee00`  
		Last Modified: Tue, 31 Aug 2021 03:11:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.31` - linux; ppc64le

```console
$ docker pull mariadb@sha256:ee3e3a13e267f025f2f76988ac95eff3e8771e80bdd6a19a4dfe4191baaaa2f8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.9 MB (130878367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0ee69d70a05d108b91f57174ad144788a86814c14f746ed448af3b789e11c55`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 26 Jul 2021 23:12:46 GMT
ADD file:68eb628c2202763afa91d554dde9668d8a468fe53fdbd2fe98627a5f91d224b4 in / 
# Mon, 26 Jul 2021 23:12:49 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 02:05:55 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 27 Jul 2021 02:06:47 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:06:50 GMT
ENV GOSU_VERSION=1.13
# Tue, 27 Jul 2021 02:07:32 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 27 Jul 2021 02:07:42 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 27 Jul 2021 02:08:11 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:08:14 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 27 Jul 2021 02:08:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 27 Jul 2021 02:18:29 GMT
ARG MARIADB_MAJOR=10.3
# Tue, 27 Jul 2021 02:18:30 GMT
ENV MARIADB_MAJOR=10.3
# Mon, 09 Aug 2021 19:33:17 GMT
ARG MARIADB_VERSION=1:10.3.31+maria~focal
# Mon, 09 Aug 2021 19:33:24 GMT
ENV MARIADB_VERSION=1:10.3.31+maria~focal
# Mon, 09 Aug 2021 19:33:42 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
# Mon, 09 Aug 2021 19:34:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 09 Aug 2021 19:38:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 09 Aug 2021 19:38:30 GMT
VOLUME [/var/lib/mysql]
# Mon, 09 Aug 2021 19:38:33 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Mon, 09 Aug 2021 19:38:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 09 Aug 2021 19:38:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Aug 2021 19:39:08 GMT
EXPOSE 3306
# Mon, 09 Aug 2021 19:39:16 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:1a396eed835b3b7b4101a9863d174e145ddbb1de1502a63bae726b0f81e7ca93`  
		Last Modified: Mon, 26 Jul 2021 23:15:51 GMT  
		Size: 33.3 MB (33290427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65be85b12a63573ebccb059357c5c0db6046f4a074454eea617c402e3bf99c1f`  
		Last Modified: Tue, 27 Jul 2021 02:26:16 GMT  
		Size: 1.8 KB (1760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:803c8e5bf0c59b9b01b70cac07bb24bc696bc577d8e74c79ff15bcbd480874b4`  
		Last Modified: Tue, 27 Jul 2021 02:26:17 GMT  
		Size: 6.7 MB (6667884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62bd7bf9c00152c4fb338b2c1a01d5b241ceda5c58d9e700a353072ab80fb4b9`  
		Last Modified: Tue, 27 Jul 2021 02:26:17 GMT  
		Size: 3.7 MB (3670853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:372602ac4ce9a3a693cb97ec9b3e71b449fdafbaded2ce2937fec39cec9c9b6e`  
		Last Modified: Tue, 27 Jul 2021 02:26:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a80c4de70a1ded78cf0175b1f5fda38b3119857dd2d8d9f1fafcdc39eafef0e`  
		Last Modified: Tue, 27 Jul 2021 02:26:13 GMT  
		Size: 2.6 MB (2569871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc8dec87672a96e86220faa6c3e98577b2a9090fc81d81efb4681fe59e732b7`  
		Last Modified: Tue, 27 Jul 2021 02:26:12 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d4c44c1594096752ada6ed92604830640dfb30532bb4bef9286d87106641171`  
		Last Modified: Mon, 09 Aug 2021 19:47:10 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2768461faac96a25d8dda5bb9ca72d8f376094a119254fec9101de609a6b5d99`  
		Last Modified: Mon, 09 Aug 2021 19:47:27 GMT  
		Size: 84.7 MB (84668868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea5921594fde1ae68d8eb7c9e67dc38772e2d8bb4afc3fade4f6dc4484146ffd`  
		Last Modified: Mon, 09 Aug 2021 19:47:10 GMT  
		Size: 5.6 KB (5614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bdcee0fbec51cf829dd268049dbc5fbd6ff4b409fac5d1df8cfa0a3895787cd`  
		Last Modified: Mon, 09 Aug 2021 19:47:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3.31-focal`

```console
$ docker pull mariadb@sha256:6cd37e22c049027eb83c8070cdc6f3df8c769aab00af40bcf1679c8391c095ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3.31-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:1ab45fcbf5231f9f3527e2c57e0c6a57e0ee0e12dc37373f2b57aece0d9e0807
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.0 MB (120014376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2c8dae1f6f5606d625fe0e3aaa1f8791e4d00674bf05c0cd907e7565d3c5403`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:05:00 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 27 Jul 2021 00:05:14 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:05:15 GMT
ENV GOSU_VERSION=1.13
# Tue, 27 Jul 2021 00:05:26 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 27 Jul 2021 00:05:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 27 Jul 2021 00:05:34 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:05:35 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 27 Jul 2021 00:05:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 27 Jul 2021 00:07:32 GMT
ARG MARIADB_MAJOR=10.3
# Tue, 27 Jul 2021 00:07:32 GMT
ENV MARIADB_MAJOR=10.3
# Mon, 09 Aug 2021 19:26:04 GMT
ARG MARIADB_VERSION=1:10.3.31+maria~focal
# Mon, 09 Aug 2021 19:26:04 GMT
ENV MARIADB_VERSION=1:10.3.31+maria~focal
# Mon, 09 Aug 2021 19:26:04 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
# Mon, 09 Aug 2021 19:26:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 09 Aug 2021 19:26:31 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 09 Aug 2021 19:26:31 GMT
VOLUME [/var/lib/mysql]
# Mon, 09 Aug 2021 19:26:31 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Mon, 09 Aug 2021 19:26:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 09 Aug 2021 19:26:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Aug 2021 19:26:32 GMT
EXPOSE 3306
# Mon, 09 Aug 2021 19:26:32 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf20e69555c2118df81cd7906473b0bbef5210f014d45113251b1298fb1c996`  
		Last Modified: Tue, 27 Jul 2021 00:10:02 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69afd1ffc85b8fe385e48d00e89467a4e080c81b2447ce86ebf964f3e43efb9`  
		Last Modified: Tue, 27 Jul 2021 00:10:04 GMT  
		Size: 5.5 MB (5488764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e720dc7fcd8609016e69543f354117290ffee7c9ea1bdd97d7ca84bcc06d616`  
		Last Modified: Tue, 27 Jul 2021 00:10:03 GMT  
		Size: 3.6 MB (3582379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a81d177e410065c8eec2b5c018ab6ac60b2a5161184890bc3bf7627e78fb2dd`  
		Last Modified: Tue, 27 Jul 2021 00:10:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827c8c103c898d23db5f0cfc69b6faa45038d27b1ec3c15cb5d5b29ee60fca0b`  
		Last Modified: Tue, 27 Jul 2021 00:09:59 GMT  
		Size: 2.3 MB (2274133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2108ccd013748c7fce6a19a3f7434b860401f78326ac7373c486eafa3c719354`  
		Last Modified: Tue, 27 Jul 2021 00:09:59 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8900c3d54d69bc9fab7b747feb0a470376a1a346e1ba78752ead65506d06f33f`  
		Last Modified: Mon, 09 Aug 2021 19:29:42 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496d3f780dd791eb10b78b4b0376c3afed298ac67dc52262a1278dabfc1d318f`  
		Last Modified: Mon, 09 Aug 2021 19:29:54 GMT  
		Size: 80.1 MB (80090705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77805c057f07ba4de9b922b741a8b078369c3e440e1fa4b80d1c645510e6df66`  
		Last Modified: Mon, 09 Aug 2021 19:29:42 GMT  
		Size: 5.6 KB (5613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3fa47ecdca663b37feca04369ec700446cb994ecc1d7d09c6436613e0c34ce9`  
		Last Modified: Mon, 09 Aug 2021 19:29:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.31-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:86cb5b855f40bbdbc56f3e4e9a207f8e7be3c0020d8facad8b781b2288767132
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117624368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23b1ae977ba9883f9e1eabf5adb70757edf5179897714cf603dc7dcbd31fbf13`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:44 GMT
ADD file:cec21619ecbd37b4cf8da15153b8957a343cd25c6f714e3ac3969b6003704a58 in / 
# Tue, 31 Aug 2021 01:40:45 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:04:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 31 Aug 2021 03:04:38 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:04:38 GMT
ENV GOSU_VERSION=1.13
# Tue, 31 Aug 2021 03:04:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 31 Aug 2021 03:04:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 31 Aug 2021 03:04:57 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:04:57 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 31 Aug 2021 03:05:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 31 Aug 2021 03:06:44 GMT
ARG MARIADB_MAJOR=10.3
# Tue, 31 Aug 2021 03:06:44 GMT
ENV MARIADB_MAJOR=10.3
# Tue, 31 Aug 2021 03:06:44 GMT
ARG MARIADB_VERSION=1:10.3.31+maria~focal
# Tue, 31 Aug 2021 03:06:44 GMT
ENV MARIADB_VERSION=1:10.3.31+maria~focal
# Tue, 31 Aug 2021 03:06:45 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
# Tue, 31 Aug 2021 03:06:45 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 31 Aug 2021 03:07:10 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 31 Aug 2021 03:07:11 GMT
VOLUME [/var/lib/mysql]
# Tue, 31 Aug 2021 03:07:11 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Tue, 31 Aug 2021 03:07:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 31 Aug 2021 03:07:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Aug 2021 03:07:12 GMT
EXPOSE 3306
# Tue, 31 Aug 2021 03:07:12 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ab2d02b1ec420fdb84c9f52abda403b6aef20f5de904a2ecda5ae4f5cd6e4d46`  
		Last Modified: Tue, 31 Aug 2021 01:42:34 GMT  
		Size: 27.2 MB (27173099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d16f1b8a1bc9060d0c98a0e09c73ceab3d694a99f57672d6e44f2f5dcf09eae`  
		Last Modified: Tue, 31 Aug 2021 03:09:41 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16d8285f3be08ea7340eaf6dced5161164096c3fb3345fe8c5d6d64496bc143`  
		Last Modified: Tue, 31 Aug 2021 03:09:40 GMT  
		Size: 5.5 MB (5455084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ffd6c9eed67b115939ab5f6d4bb8ffd2f0f152fe9a61024122b558e83ce912e`  
		Last Modified: Tue, 31 Aug 2021 03:09:39 GMT  
		Size: 3.4 MB (3368457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdbc2935c20fd14d96044dcdb65fb79a0f676bcdf334058da282716411d3ff9b`  
		Last Modified: Tue, 31 Aug 2021 03:09:39 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b302bb5f11cae70b4c8ec1079e6de6c62dacfdce3e8f3ccdfabd6ce44b63d2`  
		Last Modified: Tue, 31 Aug 2021 03:09:37 GMT  
		Size: 2.2 MB (2203569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21de8a622698dffd65e882759b0b6e4fe0e56b60d892f2e4446f94439a1270f`  
		Last Modified: Tue, 31 Aug 2021 03:09:36 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06baf7b3e62e04d357bc19a03d9eef62d4e2e56d174f435674c61b5a62c3040e`  
		Last Modified: Tue, 31 Aug 2021 03:11:34 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f36d11e8b12a687bb22ae80bd9efdf894a7ab2aa15ce371f9ebed4b5e9eeea9`  
		Last Modified: Tue, 31 Aug 2021 03:11:47 GMT  
		Size: 79.4 MB (79413709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35884153062497a3274b9fe8217cf811b74e887e60e4b0391ab9f4a00c97bda9`  
		Last Modified: Tue, 31 Aug 2021 03:11:34 GMT  
		Size: 5.6 KB (5610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae1550e290c604c88c7286305167ec6ca5ce8ae62cf657e726e53e21d6abee00`  
		Last Modified: Tue, 31 Aug 2021 03:11:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.31-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:ee3e3a13e267f025f2f76988ac95eff3e8771e80bdd6a19a4dfe4191baaaa2f8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.9 MB (130878367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0ee69d70a05d108b91f57174ad144788a86814c14f746ed448af3b789e11c55`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 26 Jul 2021 23:12:46 GMT
ADD file:68eb628c2202763afa91d554dde9668d8a468fe53fdbd2fe98627a5f91d224b4 in / 
# Mon, 26 Jul 2021 23:12:49 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 02:05:55 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 27 Jul 2021 02:06:47 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:06:50 GMT
ENV GOSU_VERSION=1.13
# Tue, 27 Jul 2021 02:07:32 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 27 Jul 2021 02:07:42 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 27 Jul 2021 02:08:11 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:08:14 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 27 Jul 2021 02:08:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 27 Jul 2021 02:18:29 GMT
ARG MARIADB_MAJOR=10.3
# Tue, 27 Jul 2021 02:18:30 GMT
ENV MARIADB_MAJOR=10.3
# Mon, 09 Aug 2021 19:33:17 GMT
ARG MARIADB_VERSION=1:10.3.31+maria~focal
# Mon, 09 Aug 2021 19:33:24 GMT
ENV MARIADB_VERSION=1:10.3.31+maria~focal
# Mon, 09 Aug 2021 19:33:42 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
# Mon, 09 Aug 2021 19:34:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 09 Aug 2021 19:38:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 09 Aug 2021 19:38:30 GMT
VOLUME [/var/lib/mysql]
# Mon, 09 Aug 2021 19:38:33 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Mon, 09 Aug 2021 19:38:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 09 Aug 2021 19:38:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Aug 2021 19:39:08 GMT
EXPOSE 3306
# Mon, 09 Aug 2021 19:39:16 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:1a396eed835b3b7b4101a9863d174e145ddbb1de1502a63bae726b0f81e7ca93`  
		Last Modified: Mon, 26 Jul 2021 23:15:51 GMT  
		Size: 33.3 MB (33290427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65be85b12a63573ebccb059357c5c0db6046f4a074454eea617c402e3bf99c1f`  
		Last Modified: Tue, 27 Jul 2021 02:26:16 GMT  
		Size: 1.8 KB (1760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:803c8e5bf0c59b9b01b70cac07bb24bc696bc577d8e74c79ff15bcbd480874b4`  
		Last Modified: Tue, 27 Jul 2021 02:26:17 GMT  
		Size: 6.7 MB (6667884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62bd7bf9c00152c4fb338b2c1a01d5b241ceda5c58d9e700a353072ab80fb4b9`  
		Last Modified: Tue, 27 Jul 2021 02:26:17 GMT  
		Size: 3.7 MB (3670853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:372602ac4ce9a3a693cb97ec9b3e71b449fdafbaded2ce2937fec39cec9c9b6e`  
		Last Modified: Tue, 27 Jul 2021 02:26:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a80c4de70a1ded78cf0175b1f5fda38b3119857dd2d8d9f1fafcdc39eafef0e`  
		Last Modified: Tue, 27 Jul 2021 02:26:13 GMT  
		Size: 2.6 MB (2569871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc8dec87672a96e86220faa6c3e98577b2a9090fc81d81efb4681fe59e732b7`  
		Last Modified: Tue, 27 Jul 2021 02:26:12 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d4c44c1594096752ada6ed92604830640dfb30532bb4bef9286d87106641171`  
		Last Modified: Mon, 09 Aug 2021 19:47:10 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2768461faac96a25d8dda5bb9ca72d8f376094a119254fec9101de609a6b5d99`  
		Last Modified: Mon, 09 Aug 2021 19:47:27 GMT  
		Size: 84.7 MB (84668868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea5921594fde1ae68d8eb7c9e67dc38772e2d8bb4afc3fade4f6dc4484146ffd`  
		Last Modified: Mon, 09 Aug 2021 19:47:10 GMT  
		Size: 5.6 KB (5614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bdcee0fbec51cf829dd268049dbc5fbd6ff4b409fac5d1df8cfa0a3895787cd`  
		Last Modified: Mon, 09 Aug 2021 19:47:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4`

```console
$ docker pull mariadb@sha256:c5d8ca208661cce5f59a8b935a4036cf2a5a36d06189883a821596f8e460ee33
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4` - linux; amd64

```console
$ docker pull mariadb@sha256:f757259fb431216040a77292d79428710cdcc9f3c1db17811c2029e7131f9950
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.7 MB (124736934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59f9f97d14cefa84e69d9df6e30855f8848c94ff3b52b1c80bb988bd60827682`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:05:00 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 27 Jul 2021 00:05:14 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:05:15 GMT
ENV GOSU_VERSION=1.13
# Tue, 27 Jul 2021 00:05:26 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 27 Jul 2021 00:05:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 27 Jul 2021 00:05:34 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:05:35 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 27 Jul 2021 00:05:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 27 Jul 2021 00:06:56 GMT
ARG MARIADB_MAJOR=10.4
# Tue, 27 Jul 2021 00:06:56 GMT
ENV MARIADB_MAJOR=10.4
# Mon, 09 Aug 2021 19:25:34 GMT
ARG MARIADB_VERSION=1:10.4.21+maria~focal
# Mon, 09 Aug 2021 19:25:34 GMT
ENV MARIADB_VERSION=1:10.4.21+maria~focal
# Mon, 09 Aug 2021 19:25:34 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
# Mon, 09 Aug 2021 19:25:35 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 09 Aug 2021 19:25:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 09 Aug 2021 19:25:58 GMT
VOLUME [/var/lib/mysql]
# Mon, 09 Aug 2021 19:25:58 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Mon, 09 Aug 2021 19:25:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 09 Aug 2021 19:25:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Aug 2021 19:25:59 GMT
EXPOSE 3306
# Mon, 09 Aug 2021 19:25:59 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf20e69555c2118df81cd7906473b0bbef5210f014d45113251b1298fb1c996`  
		Last Modified: Tue, 27 Jul 2021 00:10:02 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69afd1ffc85b8fe385e48d00e89467a4e080c81b2447ce86ebf964f3e43efb9`  
		Last Modified: Tue, 27 Jul 2021 00:10:04 GMT  
		Size: 5.5 MB (5488764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e720dc7fcd8609016e69543f354117290ffee7c9ea1bdd97d7ca84bcc06d616`  
		Last Modified: Tue, 27 Jul 2021 00:10:03 GMT  
		Size: 3.6 MB (3582379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a81d177e410065c8eec2b5c018ab6ac60b2a5161184890bc3bf7627e78fb2dd`  
		Last Modified: Tue, 27 Jul 2021 00:10:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827c8c103c898d23db5f0cfc69b6faa45038d27b1ec3c15cb5d5b29ee60fca0b`  
		Last Modified: Tue, 27 Jul 2021 00:09:59 GMT  
		Size: 2.3 MB (2274133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2108ccd013748c7fce6a19a3f7434b860401f78326ac7373c486eafa3c719354`  
		Last Modified: Tue, 27 Jul 2021 00:09:59 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9b140ec558f045515897d54da2f1b097d349f88038b068e731417640c41c08`  
		Last Modified: Mon, 09 Aug 2021 19:29:13 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eedef259b7b484e50a0cbf6f8ee8c2667b10d8bb9f321fa1f0aa88999912963`  
		Last Modified: Mon, 09 Aug 2021 19:29:25 GMT  
		Size: 84.8 MB (84813265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1b94f4075293104c9899b2260662705f0b15e3f761324aacd2cc2db7d251fdf`  
		Last Modified: Mon, 09 Aug 2021 19:29:13 GMT  
		Size: 5.6 KB (5612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3699fac03dbbc7d3b70481b014e6954b4ef80a698aad277b545b6ea5f875e0fc`  
		Last Modified: Mon, 09 Aug 2021 19:29:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:d33d4b68778b3d6fa9e69b7f03d5a75fea1293be570e96e536bdf4d103894800
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.3 MB (122257993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f93e9279266c814e51034e150a9a6531c873f22b8851b0110c42e5d8cbffe33c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:44 GMT
ADD file:cec21619ecbd37b4cf8da15153b8957a343cd25c6f714e3ac3969b6003704a58 in / 
# Tue, 31 Aug 2021 01:40:45 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:04:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 31 Aug 2021 03:04:38 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:04:38 GMT
ENV GOSU_VERSION=1.13
# Tue, 31 Aug 2021 03:04:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 31 Aug 2021 03:04:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 31 Aug 2021 03:04:57 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:04:57 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 31 Aug 2021 03:05:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 31 Aug 2021 03:06:12 GMT
ARG MARIADB_MAJOR=10.4
# Tue, 31 Aug 2021 03:06:13 GMT
ENV MARIADB_MAJOR=10.4
# Tue, 31 Aug 2021 03:06:13 GMT
ARG MARIADB_VERSION=1:10.4.21+maria~focal
# Tue, 31 Aug 2021 03:06:13 GMT
ENV MARIADB_VERSION=1:10.4.21+maria~focal
# Tue, 31 Aug 2021 03:06:13 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
# Tue, 31 Aug 2021 03:06:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 31 Aug 2021 03:06:35 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 31 Aug 2021 03:06:36 GMT
VOLUME [/var/lib/mysql]
# Tue, 31 Aug 2021 03:06:36 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Tue, 31 Aug 2021 03:06:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 31 Aug 2021 03:06:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Aug 2021 03:06:37 GMT
EXPOSE 3306
# Tue, 31 Aug 2021 03:06:38 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ab2d02b1ec420fdb84c9f52abda403b6aef20f5de904a2ecda5ae4f5cd6e4d46`  
		Last Modified: Tue, 31 Aug 2021 01:42:34 GMT  
		Size: 27.2 MB (27173099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d16f1b8a1bc9060d0c98a0e09c73ceab3d694a99f57672d6e44f2f5dcf09eae`  
		Last Modified: Tue, 31 Aug 2021 03:09:41 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16d8285f3be08ea7340eaf6dced5161164096c3fb3345fe8c5d6d64496bc143`  
		Last Modified: Tue, 31 Aug 2021 03:09:40 GMT  
		Size: 5.5 MB (5455084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ffd6c9eed67b115939ab5f6d4bb8ffd2f0f152fe9a61024122b558e83ce912e`  
		Last Modified: Tue, 31 Aug 2021 03:09:39 GMT  
		Size: 3.4 MB (3368457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdbc2935c20fd14d96044dcdb65fb79a0f676bcdf334058da282716411d3ff9b`  
		Last Modified: Tue, 31 Aug 2021 03:09:39 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b302bb5f11cae70b4c8ec1079e6de6c62dacfdce3e8f3ccdfabd6ce44b63d2`  
		Last Modified: Tue, 31 Aug 2021 03:09:37 GMT  
		Size: 2.2 MB (2203569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21de8a622698dffd65e882759b0b6e4fe0e56b60d892f2e4446f94439a1270f`  
		Last Modified: Tue, 31 Aug 2021 03:09:36 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603fdf9d39e401c1b6b363713b28ab5661faf0b8a1990513574d46b811791b8c`  
		Last Modified: Tue, 31 Aug 2021 03:10:59 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b2986aa34c7795fb597d052475d4e402697ef596122ca7f265fa0767ae468b`  
		Last Modified: Tue, 31 Aug 2021 03:11:13 GMT  
		Size: 84.0 MB (84047333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02e6f22166fb1fb2f67bf8c6fbbc5901ee34862717159fce3c85c4fce0c5f173`  
		Last Modified: Tue, 31 Aug 2021 03:10:59 GMT  
		Size: 5.6 KB (5607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147f1688dace9eb048fa4d04a4e80f2ecc67c91745a3d9c511773b1958f78363`  
		Last Modified: Tue, 31 Aug 2021 03:10:59 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4` - linux; ppc64le

```console
$ docker pull mariadb@sha256:c6313d6768416158bb0c4b766d0c73e2b37599a3e57073adcbd2f20a3eb90436
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.5 MB (135463813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:375c0548a54460915cdbdb18da2c09f8ee0740f29908f6fd430d24253ac55f79`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 26 Jul 2021 23:12:46 GMT
ADD file:68eb628c2202763afa91d554dde9668d8a468fe53fdbd2fe98627a5f91d224b4 in / 
# Mon, 26 Jul 2021 23:12:49 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 02:05:55 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 27 Jul 2021 02:06:47 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:06:50 GMT
ENV GOSU_VERSION=1.13
# Tue, 27 Jul 2021 02:07:32 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 27 Jul 2021 02:07:42 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 27 Jul 2021 02:08:11 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:08:14 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 27 Jul 2021 02:08:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 27 Jul 2021 02:15:03 GMT
ARG MARIADB_MAJOR=10.4
# Tue, 27 Jul 2021 02:15:06 GMT
ENV MARIADB_MAJOR=10.4
# Mon, 09 Aug 2021 19:28:45 GMT
ARG MARIADB_VERSION=1:10.4.21+maria~focal
# Mon, 09 Aug 2021 19:28:48 GMT
ENV MARIADB_VERSION=1:10.4.21+maria~focal
# Mon, 09 Aug 2021 19:28:52 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
# Mon, 09 Aug 2021 19:28:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 09 Aug 2021 19:32:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 09 Aug 2021 19:32:31 GMT
VOLUME [/var/lib/mysql]
# Mon, 09 Aug 2021 19:32:33 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Mon, 09 Aug 2021 19:32:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 09 Aug 2021 19:32:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Aug 2021 19:32:48 GMT
EXPOSE 3306
# Mon, 09 Aug 2021 19:32:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:1a396eed835b3b7b4101a9863d174e145ddbb1de1502a63bae726b0f81e7ca93`  
		Last Modified: Mon, 26 Jul 2021 23:15:51 GMT  
		Size: 33.3 MB (33290427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65be85b12a63573ebccb059357c5c0db6046f4a074454eea617c402e3bf99c1f`  
		Last Modified: Tue, 27 Jul 2021 02:26:16 GMT  
		Size: 1.8 KB (1760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:803c8e5bf0c59b9b01b70cac07bb24bc696bc577d8e74c79ff15bcbd480874b4`  
		Last Modified: Tue, 27 Jul 2021 02:26:17 GMT  
		Size: 6.7 MB (6667884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62bd7bf9c00152c4fb338b2c1a01d5b241ceda5c58d9e700a353072ab80fb4b9`  
		Last Modified: Tue, 27 Jul 2021 02:26:17 GMT  
		Size: 3.7 MB (3670853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:372602ac4ce9a3a693cb97ec9b3e71b449fdafbaded2ce2937fec39cec9c9b6e`  
		Last Modified: Tue, 27 Jul 2021 02:26:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a80c4de70a1ded78cf0175b1f5fda38b3119857dd2d8d9f1fafcdc39eafef0e`  
		Last Modified: Tue, 27 Jul 2021 02:26:13 GMT  
		Size: 2.6 MB (2569871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc8dec87672a96e86220faa6c3e98577b2a9090fc81d81efb4681fe59e732b7`  
		Last Modified: Tue, 27 Jul 2021 02:26:12 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bd48726927856271f322485a6de75cece86f85c05479ff7e70e2e6d5ebbb424`  
		Last Modified: Mon, 09 Aug 2021 19:46:33 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f067682d4150a7de01414baa115d5a6375406c67fabc09fa0e7652d396e00c`  
		Last Modified: Mon, 09 Aug 2021 19:46:50 GMT  
		Size: 89.3 MB (89254317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9adb83fc0fd3a0ed26d72ceeaf19a3a310f541466d600710ce7e75e7522f3c09`  
		Last Modified: Mon, 09 Aug 2021 19:46:33 GMT  
		Size: 5.6 KB (5613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4523f2d5de9af7d4a2a77dfd0db6d8dd034f14df578bbfff3fcc6793ba0d352`  
		Last Modified: Mon, 09 Aug 2021 19:46:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4-focal`

```console
$ docker pull mariadb@sha256:c5d8ca208661cce5f59a8b935a4036cf2a5a36d06189883a821596f8e460ee33
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:f757259fb431216040a77292d79428710cdcc9f3c1db17811c2029e7131f9950
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.7 MB (124736934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59f9f97d14cefa84e69d9df6e30855f8848c94ff3b52b1c80bb988bd60827682`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:05:00 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 27 Jul 2021 00:05:14 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:05:15 GMT
ENV GOSU_VERSION=1.13
# Tue, 27 Jul 2021 00:05:26 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 27 Jul 2021 00:05:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 27 Jul 2021 00:05:34 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:05:35 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 27 Jul 2021 00:05:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 27 Jul 2021 00:06:56 GMT
ARG MARIADB_MAJOR=10.4
# Tue, 27 Jul 2021 00:06:56 GMT
ENV MARIADB_MAJOR=10.4
# Mon, 09 Aug 2021 19:25:34 GMT
ARG MARIADB_VERSION=1:10.4.21+maria~focal
# Mon, 09 Aug 2021 19:25:34 GMT
ENV MARIADB_VERSION=1:10.4.21+maria~focal
# Mon, 09 Aug 2021 19:25:34 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
# Mon, 09 Aug 2021 19:25:35 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 09 Aug 2021 19:25:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 09 Aug 2021 19:25:58 GMT
VOLUME [/var/lib/mysql]
# Mon, 09 Aug 2021 19:25:58 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Mon, 09 Aug 2021 19:25:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 09 Aug 2021 19:25:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Aug 2021 19:25:59 GMT
EXPOSE 3306
# Mon, 09 Aug 2021 19:25:59 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf20e69555c2118df81cd7906473b0bbef5210f014d45113251b1298fb1c996`  
		Last Modified: Tue, 27 Jul 2021 00:10:02 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69afd1ffc85b8fe385e48d00e89467a4e080c81b2447ce86ebf964f3e43efb9`  
		Last Modified: Tue, 27 Jul 2021 00:10:04 GMT  
		Size: 5.5 MB (5488764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e720dc7fcd8609016e69543f354117290ffee7c9ea1bdd97d7ca84bcc06d616`  
		Last Modified: Tue, 27 Jul 2021 00:10:03 GMT  
		Size: 3.6 MB (3582379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a81d177e410065c8eec2b5c018ab6ac60b2a5161184890bc3bf7627e78fb2dd`  
		Last Modified: Tue, 27 Jul 2021 00:10:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827c8c103c898d23db5f0cfc69b6faa45038d27b1ec3c15cb5d5b29ee60fca0b`  
		Last Modified: Tue, 27 Jul 2021 00:09:59 GMT  
		Size: 2.3 MB (2274133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2108ccd013748c7fce6a19a3f7434b860401f78326ac7373c486eafa3c719354`  
		Last Modified: Tue, 27 Jul 2021 00:09:59 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9b140ec558f045515897d54da2f1b097d349f88038b068e731417640c41c08`  
		Last Modified: Mon, 09 Aug 2021 19:29:13 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eedef259b7b484e50a0cbf6f8ee8c2667b10d8bb9f321fa1f0aa88999912963`  
		Last Modified: Mon, 09 Aug 2021 19:29:25 GMT  
		Size: 84.8 MB (84813265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1b94f4075293104c9899b2260662705f0b15e3f761324aacd2cc2db7d251fdf`  
		Last Modified: Mon, 09 Aug 2021 19:29:13 GMT  
		Size: 5.6 KB (5612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3699fac03dbbc7d3b70481b014e6954b4ef80a698aad277b545b6ea5f875e0fc`  
		Last Modified: Mon, 09 Aug 2021 19:29:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:d33d4b68778b3d6fa9e69b7f03d5a75fea1293be570e96e536bdf4d103894800
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.3 MB (122257993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f93e9279266c814e51034e150a9a6531c873f22b8851b0110c42e5d8cbffe33c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:44 GMT
ADD file:cec21619ecbd37b4cf8da15153b8957a343cd25c6f714e3ac3969b6003704a58 in / 
# Tue, 31 Aug 2021 01:40:45 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:04:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 31 Aug 2021 03:04:38 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:04:38 GMT
ENV GOSU_VERSION=1.13
# Tue, 31 Aug 2021 03:04:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 31 Aug 2021 03:04:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 31 Aug 2021 03:04:57 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:04:57 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 31 Aug 2021 03:05:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 31 Aug 2021 03:06:12 GMT
ARG MARIADB_MAJOR=10.4
# Tue, 31 Aug 2021 03:06:13 GMT
ENV MARIADB_MAJOR=10.4
# Tue, 31 Aug 2021 03:06:13 GMT
ARG MARIADB_VERSION=1:10.4.21+maria~focal
# Tue, 31 Aug 2021 03:06:13 GMT
ENV MARIADB_VERSION=1:10.4.21+maria~focal
# Tue, 31 Aug 2021 03:06:13 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
# Tue, 31 Aug 2021 03:06:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 31 Aug 2021 03:06:35 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 31 Aug 2021 03:06:36 GMT
VOLUME [/var/lib/mysql]
# Tue, 31 Aug 2021 03:06:36 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Tue, 31 Aug 2021 03:06:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 31 Aug 2021 03:06:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Aug 2021 03:06:37 GMT
EXPOSE 3306
# Tue, 31 Aug 2021 03:06:38 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ab2d02b1ec420fdb84c9f52abda403b6aef20f5de904a2ecda5ae4f5cd6e4d46`  
		Last Modified: Tue, 31 Aug 2021 01:42:34 GMT  
		Size: 27.2 MB (27173099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d16f1b8a1bc9060d0c98a0e09c73ceab3d694a99f57672d6e44f2f5dcf09eae`  
		Last Modified: Tue, 31 Aug 2021 03:09:41 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16d8285f3be08ea7340eaf6dced5161164096c3fb3345fe8c5d6d64496bc143`  
		Last Modified: Tue, 31 Aug 2021 03:09:40 GMT  
		Size: 5.5 MB (5455084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ffd6c9eed67b115939ab5f6d4bb8ffd2f0f152fe9a61024122b558e83ce912e`  
		Last Modified: Tue, 31 Aug 2021 03:09:39 GMT  
		Size: 3.4 MB (3368457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdbc2935c20fd14d96044dcdb65fb79a0f676bcdf334058da282716411d3ff9b`  
		Last Modified: Tue, 31 Aug 2021 03:09:39 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b302bb5f11cae70b4c8ec1079e6de6c62dacfdce3e8f3ccdfabd6ce44b63d2`  
		Last Modified: Tue, 31 Aug 2021 03:09:37 GMT  
		Size: 2.2 MB (2203569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21de8a622698dffd65e882759b0b6e4fe0e56b60d892f2e4446f94439a1270f`  
		Last Modified: Tue, 31 Aug 2021 03:09:36 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603fdf9d39e401c1b6b363713b28ab5661faf0b8a1990513574d46b811791b8c`  
		Last Modified: Tue, 31 Aug 2021 03:10:59 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b2986aa34c7795fb597d052475d4e402697ef596122ca7f265fa0767ae468b`  
		Last Modified: Tue, 31 Aug 2021 03:11:13 GMT  
		Size: 84.0 MB (84047333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02e6f22166fb1fb2f67bf8c6fbbc5901ee34862717159fce3c85c4fce0c5f173`  
		Last Modified: Tue, 31 Aug 2021 03:10:59 GMT  
		Size: 5.6 KB (5607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147f1688dace9eb048fa4d04a4e80f2ecc67c91745a3d9c511773b1958f78363`  
		Last Modified: Tue, 31 Aug 2021 03:10:59 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:c6313d6768416158bb0c4b766d0c73e2b37599a3e57073adcbd2f20a3eb90436
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.5 MB (135463813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:375c0548a54460915cdbdb18da2c09f8ee0740f29908f6fd430d24253ac55f79`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 26 Jul 2021 23:12:46 GMT
ADD file:68eb628c2202763afa91d554dde9668d8a468fe53fdbd2fe98627a5f91d224b4 in / 
# Mon, 26 Jul 2021 23:12:49 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 02:05:55 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 27 Jul 2021 02:06:47 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:06:50 GMT
ENV GOSU_VERSION=1.13
# Tue, 27 Jul 2021 02:07:32 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 27 Jul 2021 02:07:42 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 27 Jul 2021 02:08:11 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:08:14 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 27 Jul 2021 02:08:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 27 Jul 2021 02:15:03 GMT
ARG MARIADB_MAJOR=10.4
# Tue, 27 Jul 2021 02:15:06 GMT
ENV MARIADB_MAJOR=10.4
# Mon, 09 Aug 2021 19:28:45 GMT
ARG MARIADB_VERSION=1:10.4.21+maria~focal
# Mon, 09 Aug 2021 19:28:48 GMT
ENV MARIADB_VERSION=1:10.4.21+maria~focal
# Mon, 09 Aug 2021 19:28:52 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
# Mon, 09 Aug 2021 19:28:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 09 Aug 2021 19:32:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 09 Aug 2021 19:32:31 GMT
VOLUME [/var/lib/mysql]
# Mon, 09 Aug 2021 19:32:33 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Mon, 09 Aug 2021 19:32:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 09 Aug 2021 19:32:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Aug 2021 19:32:48 GMT
EXPOSE 3306
# Mon, 09 Aug 2021 19:32:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:1a396eed835b3b7b4101a9863d174e145ddbb1de1502a63bae726b0f81e7ca93`  
		Last Modified: Mon, 26 Jul 2021 23:15:51 GMT  
		Size: 33.3 MB (33290427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65be85b12a63573ebccb059357c5c0db6046f4a074454eea617c402e3bf99c1f`  
		Last Modified: Tue, 27 Jul 2021 02:26:16 GMT  
		Size: 1.8 KB (1760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:803c8e5bf0c59b9b01b70cac07bb24bc696bc577d8e74c79ff15bcbd480874b4`  
		Last Modified: Tue, 27 Jul 2021 02:26:17 GMT  
		Size: 6.7 MB (6667884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62bd7bf9c00152c4fb338b2c1a01d5b241ceda5c58d9e700a353072ab80fb4b9`  
		Last Modified: Tue, 27 Jul 2021 02:26:17 GMT  
		Size: 3.7 MB (3670853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:372602ac4ce9a3a693cb97ec9b3e71b449fdafbaded2ce2937fec39cec9c9b6e`  
		Last Modified: Tue, 27 Jul 2021 02:26:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a80c4de70a1ded78cf0175b1f5fda38b3119857dd2d8d9f1fafcdc39eafef0e`  
		Last Modified: Tue, 27 Jul 2021 02:26:13 GMT  
		Size: 2.6 MB (2569871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc8dec87672a96e86220faa6c3e98577b2a9090fc81d81efb4681fe59e732b7`  
		Last Modified: Tue, 27 Jul 2021 02:26:12 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bd48726927856271f322485a6de75cece86f85c05479ff7e70e2e6d5ebbb424`  
		Last Modified: Mon, 09 Aug 2021 19:46:33 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f067682d4150a7de01414baa115d5a6375406c67fabc09fa0e7652d396e00c`  
		Last Modified: Mon, 09 Aug 2021 19:46:50 GMT  
		Size: 89.3 MB (89254317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9adb83fc0fd3a0ed26d72ceeaf19a3a310f541466d600710ce7e75e7522f3c09`  
		Last Modified: Mon, 09 Aug 2021 19:46:33 GMT  
		Size: 5.6 KB (5613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4523f2d5de9af7d4a2a77dfd0db6d8dd034f14df578bbfff3fcc6793ba0d352`  
		Last Modified: Mon, 09 Aug 2021 19:46:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4.21`

```console
$ docker pull mariadb@sha256:c5d8ca208661cce5f59a8b935a4036cf2a5a36d06189883a821596f8e460ee33
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4.21` - linux; amd64

```console
$ docker pull mariadb@sha256:f757259fb431216040a77292d79428710cdcc9f3c1db17811c2029e7131f9950
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.7 MB (124736934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59f9f97d14cefa84e69d9df6e30855f8848c94ff3b52b1c80bb988bd60827682`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:05:00 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 27 Jul 2021 00:05:14 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:05:15 GMT
ENV GOSU_VERSION=1.13
# Tue, 27 Jul 2021 00:05:26 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 27 Jul 2021 00:05:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 27 Jul 2021 00:05:34 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:05:35 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 27 Jul 2021 00:05:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 27 Jul 2021 00:06:56 GMT
ARG MARIADB_MAJOR=10.4
# Tue, 27 Jul 2021 00:06:56 GMT
ENV MARIADB_MAJOR=10.4
# Mon, 09 Aug 2021 19:25:34 GMT
ARG MARIADB_VERSION=1:10.4.21+maria~focal
# Mon, 09 Aug 2021 19:25:34 GMT
ENV MARIADB_VERSION=1:10.4.21+maria~focal
# Mon, 09 Aug 2021 19:25:34 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
# Mon, 09 Aug 2021 19:25:35 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 09 Aug 2021 19:25:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 09 Aug 2021 19:25:58 GMT
VOLUME [/var/lib/mysql]
# Mon, 09 Aug 2021 19:25:58 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Mon, 09 Aug 2021 19:25:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 09 Aug 2021 19:25:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Aug 2021 19:25:59 GMT
EXPOSE 3306
# Mon, 09 Aug 2021 19:25:59 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf20e69555c2118df81cd7906473b0bbef5210f014d45113251b1298fb1c996`  
		Last Modified: Tue, 27 Jul 2021 00:10:02 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69afd1ffc85b8fe385e48d00e89467a4e080c81b2447ce86ebf964f3e43efb9`  
		Last Modified: Tue, 27 Jul 2021 00:10:04 GMT  
		Size: 5.5 MB (5488764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e720dc7fcd8609016e69543f354117290ffee7c9ea1bdd97d7ca84bcc06d616`  
		Last Modified: Tue, 27 Jul 2021 00:10:03 GMT  
		Size: 3.6 MB (3582379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a81d177e410065c8eec2b5c018ab6ac60b2a5161184890bc3bf7627e78fb2dd`  
		Last Modified: Tue, 27 Jul 2021 00:10:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827c8c103c898d23db5f0cfc69b6faa45038d27b1ec3c15cb5d5b29ee60fca0b`  
		Last Modified: Tue, 27 Jul 2021 00:09:59 GMT  
		Size: 2.3 MB (2274133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2108ccd013748c7fce6a19a3f7434b860401f78326ac7373c486eafa3c719354`  
		Last Modified: Tue, 27 Jul 2021 00:09:59 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9b140ec558f045515897d54da2f1b097d349f88038b068e731417640c41c08`  
		Last Modified: Mon, 09 Aug 2021 19:29:13 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eedef259b7b484e50a0cbf6f8ee8c2667b10d8bb9f321fa1f0aa88999912963`  
		Last Modified: Mon, 09 Aug 2021 19:29:25 GMT  
		Size: 84.8 MB (84813265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1b94f4075293104c9899b2260662705f0b15e3f761324aacd2cc2db7d251fdf`  
		Last Modified: Mon, 09 Aug 2021 19:29:13 GMT  
		Size: 5.6 KB (5612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3699fac03dbbc7d3b70481b014e6954b4ef80a698aad277b545b6ea5f875e0fc`  
		Last Modified: Mon, 09 Aug 2021 19:29:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.21` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:d33d4b68778b3d6fa9e69b7f03d5a75fea1293be570e96e536bdf4d103894800
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.3 MB (122257993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f93e9279266c814e51034e150a9a6531c873f22b8851b0110c42e5d8cbffe33c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:44 GMT
ADD file:cec21619ecbd37b4cf8da15153b8957a343cd25c6f714e3ac3969b6003704a58 in / 
# Tue, 31 Aug 2021 01:40:45 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:04:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 31 Aug 2021 03:04:38 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:04:38 GMT
ENV GOSU_VERSION=1.13
# Tue, 31 Aug 2021 03:04:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 31 Aug 2021 03:04:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 31 Aug 2021 03:04:57 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:04:57 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 31 Aug 2021 03:05:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 31 Aug 2021 03:06:12 GMT
ARG MARIADB_MAJOR=10.4
# Tue, 31 Aug 2021 03:06:13 GMT
ENV MARIADB_MAJOR=10.4
# Tue, 31 Aug 2021 03:06:13 GMT
ARG MARIADB_VERSION=1:10.4.21+maria~focal
# Tue, 31 Aug 2021 03:06:13 GMT
ENV MARIADB_VERSION=1:10.4.21+maria~focal
# Tue, 31 Aug 2021 03:06:13 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
# Tue, 31 Aug 2021 03:06:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 31 Aug 2021 03:06:35 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 31 Aug 2021 03:06:36 GMT
VOLUME [/var/lib/mysql]
# Tue, 31 Aug 2021 03:06:36 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Tue, 31 Aug 2021 03:06:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 31 Aug 2021 03:06:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Aug 2021 03:06:37 GMT
EXPOSE 3306
# Tue, 31 Aug 2021 03:06:38 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ab2d02b1ec420fdb84c9f52abda403b6aef20f5de904a2ecda5ae4f5cd6e4d46`  
		Last Modified: Tue, 31 Aug 2021 01:42:34 GMT  
		Size: 27.2 MB (27173099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d16f1b8a1bc9060d0c98a0e09c73ceab3d694a99f57672d6e44f2f5dcf09eae`  
		Last Modified: Tue, 31 Aug 2021 03:09:41 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16d8285f3be08ea7340eaf6dced5161164096c3fb3345fe8c5d6d64496bc143`  
		Last Modified: Tue, 31 Aug 2021 03:09:40 GMT  
		Size: 5.5 MB (5455084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ffd6c9eed67b115939ab5f6d4bb8ffd2f0f152fe9a61024122b558e83ce912e`  
		Last Modified: Tue, 31 Aug 2021 03:09:39 GMT  
		Size: 3.4 MB (3368457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdbc2935c20fd14d96044dcdb65fb79a0f676bcdf334058da282716411d3ff9b`  
		Last Modified: Tue, 31 Aug 2021 03:09:39 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b302bb5f11cae70b4c8ec1079e6de6c62dacfdce3e8f3ccdfabd6ce44b63d2`  
		Last Modified: Tue, 31 Aug 2021 03:09:37 GMT  
		Size: 2.2 MB (2203569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21de8a622698dffd65e882759b0b6e4fe0e56b60d892f2e4446f94439a1270f`  
		Last Modified: Tue, 31 Aug 2021 03:09:36 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603fdf9d39e401c1b6b363713b28ab5661faf0b8a1990513574d46b811791b8c`  
		Last Modified: Tue, 31 Aug 2021 03:10:59 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b2986aa34c7795fb597d052475d4e402697ef596122ca7f265fa0767ae468b`  
		Last Modified: Tue, 31 Aug 2021 03:11:13 GMT  
		Size: 84.0 MB (84047333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02e6f22166fb1fb2f67bf8c6fbbc5901ee34862717159fce3c85c4fce0c5f173`  
		Last Modified: Tue, 31 Aug 2021 03:10:59 GMT  
		Size: 5.6 KB (5607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147f1688dace9eb048fa4d04a4e80f2ecc67c91745a3d9c511773b1958f78363`  
		Last Modified: Tue, 31 Aug 2021 03:10:59 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.21` - linux; ppc64le

```console
$ docker pull mariadb@sha256:c6313d6768416158bb0c4b766d0c73e2b37599a3e57073adcbd2f20a3eb90436
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.5 MB (135463813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:375c0548a54460915cdbdb18da2c09f8ee0740f29908f6fd430d24253ac55f79`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 26 Jul 2021 23:12:46 GMT
ADD file:68eb628c2202763afa91d554dde9668d8a468fe53fdbd2fe98627a5f91d224b4 in / 
# Mon, 26 Jul 2021 23:12:49 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 02:05:55 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 27 Jul 2021 02:06:47 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:06:50 GMT
ENV GOSU_VERSION=1.13
# Tue, 27 Jul 2021 02:07:32 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 27 Jul 2021 02:07:42 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 27 Jul 2021 02:08:11 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:08:14 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 27 Jul 2021 02:08:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 27 Jul 2021 02:15:03 GMT
ARG MARIADB_MAJOR=10.4
# Tue, 27 Jul 2021 02:15:06 GMT
ENV MARIADB_MAJOR=10.4
# Mon, 09 Aug 2021 19:28:45 GMT
ARG MARIADB_VERSION=1:10.4.21+maria~focal
# Mon, 09 Aug 2021 19:28:48 GMT
ENV MARIADB_VERSION=1:10.4.21+maria~focal
# Mon, 09 Aug 2021 19:28:52 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
# Mon, 09 Aug 2021 19:28:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 09 Aug 2021 19:32:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 09 Aug 2021 19:32:31 GMT
VOLUME [/var/lib/mysql]
# Mon, 09 Aug 2021 19:32:33 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Mon, 09 Aug 2021 19:32:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 09 Aug 2021 19:32:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Aug 2021 19:32:48 GMT
EXPOSE 3306
# Mon, 09 Aug 2021 19:32:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:1a396eed835b3b7b4101a9863d174e145ddbb1de1502a63bae726b0f81e7ca93`  
		Last Modified: Mon, 26 Jul 2021 23:15:51 GMT  
		Size: 33.3 MB (33290427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65be85b12a63573ebccb059357c5c0db6046f4a074454eea617c402e3bf99c1f`  
		Last Modified: Tue, 27 Jul 2021 02:26:16 GMT  
		Size: 1.8 KB (1760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:803c8e5bf0c59b9b01b70cac07bb24bc696bc577d8e74c79ff15bcbd480874b4`  
		Last Modified: Tue, 27 Jul 2021 02:26:17 GMT  
		Size: 6.7 MB (6667884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62bd7bf9c00152c4fb338b2c1a01d5b241ceda5c58d9e700a353072ab80fb4b9`  
		Last Modified: Tue, 27 Jul 2021 02:26:17 GMT  
		Size: 3.7 MB (3670853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:372602ac4ce9a3a693cb97ec9b3e71b449fdafbaded2ce2937fec39cec9c9b6e`  
		Last Modified: Tue, 27 Jul 2021 02:26:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a80c4de70a1ded78cf0175b1f5fda38b3119857dd2d8d9f1fafcdc39eafef0e`  
		Last Modified: Tue, 27 Jul 2021 02:26:13 GMT  
		Size: 2.6 MB (2569871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc8dec87672a96e86220faa6c3e98577b2a9090fc81d81efb4681fe59e732b7`  
		Last Modified: Tue, 27 Jul 2021 02:26:12 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bd48726927856271f322485a6de75cece86f85c05479ff7e70e2e6d5ebbb424`  
		Last Modified: Mon, 09 Aug 2021 19:46:33 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f067682d4150a7de01414baa115d5a6375406c67fabc09fa0e7652d396e00c`  
		Last Modified: Mon, 09 Aug 2021 19:46:50 GMT  
		Size: 89.3 MB (89254317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9adb83fc0fd3a0ed26d72ceeaf19a3a310f541466d600710ce7e75e7522f3c09`  
		Last Modified: Mon, 09 Aug 2021 19:46:33 GMT  
		Size: 5.6 KB (5613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4523f2d5de9af7d4a2a77dfd0db6d8dd034f14df578bbfff3fcc6793ba0d352`  
		Last Modified: Mon, 09 Aug 2021 19:46:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4.21-focal`

```console
$ docker pull mariadb@sha256:c5d8ca208661cce5f59a8b935a4036cf2a5a36d06189883a821596f8e460ee33
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4.21-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:f757259fb431216040a77292d79428710cdcc9f3c1db17811c2029e7131f9950
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.7 MB (124736934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59f9f97d14cefa84e69d9df6e30855f8848c94ff3b52b1c80bb988bd60827682`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:05:00 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 27 Jul 2021 00:05:14 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:05:15 GMT
ENV GOSU_VERSION=1.13
# Tue, 27 Jul 2021 00:05:26 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 27 Jul 2021 00:05:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 27 Jul 2021 00:05:34 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:05:35 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 27 Jul 2021 00:05:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 27 Jul 2021 00:06:56 GMT
ARG MARIADB_MAJOR=10.4
# Tue, 27 Jul 2021 00:06:56 GMT
ENV MARIADB_MAJOR=10.4
# Mon, 09 Aug 2021 19:25:34 GMT
ARG MARIADB_VERSION=1:10.4.21+maria~focal
# Mon, 09 Aug 2021 19:25:34 GMT
ENV MARIADB_VERSION=1:10.4.21+maria~focal
# Mon, 09 Aug 2021 19:25:34 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
# Mon, 09 Aug 2021 19:25:35 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 09 Aug 2021 19:25:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 09 Aug 2021 19:25:58 GMT
VOLUME [/var/lib/mysql]
# Mon, 09 Aug 2021 19:25:58 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Mon, 09 Aug 2021 19:25:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 09 Aug 2021 19:25:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Aug 2021 19:25:59 GMT
EXPOSE 3306
# Mon, 09 Aug 2021 19:25:59 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf20e69555c2118df81cd7906473b0bbef5210f014d45113251b1298fb1c996`  
		Last Modified: Tue, 27 Jul 2021 00:10:02 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69afd1ffc85b8fe385e48d00e89467a4e080c81b2447ce86ebf964f3e43efb9`  
		Last Modified: Tue, 27 Jul 2021 00:10:04 GMT  
		Size: 5.5 MB (5488764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e720dc7fcd8609016e69543f354117290ffee7c9ea1bdd97d7ca84bcc06d616`  
		Last Modified: Tue, 27 Jul 2021 00:10:03 GMT  
		Size: 3.6 MB (3582379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a81d177e410065c8eec2b5c018ab6ac60b2a5161184890bc3bf7627e78fb2dd`  
		Last Modified: Tue, 27 Jul 2021 00:10:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827c8c103c898d23db5f0cfc69b6faa45038d27b1ec3c15cb5d5b29ee60fca0b`  
		Last Modified: Tue, 27 Jul 2021 00:09:59 GMT  
		Size: 2.3 MB (2274133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2108ccd013748c7fce6a19a3f7434b860401f78326ac7373c486eafa3c719354`  
		Last Modified: Tue, 27 Jul 2021 00:09:59 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9b140ec558f045515897d54da2f1b097d349f88038b068e731417640c41c08`  
		Last Modified: Mon, 09 Aug 2021 19:29:13 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eedef259b7b484e50a0cbf6f8ee8c2667b10d8bb9f321fa1f0aa88999912963`  
		Last Modified: Mon, 09 Aug 2021 19:29:25 GMT  
		Size: 84.8 MB (84813265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1b94f4075293104c9899b2260662705f0b15e3f761324aacd2cc2db7d251fdf`  
		Last Modified: Mon, 09 Aug 2021 19:29:13 GMT  
		Size: 5.6 KB (5612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3699fac03dbbc7d3b70481b014e6954b4ef80a698aad277b545b6ea5f875e0fc`  
		Last Modified: Mon, 09 Aug 2021 19:29:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.21-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:d33d4b68778b3d6fa9e69b7f03d5a75fea1293be570e96e536bdf4d103894800
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.3 MB (122257993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f93e9279266c814e51034e150a9a6531c873f22b8851b0110c42e5d8cbffe33c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:44 GMT
ADD file:cec21619ecbd37b4cf8da15153b8957a343cd25c6f714e3ac3969b6003704a58 in / 
# Tue, 31 Aug 2021 01:40:45 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:04:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 31 Aug 2021 03:04:38 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:04:38 GMT
ENV GOSU_VERSION=1.13
# Tue, 31 Aug 2021 03:04:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 31 Aug 2021 03:04:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 31 Aug 2021 03:04:57 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:04:57 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 31 Aug 2021 03:05:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 31 Aug 2021 03:06:12 GMT
ARG MARIADB_MAJOR=10.4
# Tue, 31 Aug 2021 03:06:13 GMT
ENV MARIADB_MAJOR=10.4
# Tue, 31 Aug 2021 03:06:13 GMT
ARG MARIADB_VERSION=1:10.4.21+maria~focal
# Tue, 31 Aug 2021 03:06:13 GMT
ENV MARIADB_VERSION=1:10.4.21+maria~focal
# Tue, 31 Aug 2021 03:06:13 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
# Tue, 31 Aug 2021 03:06:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 31 Aug 2021 03:06:35 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 31 Aug 2021 03:06:36 GMT
VOLUME [/var/lib/mysql]
# Tue, 31 Aug 2021 03:06:36 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Tue, 31 Aug 2021 03:06:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 31 Aug 2021 03:06:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Aug 2021 03:06:37 GMT
EXPOSE 3306
# Tue, 31 Aug 2021 03:06:38 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ab2d02b1ec420fdb84c9f52abda403b6aef20f5de904a2ecda5ae4f5cd6e4d46`  
		Last Modified: Tue, 31 Aug 2021 01:42:34 GMT  
		Size: 27.2 MB (27173099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d16f1b8a1bc9060d0c98a0e09c73ceab3d694a99f57672d6e44f2f5dcf09eae`  
		Last Modified: Tue, 31 Aug 2021 03:09:41 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16d8285f3be08ea7340eaf6dced5161164096c3fb3345fe8c5d6d64496bc143`  
		Last Modified: Tue, 31 Aug 2021 03:09:40 GMT  
		Size: 5.5 MB (5455084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ffd6c9eed67b115939ab5f6d4bb8ffd2f0f152fe9a61024122b558e83ce912e`  
		Last Modified: Tue, 31 Aug 2021 03:09:39 GMT  
		Size: 3.4 MB (3368457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdbc2935c20fd14d96044dcdb65fb79a0f676bcdf334058da282716411d3ff9b`  
		Last Modified: Tue, 31 Aug 2021 03:09:39 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b302bb5f11cae70b4c8ec1079e6de6c62dacfdce3e8f3ccdfabd6ce44b63d2`  
		Last Modified: Tue, 31 Aug 2021 03:09:37 GMT  
		Size: 2.2 MB (2203569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21de8a622698dffd65e882759b0b6e4fe0e56b60d892f2e4446f94439a1270f`  
		Last Modified: Tue, 31 Aug 2021 03:09:36 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603fdf9d39e401c1b6b363713b28ab5661faf0b8a1990513574d46b811791b8c`  
		Last Modified: Tue, 31 Aug 2021 03:10:59 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b2986aa34c7795fb597d052475d4e402697ef596122ca7f265fa0767ae468b`  
		Last Modified: Tue, 31 Aug 2021 03:11:13 GMT  
		Size: 84.0 MB (84047333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02e6f22166fb1fb2f67bf8c6fbbc5901ee34862717159fce3c85c4fce0c5f173`  
		Last Modified: Tue, 31 Aug 2021 03:10:59 GMT  
		Size: 5.6 KB (5607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147f1688dace9eb048fa4d04a4e80f2ecc67c91745a3d9c511773b1958f78363`  
		Last Modified: Tue, 31 Aug 2021 03:10:59 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.21-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:c6313d6768416158bb0c4b766d0c73e2b37599a3e57073adcbd2f20a3eb90436
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.5 MB (135463813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:375c0548a54460915cdbdb18da2c09f8ee0740f29908f6fd430d24253ac55f79`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 26 Jul 2021 23:12:46 GMT
ADD file:68eb628c2202763afa91d554dde9668d8a468fe53fdbd2fe98627a5f91d224b4 in / 
# Mon, 26 Jul 2021 23:12:49 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 02:05:55 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 27 Jul 2021 02:06:47 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:06:50 GMT
ENV GOSU_VERSION=1.13
# Tue, 27 Jul 2021 02:07:32 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 27 Jul 2021 02:07:42 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 27 Jul 2021 02:08:11 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:08:14 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 27 Jul 2021 02:08:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 27 Jul 2021 02:15:03 GMT
ARG MARIADB_MAJOR=10.4
# Tue, 27 Jul 2021 02:15:06 GMT
ENV MARIADB_MAJOR=10.4
# Mon, 09 Aug 2021 19:28:45 GMT
ARG MARIADB_VERSION=1:10.4.21+maria~focal
# Mon, 09 Aug 2021 19:28:48 GMT
ENV MARIADB_VERSION=1:10.4.21+maria~focal
# Mon, 09 Aug 2021 19:28:52 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
# Mon, 09 Aug 2021 19:28:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 09 Aug 2021 19:32:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 09 Aug 2021 19:32:31 GMT
VOLUME [/var/lib/mysql]
# Mon, 09 Aug 2021 19:32:33 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Mon, 09 Aug 2021 19:32:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 09 Aug 2021 19:32:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Aug 2021 19:32:48 GMT
EXPOSE 3306
# Mon, 09 Aug 2021 19:32:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:1a396eed835b3b7b4101a9863d174e145ddbb1de1502a63bae726b0f81e7ca93`  
		Last Modified: Mon, 26 Jul 2021 23:15:51 GMT  
		Size: 33.3 MB (33290427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65be85b12a63573ebccb059357c5c0db6046f4a074454eea617c402e3bf99c1f`  
		Last Modified: Tue, 27 Jul 2021 02:26:16 GMT  
		Size: 1.8 KB (1760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:803c8e5bf0c59b9b01b70cac07bb24bc696bc577d8e74c79ff15bcbd480874b4`  
		Last Modified: Tue, 27 Jul 2021 02:26:17 GMT  
		Size: 6.7 MB (6667884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62bd7bf9c00152c4fb338b2c1a01d5b241ceda5c58d9e700a353072ab80fb4b9`  
		Last Modified: Tue, 27 Jul 2021 02:26:17 GMT  
		Size: 3.7 MB (3670853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:372602ac4ce9a3a693cb97ec9b3e71b449fdafbaded2ce2937fec39cec9c9b6e`  
		Last Modified: Tue, 27 Jul 2021 02:26:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a80c4de70a1ded78cf0175b1f5fda38b3119857dd2d8d9f1fafcdc39eafef0e`  
		Last Modified: Tue, 27 Jul 2021 02:26:13 GMT  
		Size: 2.6 MB (2569871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc8dec87672a96e86220faa6c3e98577b2a9090fc81d81efb4681fe59e732b7`  
		Last Modified: Tue, 27 Jul 2021 02:26:12 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bd48726927856271f322485a6de75cece86f85c05479ff7e70e2e6d5ebbb424`  
		Last Modified: Mon, 09 Aug 2021 19:46:33 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f067682d4150a7de01414baa115d5a6375406c67fabc09fa0e7652d396e00c`  
		Last Modified: Mon, 09 Aug 2021 19:46:50 GMT  
		Size: 89.3 MB (89254317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9adb83fc0fd3a0ed26d72ceeaf19a3a310f541466d600710ce7e75e7522f3c09`  
		Last Modified: Mon, 09 Aug 2021 19:46:33 GMT  
		Size: 5.6 KB (5613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4523f2d5de9af7d4a2a77dfd0db6d8dd034f14df578bbfff3fcc6793ba0d352`  
		Last Modified: Mon, 09 Aug 2021 19:46:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5`

```console
$ docker pull mariadb@sha256:334eba05f9f47284cda296cb6b5857a28b681f045b1a59b835131e2b22331311
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.5` - linux; amd64

```console
$ docker pull mariadb@sha256:714b7e3ed906a2d4a0c11ded8dcadc804dde593be5474ef88f911ce6b54dadad
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.9 MB (126860537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9643f47b304c4a77314f35c725cf5dc7e63b29f9a0350e52b99d1e8ca6067276`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:05:00 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 27 Jul 2021 00:05:14 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:05:15 GMT
ENV GOSU_VERSION=1.13
# Tue, 27 Jul 2021 00:05:26 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 27 Jul 2021 00:05:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 27 Jul 2021 00:05:34 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:05:35 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 27 Jul 2021 00:05:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 27 Jul 2021 00:06:25 GMT
ARG MARIADB_MAJOR=10.5
# Tue, 27 Jul 2021 00:06:25 GMT
ENV MARIADB_MAJOR=10.5
# Mon, 09 Aug 2021 19:25:04 GMT
ARG MARIADB_VERSION=1:10.5.12+maria~focal
# Mon, 09 Aug 2021 19:25:04 GMT
ENV MARIADB_VERSION=1:10.5.12+maria~focal
# Mon, 09 Aug 2021 19:25:04 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
# Mon, 09 Aug 2021 19:25:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 09 Aug 2021 19:25:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 09 Aug 2021 19:25:27 GMT
VOLUME [/var/lib/mysql]
# Mon, 09 Aug 2021 19:25:27 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Mon, 09 Aug 2021 19:25:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Aug 2021 19:25:28 GMT
EXPOSE 3306
# Mon, 09 Aug 2021 19:25:28 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf20e69555c2118df81cd7906473b0bbef5210f014d45113251b1298fb1c996`  
		Last Modified: Tue, 27 Jul 2021 00:10:02 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69afd1ffc85b8fe385e48d00e89467a4e080c81b2447ce86ebf964f3e43efb9`  
		Last Modified: Tue, 27 Jul 2021 00:10:04 GMT  
		Size: 5.5 MB (5488764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e720dc7fcd8609016e69543f354117290ffee7c9ea1bdd97d7ca84bcc06d616`  
		Last Modified: Tue, 27 Jul 2021 00:10:03 GMT  
		Size: 3.6 MB (3582379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a81d177e410065c8eec2b5c018ab6ac60b2a5161184890bc3bf7627e78fb2dd`  
		Last Modified: Tue, 27 Jul 2021 00:10:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827c8c103c898d23db5f0cfc69b6faa45038d27b1ec3c15cb5d5b29ee60fca0b`  
		Last Modified: Tue, 27 Jul 2021 00:09:59 GMT  
		Size: 2.3 MB (2274133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2108ccd013748c7fce6a19a3f7434b860401f78326ac7373c486eafa3c719354`  
		Last Modified: Tue, 27 Jul 2021 00:09:59 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd18312032de063877ef5ff92e06d0c5b2e33d2f09d4ebaca4062371d5919e2`  
		Last Modified: Mon, 09 Aug 2021 19:28:44 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63f5eb96adc50bc11b45b80d6c343b69bfa553f315a2d8a25e9f48221c720b17`  
		Last Modified: Mon, 09 Aug 2021 19:28:57 GMT  
		Size: 86.9 MB (86936993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a7dacc2466ab5456742e63e09e203e507a8be337cc4f5bddd587740684f8f9`  
		Last Modified: Mon, 09 Aug 2021 19:28:44 GMT  
		Size: 5.6 KB (5611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:155422bcef7935decf5e25e3b349dbcde5f99df70fa0b8eecc5b54f6656e23ab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124311821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27733d6f266bbcd2d324301e21ac627d3ca04a6b607888667e011a638b1bbeb8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:44 GMT
ADD file:cec21619ecbd37b4cf8da15153b8957a343cd25c6f714e3ac3969b6003704a58 in / 
# Tue, 31 Aug 2021 01:40:45 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:04:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 31 Aug 2021 03:04:38 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:04:38 GMT
ENV GOSU_VERSION=1.13
# Tue, 31 Aug 2021 03:04:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 31 Aug 2021 03:04:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 31 Aug 2021 03:04:57 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:04:57 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 31 Aug 2021 03:05:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 31 Aug 2021 03:05:41 GMT
ARG MARIADB_MAJOR=10.5
# Tue, 31 Aug 2021 03:05:41 GMT
ENV MARIADB_MAJOR=10.5
# Tue, 31 Aug 2021 03:05:42 GMT
ARG MARIADB_VERSION=1:10.5.12+maria~focal
# Tue, 31 Aug 2021 03:05:42 GMT
ENV MARIADB_VERSION=1:10.5.12+maria~focal
# Tue, 31 Aug 2021 03:05:42 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
# Tue, 31 Aug 2021 03:05:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 31 Aug 2021 03:06:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 31 Aug 2021 03:06:03 GMT
VOLUME [/var/lib/mysql]
# Tue, 31 Aug 2021 03:06:04 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Tue, 31 Aug 2021 03:06:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Aug 2021 03:06:04 GMT
EXPOSE 3306
# Tue, 31 Aug 2021 03:06:04 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ab2d02b1ec420fdb84c9f52abda403b6aef20f5de904a2ecda5ae4f5cd6e4d46`  
		Last Modified: Tue, 31 Aug 2021 01:42:34 GMT  
		Size: 27.2 MB (27173099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d16f1b8a1bc9060d0c98a0e09c73ceab3d694a99f57672d6e44f2f5dcf09eae`  
		Last Modified: Tue, 31 Aug 2021 03:09:41 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16d8285f3be08ea7340eaf6dced5161164096c3fb3345fe8c5d6d64496bc143`  
		Last Modified: Tue, 31 Aug 2021 03:09:40 GMT  
		Size: 5.5 MB (5455084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ffd6c9eed67b115939ab5f6d4bb8ffd2f0f152fe9a61024122b558e83ce912e`  
		Last Modified: Tue, 31 Aug 2021 03:09:39 GMT  
		Size: 3.4 MB (3368457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdbc2935c20fd14d96044dcdb65fb79a0f676bcdf334058da282716411d3ff9b`  
		Last Modified: Tue, 31 Aug 2021 03:09:39 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b302bb5f11cae70b4c8ec1079e6de6c62dacfdce3e8f3ccdfabd6ce44b63d2`  
		Last Modified: Tue, 31 Aug 2021 03:09:37 GMT  
		Size: 2.2 MB (2203569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21de8a622698dffd65e882759b0b6e4fe0e56b60d892f2e4446f94439a1270f`  
		Last Modified: Tue, 31 Aug 2021 03:09:36 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d90417b10f36ce35fa1e4bce541ddb0e5a4d650237bbbac7d590fe6b84c03789`  
		Last Modified: Tue, 31 Aug 2021 03:10:24 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe757cf1d42c8bbba22076f6747facadb9dec82a418ca34eb66229b9e7114c6c`  
		Last Modified: Tue, 31 Aug 2021 03:10:39 GMT  
		Size: 86.1 MB (86101283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5caa80c0b81366945776f22bd92fdc75ab775a4a8768f3bd30e6f58bba416225`  
		Last Modified: Tue, 31 Aug 2021 03:10:24 GMT  
		Size: 5.6 KB (5609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; ppc64le

```console
$ docker pull mariadb@sha256:a22827c392d5d8aa35de016791f7037b3a783257bc715118bdca87dbdc3f1623
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.6 MB (137580509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a6ffd715dfd27be255eb10756b6b1dddf856f016349451df5b3d3ca927a22eb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 26 Jul 2021 23:12:46 GMT
ADD file:68eb628c2202763afa91d554dde9668d8a468fe53fdbd2fe98627a5f91d224b4 in / 
# Mon, 26 Jul 2021 23:12:49 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 02:05:55 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 27 Jul 2021 02:06:47 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:06:50 GMT
ENV GOSU_VERSION=1.13
# Tue, 27 Jul 2021 02:07:32 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 27 Jul 2021 02:07:42 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 27 Jul 2021 02:08:11 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:08:14 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 27 Jul 2021 02:08:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 27 Jul 2021 02:11:32 GMT
ARG MARIADB_MAJOR=10.5
# Tue, 27 Jul 2021 02:11:34 GMT
ENV MARIADB_MAJOR=10.5
# Mon, 09 Aug 2021 19:23:36 GMT
ARG MARIADB_VERSION=1:10.5.12+maria~focal
# Mon, 09 Aug 2021 19:23:45 GMT
ENV MARIADB_VERSION=1:10.5.12+maria~focal
# Mon, 09 Aug 2021 19:23:49 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
# Mon, 09 Aug 2021 19:24:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 09 Aug 2021 19:28:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 09 Aug 2021 19:28:14 GMT
VOLUME [/var/lib/mysql]
# Mon, 09 Aug 2021 19:28:18 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Mon, 09 Aug 2021 19:28:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Aug 2021 19:28:30 GMT
EXPOSE 3306
# Mon, 09 Aug 2021 19:28:33 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:1a396eed835b3b7b4101a9863d174e145ddbb1de1502a63bae726b0f81e7ca93`  
		Last Modified: Mon, 26 Jul 2021 23:15:51 GMT  
		Size: 33.3 MB (33290427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65be85b12a63573ebccb059357c5c0db6046f4a074454eea617c402e3bf99c1f`  
		Last Modified: Tue, 27 Jul 2021 02:26:16 GMT  
		Size: 1.8 KB (1760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:803c8e5bf0c59b9b01b70cac07bb24bc696bc577d8e74c79ff15bcbd480874b4`  
		Last Modified: Tue, 27 Jul 2021 02:26:17 GMT  
		Size: 6.7 MB (6667884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62bd7bf9c00152c4fb338b2c1a01d5b241ceda5c58d9e700a353072ab80fb4b9`  
		Last Modified: Tue, 27 Jul 2021 02:26:17 GMT  
		Size: 3.7 MB (3670853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:372602ac4ce9a3a693cb97ec9b3e71b449fdafbaded2ce2937fec39cec9c9b6e`  
		Last Modified: Tue, 27 Jul 2021 02:26:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a80c4de70a1ded78cf0175b1f5fda38b3119857dd2d8d9f1fafcdc39eafef0e`  
		Last Modified: Tue, 27 Jul 2021 02:26:13 GMT  
		Size: 2.6 MB (2569871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc8dec87672a96e86220faa6c3e98577b2a9090fc81d81efb4681fe59e732b7`  
		Last Modified: Tue, 27 Jul 2021 02:26:12 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8e4a78feeb863bb4a36ec743301f11db8142e4252ab6db2dd94470d0ffb950`  
		Last Modified: Mon, 09 Aug 2021 19:45:56 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96967b218a123706ee5fe6b9cf79c4124c016aa86825dec7ba7ddae281301f63`  
		Last Modified: Mon, 09 Aug 2021 19:46:14 GMT  
		Size: 91.4 MB (91371131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b234b373bbf599e2b861274d9dfe19b7b3a14f24555c4b292df94ca2cf425c5`  
		Last Modified: Mon, 09 Aug 2021 19:45:56 GMT  
		Size: 5.6 KB (5614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; s390x

```console
$ docker pull mariadb@sha256:9373b966fe815dcb87a102c954e3da3fc62040cea5d20c0715de3bf8ba678ef5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.1 MB (126054236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7aae9fe04321546d598fe4969a87ca9b73346d340df7178085fb136fd27bb5b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:23 GMT
ADD file:979855f79ebaca36cc7878f71b2326f1cd189970fdb223b37cd64ee12d1c9a2b in / 
# Tue, 31 Aug 2021 01:42:27 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:49:44 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 31 Aug 2021 02:49:51 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:49:51 GMT
ENV GOSU_VERSION=1.13
# Tue, 31 Aug 2021 02:50:04 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 31 Aug 2021 02:50:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 31 Aug 2021 02:50:12 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:50:12 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 31 Aug 2021 02:50:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 31 Aug 2021 02:51:03 GMT
ARG MARIADB_MAJOR=10.5
# Tue, 31 Aug 2021 02:51:03 GMT
ENV MARIADB_MAJOR=10.5
# Tue, 31 Aug 2021 02:51:04 GMT
ARG MARIADB_VERSION=1:10.5.12+maria~focal
# Tue, 31 Aug 2021 02:51:04 GMT
ENV MARIADB_VERSION=1:10.5.12+maria~focal
# Tue, 31 Aug 2021 02:51:04 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
# Tue, 31 Aug 2021 02:51:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 31 Aug 2021 02:51:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 31 Aug 2021 02:51:36 GMT
VOLUME [/var/lib/mysql]
# Tue, 31 Aug 2021 02:51:37 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Tue, 31 Aug 2021 02:51:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Aug 2021 02:51:37 GMT
EXPOSE 3306
# Tue, 31 Aug 2021 02:51:37 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:9fbf86d355c92d30b8de4c0360b0d79e1100e392d0885b6b5b302a1c3781dbf1`  
		Last Modified: Tue, 31 Aug 2021 01:44:13 GMT  
		Size: 27.1 MB (27127470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5652d937cd93c6c333210a7c5783a5defbac72c096a74537a0e99da179e69e15`  
		Last Modified: Tue, 31 Aug 2021 02:52:15 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1b48caf1d89a34f08f8ee38f48260ccfd25cfdc0e5425a1f7e2e1c3bc1c8cf0`  
		Last Modified: Tue, 31 Aug 2021 02:52:16 GMT  
		Size: 5.4 MB (5380989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352b2892aadbd934d1a0415ca24f71baf53ef4b324fe9f8772a37405d8607dba`  
		Last Modified: Tue, 31 Aug 2021 02:52:16 GMT  
		Size: 3.2 MB (3241880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354edb6860dbb419b59714606f392488735bc5e9adc7496059e98f51de24d84a`  
		Last Modified: Tue, 31 Aug 2021 02:52:15 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9934bdf22d9a668fcaab9695424d4074294aef89d849a8c8ba80b0bb31ab2ab9`  
		Last Modified: Tue, 31 Aug 2021 02:52:13 GMT  
		Size: 2.2 MB (2186296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a940a6a2154f17326f40b9d4619aa517978b7eed0f68a8a68738928defef66`  
		Last Modified: Tue, 31 Aug 2021 02:52:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d59cabe74a3e7d613c1b80e665c9d8541a8fb4d41ab6cccf7ef511b3569bc83f`  
		Last Modified: Tue, 31 Aug 2021 02:52:48 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fa3d9203216e56ee658b3d6a772799aa5553bbff52dd9ef9ff3d46d26606344`  
		Last Modified: Tue, 31 Aug 2021 02:53:01 GMT  
		Size: 88.1 MB (88107279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95dfd07848bf5afc8800b1141a2c38c414b30cef83cbd4348dd432a963366095`  
		Last Modified: Tue, 31 Aug 2021 02:52:48 GMT  
		Size: 5.6 KB (5606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5-focal`

```console
$ docker pull mariadb@sha256:334eba05f9f47284cda296cb6b5857a28b681f045b1a59b835131e2b22331311
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.5-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:714b7e3ed906a2d4a0c11ded8dcadc804dde593be5474ef88f911ce6b54dadad
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.9 MB (126860537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9643f47b304c4a77314f35c725cf5dc7e63b29f9a0350e52b99d1e8ca6067276`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:05:00 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 27 Jul 2021 00:05:14 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:05:15 GMT
ENV GOSU_VERSION=1.13
# Tue, 27 Jul 2021 00:05:26 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 27 Jul 2021 00:05:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 27 Jul 2021 00:05:34 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:05:35 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 27 Jul 2021 00:05:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 27 Jul 2021 00:06:25 GMT
ARG MARIADB_MAJOR=10.5
# Tue, 27 Jul 2021 00:06:25 GMT
ENV MARIADB_MAJOR=10.5
# Mon, 09 Aug 2021 19:25:04 GMT
ARG MARIADB_VERSION=1:10.5.12+maria~focal
# Mon, 09 Aug 2021 19:25:04 GMT
ENV MARIADB_VERSION=1:10.5.12+maria~focal
# Mon, 09 Aug 2021 19:25:04 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
# Mon, 09 Aug 2021 19:25:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 09 Aug 2021 19:25:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 09 Aug 2021 19:25:27 GMT
VOLUME [/var/lib/mysql]
# Mon, 09 Aug 2021 19:25:27 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Mon, 09 Aug 2021 19:25:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Aug 2021 19:25:28 GMT
EXPOSE 3306
# Mon, 09 Aug 2021 19:25:28 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf20e69555c2118df81cd7906473b0bbef5210f014d45113251b1298fb1c996`  
		Last Modified: Tue, 27 Jul 2021 00:10:02 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69afd1ffc85b8fe385e48d00e89467a4e080c81b2447ce86ebf964f3e43efb9`  
		Last Modified: Tue, 27 Jul 2021 00:10:04 GMT  
		Size: 5.5 MB (5488764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e720dc7fcd8609016e69543f354117290ffee7c9ea1bdd97d7ca84bcc06d616`  
		Last Modified: Tue, 27 Jul 2021 00:10:03 GMT  
		Size: 3.6 MB (3582379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a81d177e410065c8eec2b5c018ab6ac60b2a5161184890bc3bf7627e78fb2dd`  
		Last Modified: Tue, 27 Jul 2021 00:10:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827c8c103c898d23db5f0cfc69b6faa45038d27b1ec3c15cb5d5b29ee60fca0b`  
		Last Modified: Tue, 27 Jul 2021 00:09:59 GMT  
		Size: 2.3 MB (2274133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2108ccd013748c7fce6a19a3f7434b860401f78326ac7373c486eafa3c719354`  
		Last Modified: Tue, 27 Jul 2021 00:09:59 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd18312032de063877ef5ff92e06d0c5b2e33d2f09d4ebaca4062371d5919e2`  
		Last Modified: Mon, 09 Aug 2021 19:28:44 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63f5eb96adc50bc11b45b80d6c343b69bfa553f315a2d8a25e9f48221c720b17`  
		Last Modified: Mon, 09 Aug 2021 19:28:57 GMT  
		Size: 86.9 MB (86936993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a7dacc2466ab5456742e63e09e203e507a8be337cc4f5bddd587740684f8f9`  
		Last Modified: Mon, 09 Aug 2021 19:28:44 GMT  
		Size: 5.6 KB (5611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:155422bcef7935decf5e25e3b349dbcde5f99df70fa0b8eecc5b54f6656e23ab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124311821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27733d6f266bbcd2d324301e21ac627d3ca04a6b607888667e011a638b1bbeb8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:44 GMT
ADD file:cec21619ecbd37b4cf8da15153b8957a343cd25c6f714e3ac3969b6003704a58 in / 
# Tue, 31 Aug 2021 01:40:45 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:04:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 31 Aug 2021 03:04:38 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:04:38 GMT
ENV GOSU_VERSION=1.13
# Tue, 31 Aug 2021 03:04:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 31 Aug 2021 03:04:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 31 Aug 2021 03:04:57 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:04:57 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 31 Aug 2021 03:05:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 31 Aug 2021 03:05:41 GMT
ARG MARIADB_MAJOR=10.5
# Tue, 31 Aug 2021 03:05:41 GMT
ENV MARIADB_MAJOR=10.5
# Tue, 31 Aug 2021 03:05:42 GMT
ARG MARIADB_VERSION=1:10.5.12+maria~focal
# Tue, 31 Aug 2021 03:05:42 GMT
ENV MARIADB_VERSION=1:10.5.12+maria~focal
# Tue, 31 Aug 2021 03:05:42 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
# Tue, 31 Aug 2021 03:05:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 31 Aug 2021 03:06:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 31 Aug 2021 03:06:03 GMT
VOLUME [/var/lib/mysql]
# Tue, 31 Aug 2021 03:06:04 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Tue, 31 Aug 2021 03:06:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Aug 2021 03:06:04 GMT
EXPOSE 3306
# Tue, 31 Aug 2021 03:06:04 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ab2d02b1ec420fdb84c9f52abda403b6aef20f5de904a2ecda5ae4f5cd6e4d46`  
		Last Modified: Tue, 31 Aug 2021 01:42:34 GMT  
		Size: 27.2 MB (27173099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d16f1b8a1bc9060d0c98a0e09c73ceab3d694a99f57672d6e44f2f5dcf09eae`  
		Last Modified: Tue, 31 Aug 2021 03:09:41 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16d8285f3be08ea7340eaf6dced5161164096c3fb3345fe8c5d6d64496bc143`  
		Last Modified: Tue, 31 Aug 2021 03:09:40 GMT  
		Size: 5.5 MB (5455084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ffd6c9eed67b115939ab5f6d4bb8ffd2f0f152fe9a61024122b558e83ce912e`  
		Last Modified: Tue, 31 Aug 2021 03:09:39 GMT  
		Size: 3.4 MB (3368457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdbc2935c20fd14d96044dcdb65fb79a0f676bcdf334058da282716411d3ff9b`  
		Last Modified: Tue, 31 Aug 2021 03:09:39 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b302bb5f11cae70b4c8ec1079e6de6c62dacfdce3e8f3ccdfabd6ce44b63d2`  
		Last Modified: Tue, 31 Aug 2021 03:09:37 GMT  
		Size: 2.2 MB (2203569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21de8a622698dffd65e882759b0b6e4fe0e56b60d892f2e4446f94439a1270f`  
		Last Modified: Tue, 31 Aug 2021 03:09:36 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d90417b10f36ce35fa1e4bce541ddb0e5a4d650237bbbac7d590fe6b84c03789`  
		Last Modified: Tue, 31 Aug 2021 03:10:24 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe757cf1d42c8bbba22076f6747facadb9dec82a418ca34eb66229b9e7114c6c`  
		Last Modified: Tue, 31 Aug 2021 03:10:39 GMT  
		Size: 86.1 MB (86101283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5caa80c0b81366945776f22bd92fdc75ab775a4a8768f3bd30e6f58bba416225`  
		Last Modified: Tue, 31 Aug 2021 03:10:24 GMT  
		Size: 5.6 KB (5609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:a22827c392d5d8aa35de016791f7037b3a783257bc715118bdca87dbdc3f1623
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.6 MB (137580509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a6ffd715dfd27be255eb10756b6b1dddf856f016349451df5b3d3ca927a22eb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 26 Jul 2021 23:12:46 GMT
ADD file:68eb628c2202763afa91d554dde9668d8a468fe53fdbd2fe98627a5f91d224b4 in / 
# Mon, 26 Jul 2021 23:12:49 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 02:05:55 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 27 Jul 2021 02:06:47 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:06:50 GMT
ENV GOSU_VERSION=1.13
# Tue, 27 Jul 2021 02:07:32 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 27 Jul 2021 02:07:42 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 27 Jul 2021 02:08:11 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:08:14 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 27 Jul 2021 02:08:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 27 Jul 2021 02:11:32 GMT
ARG MARIADB_MAJOR=10.5
# Tue, 27 Jul 2021 02:11:34 GMT
ENV MARIADB_MAJOR=10.5
# Mon, 09 Aug 2021 19:23:36 GMT
ARG MARIADB_VERSION=1:10.5.12+maria~focal
# Mon, 09 Aug 2021 19:23:45 GMT
ENV MARIADB_VERSION=1:10.5.12+maria~focal
# Mon, 09 Aug 2021 19:23:49 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
# Mon, 09 Aug 2021 19:24:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 09 Aug 2021 19:28:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 09 Aug 2021 19:28:14 GMT
VOLUME [/var/lib/mysql]
# Mon, 09 Aug 2021 19:28:18 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Mon, 09 Aug 2021 19:28:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Aug 2021 19:28:30 GMT
EXPOSE 3306
# Mon, 09 Aug 2021 19:28:33 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:1a396eed835b3b7b4101a9863d174e145ddbb1de1502a63bae726b0f81e7ca93`  
		Last Modified: Mon, 26 Jul 2021 23:15:51 GMT  
		Size: 33.3 MB (33290427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65be85b12a63573ebccb059357c5c0db6046f4a074454eea617c402e3bf99c1f`  
		Last Modified: Tue, 27 Jul 2021 02:26:16 GMT  
		Size: 1.8 KB (1760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:803c8e5bf0c59b9b01b70cac07bb24bc696bc577d8e74c79ff15bcbd480874b4`  
		Last Modified: Tue, 27 Jul 2021 02:26:17 GMT  
		Size: 6.7 MB (6667884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62bd7bf9c00152c4fb338b2c1a01d5b241ceda5c58d9e700a353072ab80fb4b9`  
		Last Modified: Tue, 27 Jul 2021 02:26:17 GMT  
		Size: 3.7 MB (3670853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:372602ac4ce9a3a693cb97ec9b3e71b449fdafbaded2ce2937fec39cec9c9b6e`  
		Last Modified: Tue, 27 Jul 2021 02:26:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a80c4de70a1ded78cf0175b1f5fda38b3119857dd2d8d9f1fafcdc39eafef0e`  
		Last Modified: Tue, 27 Jul 2021 02:26:13 GMT  
		Size: 2.6 MB (2569871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc8dec87672a96e86220faa6c3e98577b2a9090fc81d81efb4681fe59e732b7`  
		Last Modified: Tue, 27 Jul 2021 02:26:12 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8e4a78feeb863bb4a36ec743301f11db8142e4252ab6db2dd94470d0ffb950`  
		Last Modified: Mon, 09 Aug 2021 19:45:56 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96967b218a123706ee5fe6b9cf79c4124c016aa86825dec7ba7ddae281301f63`  
		Last Modified: Mon, 09 Aug 2021 19:46:14 GMT  
		Size: 91.4 MB (91371131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b234b373bbf599e2b861274d9dfe19b7b3a14f24555c4b292df94ca2cf425c5`  
		Last Modified: Mon, 09 Aug 2021 19:45:56 GMT  
		Size: 5.6 KB (5614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:9373b966fe815dcb87a102c954e3da3fc62040cea5d20c0715de3bf8ba678ef5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.1 MB (126054236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7aae9fe04321546d598fe4969a87ca9b73346d340df7178085fb136fd27bb5b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:23 GMT
ADD file:979855f79ebaca36cc7878f71b2326f1cd189970fdb223b37cd64ee12d1c9a2b in / 
# Tue, 31 Aug 2021 01:42:27 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:49:44 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 31 Aug 2021 02:49:51 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:49:51 GMT
ENV GOSU_VERSION=1.13
# Tue, 31 Aug 2021 02:50:04 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 31 Aug 2021 02:50:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 31 Aug 2021 02:50:12 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:50:12 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 31 Aug 2021 02:50:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 31 Aug 2021 02:51:03 GMT
ARG MARIADB_MAJOR=10.5
# Tue, 31 Aug 2021 02:51:03 GMT
ENV MARIADB_MAJOR=10.5
# Tue, 31 Aug 2021 02:51:04 GMT
ARG MARIADB_VERSION=1:10.5.12+maria~focal
# Tue, 31 Aug 2021 02:51:04 GMT
ENV MARIADB_VERSION=1:10.5.12+maria~focal
# Tue, 31 Aug 2021 02:51:04 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
# Tue, 31 Aug 2021 02:51:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 31 Aug 2021 02:51:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 31 Aug 2021 02:51:36 GMT
VOLUME [/var/lib/mysql]
# Tue, 31 Aug 2021 02:51:37 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Tue, 31 Aug 2021 02:51:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Aug 2021 02:51:37 GMT
EXPOSE 3306
# Tue, 31 Aug 2021 02:51:37 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:9fbf86d355c92d30b8de4c0360b0d79e1100e392d0885b6b5b302a1c3781dbf1`  
		Last Modified: Tue, 31 Aug 2021 01:44:13 GMT  
		Size: 27.1 MB (27127470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5652d937cd93c6c333210a7c5783a5defbac72c096a74537a0e99da179e69e15`  
		Last Modified: Tue, 31 Aug 2021 02:52:15 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1b48caf1d89a34f08f8ee38f48260ccfd25cfdc0e5425a1f7e2e1c3bc1c8cf0`  
		Last Modified: Tue, 31 Aug 2021 02:52:16 GMT  
		Size: 5.4 MB (5380989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352b2892aadbd934d1a0415ca24f71baf53ef4b324fe9f8772a37405d8607dba`  
		Last Modified: Tue, 31 Aug 2021 02:52:16 GMT  
		Size: 3.2 MB (3241880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354edb6860dbb419b59714606f392488735bc5e9adc7496059e98f51de24d84a`  
		Last Modified: Tue, 31 Aug 2021 02:52:15 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9934bdf22d9a668fcaab9695424d4074294aef89d849a8c8ba80b0bb31ab2ab9`  
		Last Modified: Tue, 31 Aug 2021 02:52:13 GMT  
		Size: 2.2 MB (2186296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a940a6a2154f17326f40b9d4619aa517978b7eed0f68a8a68738928defef66`  
		Last Modified: Tue, 31 Aug 2021 02:52:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d59cabe74a3e7d613c1b80e665c9d8541a8fb4d41ab6cccf7ef511b3569bc83f`  
		Last Modified: Tue, 31 Aug 2021 02:52:48 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fa3d9203216e56ee658b3d6a772799aa5553bbff52dd9ef9ff3d46d26606344`  
		Last Modified: Tue, 31 Aug 2021 02:53:01 GMT  
		Size: 88.1 MB (88107279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95dfd07848bf5afc8800b1141a2c38c414b30cef83cbd4348dd432a963366095`  
		Last Modified: Tue, 31 Aug 2021 02:52:48 GMT  
		Size: 5.6 KB (5606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5.12`

```console
$ docker pull mariadb@sha256:334eba05f9f47284cda296cb6b5857a28b681f045b1a59b835131e2b22331311
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.5.12` - linux; amd64

```console
$ docker pull mariadb@sha256:714b7e3ed906a2d4a0c11ded8dcadc804dde593be5474ef88f911ce6b54dadad
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.9 MB (126860537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9643f47b304c4a77314f35c725cf5dc7e63b29f9a0350e52b99d1e8ca6067276`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:05:00 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 27 Jul 2021 00:05:14 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:05:15 GMT
ENV GOSU_VERSION=1.13
# Tue, 27 Jul 2021 00:05:26 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 27 Jul 2021 00:05:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 27 Jul 2021 00:05:34 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:05:35 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 27 Jul 2021 00:05:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 27 Jul 2021 00:06:25 GMT
ARG MARIADB_MAJOR=10.5
# Tue, 27 Jul 2021 00:06:25 GMT
ENV MARIADB_MAJOR=10.5
# Mon, 09 Aug 2021 19:25:04 GMT
ARG MARIADB_VERSION=1:10.5.12+maria~focal
# Mon, 09 Aug 2021 19:25:04 GMT
ENV MARIADB_VERSION=1:10.5.12+maria~focal
# Mon, 09 Aug 2021 19:25:04 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
# Mon, 09 Aug 2021 19:25:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 09 Aug 2021 19:25:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 09 Aug 2021 19:25:27 GMT
VOLUME [/var/lib/mysql]
# Mon, 09 Aug 2021 19:25:27 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Mon, 09 Aug 2021 19:25:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Aug 2021 19:25:28 GMT
EXPOSE 3306
# Mon, 09 Aug 2021 19:25:28 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf20e69555c2118df81cd7906473b0bbef5210f014d45113251b1298fb1c996`  
		Last Modified: Tue, 27 Jul 2021 00:10:02 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69afd1ffc85b8fe385e48d00e89467a4e080c81b2447ce86ebf964f3e43efb9`  
		Last Modified: Tue, 27 Jul 2021 00:10:04 GMT  
		Size: 5.5 MB (5488764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e720dc7fcd8609016e69543f354117290ffee7c9ea1bdd97d7ca84bcc06d616`  
		Last Modified: Tue, 27 Jul 2021 00:10:03 GMT  
		Size: 3.6 MB (3582379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a81d177e410065c8eec2b5c018ab6ac60b2a5161184890bc3bf7627e78fb2dd`  
		Last Modified: Tue, 27 Jul 2021 00:10:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827c8c103c898d23db5f0cfc69b6faa45038d27b1ec3c15cb5d5b29ee60fca0b`  
		Last Modified: Tue, 27 Jul 2021 00:09:59 GMT  
		Size: 2.3 MB (2274133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2108ccd013748c7fce6a19a3f7434b860401f78326ac7373c486eafa3c719354`  
		Last Modified: Tue, 27 Jul 2021 00:09:59 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd18312032de063877ef5ff92e06d0c5b2e33d2f09d4ebaca4062371d5919e2`  
		Last Modified: Mon, 09 Aug 2021 19:28:44 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63f5eb96adc50bc11b45b80d6c343b69bfa553f315a2d8a25e9f48221c720b17`  
		Last Modified: Mon, 09 Aug 2021 19:28:57 GMT  
		Size: 86.9 MB (86936993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a7dacc2466ab5456742e63e09e203e507a8be337cc4f5bddd587740684f8f9`  
		Last Modified: Mon, 09 Aug 2021 19:28:44 GMT  
		Size: 5.6 KB (5611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.12` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:155422bcef7935decf5e25e3b349dbcde5f99df70fa0b8eecc5b54f6656e23ab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124311821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27733d6f266bbcd2d324301e21ac627d3ca04a6b607888667e011a638b1bbeb8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:44 GMT
ADD file:cec21619ecbd37b4cf8da15153b8957a343cd25c6f714e3ac3969b6003704a58 in / 
# Tue, 31 Aug 2021 01:40:45 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:04:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 31 Aug 2021 03:04:38 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:04:38 GMT
ENV GOSU_VERSION=1.13
# Tue, 31 Aug 2021 03:04:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 31 Aug 2021 03:04:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 31 Aug 2021 03:04:57 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:04:57 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 31 Aug 2021 03:05:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 31 Aug 2021 03:05:41 GMT
ARG MARIADB_MAJOR=10.5
# Tue, 31 Aug 2021 03:05:41 GMT
ENV MARIADB_MAJOR=10.5
# Tue, 31 Aug 2021 03:05:42 GMT
ARG MARIADB_VERSION=1:10.5.12+maria~focal
# Tue, 31 Aug 2021 03:05:42 GMT
ENV MARIADB_VERSION=1:10.5.12+maria~focal
# Tue, 31 Aug 2021 03:05:42 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
# Tue, 31 Aug 2021 03:05:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 31 Aug 2021 03:06:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 31 Aug 2021 03:06:03 GMT
VOLUME [/var/lib/mysql]
# Tue, 31 Aug 2021 03:06:04 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Tue, 31 Aug 2021 03:06:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Aug 2021 03:06:04 GMT
EXPOSE 3306
# Tue, 31 Aug 2021 03:06:04 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ab2d02b1ec420fdb84c9f52abda403b6aef20f5de904a2ecda5ae4f5cd6e4d46`  
		Last Modified: Tue, 31 Aug 2021 01:42:34 GMT  
		Size: 27.2 MB (27173099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d16f1b8a1bc9060d0c98a0e09c73ceab3d694a99f57672d6e44f2f5dcf09eae`  
		Last Modified: Tue, 31 Aug 2021 03:09:41 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16d8285f3be08ea7340eaf6dced5161164096c3fb3345fe8c5d6d64496bc143`  
		Last Modified: Tue, 31 Aug 2021 03:09:40 GMT  
		Size: 5.5 MB (5455084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ffd6c9eed67b115939ab5f6d4bb8ffd2f0f152fe9a61024122b558e83ce912e`  
		Last Modified: Tue, 31 Aug 2021 03:09:39 GMT  
		Size: 3.4 MB (3368457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdbc2935c20fd14d96044dcdb65fb79a0f676bcdf334058da282716411d3ff9b`  
		Last Modified: Tue, 31 Aug 2021 03:09:39 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b302bb5f11cae70b4c8ec1079e6de6c62dacfdce3e8f3ccdfabd6ce44b63d2`  
		Last Modified: Tue, 31 Aug 2021 03:09:37 GMT  
		Size: 2.2 MB (2203569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21de8a622698dffd65e882759b0b6e4fe0e56b60d892f2e4446f94439a1270f`  
		Last Modified: Tue, 31 Aug 2021 03:09:36 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d90417b10f36ce35fa1e4bce541ddb0e5a4d650237bbbac7d590fe6b84c03789`  
		Last Modified: Tue, 31 Aug 2021 03:10:24 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe757cf1d42c8bbba22076f6747facadb9dec82a418ca34eb66229b9e7114c6c`  
		Last Modified: Tue, 31 Aug 2021 03:10:39 GMT  
		Size: 86.1 MB (86101283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5caa80c0b81366945776f22bd92fdc75ab775a4a8768f3bd30e6f58bba416225`  
		Last Modified: Tue, 31 Aug 2021 03:10:24 GMT  
		Size: 5.6 KB (5609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.12` - linux; ppc64le

```console
$ docker pull mariadb@sha256:a22827c392d5d8aa35de016791f7037b3a783257bc715118bdca87dbdc3f1623
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.6 MB (137580509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a6ffd715dfd27be255eb10756b6b1dddf856f016349451df5b3d3ca927a22eb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 26 Jul 2021 23:12:46 GMT
ADD file:68eb628c2202763afa91d554dde9668d8a468fe53fdbd2fe98627a5f91d224b4 in / 
# Mon, 26 Jul 2021 23:12:49 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 02:05:55 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 27 Jul 2021 02:06:47 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:06:50 GMT
ENV GOSU_VERSION=1.13
# Tue, 27 Jul 2021 02:07:32 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 27 Jul 2021 02:07:42 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 27 Jul 2021 02:08:11 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:08:14 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 27 Jul 2021 02:08:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 27 Jul 2021 02:11:32 GMT
ARG MARIADB_MAJOR=10.5
# Tue, 27 Jul 2021 02:11:34 GMT
ENV MARIADB_MAJOR=10.5
# Mon, 09 Aug 2021 19:23:36 GMT
ARG MARIADB_VERSION=1:10.5.12+maria~focal
# Mon, 09 Aug 2021 19:23:45 GMT
ENV MARIADB_VERSION=1:10.5.12+maria~focal
# Mon, 09 Aug 2021 19:23:49 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
# Mon, 09 Aug 2021 19:24:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 09 Aug 2021 19:28:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 09 Aug 2021 19:28:14 GMT
VOLUME [/var/lib/mysql]
# Mon, 09 Aug 2021 19:28:18 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Mon, 09 Aug 2021 19:28:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Aug 2021 19:28:30 GMT
EXPOSE 3306
# Mon, 09 Aug 2021 19:28:33 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:1a396eed835b3b7b4101a9863d174e145ddbb1de1502a63bae726b0f81e7ca93`  
		Last Modified: Mon, 26 Jul 2021 23:15:51 GMT  
		Size: 33.3 MB (33290427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65be85b12a63573ebccb059357c5c0db6046f4a074454eea617c402e3bf99c1f`  
		Last Modified: Tue, 27 Jul 2021 02:26:16 GMT  
		Size: 1.8 KB (1760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:803c8e5bf0c59b9b01b70cac07bb24bc696bc577d8e74c79ff15bcbd480874b4`  
		Last Modified: Tue, 27 Jul 2021 02:26:17 GMT  
		Size: 6.7 MB (6667884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62bd7bf9c00152c4fb338b2c1a01d5b241ceda5c58d9e700a353072ab80fb4b9`  
		Last Modified: Tue, 27 Jul 2021 02:26:17 GMT  
		Size: 3.7 MB (3670853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:372602ac4ce9a3a693cb97ec9b3e71b449fdafbaded2ce2937fec39cec9c9b6e`  
		Last Modified: Tue, 27 Jul 2021 02:26:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a80c4de70a1ded78cf0175b1f5fda38b3119857dd2d8d9f1fafcdc39eafef0e`  
		Last Modified: Tue, 27 Jul 2021 02:26:13 GMT  
		Size: 2.6 MB (2569871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc8dec87672a96e86220faa6c3e98577b2a9090fc81d81efb4681fe59e732b7`  
		Last Modified: Tue, 27 Jul 2021 02:26:12 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8e4a78feeb863bb4a36ec743301f11db8142e4252ab6db2dd94470d0ffb950`  
		Last Modified: Mon, 09 Aug 2021 19:45:56 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96967b218a123706ee5fe6b9cf79c4124c016aa86825dec7ba7ddae281301f63`  
		Last Modified: Mon, 09 Aug 2021 19:46:14 GMT  
		Size: 91.4 MB (91371131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b234b373bbf599e2b861274d9dfe19b7b3a14f24555c4b292df94ca2cf425c5`  
		Last Modified: Mon, 09 Aug 2021 19:45:56 GMT  
		Size: 5.6 KB (5614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.12` - linux; s390x

```console
$ docker pull mariadb@sha256:9373b966fe815dcb87a102c954e3da3fc62040cea5d20c0715de3bf8ba678ef5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.1 MB (126054236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7aae9fe04321546d598fe4969a87ca9b73346d340df7178085fb136fd27bb5b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:23 GMT
ADD file:979855f79ebaca36cc7878f71b2326f1cd189970fdb223b37cd64ee12d1c9a2b in / 
# Tue, 31 Aug 2021 01:42:27 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:49:44 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 31 Aug 2021 02:49:51 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:49:51 GMT
ENV GOSU_VERSION=1.13
# Tue, 31 Aug 2021 02:50:04 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 31 Aug 2021 02:50:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 31 Aug 2021 02:50:12 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:50:12 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 31 Aug 2021 02:50:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 31 Aug 2021 02:51:03 GMT
ARG MARIADB_MAJOR=10.5
# Tue, 31 Aug 2021 02:51:03 GMT
ENV MARIADB_MAJOR=10.5
# Tue, 31 Aug 2021 02:51:04 GMT
ARG MARIADB_VERSION=1:10.5.12+maria~focal
# Tue, 31 Aug 2021 02:51:04 GMT
ENV MARIADB_VERSION=1:10.5.12+maria~focal
# Tue, 31 Aug 2021 02:51:04 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
# Tue, 31 Aug 2021 02:51:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 31 Aug 2021 02:51:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 31 Aug 2021 02:51:36 GMT
VOLUME [/var/lib/mysql]
# Tue, 31 Aug 2021 02:51:37 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Tue, 31 Aug 2021 02:51:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Aug 2021 02:51:37 GMT
EXPOSE 3306
# Tue, 31 Aug 2021 02:51:37 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:9fbf86d355c92d30b8de4c0360b0d79e1100e392d0885b6b5b302a1c3781dbf1`  
		Last Modified: Tue, 31 Aug 2021 01:44:13 GMT  
		Size: 27.1 MB (27127470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5652d937cd93c6c333210a7c5783a5defbac72c096a74537a0e99da179e69e15`  
		Last Modified: Tue, 31 Aug 2021 02:52:15 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1b48caf1d89a34f08f8ee38f48260ccfd25cfdc0e5425a1f7e2e1c3bc1c8cf0`  
		Last Modified: Tue, 31 Aug 2021 02:52:16 GMT  
		Size: 5.4 MB (5380989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352b2892aadbd934d1a0415ca24f71baf53ef4b324fe9f8772a37405d8607dba`  
		Last Modified: Tue, 31 Aug 2021 02:52:16 GMT  
		Size: 3.2 MB (3241880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354edb6860dbb419b59714606f392488735bc5e9adc7496059e98f51de24d84a`  
		Last Modified: Tue, 31 Aug 2021 02:52:15 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9934bdf22d9a668fcaab9695424d4074294aef89d849a8c8ba80b0bb31ab2ab9`  
		Last Modified: Tue, 31 Aug 2021 02:52:13 GMT  
		Size: 2.2 MB (2186296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a940a6a2154f17326f40b9d4619aa517978b7eed0f68a8a68738928defef66`  
		Last Modified: Tue, 31 Aug 2021 02:52:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d59cabe74a3e7d613c1b80e665c9d8541a8fb4d41ab6cccf7ef511b3569bc83f`  
		Last Modified: Tue, 31 Aug 2021 02:52:48 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fa3d9203216e56ee658b3d6a772799aa5553bbff52dd9ef9ff3d46d26606344`  
		Last Modified: Tue, 31 Aug 2021 02:53:01 GMT  
		Size: 88.1 MB (88107279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95dfd07848bf5afc8800b1141a2c38c414b30cef83cbd4348dd432a963366095`  
		Last Modified: Tue, 31 Aug 2021 02:52:48 GMT  
		Size: 5.6 KB (5606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5.12-focal`

```console
$ docker pull mariadb@sha256:334eba05f9f47284cda296cb6b5857a28b681f045b1a59b835131e2b22331311
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.5.12-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:714b7e3ed906a2d4a0c11ded8dcadc804dde593be5474ef88f911ce6b54dadad
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.9 MB (126860537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9643f47b304c4a77314f35c725cf5dc7e63b29f9a0350e52b99d1e8ca6067276`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:05:00 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 27 Jul 2021 00:05:14 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:05:15 GMT
ENV GOSU_VERSION=1.13
# Tue, 27 Jul 2021 00:05:26 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 27 Jul 2021 00:05:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 27 Jul 2021 00:05:34 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:05:35 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 27 Jul 2021 00:05:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 27 Jul 2021 00:06:25 GMT
ARG MARIADB_MAJOR=10.5
# Tue, 27 Jul 2021 00:06:25 GMT
ENV MARIADB_MAJOR=10.5
# Mon, 09 Aug 2021 19:25:04 GMT
ARG MARIADB_VERSION=1:10.5.12+maria~focal
# Mon, 09 Aug 2021 19:25:04 GMT
ENV MARIADB_VERSION=1:10.5.12+maria~focal
# Mon, 09 Aug 2021 19:25:04 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
# Mon, 09 Aug 2021 19:25:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 09 Aug 2021 19:25:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 09 Aug 2021 19:25:27 GMT
VOLUME [/var/lib/mysql]
# Mon, 09 Aug 2021 19:25:27 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Mon, 09 Aug 2021 19:25:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Aug 2021 19:25:28 GMT
EXPOSE 3306
# Mon, 09 Aug 2021 19:25:28 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf20e69555c2118df81cd7906473b0bbef5210f014d45113251b1298fb1c996`  
		Last Modified: Tue, 27 Jul 2021 00:10:02 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69afd1ffc85b8fe385e48d00e89467a4e080c81b2447ce86ebf964f3e43efb9`  
		Last Modified: Tue, 27 Jul 2021 00:10:04 GMT  
		Size: 5.5 MB (5488764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e720dc7fcd8609016e69543f354117290ffee7c9ea1bdd97d7ca84bcc06d616`  
		Last Modified: Tue, 27 Jul 2021 00:10:03 GMT  
		Size: 3.6 MB (3582379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a81d177e410065c8eec2b5c018ab6ac60b2a5161184890bc3bf7627e78fb2dd`  
		Last Modified: Tue, 27 Jul 2021 00:10:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827c8c103c898d23db5f0cfc69b6faa45038d27b1ec3c15cb5d5b29ee60fca0b`  
		Last Modified: Tue, 27 Jul 2021 00:09:59 GMT  
		Size: 2.3 MB (2274133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2108ccd013748c7fce6a19a3f7434b860401f78326ac7373c486eafa3c719354`  
		Last Modified: Tue, 27 Jul 2021 00:09:59 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd18312032de063877ef5ff92e06d0c5b2e33d2f09d4ebaca4062371d5919e2`  
		Last Modified: Mon, 09 Aug 2021 19:28:44 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63f5eb96adc50bc11b45b80d6c343b69bfa553f315a2d8a25e9f48221c720b17`  
		Last Modified: Mon, 09 Aug 2021 19:28:57 GMT  
		Size: 86.9 MB (86936993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a7dacc2466ab5456742e63e09e203e507a8be337cc4f5bddd587740684f8f9`  
		Last Modified: Mon, 09 Aug 2021 19:28:44 GMT  
		Size: 5.6 KB (5611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.12-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:155422bcef7935decf5e25e3b349dbcde5f99df70fa0b8eecc5b54f6656e23ab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124311821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27733d6f266bbcd2d324301e21ac627d3ca04a6b607888667e011a638b1bbeb8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:44 GMT
ADD file:cec21619ecbd37b4cf8da15153b8957a343cd25c6f714e3ac3969b6003704a58 in / 
# Tue, 31 Aug 2021 01:40:45 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:04:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 31 Aug 2021 03:04:38 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:04:38 GMT
ENV GOSU_VERSION=1.13
# Tue, 31 Aug 2021 03:04:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 31 Aug 2021 03:04:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 31 Aug 2021 03:04:57 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:04:57 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 31 Aug 2021 03:05:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 31 Aug 2021 03:05:41 GMT
ARG MARIADB_MAJOR=10.5
# Tue, 31 Aug 2021 03:05:41 GMT
ENV MARIADB_MAJOR=10.5
# Tue, 31 Aug 2021 03:05:42 GMT
ARG MARIADB_VERSION=1:10.5.12+maria~focal
# Tue, 31 Aug 2021 03:05:42 GMT
ENV MARIADB_VERSION=1:10.5.12+maria~focal
# Tue, 31 Aug 2021 03:05:42 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
# Tue, 31 Aug 2021 03:05:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 31 Aug 2021 03:06:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 31 Aug 2021 03:06:03 GMT
VOLUME [/var/lib/mysql]
# Tue, 31 Aug 2021 03:06:04 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Tue, 31 Aug 2021 03:06:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Aug 2021 03:06:04 GMT
EXPOSE 3306
# Tue, 31 Aug 2021 03:06:04 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ab2d02b1ec420fdb84c9f52abda403b6aef20f5de904a2ecda5ae4f5cd6e4d46`  
		Last Modified: Tue, 31 Aug 2021 01:42:34 GMT  
		Size: 27.2 MB (27173099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d16f1b8a1bc9060d0c98a0e09c73ceab3d694a99f57672d6e44f2f5dcf09eae`  
		Last Modified: Tue, 31 Aug 2021 03:09:41 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16d8285f3be08ea7340eaf6dced5161164096c3fb3345fe8c5d6d64496bc143`  
		Last Modified: Tue, 31 Aug 2021 03:09:40 GMT  
		Size: 5.5 MB (5455084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ffd6c9eed67b115939ab5f6d4bb8ffd2f0f152fe9a61024122b558e83ce912e`  
		Last Modified: Tue, 31 Aug 2021 03:09:39 GMT  
		Size: 3.4 MB (3368457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdbc2935c20fd14d96044dcdb65fb79a0f676bcdf334058da282716411d3ff9b`  
		Last Modified: Tue, 31 Aug 2021 03:09:39 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b302bb5f11cae70b4c8ec1079e6de6c62dacfdce3e8f3ccdfabd6ce44b63d2`  
		Last Modified: Tue, 31 Aug 2021 03:09:37 GMT  
		Size: 2.2 MB (2203569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21de8a622698dffd65e882759b0b6e4fe0e56b60d892f2e4446f94439a1270f`  
		Last Modified: Tue, 31 Aug 2021 03:09:36 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d90417b10f36ce35fa1e4bce541ddb0e5a4d650237bbbac7d590fe6b84c03789`  
		Last Modified: Tue, 31 Aug 2021 03:10:24 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe757cf1d42c8bbba22076f6747facadb9dec82a418ca34eb66229b9e7114c6c`  
		Last Modified: Tue, 31 Aug 2021 03:10:39 GMT  
		Size: 86.1 MB (86101283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5caa80c0b81366945776f22bd92fdc75ab775a4a8768f3bd30e6f58bba416225`  
		Last Modified: Tue, 31 Aug 2021 03:10:24 GMT  
		Size: 5.6 KB (5609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.12-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:a22827c392d5d8aa35de016791f7037b3a783257bc715118bdca87dbdc3f1623
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.6 MB (137580509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a6ffd715dfd27be255eb10756b6b1dddf856f016349451df5b3d3ca927a22eb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 26 Jul 2021 23:12:46 GMT
ADD file:68eb628c2202763afa91d554dde9668d8a468fe53fdbd2fe98627a5f91d224b4 in / 
# Mon, 26 Jul 2021 23:12:49 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 02:05:55 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 27 Jul 2021 02:06:47 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:06:50 GMT
ENV GOSU_VERSION=1.13
# Tue, 27 Jul 2021 02:07:32 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 27 Jul 2021 02:07:42 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 27 Jul 2021 02:08:11 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:08:14 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 27 Jul 2021 02:08:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 27 Jul 2021 02:11:32 GMT
ARG MARIADB_MAJOR=10.5
# Tue, 27 Jul 2021 02:11:34 GMT
ENV MARIADB_MAJOR=10.5
# Mon, 09 Aug 2021 19:23:36 GMT
ARG MARIADB_VERSION=1:10.5.12+maria~focal
# Mon, 09 Aug 2021 19:23:45 GMT
ENV MARIADB_VERSION=1:10.5.12+maria~focal
# Mon, 09 Aug 2021 19:23:49 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
# Mon, 09 Aug 2021 19:24:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 09 Aug 2021 19:28:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 09 Aug 2021 19:28:14 GMT
VOLUME [/var/lib/mysql]
# Mon, 09 Aug 2021 19:28:18 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Mon, 09 Aug 2021 19:28:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Aug 2021 19:28:30 GMT
EXPOSE 3306
# Mon, 09 Aug 2021 19:28:33 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:1a396eed835b3b7b4101a9863d174e145ddbb1de1502a63bae726b0f81e7ca93`  
		Last Modified: Mon, 26 Jul 2021 23:15:51 GMT  
		Size: 33.3 MB (33290427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65be85b12a63573ebccb059357c5c0db6046f4a074454eea617c402e3bf99c1f`  
		Last Modified: Tue, 27 Jul 2021 02:26:16 GMT  
		Size: 1.8 KB (1760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:803c8e5bf0c59b9b01b70cac07bb24bc696bc577d8e74c79ff15bcbd480874b4`  
		Last Modified: Tue, 27 Jul 2021 02:26:17 GMT  
		Size: 6.7 MB (6667884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62bd7bf9c00152c4fb338b2c1a01d5b241ceda5c58d9e700a353072ab80fb4b9`  
		Last Modified: Tue, 27 Jul 2021 02:26:17 GMT  
		Size: 3.7 MB (3670853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:372602ac4ce9a3a693cb97ec9b3e71b449fdafbaded2ce2937fec39cec9c9b6e`  
		Last Modified: Tue, 27 Jul 2021 02:26:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a80c4de70a1ded78cf0175b1f5fda38b3119857dd2d8d9f1fafcdc39eafef0e`  
		Last Modified: Tue, 27 Jul 2021 02:26:13 GMT  
		Size: 2.6 MB (2569871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc8dec87672a96e86220faa6c3e98577b2a9090fc81d81efb4681fe59e732b7`  
		Last Modified: Tue, 27 Jul 2021 02:26:12 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8e4a78feeb863bb4a36ec743301f11db8142e4252ab6db2dd94470d0ffb950`  
		Last Modified: Mon, 09 Aug 2021 19:45:56 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96967b218a123706ee5fe6b9cf79c4124c016aa86825dec7ba7ddae281301f63`  
		Last Modified: Mon, 09 Aug 2021 19:46:14 GMT  
		Size: 91.4 MB (91371131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b234b373bbf599e2b861274d9dfe19b7b3a14f24555c4b292df94ca2cf425c5`  
		Last Modified: Mon, 09 Aug 2021 19:45:56 GMT  
		Size: 5.6 KB (5614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.12-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:9373b966fe815dcb87a102c954e3da3fc62040cea5d20c0715de3bf8ba678ef5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.1 MB (126054236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7aae9fe04321546d598fe4969a87ca9b73346d340df7178085fb136fd27bb5b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:23 GMT
ADD file:979855f79ebaca36cc7878f71b2326f1cd189970fdb223b37cd64ee12d1c9a2b in / 
# Tue, 31 Aug 2021 01:42:27 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:49:44 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 31 Aug 2021 02:49:51 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:49:51 GMT
ENV GOSU_VERSION=1.13
# Tue, 31 Aug 2021 02:50:04 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 31 Aug 2021 02:50:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 31 Aug 2021 02:50:12 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:50:12 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 31 Aug 2021 02:50:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 31 Aug 2021 02:51:03 GMT
ARG MARIADB_MAJOR=10.5
# Tue, 31 Aug 2021 02:51:03 GMT
ENV MARIADB_MAJOR=10.5
# Tue, 31 Aug 2021 02:51:04 GMT
ARG MARIADB_VERSION=1:10.5.12+maria~focal
# Tue, 31 Aug 2021 02:51:04 GMT
ENV MARIADB_VERSION=1:10.5.12+maria~focal
# Tue, 31 Aug 2021 02:51:04 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
# Tue, 31 Aug 2021 02:51:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 31 Aug 2021 02:51:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 31 Aug 2021 02:51:36 GMT
VOLUME [/var/lib/mysql]
# Tue, 31 Aug 2021 02:51:37 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Tue, 31 Aug 2021 02:51:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Aug 2021 02:51:37 GMT
EXPOSE 3306
# Tue, 31 Aug 2021 02:51:37 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:9fbf86d355c92d30b8de4c0360b0d79e1100e392d0885b6b5b302a1c3781dbf1`  
		Last Modified: Tue, 31 Aug 2021 01:44:13 GMT  
		Size: 27.1 MB (27127470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5652d937cd93c6c333210a7c5783a5defbac72c096a74537a0e99da179e69e15`  
		Last Modified: Tue, 31 Aug 2021 02:52:15 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1b48caf1d89a34f08f8ee38f48260ccfd25cfdc0e5425a1f7e2e1c3bc1c8cf0`  
		Last Modified: Tue, 31 Aug 2021 02:52:16 GMT  
		Size: 5.4 MB (5380989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352b2892aadbd934d1a0415ca24f71baf53ef4b324fe9f8772a37405d8607dba`  
		Last Modified: Tue, 31 Aug 2021 02:52:16 GMT  
		Size: 3.2 MB (3241880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354edb6860dbb419b59714606f392488735bc5e9adc7496059e98f51de24d84a`  
		Last Modified: Tue, 31 Aug 2021 02:52:15 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9934bdf22d9a668fcaab9695424d4074294aef89d849a8c8ba80b0bb31ab2ab9`  
		Last Modified: Tue, 31 Aug 2021 02:52:13 GMT  
		Size: 2.2 MB (2186296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a940a6a2154f17326f40b9d4619aa517978b7eed0f68a8a68738928defef66`  
		Last Modified: Tue, 31 Aug 2021 02:52:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d59cabe74a3e7d613c1b80e665c9d8541a8fb4d41ab6cccf7ef511b3569bc83f`  
		Last Modified: Tue, 31 Aug 2021 02:52:48 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fa3d9203216e56ee658b3d6a772799aa5553bbff52dd9ef9ff3d46d26606344`  
		Last Modified: Tue, 31 Aug 2021 02:53:01 GMT  
		Size: 88.1 MB (88107279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95dfd07848bf5afc8800b1141a2c38c414b30cef83cbd4348dd432a963366095`  
		Last Modified: Tue, 31 Aug 2021 02:52:48 GMT  
		Size: 5.6 KB (5606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.6`

```console
$ docker pull mariadb@sha256:b95f3b88e2880bf1191712c122a4c5998b380c4f1afb87ab9fc1415c0ea0b9ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.6` - linux; amd64

```console
$ docker pull mariadb@sha256:2e955f90e3af94a992b3e63d34c93e875706d0ec672b18202630ded0706dde71
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.0 MB (127012840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45eaeedf03deed202dade660cbfe44ae17cac512cfd23ca2becab1cd20b5a6f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:05:00 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 27 Jul 2021 00:05:14 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:05:15 GMT
ENV GOSU_VERSION=1.13
# Tue, 27 Jul 2021 00:05:26 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 27 Jul 2021 00:05:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 27 Jul 2021 00:05:34 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:05:35 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 27 Jul 2021 00:05:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 27 Jul 2021 00:05:37 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 27 Jul 2021 00:05:37 GMT
ENV MARIADB_MAJOR=10.6
# Mon, 09 Aug 2021 19:24:13 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Mon, 09 Aug 2021 19:24:14 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Mon, 09 Aug 2021 19:24:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Mon, 09 Aug 2021 19:24:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 09 Aug 2021 19:24:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 09 Aug 2021 19:24:55 GMT
VOLUME [/var/lib/mysql]
# Mon, 09 Aug 2021 19:24:55 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Mon, 09 Aug 2021 19:24:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Aug 2021 19:24:55 GMT
EXPOSE 3306
# Mon, 09 Aug 2021 19:24:56 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf20e69555c2118df81cd7906473b0bbef5210f014d45113251b1298fb1c996`  
		Last Modified: Tue, 27 Jul 2021 00:10:02 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69afd1ffc85b8fe385e48d00e89467a4e080c81b2447ce86ebf964f3e43efb9`  
		Last Modified: Tue, 27 Jul 2021 00:10:04 GMT  
		Size: 5.5 MB (5488764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e720dc7fcd8609016e69543f354117290ffee7c9ea1bdd97d7ca84bcc06d616`  
		Last Modified: Tue, 27 Jul 2021 00:10:03 GMT  
		Size: 3.6 MB (3582379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a81d177e410065c8eec2b5c018ab6ac60b2a5161184890bc3bf7627e78fb2dd`  
		Last Modified: Tue, 27 Jul 2021 00:10:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827c8c103c898d23db5f0cfc69b6faa45038d27b1ec3c15cb5d5b29ee60fca0b`  
		Last Modified: Tue, 27 Jul 2021 00:09:59 GMT  
		Size: 2.3 MB (2274133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2108ccd013748c7fce6a19a3f7434b860401f78326ac7373c486eafa3c719354`  
		Last Modified: Tue, 27 Jul 2021 00:09:59 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05414cb5e8f4dcf16b70640f3bcf904bafddd184d3971881c10b194fb74e8a0`  
		Last Modified: Mon, 09 Aug 2021 19:27:56 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6981930106c6d6380293a728b1bda2840d2392194e1b19649b7a863e1174054`  
		Last Modified: Mon, 09 Aug 2021 19:28:09 GMT  
		Size: 87.1 MB (87089293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009b7e8d11861e3f00504f9b3ff616177ec6f4e7f14f2e0162b0f92811c73bca`  
		Last Modified: Mon, 09 Aug 2021 19:27:56 GMT  
		Size: 5.6 KB (5613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:d6a5e003eae42397f7ee4589e9f21e231d3721ac131970d2286bd616e7f55bb4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124308266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63449ffc5ac65f64a30f340aa4db0c8d502f74c51962eb9b969f08999b20604e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:44 GMT
ADD file:cec21619ecbd37b4cf8da15153b8957a343cd25c6f714e3ac3969b6003704a58 in / 
# Tue, 31 Aug 2021 01:40:45 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:04:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 31 Aug 2021 03:04:38 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:04:38 GMT
ENV GOSU_VERSION=1.13
# Tue, 31 Aug 2021 03:04:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 31 Aug 2021 03:04:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 31 Aug 2021 03:04:57 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:04:57 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 31 Aug 2021 03:05:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 31 Aug 2021 03:05:05 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 31 Aug 2021 03:05:05 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 31 Aug 2021 03:05:05 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Tue, 31 Aug 2021 03:05:05 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Tue, 31 Aug 2021 03:05:05 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Tue, 31 Aug 2021 03:05:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 31 Aug 2021 03:05:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 31 Aug 2021 03:05:28 GMT
VOLUME [/var/lib/mysql]
# Tue, 31 Aug 2021 03:05:29 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Tue, 31 Aug 2021 03:05:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Aug 2021 03:05:29 GMT
EXPOSE 3306
# Tue, 31 Aug 2021 03:05:29 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ab2d02b1ec420fdb84c9f52abda403b6aef20f5de904a2ecda5ae4f5cd6e4d46`  
		Last Modified: Tue, 31 Aug 2021 01:42:34 GMT  
		Size: 27.2 MB (27173099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d16f1b8a1bc9060d0c98a0e09c73ceab3d694a99f57672d6e44f2f5dcf09eae`  
		Last Modified: Tue, 31 Aug 2021 03:09:41 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16d8285f3be08ea7340eaf6dced5161164096c3fb3345fe8c5d6d64496bc143`  
		Last Modified: Tue, 31 Aug 2021 03:09:40 GMT  
		Size: 5.5 MB (5455084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ffd6c9eed67b115939ab5f6d4bb8ffd2f0f152fe9a61024122b558e83ce912e`  
		Last Modified: Tue, 31 Aug 2021 03:09:39 GMT  
		Size: 3.4 MB (3368457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdbc2935c20fd14d96044dcdb65fb79a0f676bcdf334058da282716411d3ff9b`  
		Last Modified: Tue, 31 Aug 2021 03:09:39 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b302bb5f11cae70b4c8ec1079e6de6c62dacfdce3e8f3ccdfabd6ce44b63d2`  
		Last Modified: Tue, 31 Aug 2021 03:09:37 GMT  
		Size: 2.2 MB (2203569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21de8a622698dffd65e882759b0b6e4fe0e56b60d892f2e4446f94439a1270f`  
		Last Modified: Tue, 31 Aug 2021 03:09:36 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9389e144f5d4ea04b6dc1760537798680338137683d9e509ac7072a5c7282d9`  
		Last Modified: Tue, 31 Aug 2021 03:09:36 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed66c3adfe54028b15ff801e6142c6ae4f65eb2bfd313aed2281deb53c447a1a`  
		Last Modified: Tue, 31 Aug 2021 03:09:51 GMT  
		Size: 86.1 MB (86097727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440559db5c8c5208fa4fd147135bce07d75b0f4a04cc838207b125cb6e4cfcbe`  
		Last Modified: Tue, 31 Aug 2021 03:09:38 GMT  
		Size: 5.6 KB (5609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6` - linux; ppc64le

```console
$ docker pull mariadb@sha256:0cf82c9d58ae3326749b0fe0ed1f094d02516dba9c3e6fdf9d2c193f2fa48b4a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137540073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20c817c255cdeba976f7d5a97418f28626785a200c99e223a6450298661f4b64`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 26 Jul 2021 23:12:46 GMT
ADD file:68eb628c2202763afa91d554dde9668d8a468fe53fdbd2fe98627a5f91d224b4 in / 
# Mon, 26 Jul 2021 23:12:49 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 02:05:55 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 27 Jul 2021 02:06:47 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:06:50 GMT
ENV GOSU_VERSION=1.13
# Tue, 27 Jul 2021 02:07:32 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 27 Jul 2021 02:07:42 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 27 Jul 2021 02:08:11 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:08:14 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 27 Jul 2021 02:08:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 27 Jul 2021 02:08:24 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 27 Jul 2021 02:08:25 GMT
ENV MARIADB_MAJOR=10.6
# Mon, 09 Aug 2021 19:17:05 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Mon, 09 Aug 2021 19:17:08 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Mon, 09 Aug 2021 19:17:10 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Mon, 09 Aug 2021 19:17:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 09 Aug 2021 19:22:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 09 Aug 2021 19:22:56 GMT
VOLUME [/var/lib/mysql]
# Mon, 09 Aug 2021 19:23:00 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Mon, 09 Aug 2021 19:23:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Aug 2021 19:23:12 GMT
EXPOSE 3306
# Mon, 09 Aug 2021 19:23:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:1a396eed835b3b7b4101a9863d174e145ddbb1de1502a63bae726b0f81e7ca93`  
		Last Modified: Mon, 26 Jul 2021 23:15:51 GMT  
		Size: 33.3 MB (33290427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65be85b12a63573ebccb059357c5c0db6046f4a074454eea617c402e3bf99c1f`  
		Last Modified: Tue, 27 Jul 2021 02:26:16 GMT  
		Size: 1.8 KB (1760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:803c8e5bf0c59b9b01b70cac07bb24bc696bc577d8e74c79ff15bcbd480874b4`  
		Last Modified: Tue, 27 Jul 2021 02:26:17 GMT  
		Size: 6.7 MB (6667884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62bd7bf9c00152c4fb338b2c1a01d5b241ceda5c58d9e700a353072ab80fb4b9`  
		Last Modified: Tue, 27 Jul 2021 02:26:17 GMT  
		Size: 3.7 MB (3670853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:372602ac4ce9a3a693cb97ec9b3e71b449fdafbaded2ce2937fec39cec9c9b6e`  
		Last Modified: Tue, 27 Jul 2021 02:26:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a80c4de70a1ded78cf0175b1f5fda38b3119857dd2d8d9f1fafcdc39eafef0e`  
		Last Modified: Tue, 27 Jul 2021 02:26:13 GMT  
		Size: 2.6 MB (2569871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc8dec87672a96e86220faa6c3e98577b2a9090fc81d81efb4681fe59e732b7`  
		Last Modified: Tue, 27 Jul 2021 02:26:12 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce893fcc2e86ea1fb70c9730683306fb99ed9b96529607badefbeb824f32081`  
		Last Modified: Mon, 09 Aug 2021 19:45:06 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea2b83ad4dfbaa9a9aa432f398880354589538421ef773a7bdc59bf41856282`  
		Last Modified: Mon, 09 Aug 2021 19:45:24 GMT  
		Size: 91.3 MB (91330692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e301a165b39ae64033fe826324cbfdf9f8e0e01fd8d20d7e69f7a8b771aa41`  
		Last Modified: Mon, 09 Aug 2021 19:45:06 GMT  
		Size: 5.6 KB (5617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6` - linux; s390x

```console
$ docker pull mariadb@sha256:f338e06fc65ca71eda1ac48527970da30cd5b3f1316fbb5974cd2ea2ffa87152
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.0 MB (126020736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12c9756f3b2fe668579749a2963c372a54db873f6e054bbf6f6ca8702b5d6d1f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:23 GMT
ADD file:979855f79ebaca36cc7878f71b2326f1cd189970fdb223b37cd64ee12d1c9a2b in / 
# Tue, 31 Aug 2021 01:42:27 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:49:44 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 31 Aug 2021 02:49:51 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:49:51 GMT
ENV GOSU_VERSION=1.13
# Tue, 31 Aug 2021 02:50:04 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 31 Aug 2021 02:50:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 31 Aug 2021 02:50:12 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:50:12 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 31 Aug 2021 02:50:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 31 Aug 2021 02:50:18 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 31 Aug 2021 02:50:18 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 31 Aug 2021 02:50:19 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Tue, 31 Aug 2021 02:50:19 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Tue, 31 Aug 2021 02:50:19 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Tue, 31 Aug 2021 02:50:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 31 Aug 2021 02:50:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 31 Aug 2021 02:50:49 GMT
VOLUME [/var/lib/mysql]
# Tue, 31 Aug 2021 02:50:49 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Tue, 31 Aug 2021 02:50:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Aug 2021 02:50:49 GMT
EXPOSE 3306
# Tue, 31 Aug 2021 02:50:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:9fbf86d355c92d30b8de4c0360b0d79e1100e392d0885b6b5b302a1c3781dbf1`  
		Last Modified: Tue, 31 Aug 2021 01:44:13 GMT  
		Size: 27.1 MB (27127470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5652d937cd93c6c333210a7c5783a5defbac72c096a74537a0e99da179e69e15`  
		Last Modified: Tue, 31 Aug 2021 02:52:15 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1b48caf1d89a34f08f8ee38f48260ccfd25cfdc0e5425a1f7e2e1c3bc1c8cf0`  
		Last Modified: Tue, 31 Aug 2021 02:52:16 GMT  
		Size: 5.4 MB (5380989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352b2892aadbd934d1a0415ca24f71baf53ef4b324fe9f8772a37405d8607dba`  
		Last Modified: Tue, 31 Aug 2021 02:52:16 GMT  
		Size: 3.2 MB (3241880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354edb6860dbb419b59714606f392488735bc5e9adc7496059e98f51de24d84a`  
		Last Modified: Tue, 31 Aug 2021 02:52:15 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9934bdf22d9a668fcaab9695424d4074294aef89d849a8c8ba80b0bb31ab2ab9`  
		Last Modified: Tue, 31 Aug 2021 02:52:13 GMT  
		Size: 2.2 MB (2186296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a940a6a2154f17326f40b9d4619aa517978b7eed0f68a8a68738928defef66`  
		Last Modified: Tue, 31 Aug 2021 02:52:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6840dfebdaf0d0162e783790b87c1c9eff72aca9dc017163baa2059ac974ec21`  
		Last Modified: Tue, 31 Aug 2021 02:52:13 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:badfbe5adb85e7a406e6d7af361229a125b295cec1d104f15f0334488fb8e38d`  
		Last Modified: Tue, 31 Aug 2021 02:52:26 GMT  
		Size: 88.1 MB (88073778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa96305d4f85828482207efa32cb56c1fcbf6bf32d41e5f7ca27f479f57acec9`  
		Last Modified: Tue, 31 Aug 2021 02:52:13 GMT  
		Size: 5.6 KB (5608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.6-focal`

```console
$ docker pull mariadb@sha256:b95f3b88e2880bf1191712c122a4c5998b380c4f1afb87ab9fc1415c0ea0b9ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.6-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:2e955f90e3af94a992b3e63d34c93e875706d0ec672b18202630ded0706dde71
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.0 MB (127012840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45eaeedf03deed202dade660cbfe44ae17cac512cfd23ca2becab1cd20b5a6f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:05:00 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 27 Jul 2021 00:05:14 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:05:15 GMT
ENV GOSU_VERSION=1.13
# Tue, 27 Jul 2021 00:05:26 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 27 Jul 2021 00:05:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 27 Jul 2021 00:05:34 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:05:35 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 27 Jul 2021 00:05:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 27 Jul 2021 00:05:37 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 27 Jul 2021 00:05:37 GMT
ENV MARIADB_MAJOR=10.6
# Mon, 09 Aug 2021 19:24:13 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Mon, 09 Aug 2021 19:24:14 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Mon, 09 Aug 2021 19:24:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Mon, 09 Aug 2021 19:24:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 09 Aug 2021 19:24:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 09 Aug 2021 19:24:55 GMT
VOLUME [/var/lib/mysql]
# Mon, 09 Aug 2021 19:24:55 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Mon, 09 Aug 2021 19:24:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Aug 2021 19:24:55 GMT
EXPOSE 3306
# Mon, 09 Aug 2021 19:24:56 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf20e69555c2118df81cd7906473b0bbef5210f014d45113251b1298fb1c996`  
		Last Modified: Tue, 27 Jul 2021 00:10:02 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69afd1ffc85b8fe385e48d00e89467a4e080c81b2447ce86ebf964f3e43efb9`  
		Last Modified: Tue, 27 Jul 2021 00:10:04 GMT  
		Size: 5.5 MB (5488764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e720dc7fcd8609016e69543f354117290ffee7c9ea1bdd97d7ca84bcc06d616`  
		Last Modified: Tue, 27 Jul 2021 00:10:03 GMT  
		Size: 3.6 MB (3582379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a81d177e410065c8eec2b5c018ab6ac60b2a5161184890bc3bf7627e78fb2dd`  
		Last Modified: Tue, 27 Jul 2021 00:10:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827c8c103c898d23db5f0cfc69b6faa45038d27b1ec3c15cb5d5b29ee60fca0b`  
		Last Modified: Tue, 27 Jul 2021 00:09:59 GMT  
		Size: 2.3 MB (2274133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2108ccd013748c7fce6a19a3f7434b860401f78326ac7373c486eafa3c719354`  
		Last Modified: Tue, 27 Jul 2021 00:09:59 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05414cb5e8f4dcf16b70640f3bcf904bafddd184d3971881c10b194fb74e8a0`  
		Last Modified: Mon, 09 Aug 2021 19:27:56 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6981930106c6d6380293a728b1bda2840d2392194e1b19649b7a863e1174054`  
		Last Modified: Mon, 09 Aug 2021 19:28:09 GMT  
		Size: 87.1 MB (87089293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009b7e8d11861e3f00504f9b3ff616177ec6f4e7f14f2e0162b0f92811c73bca`  
		Last Modified: Mon, 09 Aug 2021 19:27:56 GMT  
		Size: 5.6 KB (5613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:d6a5e003eae42397f7ee4589e9f21e231d3721ac131970d2286bd616e7f55bb4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124308266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63449ffc5ac65f64a30f340aa4db0c8d502f74c51962eb9b969f08999b20604e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:44 GMT
ADD file:cec21619ecbd37b4cf8da15153b8957a343cd25c6f714e3ac3969b6003704a58 in / 
# Tue, 31 Aug 2021 01:40:45 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:04:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 31 Aug 2021 03:04:38 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:04:38 GMT
ENV GOSU_VERSION=1.13
# Tue, 31 Aug 2021 03:04:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 31 Aug 2021 03:04:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 31 Aug 2021 03:04:57 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:04:57 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 31 Aug 2021 03:05:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 31 Aug 2021 03:05:05 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 31 Aug 2021 03:05:05 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 31 Aug 2021 03:05:05 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Tue, 31 Aug 2021 03:05:05 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Tue, 31 Aug 2021 03:05:05 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Tue, 31 Aug 2021 03:05:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 31 Aug 2021 03:05:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 31 Aug 2021 03:05:28 GMT
VOLUME [/var/lib/mysql]
# Tue, 31 Aug 2021 03:05:29 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Tue, 31 Aug 2021 03:05:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Aug 2021 03:05:29 GMT
EXPOSE 3306
# Tue, 31 Aug 2021 03:05:29 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ab2d02b1ec420fdb84c9f52abda403b6aef20f5de904a2ecda5ae4f5cd6e4d46`  
		Last Modified: Tue, 31 Aug 2021 01:42:34 GMT  
		Size: 27.2 MB (27173099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d16f1b8a1bc9060d0c98a0e09c73ceab3d694a99f57672d6e44f2f5dcf09eae`  
		Last Modified: Tue, 31 Aug 2021 03:09:41 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16d8285f3be08ea7340eaf6dced5161164096c3fb3345fe8c5d6d64496bc143`  
		Last Modified: Tue, 31 Aug 2021 03:09:40 GMT  
		Size: 5.5 MB (5455084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ffd6c9eed67b115939ab5f6d4bb8ffd2f0f152fe9a61024122b558e83ce912e`  
		Last Modified: Tue, 31 Aug 2021 03:09:39 GMT  
		Size: 3.4 MB (3368457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdbc2935c20fd14d96044dcdb65fb79a0f676bcdf334058da282716411d3ff9b`  
		Last Modified: Tue, 31 Aug 2021 03:09:39 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b302bb5f11cae70b4c8ec1079e6de6c62dacfdce3e8f3ccdfabd6ce44b63d2`  
		Last Modified: Tue, 31 Aug 2021 03:09:37 GMT  
		Size: 2.2 MB (2203569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21de8a622698dffd65e882759b0b6e4fe0e56b60d892f2e4446f94439a1270f`  
		Last Modified: Tue, 31 Aug 2021 03:09:36 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9389e144f5d4ea04b6dc1760537798680338137683d9e509ac7072a5c7282d9`  
		Last Modified: Tue, 31 Aug 2021 03:09:36 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed66c3adfe54028b15ff801e6142c6ae4f65eb2bfd313aed2281deb53c447a1a`  
		Last Modified: Tue, 31 Aug 2021 03:09:51 GMT  
		Size: 86.1 MB (86097727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440559db5c8c5208fa4fd147135bce07d75b0f4a04cc838207b125cb6e4cfcbe`  
		Last Modified: Tue, 31 Aug 2021 03:09:38 GMT  
		Size: 5.6 KB (5609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:0cf82c9d58ae3326749b0fe0ed1f094d02516dba9c3e6fdf9d2c193f2fa48b4a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137540073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20c817c255cdeba976f7d5a97418f28626785a200c99e223a6450298661f4b64`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 26 Jul 2021 23:12:46 GMT
ADD file:68eb628c2202763afa91d554dde9668d8a468fe53fdbd2fe98627a5f91d224b4 in / 
# Mon, 26 Jul 2021 23:12:49 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 02:05:55 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 27 Jul 2021 02:06:47 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:06:50 GMT
ENV GOSU_VERSION=1.13
# Tue, 27 Jul 2021 02:07:32 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 27 Jul 2021 02:07:42 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 27 Jul 2021 02:08:11 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:08:14 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 27 Jul 2021 02:08:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 27 Jul 2021 02:08:24 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 27 Jul 2021 02:08:25 GMT
ENV MARIADB_MAJOR=10.6
# Mon, 09 Aug 2021 19:17:05 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Mon, 09 Aug 2021 19:17:08 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Mon, 09 Aug 2021 19:17:10 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Mon, 09 Aug 2021 19:17:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 09 Aug 2021 19:22:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 09 Aug 2021 19:22:56 GMT
VOLUME [/var/lib/mysql]
# Mon, 09 Aug 2021 19:23:00 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Mon, 09 Aug 2021 19:23:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Aug 2021 19:23:12 GMT
EXPOSE 3306
# Mon, 09 Aug 2021 19:23:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:1a396eed835b3b7b4101a9863d174e145ddbb1de1502a63bae726b0f81e7ca93`  
		Last Modified: Mon, 26 Jul 2021 23:15:51 GMT  
		Size: 33.3 MB (33290427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65be85b12a63573ebccb059357c5c0db6046f4a074454eea617c402e3bf99c1f`  
		Last Modified: Tue, 27 Jul 2021 02:26:16 GMT  
		Size: 1.8 KB (1760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:803c8e5bf0c59b9b01b70cac07bb24bc696bc577d8e74c79ff15bcbd480874b4`  
		Last Modified: Tue, 27 Jul 2021 02:26:17 GMT  
		Size: 6.7 MB (6667884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62bd7bf9c00152c4fb338b2c1a01d5b241ceda5c58d9e700a353072ab80fb4b9`  
		Last Modified: Tue, 27 Jul 2021 02:26:17 GMT  
		Size: 3.7 MB (3670853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:372602ac4ce9a3a693cb97ec9b3e71b449fdafbaded2ce2937fec39cec9c9b6e`  
		Last Modified: Tue, 27 Jul 2021 02:26:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a80c4de70a1ded78cf0175b1f5fda38b3119857dd2d8d9f1fafcdc39eafef0e`  
		Last Modified: Tue, 27 Jul 2021 02:26:13 GMT  
		Size: 2.6 MB (2569871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc8dec87672a96e86220faa6c3e98577b2a9090fc81d81efb4681fe59e732b7`  
		Last Modified: Tue, 27 Jul 2021 02:26:12 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce893fcc2e86ea1fb70c9730683306fb99ed9b96529607badefbeb824f32081`  
		Last Modified: Mon, 09 Aug 2021 19:45:06 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea2b83ad4dfbaa9a9aa432f398880354589538421ef773a7bdc59bf41856282`  
		Last Modified: Mon, 09 Aug 2021 19:45:24 GMT  
		Size: 91.3 MB (91330692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e301a165b39ae64033fe826324cbfdf9f8e0e01fd8d20d7e69f7a8b771aa41`  
		Last Modified: Mon, 09 Aug 2021 19:45:06 GMT  
		Size: 5.6 KB (5617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:f338e06fc65ca71eda1ac48527970da30cd5b3f1316fbb5974cd2ea2ffa87152
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.0 MB (126020736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12c9756f3b2fe668579749a2963c372a54db873f6e054bbf6f6ca8702b5d6d1f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:23 GMT
ADD file:979855f79ebaca36cc7878f71b2326f1cd189970fdb223b37cd64ee12d1c9a2b in / 
# Tue, 31 Aug 2021 01:42:27 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:49:44 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 31 Aug 2021 02:49:51 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:49:51 GMT
ENV GOSU_VERSION=1.13
# Tue, 31 Aug 2021 02:50:04 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 31 Aug 2021 02:50:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 31 Aug 2021 02:50:12 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:50:12 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 31 Aug 2021 02:50:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 31 Aug 2021 02:50:18 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 31 Aug 2021 02:50:18 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 31 Aug 2021 02:50:19 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Tue, 31 Aug 2021 02:50:19 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Tue, 31 Aug 2021 02:50:19 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Tue, 31 Aug 2021 02:50:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 31 Aug 2021 02:50:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 31 Aug 2021 02:50:49 GMT
VOLUME [/var/lib/mysql]
# Tue, 31 Aug 2021 02:50:49 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Tue, 31 Aug 2021 02:50:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Aug 2021 02:50:49 GMT
EXPOSE 3306
# Tue, 31 Aug 2021 02:50:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:9fbf86d355c92d30b8de4c0360b0d79e1100e392d0885b6b5b302a1c3781dbf1`  
		Last Modified: Tue, 31 Aug 2021 01:44:13 GMT  
		Size: 27.1 MB (27127470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5652d937cd93c6c333210a7c5783a5defbac72c096a74537a0e99da179e69e15`  
		Last Modified: Tue, 31 Aug 2021 02:52:15 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1b48caf1d89a34f08f8ee38f48260ccfd25cfdc0e5425a1f7e2e1c3bc1c8cf0`  
		Last Modified: Tue, 31 Aug 2021 02:52:16 GMT  
		Size: 5.4 MB (5380989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352b2892aadbd934d1a0415ca24f71baf53ef4b324fe9f8772a37405d8607dba`  
		Last Modified: Tue, 31 Aug 2021 02:52:16 GMT  
		Size: 3.2 MB (3241880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354edb6860dbb419b59714606f392488735bc5e9adc7496059e98f51de24d84a`  
		Last Modified: Tue, 31 Aug 2021 02:52:15 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9934bdf22d9a668fcaab9695424d4074294aef89d849a8c8ba80b0bb31ab2ab9`  
		Last Modified: Tue, 31 Aug 2021 02:52:13 GMT  
		Size: 2.2 MB (2186296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a940a6a2154f17326f40b9d4619aa517978b7eed0f68a8a68738928defef66`  
		Last Modified: Tue, 31 Aug 2021 02:52:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6840dfebdaf0d0162e783790b87c1c9eff72aca9dc017163baa2059ac974ec21`  
		Last Modified: Tue, 31 Aug 2021 02:52:13 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:badfbe5adb85e7a406e6d7af361229a125b295cec1d104f15f0334488fb8e38d`  
		Last Modified: Tue, 31 Aug 2021 02:52:26 GMT  
		Size: 88.1 MB (88073778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa96305d4f85828482207efa32cb56c1fcbf6bf32d41e5f7ca27f479f57acec9`  
		Last Modified: Tue, 31 Aug 2021 02:52:13 GMT  
		Size: 5.6 KB (5608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.6.4`

```console
$ docker pull mariadb@sha256:b95f3b88e2880bf1191712c122a4c5998b380c4f1afb87ab9fc1415c0ea0b9ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.6.4` - linux; amd64

```console
$ docker pull mariadb@sha256:2e955f90e3af94a992b3e63d34c93e875706d0ec672b18202630ded0706dde71
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.0 MB (127012840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45eaeedf03deed202dade660cbfe44ae17cac512cfd23ca2becab1cd20b5a6f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:05:00 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 27 Jul 2021 00:05:14 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:05:15 GMT
ENV GOSU_VERSION=1.13
# Tue, 27 Jul 2021 00:05:26 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 27 Jul 2021 00:05:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 27 Jul 2021 00:05:34 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:05:35 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 27 Jul 2021 00:05:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 27 Jul 2021 00:05:37 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 27 Jul 2021 00:05:37 GMT
ENV MARIADB_MAJOR=10.6
# Mon, 09 Aug 2021 19:24:13 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Mon, 09 Aug 2021 19:24:14 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Mon, 09 Aug 2021 19:24:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Mon, 09 Aug 2021 19:24:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 09 Aug 2021 19:24:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 09 Aug 2021 19:24:55 GMT
VOLUME [/var/lib/mysql]
# Mon, 09 Aug 2021 19:24:55 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Mon, 09 Aug 2021 19:24:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Aug 2021 19:24:55 GMT
EXPOSE 3306
# Mon, 09 Aug 2021 19:24:56 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf20e69555c2118df81cd7906473b0bbef5210f014d45113251b1298fb1c996`  
		Last Modified: Tue, 27 Jul 2021 00:10:02 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69afd1ffc85b8fe385e48d00e89467a4e080c81b2447ce86ebf964f3e43efb9`  
		Last Modified: Tue, 27 Jul 2021 00:10:04 GMT  
		Size: 5.5 MB (5488764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e720dc7fcd8609016e69543f354117290ffee7c9ea1bdd97d7ca84bcc06d616`  
		Last Modified: Tue, 27 Jul 2021 00:10:03 GMT  
		Size: 3.6 MB (3582379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a81d177e410065c8eec2b5c018ab6ac60b2a5161184890bc3bf7627e78fb2dd`  
		Last Modified: Tue, 27 Jul 2021 00:10:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827c8c103c898d23db5f0cfc69b6faa45038d27b1ec3c15cb5d5b29ee60fca0b`  
		Last Modified: Tue, 27 Jul 2021 00:09:59 GMT  
		Size: 2.3 MB (2274133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2108ccd013748c7fce6a19a3f7434b860401f78326ac7373c486eafa3c719354`  
		Last Modified: Tue, 27 Jul 2021 00:09:59 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05414cb5e8f4dcf16b70640f3bcf904bafddd184d3971881c10b194fb74e8a0`  
		Last Modified: Mon, 09 Aug 2021 19:27:56 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6981930106c6d6380293a728b1bda2840d2392194e1b19649b7a863e1174054`  
		Last Modified: Mon, 09 Aug 2021 19:28:09 GMT  
		Size: 87.1 MB (87089293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009b7e8d11861e3f00504f9b3ff616177ec6f4e7f14f2e0162b0f92811c73bca`  
		Last Modified: Mon, 09 Aug 2021 19:27:56 GMT  
		Size: 5.6 KB (5613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6.4` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:d6a5e003eae42397f7ee4589e9f21e231d3721ac131970d2286bd616e7f55bb4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124308266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63449ffc5ac65f64a30f340aa4db0c8d502f74c51962eb9b969f08999b20604e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:44 GMT
ADD file:cec21619ecbd37b4cf8da15153b8957a343cd25c6f714e3ac3969b6003704a58 in / 
# Tue, 31 Aug 2021 01:40:45 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:04:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 31 Aug 2021 03:04:38 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:04:38 GMT
ENV GOSU_VERSION=1.13
# Tue, 31 Aug 2021 03:04:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 31 Aug 2021 03:04:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 31 Aug 2021 03:04:57 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:04:57 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 31 Aug 2021 03:05:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 31 Aug 2021 03:05:05 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 31 Aug 2021 03:05:05 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 31 Aug 2021 03:05:05 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Tue, 31 Aug 2021 03:05:05 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Tue, 31 Aug 2021 03:05:05 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Tue, 31 Aug 2021 03:05:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 31 Aug 2021 03:05:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 31 Aug 2021 03:05:28 GMT
VOLUME [/var/lib/mysql]
# Tue, 31 Aug 2021 03:05:29 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Tue, 31 Aug 2021 03:05:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Aug 2021 03:05:29 GMT
EXPOSE 3306
# Tue, 31 Aug 2021 03:05:29 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ab2d02b1ec420fdb84c9f52abda403b6aef20f5de904a2ecda5ae4f5cd6e4d46`  
		Last Modified: Tue, 31 Aug 2021 01:42:34 GMT  
		Size: 27.2 MB (27173099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d16f1b8a1bc9060d0c98a0e09c73ceab3d694a99f57672d6e44f2f5dcf09eae`  
		Last Modified: Tue, 31 Aug 2021 03:09:41 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16d8285f3be08ea7340eaf6dced5161164096c3fb3345fe8c5d6d64496bc143`  
		Last Modified: Tue, 31 Aug 2021 03:09:40 GMT  
		Size: 5.5 MB (5455084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ffd6c9eed67b115939ab5f6d4bb8ffd2f0f152fe9a61024122b558e83ce912e`  
		Last Modified: Tue, 31 Aug 2021 03:09:39 GMT  
		Size: 3.4 MB (3368457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdbc2935c20fd14d96044dcdb65fb79a0f676bcdf334058da282716411d3ff9b`  
		Last Modified: Tue, 31 Aug 2021 03:09:39 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b302bb5f11cae70b4c8ec1079e6de6c62dacfdce3e8f3ccdfabd6ce44b63d2`  
		Last Modified: Tue, 31 Aug 2021 03:09:37 GMT  
		Size: 2.2 MB (2203569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21de8a622698dffd65e882759b0b6e4fe0e56b60d892f2e4446f94439a1270f`  
		Last Modified: Tue, 31 Aug 2021 03:09:36 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9389e144f5d4ea04b6dc1760537798680338137683d9e509ac7072a5c7282d9`  
		Last Modified: Tue, 31 Aug 2021 03:09:36 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed66c3adfe54028b15ff801e6142c6ae4f65eb2bfd313aed2281deb53c447a1a`  
		Last Modified: Tue, 31 Aug 2021 03:09:51 GMT  
		Size: 86.1 MB (86097727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440559db5c8c5208fa4fd147135bce07d75b0f4a04cc838207b125cb6e4cfcbe`  
		Last Modified: Tue, 31 Aug 2021 03:09:38 GMT  
		Size: 5.6 KB (5609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6.4` - linux; ppc64le

```console
$ docker pull mariadb@sha256:0cf82c9d58ae3326749b0fe0ed1f094d02516dba9c3e6fdf9d2c193f2fa48b4a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137540073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20c817c255cdeba976f7d5a97418f28626785a200c99e223a6450298661f4b64`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 26 Jul 2021 23:12:46 GMT
ADD file:68eb628c2202763afa91d554dde9668d8a468fe53fdbd2fe98627a5f91d224b4 in / 
# Mon, 26 Jul 2021 23:12:49 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 02:05:55 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 27 Jul 2021 02:06:47 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:06:50 GMT
ENV GOSU_VERSION=1.13
# Tue, 27 Jul 2021 02:07:32 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 27 Jul 2021 02:07:42 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 27 Jul 2021 02:08:11 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:08:14 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 27 Jul 2021 02:08:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 27 Jul 2021 02:08:24 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 27 Jul 2021 02:08:25 GMT
ENV MARIADB_MAJOR=10.6
# Mon, 09 Aug 2021 19:17:05 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Mon, 09 Aug 2021 19:17:08 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Mon, 09 Aug 2021 19:17:10 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Mon, 09 Aug 2021 19:17:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 09 Aug 2021 19:22:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 09 Aug 2021 19:22:56 GMT
VOLUME [/var/lib/mysql]
# Mon, 09 Aug 2021 19:23:00 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Mon, 09 Aug 2021 19:23:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Aug 2021 19:23:12 GMT
EXPOSE 3306
# Mon, 09 Aug 2021 19:23:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:1a396eed835b3b7b4101a9863d174e145ddbb1de1502a63bae726b0f81e7ca93`  
		Last Modified: Mon, 26 Jul 2021 23:15:51 GMT  
		Size: 33.3 MB (33290427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65be85b12a63573ebccb059357c5c0db6046f4a074454eea617c402e3bf99c1f`  
		Last Modified: Tue, 27 Jul 2021 02:26:16 GMT  
		Size: 1.8 KB (1760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:803c8e5bf0c59b9b01b70cac07bb24bc696bc577d8e74c79ff15bcbd480874b4`  
		Last Modified: Tue, 27 Jul 2021 02:26:17 GMT  
		Size: 6.7 MB (6667884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62bd7bf9c00152c4fb338b2c1a01d5b241ceda5c58d9e700a353072ab80fb4b9`  
		Last Modified: Tue, 27 Jul 2021 02:26:17 GMT  
		Size: 3.7 MB (3670853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:372602ac4ce9a3a693cb97ec9b3e71b449fdafbaded2ce2937fec39cec9c9b6e`  
		Last Modified: Tue, 27 Jul 2021 02:26:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a80c4de70a1ded78cf0175b1f5fda38b3119857dd2d8d9f1fafcdc39eafef0e`  
		Last Modified: Tue, 27 Jul 2021 02:26:13 GMT  
		Size: 2.6 MB (2569871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc8dec87672a96e86220faa6c3e98577b2a9090fc81d81efb4681fe59e732b7`  
		Last Modified: Tue, 27 Jul 2021 02:26:12 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce893fcc2e86ea1fb70c9730683306fb99ed9b96529607badefbeb824f32081`  
		Last Modified: Mon, 09 Aug 2021 19:45:06 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea2b83ad4dfbaa9a9aa432f398880354589538421ef773a7bdc59bf41856282`  
		Last Modified: Mon, 09 Aug 2021 19:45:24 GMT  
		Size: 91.3 MB (91330692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e301a165b39ae64033fe826324cbfdf9f8e0e01fd8d20d7e69f7a8b771aa41`  
		Last Modified: Mon, 09 Aug 2021 19:45:06 GMT  
		Size: 5.6 KB (5617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6.4` - linux; s390x

```console
$ docker pull mariadb@sha256:f338e06fc65ca71eda1ac48527970da30cd5b3f1316fbb5974cd2ea2ffa87152
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.0 MB (126020736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12c9756f3b2fe668579749a2963c372a54db873f6e054bbf6f6ca8702b5d6d1f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:23 GMT
ADD file:979855f79ebaca36cc7878f71b2326f1cd189970fdb223b37cd64ee12d1c9a2b in / 
# Tue, 31 Aug 2021 01:42:27 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:49:44 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 31 Aug 2021 02:49:51 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:49:51 GMT
ENV GOSU_VERSION=1.13
# Tue, 31 Aug 2021 02:50:04 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 31 Aug 2021 02:50:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 31 Aug 2021 02:50:12 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:50:12 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 31 Aug 2021 02:50:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 31 Aug 2021 02:50:18 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 31 Aug 2021 02:50:18 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 31 Aug 2021 02:50:19 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Tue, 31 Aug 2021 02:50:19 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Tue, 31 Aug 2021 02:50:19 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Tue, 31 Aug 2021 02:50:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 31 Aug 2021 02:50:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 31 Aug 2021 02:50:49 GMT
VOLUME [/var/lib/mysql]
# Tue, 31 Aug 2021 02:50:49 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Tue, 31 Aug 2021 02:50:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Aug 2021 02:50:49 GMT
EXPOSE 3306
# Tue, 31 Aug 2021 02:50:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:9fbf86d355c92d30b8de4c0360b0d79e1100e392d0885b6b5b302a1c3781dbf1`  
		Last Modified: Tue, 31 Aug 2021 01:44:13 GMT  
		Size: 27.1 MB (27127470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5652d937cd93c6c333210a7c5783a5defbac72c096a74537a0e99da179e69e15`  
		Last Modified: Tue, 31 Aug 2021 02:52:15 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1b48caf1d89a34f08f8ee38f48260ccfd25cfdc0e5425a1f7e2e1c3bc1c8cf0`  
		Last Modified: Tue, 31 Aug 2021 02:52:16 GMT  
		Size: 5.4 MB (5380989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352b2892aadbd934d1a0415ca24f71baf53ef4b324fe9f8772a37405d8607dba`  
		Last Modified: Tue, 31 Aug 2021 02:52:16 GMT  
		Size: 3.2 MB (3241880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354edb6860dbb419b59714606f392488735bc5e9adc7496059e98f51de24d84a`  
		Last Modified: Tue, 31 Aug 2021 02:52:15 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9934bdf22d9a668fcaab9695424d4074294aef89d849a8c8ba80b0bb31ab2ab9`  
		Last Modified: Tue, 31 Aug 2021 02:52:13 GMT  
		Size: 2.2 MB (2186296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a940a6a2154f17326f40b9d4619aa517978b7eed0f68a8a68738928defef66`  
		Last Modified: Tue, 31 Aug 2021 02:52:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6840dfebdaf0d0162e783790b87c1c9eff72aca9dc017163baa2059ac974ec21`  
		Last Modified: Tue, 31 Aug 2021 02:52:13 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:badfbe5adb85e7a406e6d7af361229a125b295cec1d104f15f0334488fb8e38d`  
		Last Modified: Tue, 31 Aug 2021 02:52:26 GMT  
		Size: 88.1 MB (88073778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa96305d4f85828482207efa32cb56c1fcbf6bf32d41e5f7ca27f479f57acec9`  
		Last Modified: Tue, 31 Aug 2021 02:52:13 GMT  
		Size: 5.6 KB (5608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.6.4-focal`

```console
$ docker pull mariadb@sha256:b95f3b88e2880bf1191712c122a4c5998b380c4f1afb87ab9fc1415c0ea0b9ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.6.4-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:2e955f90e3af94a992b3e63d34c93e875706d0ec672b18202630ded0706dde71
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.0 MB (127012840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45eaeedf03deed202dade660cbfe44ae17cac512cfd23ca2becab1cd20b5a6f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:05:00 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 27 Jul 2021 00:05:14 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:05:15 GMT
ENV GOSU_VERSION=1.13
# Tue, 27 Jul 2021 00:05:26 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 27 Jul 2021 00:05:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 27 Jul 2021 00:05:34 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:05:35 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 27 Jul 2021 00:05:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 27 Jul 2021 00:05:37 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 27 Jul 2021 00:05:37 GMT
ENV MARIADB_MAJOR=10.6
# Mon, 09 Aug 2021 19:24:13 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Mon, 09 Aug 2021 19:24:14 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Mon, 09 Aug 2021 19:24:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Mon, 09 Aug 2021 19:24:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 09 Aug 2021 19:24:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 09 Aug 2021 19:24:55 GMT
VOLUME [/var/lib/mysql]
# Mon, 09 Aug 2021 19:24:55 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Mon, 09 Aug 2021 19:24:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Aug 2021 19:24:55 GMT
EXPOSE 3306
# Mon, 09 Aug 2021 19:24:56 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf20e69555c2118df81cd7906473b0bbef5210f014d45113251b1298fb1c996`  
		Last Modified: Tue, 27 Jul 2021 00:10:02 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69afd1ffc85b8fe385e48d00e89467a4e080c81b2447ce86ebf964f3e43efb9`  
		Last Modified: Tue, 27 Jul 2021 00:10:04 GMT  
		Size: 5.5 MB (5488764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e720dc7fcd8609016e69543f354117290ffee7c9ea1bdd97d7ca84bcc06d616`  
		Last Modified: Tue, 27 Jul 2021 00:10:03 GMT  
		Size: 3.6 MB (3582379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a81d177e410065c8eec2b5c018ab6ac60b2a5161184890bc3bf7627e78fb2dd`  
		Last Modified: Tue, 27 Jul 2021 00:10:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827c8c103c898d23db5f0cfc69b6faa45038d27b1ec3c15cb5d5b29ee60fca0b`  
		Last Modified: Tue, 27 Jul 2021 00:09:59 GMT  
		Size: 2.3 MB (2274133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2108ccd013748c7fce6a19a3f7434b860401f78326ac7373c486eafa3c719354`  
		Last Modified: Tue, 27 Jul 2021 00:09:59 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05414cb5e8f4dcf16b70640f3bcf904bafddd184d3971881c10b194fb74e8a0`  
		Last Modified: Mon, 09 Aug 2021 19:27:56 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6981930106c6d6380293a728b1bda2840d2392194e1b19649b7a863e1174054`  
		Last Modified: Mon, 09 Aug 2021 19:28:09 GMT  
		Size: 87.1 MB (87089293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009b7e8d11861e3f00504f9b3ff616177ec6f4e7f14f2e0162b0f92811c73bca`  
		Last Modified: Mon, 09 Aug 2021 19:27:56 GMT  
		Size: 5.6 KB (5613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6.4-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:d6a5e003eae42397f7ee4589e9f21e231d3721ac131970d2286bd616e7f55bb4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124308266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63449ffc5ac65f64a30f340aa4db0c8d502f74c51962eb9b969f08999b20604e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:44 GMT
ADD file:cec21619ecbd37b4cf8da15153b8957a343cd25c6f714e3ac3969b6003704a58 in / 
# Tue, 31 Aug 2021 01:40:45 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:04:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 31 Aug 2021 03:04:38 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:04:38 GMT
ENV GOSU_VERSION=1.13
# Tue, 31 Aug 2021 03:04:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 31 Aug 2021 03:04:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 31 Aug 2021 03:04:57 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:04:57 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 31 Aug 2021 03:05:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 31 Aug 2021 03:05:05 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 31 Aug 2021 03:05:05 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 31 Aug 2021 03:05:05 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Tue, 31 Aug 2021 03:05:05 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Tue, 31 Aug 2021 03:05:05 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Tue, 31 Aug 2021 03:05:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 31 Aug 2021 03:05:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 31 Aug 2021 03:05:28 GMT
VOLUME [/var/lib/mysql]
# Tue, 31 Aug 2021 03:05:29 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Tue, 31 Aug 2021 03:05:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Aug 2021 03:05:29 GMT
EXPOSE 3306
# Tue, 31 Aug 2021 03:05:29 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ab2d02b1ec420fdb84c9f52abda403b6aef20f5de904a2ecda5ae4f5cd6e4d46`  
		Last Modified: Tue, 31 Aug 2021 01:42:34 GMT  
		Size: 27.2 MB (27173099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d16f1b8a1bc9060d0c98a0e09c73ceab3d694a99f57672d6e44f2f5dcf09eae`  
		Last Modified: Tue, 31 Aug 2021 03:09:41 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16d8285f3be08ea7340eaf6dced5161164096c3fb3345fe8c5d6d64496bc143`  
		Last Modified: Tue, 31 Aug 2021 03:09:40 GMT  
		Size: 5.5 MB (5455084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ffd6c9eed67b115939ab5f6d4bb8ffd2f0f152fe9a61024122b558e83ce912e`  
		Last Modified: Tue, 31 Aug 2021 03:09:39 GMT  
		Size: 3.4 MB (3368457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdbc2935c20fd14d96044dcdb65fb79a0f676bcdf334058da282716411d3ff9b`  
		Last Modified: Tue, 31 Aug 2021 03:09:39 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b302bb5f11cae70b4c8ec1079e6de6c62dacfdce3e8f3ccdfabd6ce44b63d2`  
		Last Modified: Tue, 31 Aug 2021 03:09:37 GMT  
		Size: 2.2 MB (2203569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21de8a622698dffd65e882759b0b6e4fe0e56b60d892f2e4446f94439a1270f`  
		Last Modified: Tue, 31 Aug 2021 03:09:36 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9389e144f5d4ea04b6dc1760537798680338137683d9e509ac7072a5c7282d9`  
		Last Modified: Tue, 31 Aug 2021 03:09:36 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed66c3adfe54028b15ff801e6142c6ae4f65eb2bfd313aed2281deb53c447a1a`  
		Last Modified: Tue, 31 Aug 2021 03:09:51 GMT  
		Size: 86.1 MB (86097727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440559db5c8c5208fa4fd147135bce07d75b0f4a04cc838207b125cb6e4cfcbe`  
		Last Modified: Tue, 31 Aug 2021 03:09:38 GMT  
		Size: 5.6 KB (5609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6.4-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:0cf82c9d58ae3326749b0fe0ed1f094d02516dba9c3e6fdf9d2c193f2fa48b4a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137540073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20c817c255cdeba976f7d5a97418f28626785a200c99e223a6450298661f4b64`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 26 Jul 2021 23:12:46 GMT
ADD file:68eb628c2202763afa91d554dde9668d8a468fe53fdbd2fe98627a5f91d224b4 in / 
# Mon, 26 Jul 2021 23:12:49 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 02:05:55 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 27 Jul 2021 02:06:47 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:06:50 GMT
ENV GOSU_VERSION=1.13
# Tue, 27 Jul 2021 02:07:32 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 27 Jul 2021 02:07:42 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 27 Jul 2021 02:08:11 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:08:14 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 27 Jul 2021 02:08:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 27 Jul 2021 02:08:24 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 27 Jul 2021 02:08:25 GMT
ENV MARIADB_MAJOR=10.6
# Mon, 09 Aug 2021 19:17:05 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Mon, 09 Aug 2021 19:17:08 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Mon, 09 Aug 2021 19:17:10 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Mon, 09 Aug 2021 19:17:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 09 Aug 2021 19:22:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 09 Aug 2021 19:22:56 GMT
VOLUME [/var/lib/mysql]
# Mon, 09 Aug 2021 19:23:00 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Mon, 09 Aug 2021 19:23:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Aug 2021 19:23:12 GMT
EXPOSE 3306
# Mon, 09 Aug 2021 19:23:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:1a396eed835b3b7b4101a9863d174e145ddbb1de1502a63bae726b0f81e7ca93`  
		Last Modified: Mon, 26 Jul 2021 23:15:51 GMT  
		Size: 33.3 MB (33290427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65be85b12a63573ebccb059357c5c0db6046f4a074454eea617c402e3bf99c1f`  
		Last Modified: Tue, 27 Jul 2021 02:26:16 GMT  
		Size: 1.8 KB (1760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:803c8e5bf0c59b9b01b70cac07bb24bc696bc577d8e74c79ff15bcbd480874b4`  
		Last Modified: Tue, 27 Jul 2021 02:26:17 GMT  
		Size: 6.7 MB (6667884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62bd7bf9c00152c4fb338b2c1a01d5b241ceda5c58d9e700a353072ab80fb4b9`  
		Last Modified: Tue, 27 Jul 2021 02:26:17 GMT  
		Size: 3.7 MB (3670853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:372602ac4ce9a3a693cb97ec9b3e71b449fdafbaded2ce2937fec39cec9c9b6e`  
		Last Modified: Tue, 27 Jul 2021 02:26:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a80c4de70a1ded78cf0175b1f5fda38b3119857dd2d8d9f1fafcdc39eafef0e`  
		Last Modified: Tue, 27 Jul 2021 02:26:13 GMT  
		Size: 2.6 MB (2569871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc8dec87672a96e86220faa6c3e98577b2a9090fc81d81efb4681fe59e732b7`  
		Last Modified: Tue, 27 Jul 2021 02:26:12 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce893fcc2e86ea1fb70c9730683306fb99ed9b96529607badefbeb824f32081`  
		Last Modified: Mon, 09 Aug 2021 19:45:06 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea2b83ad4dfbaa9a9aa432f398880354589538421ef773a7bdc59bf41856282`  
		Last Modified: Mon, 09 Aug 2021 19:45:24 GMT  
		Size: 91.3 MB (91330692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e301a165b39ae64033fe826324cbfdf9f8e0e01fd8d20d7e69f7a8b771aa41`  
		Last Modified: Mon, 09 Aug 2021 19:45:06 GMT  
		Size: 5.6 KB (5617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6.4-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:f338e06fc65ca71eda1ac48527970da30cd5b3f1316fbb5974cd2ea2ffa87152
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.0 MB (126020736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12c9756f3b2fe668579749a2963c372a54db873f6e054bbf6f6ca8702b5d6d1f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:23 GMT
ADD file:979855f79ebaca36cc7878f71b2326f1cd189970fdb223b37cd64ee12d1c9a2b in / 
# Tue, 31 Aug 2021 01:42:27 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:49:44 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 31 Aug 2021 02:49:51 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:49:51 GMT
ENV GOSU_VERSION=1.13
# Tue, 31 Aug 2021 02:50:04 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 31 Aug 2021 02:50:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 31 Aug 2021 02:50:12 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:50:12 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 31 Aug 2021 02:50:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 31 Aug 2021 02:50:18 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 31 Aug 2021 02:50:18 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 31 Aug 2021 02:50:19 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Tue, 31 Aug 2021 02:50:19 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Tue, 31 Aug 2021 02:50:19 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Tue, 31 Aug 2021 02:50:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 31 Aug 2021 02:50:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 31 Aug 2021 02:50:49 GMT
VOLUME [/var/lib/mysql]
# Tue, 31 Aug 2021 02:50:49 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Tue, 31 Aug 2021 02:50:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Aug 2021 02:50:49 GMT
EXPOSE 3306
# Tue, 31 Aug 2021 02:50:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:9fbf86d355c92d30b8de4c0360b0d79e1100e392d0885b6b5b302a1c3781dbf1`  
		Last Modified: Tue, 31 Aug 2021 01:44:13 GMT  
		Size: 27.1 MB (27127470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5652d937cd93c6c333210a7c5783a5defbac72c096a74537a0e99da179e69e15`  
		Last Modified: Tue, 31 Aug 2021 02:52:15 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1b48caf1d89a34f08f8ee38f48260ccfd25cfdc0e5425a1f7e2e1c3bc1c8cf0`  
		Last Modified: Tue, 31 Aug 2021 02:52:16 GMT  
		Size: 5.4 MB (5380989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352b2892aadbd934d1a0415ca24f71baf53ef4b324fe9f8772a37405d8607dba`  
		Last Modified: Tue, 31 Aug 2021 02:52:16 GMT  
		Size: 3.2 MB (3241880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354edb6860dbb419b59714606f392488735bc5e9adc7496059e98f51de24d84a`  
		Last Modified: Tue, 31 Aug 2021 02:52:15 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9934bdf22d9a668fcaab9695424d4074294aef89d849a8c8ba80b0bb31ab2ab9`  
		Last Modified: Tue, 31 Aug 2021 02:52:13 GMT  
		Size: 2.2 MB (2186296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a940a6a2154f17326f40b9d4619aa517978b7eed0f68a8a68738928defef66`  
		Last Modified: Tue, 31 Aug 2021 02:52:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6840dfebdaf0d0162e783790b87c1c9eff72aca9dc017163baa2059ac974ec21`  
		Last Modified: Tue, 31 Aug 2021 02:52:13 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:badfbe5adb85e7a406e6d7af361229a125b295cec1d104f15f0334488fb8e38d`  
		Last Modified: Tue, 31 Aug 2021 02:52:26 GMT  
		Size: 88.1 MB (88073778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa96305d4f85828482207efa32cb56c1fcbf6bf32d41e5f7ca27f479f57acec9`  
		Last Modified: Tue, 31 Aug 2021 02:52:13 GMT  
		Size: 5.6 KB (5608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:focal`

```console
$ docker pull mariadb@sha256:b95f3b88e2880bf1191712c122a4c5998b380c4f1afb87ab9fc1415c0ea0b9ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:focal` - linux; amd64

```console
$ docker pull mariadb@sha256:2e955f90e3af94a992b3e63d34c93e875706d0ec672b18202630ded0706dde71
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.0 MB (127012840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45eaeedf03deed202dade660cbfe44ae17cac512cfd23ca2becab1cd20b5a6f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:05:00 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 27 Jul 2021 00:05:14 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:05:15 GMT
ENV GOSU_VERSION=1.13
# Tue, 27 Jul 2021 00:05:26 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 27 Jul 2021 00:05:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 27 Jul 2021 00:05:34 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:05:35 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 27 Jul 2021 00:05:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 27 Jul 2021 00:05:37 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 27 Jul 2021 00:05:37 GMT
ENV MARIADB_MAJOR=10.6
# Mon, 09 Aug 2021 19:24:13 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Mon, 09 Aug 2021 19:24:14 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Mon, 09 Aug 2021 19:24:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Mon, 09 Aug 2021 19:24:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 09 Aug 2021 19:24:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 09 Aug 2021 19:24:55 GMT
VOLUME [/var/lib/mysql]
# Mon, 09 Aug 2021 19:24:55 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Mon, 09 Aug 2021 19:24:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Aug 2021 19:24:55 GMT
EXPOSE 3306
# Mon, 09 Aug 2021 19:24:56 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf20e69555c2118df81cd7906473b0bbef5210f014d45113251b1298fb1c996`  
		Last Modified: Tue, 27 Jul 2021 00:10:02 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69afd1ffc85b8fe385e48d00e89467a4e080c81b2447ce86ebf964f3e43efb9`  
		Last Modified: Tue, 27 Jul 2021 00:10:04 GMT  
		Size: 5.5 MB (5488764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e720dc7fcd8609016e69543f354117290ffee7c9ea1bdd97d7ca84bcc06d616`  
		Last Modified: Tue, 27 Jul 2021 00:10:03 GMT  
		Size: 3.6 MB (3582379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a81d177e410065c8eec2b5c018ab6ac60b2a5161184890bc3bf7627e78fb2dd`  
		Last Modified: Tue, 27 Jul 2021 00:10:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827c8c103c898d23db5f0cfc69b6faa45038d27b1ec3c15cb5d5b29ee60fca0b`  
		Last Modified: Tue, 27 Jul 2021 00:09:59 GMT  
		Size: 2.3 MB (2274133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2108ccd013748c7fce6a19a3f7434b860401f78326ac7373c486eafa3c719354`  
		Last Modified: Tue, 27 Jul 2021 00:09:59 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05414cb5e8f4dcf16b70640f3bcf904bafddd184d3971881c10b194fb74e8a0`  
		Last Modified: Mon, 09 Aug 2021 19:27:56 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6981930106c6d6380293a728b1bda2840d2392194e1b19649b7a863e1174054`  
		Last Modified: Mon, 09 Aug 2021 19:28:09 GMT  
		Size: 87.1 MB (87089293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009b7e8d11861e3f00504f9b3ff616177ec6f4e7f14f2e0162b0f92811c73bca`  
		Last Modified: Mon, 09 Aug 2021 19:27:56 GMT  
		Size: 5.6 KB (5613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:d6a5e003eae42397f7ee4589e9f21e231d3721ac131970d2286bd616e7f55bb4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124308266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63449ffc5ac65f64a30f340aa4db0c8d502f74c51962eb9b969f08999b20604e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:44 GMT
ADD file:cec21619ecbd37b4cf8da15153b8957a343cd25c6f714e3ac3969b6003704a58 in / 
# Tue, 31 Aug 2021 01:40:45 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:04:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 31 Aug 2021 03:04:38 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:04:38 GMT
ENV GOSU_VERSION=1.13
# Tue, 31 Aug 2021 03:04:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 31 Aug 2021 03:04:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 31 Aug 2021 03:04:57 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:04:57 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 31 Aug 2021 03:05:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 31 Aug 2021 03:05:05 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 31 Aug 2021 03:05:05 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 31 Aug 2021 03:05:05 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Tue, 31 Aug 2021 03:05:05 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Tue, 31 Aug 2021 03:05:05 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Tue, 31 Aug 2021 03:05:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 31 Aug 2021 03:05:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 31 Aug 2021 03:05:28 GMT
VOLUME [/var/lib/mysql]
# Tue, 31 Aug 2021 03:05:29 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Tue, 31 Aug 2021 03:05:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Aug 2021 03:05:29 GMT
EXPOSE 3306
# Tue, 31 Aug 2021 03:05:29 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ab2d02b1ec420fdb84c9f52abda403b6aef20f5de904a2ecda5ae4f5cd6e4d46`  
		Last Modified: Tue, 31 Aug 2021 01:42:34 GMT  
		Size: 27.2 MB (27173099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d16f1b8a1bc9060d0c98a0e09c73ceab3d694a99f57672d6e44f2f5dcf09eae`  
		Last Modified: Tue, 31 Aug 2021 03:09:41 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16d8285f3be08ea7340eaf6dced5161164096c3fb3345fe8c5d6d64496bc143`  
		Last Modified: Tue, 31 Aug 2021 03:09:40 GMT  
		Size: 5.5 MB (5455084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ffd6c9eed67b115939ab5f6d4bb8ffd2f0f152fe9a61024122b558e83ce912e`  
		Last Modified: Tue, 31 Aug 2021 03:09:39 GMT  
		Size: 3.4 MB (3368457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdbc2935c20fd14d96044dcdb65fb79a0f676bcdf334058da282716411d3ff9b`  
		Last Modified: Tue, 31 Aug 2021 03:09:39 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b302bb5f11cae70b4c8ec1079e6de6c62dacfdce3e8f3ccdfabd6ce44b63d2`  
		Last Modified: Tue, 31 Aug 2021 03:09:37 GMT  
		Size: 2.2 MB (2203569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21de8a622698dffd65e882759b0b6e4fe0e56b60d892f2e4446f94439a1270f`  
		Last Modified: Tue, 31 Aug 2021 03:09:36 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9389e144f5d4ea04b6dc1760537798680338137683d9e509ac7072a5c7282d9`  
		Last Modified: Tue, 31 Aug 2021 03:09:36 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed66c3adfe54028b15ff801e6142c6ae4f65eb2bfd313aed2281deb53c447a1a`  
		Last Modified: Tue, 31 Aug 2021 03:09:51 GMT  
		Size: 86.1 MB (86097727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440559db5c8c5208fa4fd147135bce07d75b0f4a04cc838207b125cb6e4cfcbe`  
		Last Modified: Tue, 31 Aug 2021 03:09:38 GMT  
		Size: 5.6 KB (5609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:0cf82c9d58ae3326749b0fe0ed1f094d02516dba9c3e6fdf9d2c193f2fa48b4a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137540073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20c817c255cdeba976f7d5a97418f28626785a200c99e223a6450298661f4b64`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 26 Jul 2021 23:12:46 GMT
ADD file:68eb628c2202763afa91d554dde9668d8a468fe53fdbd2fe98627a5f91d224b4 in / 
# Mon, 26 Jul 2021 23:12:49 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 02:05:55 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 27 Jul 2021 02:06:47 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:06:50 GMT
ENV GOSU_VERSION=1.13
# Tue, 27 Jul 2021 02:07:32 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 27 Jul 2021 02:07:42 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 27 Jul 2021 02:08:11 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:08:14 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 27 Jul 2021 02:08:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 27 Jul 2021 02:08:24 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 27 Jul 2021 02:08:25 GMT
ENV MARIADB_MAJOR=10.6
# Mon, 09 Aug 2021 19:17:05 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Mon, 09 Aug 2021 19:17:08 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Mon, 09 Aug 2021 19:17:10 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Mon, 09 Aug 2021 19:17:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 09 Aug 2021 19:22:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 09 Aug 2021 19:22:56 GMT
VOLUME [/var/lib/mysql]
# Mon, 09 Aug 2021 19:23:00 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Mon, 09 Aug 2021 19:23:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Aug 2021 19:23:12 GMT
EXPOSE 3306
# Mon, 09 Aug 2021 19:23:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:1a396eed835b3b7b4101a9863d174e145ddbb1de1502a63bae726b0f81e7ca93`  
		Last Modified: Mon, 26 Jul 2021 23:15:51 GMT  
		Size: 33.3 MB (33290427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65be85b12a63573ebccb059357c5c0db6046f4a074454eea617c402e3bf99c1f`  
		Last Modified: Tue, 27 Jul 2021 02:26:16 GMT  
		Size: 1.8 KB (1760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:803c8e5bf0c59b9b01b70cac07bb24bc696bc577d8e74c79ff15bcbd480874b4`  
		Last Modified: Tue, 27 Jul 2021 02:26:17 GMT  
		Size: 6.7 MB (6667884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62bd7bf9c00152c4fb338b2c1a01d5b241ceda5c58d9e700a353072ab80fb4b9`  
		Last Modified: Tue, 27 Jul 2021 02:26:17 GMT  
		Size: 3.7 MB (3670853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:372602ac4ce9a3a693cb97ec9b3e71b449fdafbaded2ce2937fec39cec9c9b6e`  
		Last Modified: Tue, 27 Jul 2021 02:26:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a80c4de70a1ded78cf0175b1f5fda38b3119857dd2d8d9f1fafcdc39eafef0e`  
		Last Modified: Tue, 27 Jul 2021 02:26:13 GMT  
		Size: 2.6 MB (2569871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc8dec87672a96e86220faa6c3e98577b2a9090fc81d81efb4681fe59e732b7`  
		Last Modified: Tue, 27 Jul 2021 02:26:12 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce893fcc2e86ea1fb70c9730683306fb99ed9b96529607badefbeb824f32081`  
		Last Modified: Mon, 09 Aug 2021 19:45:06 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea2b83ad4dfbaa9a9aa432f398880354589538421ef773a7bdc59bf41856282`  
		Last Modified: Mon, 09 Aug 2021 19:45:24 GMT  
		Size: 91.3 MB (91330692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e301a165b39ae64033fe826324cbfdf9f8e0e01fd8d20d7e69f7a8b771aa41`  
		Last Modified: Mon, 09 Aug 2021 19:45:06 GMT  
		Size: 5.6 KB (5617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:focal` - linux; s390x

```console
$ docker pull mariadb@sha256:f338e06fc65ca71eda1ac48527970da30cd5b3f1316fbb5974cd2ea2ffa87152
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.0 MB (126020736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12c9756f3b2fe668579749a2963c372a54db873f6e054bbf6f6ca8702b5d6d1f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:23 GMT
ADD file:979855f79ebaca36cc7878f71b2326f1cd189970fdb223b37cd64ee12d1c9a2b in / 
# Tue, 31 Aug 2021 01:42:27 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:49:44 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 31 Aug 2021 02:49:51 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:49:51 GMT
ENV GOSU_VERSION=1.13
# Tue, 31 Aug 2021 02:50:04 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 31 Aug 2021 02:50:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 31 Aug 2021 02:50:12 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:50:12 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 31 Aug 2021 02:50:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 31 Aug 2021 02:50:18 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 31 Aug 2021 02:50:18 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 31 Aug 2021 02:50:19 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Tue, 31 Aug 2021 02:50:19 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Tue, 31 Aug 2021 02:50:19 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Tue, 31 Aug 2021 02:50:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 31 Aug 2021 02:50:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 31 Aug 2021 02:50:49 GMT
VOLUME [/var/lib/mysql]
# Tue, 31 Aug 2021 02:50:49 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Tue, 31 Aug 2021 02:50:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Aug 2021 02:50:49 GMT
EXPOSE 3306
# Tue, 31 Aug 2021 02:50:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:9fbf86d355c92d30b8de4c0360b0d79e1100e392d0885b6b5b302a1c3781dbf1`  
		Last Modified: Tue, 31 Aug 2021 01:44:13 GMT  
		Size: 27.1 MB (27127470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5652d937cd93c6c333210a7c5783a5defbac72c096a74537a0e99da179e69e15`  
		Last Modified: Tue, 31 Aug 2021 02:52:15 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1b48caf1d89a34f08f8ee38f48260ccfd25cfdc0e5425a1f7e2e1c3bc1c8cf0`  
		Last Modified: Tue, 31 Aug 2021 02:52:16 GMT  
		Size: 5.4 MB (5380989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352b2892aadbd934d1a0415ca24f71baf53ef4b324fe9f8772a37405d8607dba`  
		Last Modified: Tue, 31 Aug 2021 02:52:16 GMT  
		Size: 3.2 MB (3241880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354edb6860dbb419b59714606f392488735bc5e9adc7496059e98f51de24d84a`  
		Last Modified: Tue, 31 Aug 2021 02:52:15 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9934bdf22d9a668fcaab9695424d4074294aef89d849a8c8ba80b0bb31ab2ab9`  
		Last Modified: Tue, 31 Aug 2021 02:52:13 GMT  
		Size: 2.2 MB (2186296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a940a6a2154f17326f40b9d4619aa517978b7eed0f68a8a68738928defef66`  
		Last Modified: Tue, 31 Aug 2021 02:52:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6840dfebdaf0d0162e783790b87c1c9eff72aca9dc017163baa2059ac974ec21`  
		Last Modified: Tue, 31 Aug 2021 02:52:13 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:badfbe5adb85e7a406e6d7af361229a125b295cec1d104f15f0334488fb8e38d`  
		Last Modified: Tue, 31 Aug 2021 02:52:26 GMT  
		Size: 88.1 MB (88073778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa96305d4f85828482207efa32cb56c1fcbf6bf32d41e5f7ca27f479f57acec9`  
		Last Modified: Tue, 31 Aug 2021 02:52:13 GMT  
		Size: 5.6 KB (5608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:latest`

```console
$ docker pull mariadb@sha256:b95f3b88e2880bf1191712c122a4c5998b380c4f1afb87ab9fc1415c0ea0b9ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:latest` - linux; amd64

```console
$ docker pull mariadb@sha256:2e955f90e3af94a992b3e63d34c93e875706d0ec672b18202630ded0706dde71
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.0 MB (127012840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45eaeedf03deed202dade660cbfe44ae17cac512cfd23ca2becab1cd20b5a6f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:05:00 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 27 Jul 2021 00:05:14 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:05:15 GMT
ENV GOSU_VERSION=1.13
# Tue, 27 Jul 2021 00:05:26 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 27 Jul 2021 00:05:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 27 Jul 2021 00:05:34 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:05:35 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 27 Jul 2021 00:05:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 27 Jul 2021 00:05:37 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 27 Jul 2021 00:05:37 GMT
ENV MARIADB_MAJOR=10.6
# Mon, 09 Aug 2021 19:24:13 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Mon, 09 Aug 2021 19:24:14 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Mon, 09 Aug 2021 19:24:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Mon, 09 Aug 2021 19:24:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 09 Aug 2021 19:24:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 09 Aug 2021 19:24:55 GMT
VOLUME [/var/lib/mysql]
# Mon, 09 Aug 2021 19:24:55 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Mon, 09 Aug 2021 19:24:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Aug 2021 19:24:55 GMT
EXPOSE 3306
# Mon, 09 Aug 2021 19:24:56 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf20e69555c2118df81cd7906473b0bbef5210f014d45113251b1298fb1c996`  
		Last Modified: Tue, 27 Jul 2021 00:10:02 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69afd1ffc85b8fe385e48d00e89467a4e080c81b2447ce86ebf964f3e43efb9`  
		Last Modified: Tue, 27 Jul 2021 00:10:04 GMT  
		Size: 5.5 MB (5488764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e720dc7fcd8609016e69543f354117290ffee7c9ea1bdd97d7ca84bcc06d616`  
		Last Modified: Tue, 27 Jul 2021 00:10:03 GMT  
		Size: 3.6 MB (3582379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a81d177e410065c8eec2b5c018ab6ac60b2a5161184890bc3bf7627e78fb2dd`  
		Last Modified: Tue, 27 Jul 2021 00:10:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827c8c103c898d23db5f0cfc69b6faa45038d27b1ec3c15cb5d5b29ee60fca0b`  
		Last Modified: Tue, 27 Jul 2021 00:09:59 GMT  
		Size: 2.3 MB (2274133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2108ccd013748c7fce6a19a3f7434b860401f78326ac7373c486eafa3c719354`  
		Last Modified: Tue, 27 Jul 2021 00:09:59 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05414cb5e8f4dcf16b70640f3bcf904bafddd184d3971881c10b194fb74e8a0`  
		Last Modified: Mon, 09 Aug 2021 19:27:56 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6981930106c6d6380293a728b1bda2840d2392194e1b19649b7a863e1174054`  
		Last Modified: Mon, 09 Aug 2021 19:28:09 GMT  
		Size: 87.1 MB (87089293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009b7e8d11861e3f00504f9b3ff616177ec6f4e7f14f2e0162b0f92811c73bca`  
		Last Modified: Mon, 09 Aug 2021 19:27:56 GMT  
		Size: 5.6 KB (5613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:d6a5e003eae42397f7ee4589e9f21e231d3721ac131970d2286bd616e7f55bb4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124308266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63449ffc5ac65f64a30f340aa4db0c8d502f74c51962eb9b969f08999b20604e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:44 GMT
ADD file:cec21619ecbd37b4cf8da15153b8957a343cd25c6f714e3ac3969b6003704a58 in / 
# Tue, 31 Aug 2021 01:40:45 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:04:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 31 Aug 2021 03:04:38 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:04:38 GMT
ENV GOSU_VERSION=1.13
# Tue, 31 Aug 2021 03:04:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 31 Aug 2021 03:04:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 31 Aug 2021 03:04:57 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:04:57 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 31 Aug 2021 03:05:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 31 Aug 2021 03:05:05 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 31 Aug 2021 03:05:05 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 31 Aug 2021 03:05:05 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Tue, 31 Aug 2021 03:05:05 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Tue, 31 Aug 2021 03:05:05 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Tue, 31 Aug 2021 03:05:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 31 Aug 2021 03:05:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 31 Aug 2021 03:05:28 GMT
VOLUME [/var/lib/mysql]
# Tue, 31 Aug 2021 03:05:29 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Tue, 31 Aug 2021 03:05:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Aug 2021 03:05:29 GMT
EXPOSE 3306
# Tue, 31 Aug 2021 03:05:29 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ab2d02b1ec420fdb84c9f52abda403b6aef20f5de904a2ecda5ae4f5cd6e4d46`  
		Last Modified: Tue, 31 Aug 2021 01:42:34 GMT  
		Size: 27.2 MB (27173099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d16f1b8a1bc9060d0c98a0e09c73ceab3d694a99f57672d6e44f2f5dcf09eae`  
		Last Modified: Tue, 31 Aug 2021 03:09:41 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16d8285f3be08ea7340eaf6dced5161164096c3fb3345fe8c5d6d64496bc143`  
		Last Modified: Tue, 31 Aug 2021 03:09:40 GMT  
		Size: 5.5 MB (5455084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ffd6c9eed67b115939ab5f6d4bb8ffd2f0f152fe9a61024122b558e83ce912e`  
		Last Modified: Tue, 31 Aug 2021 03:09:39 GMT  
		Size: 3.4 MB (3368457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdbc2935c20fd14d96044dcdb65fb79a0f676bcdf334058da282716411d3ff9b`  
		Last Modified: Tue, 31 Aug 2021 03:09:39 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b302bb5f11cae70b4c8ec1079e6de6c62dacfdce3e8f3ccdfabd6ce44b63d2`  
		Last Modified: Tue, 31 Aug 2021 03:09:37 GMT  
		Size: 2.2 MB (2203569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21de8a622698dffd65e882759b0b6e4fe0e56b60d892f2e4446f94439a1270f`  
		Last Modified: Tue, 31 Aug 2021 03:09:36 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9389e144f5d4ea04b6dc1760537798680338137683d9e509ac7072a5c7282d9`  
		Last Modified: Tue, 31 Aug 2021 03:09:36 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed66c3adfe54028b15ff801e6142c6ae4f65eb2bfd313aed2281deb53c447a1a`  
		Last Modified: Tue, 31 Aug 2021 03:09:51 GMT  
		Size: 86.1 MB (86097727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440559db5c8c5208fa4fd147135bce07d75b0f4a04cc838207b125cb6e4cfcbe`  
		Last Modified: Tue, 31 Aug 2021 03:09:38 GMT  
		Size: 5.6 KB (5609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; ppc64le

```console
$ docker pull mariadb@sha256:0cf82c9d58ae3326749b0fe0ed1f094d02516dba9c3e6fdf9d2c193f2fa48b4a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137540073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20c817c255cdeba976f7d5a97418f28626785a200c99e223a6450298661f4b64`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 26 Jul 2021 23:12:46 GMT
ADD file:68eb628c2202763afa91d554dde9668d8a468fe53fdbd2fe98627a5f91d224b4 in / 
# Mon, 26 Jul 2021 23:12:49 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 02:05:55 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 27 Jul 2021 02:06:47 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:06:50 GMT
ENV GOSU_VERSION=1.13
# Tue, 27 Jul 2021 02:07:32 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 27 Jul 2021 02:07:42 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 27 Jul 2021 02:08:11 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:08:14 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 27 Jul 2021 02:08:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 27 Jul 2021 02:08:24 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 27 Jul 2021 02:08:25 GMT
ENV MARIADB_MAJOR=10.6
# Mon, 09 Aug 2021 19:17:05 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Mon, 09 Aug 2021 19:17:08 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Mon, 09 Aug 2021 19:17:10 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Mon, 09 Aug 2021 19:17:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 09 Aug 2021 19:22:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 09 Aug 2021 19:22:56 GMT
VOLUME [/var/lib/mysql]
# Mon, 09 Aug 2021 19:23:00 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Mon, 09 Aug 2021 19:23:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Aug 2021 19:23:12 GMT
EXPOSE 3306
# Mon, 09 Aug 2021 19:23:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:1a396eed835b3b7b4101a9863d174e145ddbb1de1502a63bae726b0f81e7ca93`  
		Last Modified: Mon, 26 Jul 2021 23:15:51 GMT  
		Size: 33.3 MB (33290427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65be85b12a63573ebccb059357c5c0db6046f4a074454eea617c402e3bf99c1f`  
		Last Modified: Tue, 27 Jul 2021 02:26:16 GMT  
		Size: 1.8 KB (1760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:803c8e5bf0c59b9b01b70cac07bb24bc696bc577d8e74c79ff15bcbd480874b4`  
		Last Modified: Tue, 27 Jul 2021 02:26:17 GMT  
		Size: 6.7 MB (6667884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62bd7bf9c00152c4fb338b2c1a01d5b241ceda5c58d9e700a353072ab80fb4b9`  
		Last Modified: Tue, 27 Jul 2021 02:26:17 GMT  
		Size: 3.7 MB (3670853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:372602ac4ce9a3a693cb97ec9b3e71b449fdafbaded2ce2937fec39cec9c9b6e`  
		Last Modified: Tue, 27 Jul 2021 02:26:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a80c4de70a1ded78cf0175b1f5fda38b3119857dd2d8d9f1fafcdc39eafef0e`  
		Last Modified: Tue, 27 Jul 2021 02:26:13 GMT  
		Size: 2.6 MB (2569871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc8dec87672a96e86220faa6c3e98577b2a9090fc81d81efb4681fe59e732b7`  
		Last Modified: Tue, 27 Jul 2021 02:26:12 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce893fcc2e86ea1fb70c9730683306fb99ed9b96529607badefbeb824f32081`  
		Last Modified: Mon, 09 Aug 2021 19:45:06 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea2b83ad4dfbaa9a9aa432f398880354589538421ef773a7bdc59bf41856282`  
		Last Modified: Mon, 09 Aug 2021 19:45:24 GMT  
		Size: 91.3 MB (91330692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e301a165b39ae64033fe826324cbfdf9f8e0e01fd8d20d7e69f7a8b771aa41`  
		Last Modified: Mon, 09 Aug 2021 19:45:06 GMT  
		Size: 5.6 KB (5617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; s390x

```console
$ docker pull mariadb@sha256:f338e06fc65ca71eda1ac48527970da30cd5b3f1316fbb5974cd2ea2ffa87152
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.0 MB (126020736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12c9756f3b2fe668579749a2963c372a54db873f6e054bbf6f6ca8702b5d6d1f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:23 GMT
ADD file:979855f79ebaca36cc7878f71b2326f1cd189970fdb223b37cd64ee12d1c9a2b in / 
# Tue, 31 Aug 2021 01:42:27 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:49:44 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 31 Aug 2021 02:49:51 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:49:51 GMT
ENV GOSU_VERSION=1.13
# Tue, 31 Aug 2021 02:50:04 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 31 Aug 2021 02:50:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 31 Aug 2021 02:50:12 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:50:12 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 31 Aug 2021 02:50:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 31 Aug 2021 02:50:18 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 31 Aug 2021 02:50:18 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 31 Aug 2021 02:50:19 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Tue, 31 Aug 2021 02:50:19 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Tue, 31 Aug 2021 02:50:19 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Tue, 31 Aug 2021 02:50:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 31 Aug 2021 02:50:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 31 Aug 2021 02:50:49 GMT
VOLUME [/var/lib/mysql]
# Tue, 31 Aug 2021 02:50:49 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Tue, 31 Aug 2021 02:50:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Aug 2021 02:50:49 GMT
EXPOSE 3306
# Tue, 31 Aug 2021 02:50:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:9fbf86d355c92d30b8de4c0360b0d79e1100e392d0885b6b5b302a1c3781dbf1`  
		Last Modified: Tue, 31 Aug 2021 01:44:13 GMT  
		Size: 27.1 MB (27127470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5652d937cd93c6c333210a7c5783a5defbac72c096a74537a0e99da179e69e15`  
		Last Modified: Tue, 31 Aug 2021 02:52:15 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1b48caf1d89a34f08f8ee38f48260ccfd25cfdc0e5425a1f7e2e1c3bc1c8cf0`  
		Last Modified: Tue, 31 Aug 2021 02:52:16 GMT  
		Size: 5.4 MB (5380989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352b2892aadbd934d1a0415ca24f71baf53ef4b324fe9f8772a37405d8607dba`  
		Last Modified: Tue, 31 Aug 2021 02:52:16 GMT  
		Size: 3.2 MB (3241880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354edb6860dbb419b59714606f392488735bc5e9adc7496059e98f51de24d84a`  
		Last Modified: Tue, 31 Aug 2021 02:52:15 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9934bdf22d9a668fcaab9695424d4074294aef89d849a8c8ba80b0bb31ab2ab9`  
		Last Modified: Tue, 31 Aug 2021 02:52:13 GMT  
		Size: 2.2 MB (2186296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a940a6a2154f17326f40b9d4619aa517978b7eed0f68a8a68738928defef66`  
		Last Modified: Tue, 31 Aug 2021 02:52:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6840dfebdaf0d0162e783790b87c1c9eff72aca9dc017163baa2059ac974ec21`  
		Last Modified: Tue, 31 Aug 2021 02:52:13 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:badfbe5adb85e7a406e6d7af361229a125b295cec1d104f15f0334488fb8e38d`  
		Last Modified: Tue, 31 Aug 2021 02:52:26 GMT  
		Size: 88.1 MB (88073778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa96305d4f85828482207efa32cb56c1fcbf6bf32d41e5f7ca27f479f57acec9`  
		Last Modified: Tue, 31 Aug 2021 02:52:13 GMT  
		Size: 5.6 KB (5608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
