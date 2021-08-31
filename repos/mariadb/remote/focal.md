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
