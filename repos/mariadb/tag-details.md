<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mariadb`

-	[`mariadb:10`](#mariadb10)
-	[`mariadb:10-focal`](#mariadb10-focal)
-	[`mariadb:10.2`](#mariadb102)
-	[`mariadb:10.2-bionic`](#mariadb102-bionic)
-	[`mariadb:10.2.41`](#mariadb10241)
-	[`mariadb:10.2.41-bionic`](#mariadb10241-bionic)
-	[`mariadb:10.3`](#mariadb103)
-	[`mariadb:10.3-focal`](#mariadb103-focal)
-	[`mariadb:10.3.32`](#mariadb10332)
-	[`mariadb:10.3.32-focal`](#mariadb10332-focal)
-	[`mariadb:10.4`](#mariadb104)
-	[`mariadb:10.4-focal`](#mariadb104-focal)
-	[`mariadb:10.4.22`](#mariadb10422)
-	[`mariadb:10.4.22-focal`](#mariadb10422-focal)
-	[`mariadb:10.5`](#mariadb105)
-	[`mariadb:10.5-focal`](#mariadb105-focal)
-	[`mariadb:10.5.13`](#mariadb10513)
-	[`mariadb:10.5.13-focal`](#mariadb10513-focal)
-	[`mariadb:10.6`](#mariadb106)
-	[`mariadb:10.6-focal`](#mariadb106-focal)
-	[`mariadb:10.6.5`](#mariadb1065)
-	[`mariadb:10.6.5-focal`](#mariadb1065-focal)
-	[`mariadb:10.7`](#mariadb107)
-	[`mariadb:10.7-focal`](#mariadb107-focal)
-	[`mariadb:10.7.1`](#mariadb1071)
-	[`mariadb:10.7.1-focal`](#mariadb1071-focal)
-	[`mariadb:focal`](#mariadbfocal)
-	[`mariadb:latest`](#mariadblatest)

## `mariadb:10`

```console
$ docker pull mariadb@sha256:c014ba1efc5dbd711d0520c7762d57807f35549de3414eb31e942a420c8a2ed2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10` - linux; amd64

```console
$ docker pull mariadb@sha256:dd08274a61f912b78facb7d144f898c0fd53da4f0c2fcf8ea80cd05f22577221
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.0 MB (127016059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12e05d5da3c5223e9877e8eb90d68560ff66cedcb955131061d60d093a908f0c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:07:51 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 16 Oct 2021 03:07:59 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:07:59 GMT
ENV GOSU_VERSION=1.13
# Sat, 16 Oct 2021 03:08:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 16 Oct 2021 03:08:11 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 16 Oct 2021 03:08:19 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:08:19 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 16 Oct 2021 03:08:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 16 Oct 2021 03:08:27 GMT
ARG MARIADB_MAJOR=10.6
# Sat, 16 Oct 2021 03:08:27 GMT
ENV MARIADB_MAJOR=10.6
# Sat, 16 Oct 2021 03:08:27 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Sat, 16 Oct 2021 03:08:27 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Sat, 16 Oct 2021 03:08:27 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Sat, 16 Oct 2021 03:08:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 16 Oct 2021 03:09:01 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 16 Oct 2021 03:09:02 GMT
VOLUME [/var/lib/mysql]
# Sat, 16 Oct 2021 03:09:02 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Sat, 16 Oct 2021 03:09:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 03:09:02 GMT
EXPOSE 3306
# Sat, 16 Oct 2021 03:09:02 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:034655750c88e076cbd516354371b6176d01179bf595d928444e663ba1fa6845`  
		Last Modified: Sat, 16 Oct 2021 03:11:19 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b757a2a0f02848b1254cbd8b54e1d3cd4651228ede9a8c75e127f91cb415c4`  
		Last Modified: Sat, 16 Oct 2021 03:11:20 GMT  
		Size: 5.5 MB (5489306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c37daf8b6b55859dc1f92dbe017858ae03bd5bf503a3cdbf317b0b4387b1383`  
		Last Modified: Sat, 16 Oct 2021 03:11:19 GMT  
		Size: 3.6 MB (3582632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4cd9409b0f69a0ebe270f43c3a217f05b4c326e5d7c9a4ffb0cb7852ecddc81`  
		Last Modified: Sat, 16 Oct 2021 03:11:18 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbcda06785eb5474250fd32695909199c0de3375a06cf66401d277da518f3da9`  
		Last Modified: Sat, 16 Oct 2021 03:11:17 GMT  
		Size: 2.3 MB (2276882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34cd90f184c404cd4ecd88ebe612e6f180f76836efd3c24a329a3b812c5c345`  
		Last Modified: Sat, 16 Oct 2021 03:11:16 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd6cef4ce4896ed34f82cdec0226170c9ec12e780095f39a268e4f4cd87be523`  
		Last Modified: Sat, 16 Oct 2021 03:11:16 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cb89a1550ea4efead895dec48626ae277912ca9eeffae1a3c1b8c3f0f9ed02d`  
		Last Modified: Sat, 16 Oct 2021 03:11:29 GMT  
		Size: 87.1 MB (87089805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df9f153bd93044efcf8d9cd1ea5266b32bf28df2ad72e5ce195428e8c81b917b`  
		Last Modified: Sat, 16 Oct 2021 03:11:16 GMT  
		Size: 5.6 KB (5611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:52b21e64bd048fb93b8a3ac5d36eaf3027bd5a7b1c71e833bc8ac0aa1c98c72b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.2 MB (124173665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6819e5d163d1d24d896d090e1f55c38bcb9e55db811196e3919f0707a86eff03`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:45:05 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 16 Oct 2021 03:45:15 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:45:15 GMT
ENV GOSU_VERSION=1.13
# Sat, 16 Oct 2021 03:45:29 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 16 Oct 2021 03:45:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 16 Oct 2021 03:45:37 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:45:37 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 16 Oct 2021 03:45:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 16 Oct 2021 03:45:42 GMT
ARG MARIADB_MAJOR=10.6
# Sat, 16 Oct 2021 03:45:43 GMT
ENV MARIADB_MAJOR=10.6
# Sat, 16 Oct 2021 03:45:44 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Sat, 16 Oct 2021 03:45:45 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Sat, 16 Oct 2021 03:45:46 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Sat, 16 Oct 2021 03:45:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 16 Oct 2021 03:46:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 16 Oct 2021 03:46:17 GMT
VOLUME [/var/lib/mysql]
# Sat, 16 Oct 2021 03:46:19 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Sat, 16 Oct 2021 03:46:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 03:46:20 GMT
EXPOSE 3306
# Sat, 16 Oct 2021 03:46:21 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c05479159a3de34e1aedf676cd1a6793673b2e223d06a85c1caeab97e08c15`  
		Last Modified: Sat, 16 Oct 2021 03:51:12 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3fae4be7ce6b0048b0994bc5bd1e2d202fb383de08c3f2b82896678b35e8d1`  
		Last Modified: Sat, 16 Oct 2021 03:51:12 GMT  
		Size: 5.3 MB (5320781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8ca9913d50b67d55691860d8b19e4e38456f1142af47d6ebd4e933757fb2b6`  
		Last Modified: Sat, 16 Oct 2021 03:51:12 GMT  
		Size: 3.4 MB (3368038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffbd8ed1ed1586e00f393ee1417f3bf2b1d83f13c20a5035a050af97e29b9d09`  
		Last Modified: Sat, 16 Oct 2021 03:51:11 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48e61cde050f1f52a8b54730fab5e7bc4db2d6a6303e8fa2ef4eab107076a9ba`  
		Last Modified: Sat, 16 Oct 2021 03:51:09 GMT  
		Size: 2.2 MB (2207084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0b524648b0e80b14e489493c061f52515d6e5791c7f356da3be691507607ce`  
		Last Modified: Sat, 16 Oct 2021 03:51:09 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a7bc5ea6462e7abeb995a46808ebc6c2f6d5afc6361c367235fc02909f95ff`  
		Last Modified: Sat, 16 Oct 2021 03:51:09 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70ea7fb2288eb8ce16b25989a901e5f6bc945315a86d749685f03dabde2bce5`  
		Last Modified: Sat, 16 Oct 2021 03:51:22 GMT  
		Size: 86.1 MB (86096615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:968494f5cebc0a5862440af69b49d4a863460de158a94c0f339b19d08ccf4ab6`  
		Last Modified: Sat, 16 Oct 2021 03:51:09 GMT  
		Size: 5.6 KB (5613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10` - linux; ppc64le

```console
$ docker pull mariadb@sha256:aa3c316f88dd9537eeaa7201d6d3c5f8d8732196ee6c9cd5ce553816c7a060d9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137539722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a66b6be1b40e577fe733ec92528cf73ee97a8536e1fcddc9fe638aa9132f8173`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Oct 2021 00:36:38 GMT
ADD file:9246bf887411af1b286de95d779c11581dcef3c0d5a29e434162f0c085a7ce85 in / 
# Sat, 16 Oct 2021 00:36:44 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 01:34:00 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 16 Oct 2021 01:34:51 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:34:53 GMT
ENV GOSU_VERSION=1.13
# Sat, 16 Oct 2021 01:35:28 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 16 Oct 2021 01:35:36 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 16 Oct 2021 01:36:02 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:36:03 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 16 Oct 2021 01:36:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 16 Oct 2021 01:36:18 GMT
ARG MARIADB_MAJOR=10.6
# Sat, 16 Oct 2021 01:36:19 GMT
ENV MARIADB_MAJOR=10.6
# Sat, 16 Oct 2021 01:36:22 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Sat, 16 Oct 2021 01:36:24 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Sat, 16 Oct 2021 01:36:29 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Sat, 16 Oct 2021 01:36:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 16 Oct 2021 01:38:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 16 Oct 2021 01:39:01 GMT
VOLUME [/var/lib/mysql]
# Sat, 16 Oct 2021 01:39:03 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Sat, 16 Oct 2021 01:39:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 01:39:08 GMT
EXPOSE 3306
# Sat, 16 Oct 2021 01:39:15 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:77ba7971d651af68e20e7cbb6603a3f7acd8ef2893066767a93db104723556f2`  
		Last Modified: Sat, 16 Oct 2021 00:38:38 GMT  
		Size: 33.3 MB (33287238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a9c5581eb228ed7e984fa7a4e62a7f8b2a068039fde3d32fa3b208026a189d`  
		Last Modified: Sat, 16 Oct 2021 01:49:31 GMT  
		Size: 1.8 KB (1761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63d968d5ad046645779be85243a3db326487bc8905dabf68bb063ea79e1662c1`  
		Last Modified: Sat, 16 Oct 2021 01:49:32 GMT  
		Size: 6.7 MB (6667970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5bdbddf0ed762c90ab4fcfe1f42007a96e4f90ca4f0765dfcec52213a3f5c12`  
		Last Modified: Sat, 16 Oct 2021 01:49:31 GMT  
		Size: 3.7 MB (3670760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00cc95e86fb5ab1bda9839a1ecbd3c2d607bc6cfc5155f33bf32c9d7827ec98b`  
		Last Modified: Sat, 16 Oct 2021 01:49:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe2cefdba07cb9fc803227a545d4fcc196038c1020de7698bf4e333d9056cbd`  
		Last Modified: Sat, 16 Oct 2021 01:49:28 GMT  
		Size: 2.6 MB (2573066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab77c7b0e7b171541e9f7f813ef81190ef39151aea54bfe2b64f8c191ce672c`  
		Last Modified: Sat, 16 Oct 2021 01:49:27 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d188c1c418692bd6c05728f7b542eab7acbdf502f48eaf84c762ba6b27718c`  
		Last Modified: Sat, 16 Oct 2021 01:49:27 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288c0769408956c537d6b5b649bc2b69ffe5036157a0aa58dce6c17312680a33`  
		Last Modified: Sat, 16 Oct 2021 01:49:45 GMT  
		Size: 91.3 MB (91330343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d4c9a0a37f40daaa1c904e99bb499d11db46dd87bd94236295d1ad90603ba74`  
		Last Modified: Sat, 16 Oct 2021 01:49:27 GMT  
		Size: 5.6 KB (5613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10` - linux; s390x

```console
$ docker pull mariadb@sha256:90bc202cc092060b6e454b7f2d06cbe792ffd3d7a2edefe42e30964c55d24dab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.0 MB (126014128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09b71468a7107bd097e1852fade221839dfd4b89ee873666b6f7beda44310b7a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Oct 2021 00:41:46 GMT
ADD file:cf3b6f9c395392eaf2c629969f59c48cde60ae1c74c3dbb13886481999a7a4d5 in / 
# Sat, 16 Oct 2021 00:41:48 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 01:02:36 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 16 Oct 2021 01:02:41 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:02:42 GMT
ENV GOSU_VERSION=1.13
# Sat, 16 Oct 2021 01:02:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 16 Oct 2021 01:02:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 16 Oct 2021 01:02:55 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:02:55 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 16 Oct 2021 01:03:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 16 Oct 2021 01:03:03 GMT
ARG MARIADB_MAJOR=10.6
# Sat, 16 Oct 2021 01:03:03 GMT
ENV MARIADB_MAJOR=10.6
# Sat, 16 Oct 2021 01:03:03 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Sat, 16 Oct 2021 01:03:04 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Sat, 16 Oct 2021 01:03:04 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Sat, 16 Oct 2021 01:03:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 16 Oct 2021 01:03:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 16 Oct 2021 01:03:26 GMT
VOLUME [/var/lib/mysql]
# Sat, 16 Oct 2021 01:03:26 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Sat, 16 Oct 2021 01:03:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 01:03:26 GMT
EXPOSE 3306
# Sat, 16 Oct 2021 01:03:26 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:1f0267805ccac7499fadaabf65e52d4564add2bc20ed25bcf77df24d8debb103`  
		Last Modified: Sat, 16 Oct 2021 00:42:57 GMT  
		Size: 27.1 MB (27120856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcc30a1fd200d10ce23e934b30e72d36ea131fb670d30afe697304591986fe1`  
		Last Modified: Sat, 16 Oct 2021 01:04:32 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:228a3fc0a9531bf3e9e08d9800daffbe33729ba8a16fb427b07a1a36fb047e02`  
		Last Modified: Sat, 16 Oct 2021 01:04:32 GMT  
		Size: 5.4 MB (5380980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e511a129710d7aa78451eebec778e60a256b2a9e60db59a9f6d09641bd4f96`  
		Last Modified: Sat, 16 Oct 2021 01:04:32 GMT  
		Size: 3.2 MB (3239822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a9cf411b6c206dca4cd2f493440c36781e332782682bb40969b6640e8e98e9`  
		Last Modified: Sat, 16 Oct 2021 01:04:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cac3f3cdb186c64fce6e0a7efc39abe96d0e6ab755d9193c981cc44c801cc51`  
		Last Modified: Sat, 16 Oct 2021 01:04:31 GMT  
		Size: 2.2 MB (2188905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd5f55dd4f1666fe90f4ca1b3b0cc36a9092c44ae19033a4d2b7b0e2ff3dddb`  
		Last Modified: Sat, 16 Oct 2021 01:04:30 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c0ae06775bbebbdaaf444830172bb614071d5d08004722e2ac0acc7dc0106c3`  
		Last Modified: Sat, 16 Oct 2021 01:04:30 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:362403b21b44d69858c7a816e3ddbbd7cb67dac62386727c8ce11d44891fc990`  
		Last Modified: Sat, 16 Oct 2021 01:04:48 GMT  
		Size: 88.1 MB (88073232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48196c9046fbbce7d43754945286d36794d5f7eb923e2501d8a9a4ddc88b3dd3`  
		Last Modified: Sat, 16 Oct 2021 01:04:30 GMT  
		Size: 5.6 KB (5614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10-focal`

```console
$ docker pull mariadb@sha256:c014ba1efc5dbd711d0520c7762d57807f35549de3414eb31e942a420c8a2ed2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:dd08274a61f912b78facb7d144f898c0fd53da4f0c2fcf8ea80cd05f22577221
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.0 MB (127016059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12e05d5da3c5223e9877e8eb90d68560ff66cedcb955131061d60d093a908f0c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:07:51 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 16 Oct 2021 03:07:59 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:07:59 GMT
ENV GOSU_VERSION=1.13
# Sat, 16 Oct 2021 03:08:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 16 Oct 2021 03:08:11 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 16 Oct 2021 03:08:19 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:08:19 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 16 Oct 2021 03:08:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 16 Oct 2021 03:08:27 GMT
ARG MARIADB_MAJOR=10.6
# Sat, 16 Oct 2021 03:08:27 GMT
ENV MARIADB_MAJOR=10.6
# Sat, 16 Oct 2021 03:08:27 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Sat, 16 Oct 2021 03:08:27 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Sat, 16 Oct 2021 03:08:27 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Sat, 16 Oct 2021 03:08:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 16 Oct 2021 03:09:01 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 16 Oct 2021 03:09:02 GMT
VOLUME [/var/lib/mysql]
# Sat, 16 Oct 2021 03:09:02 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Sat, 16 Oct 2021 03:09:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 03:09:02 GMT
EXPOSE 3306
# Sat, 16 Oct 2021 03:09:02 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:034655750c88e076cbd516354371b6176d01179bf595d928444e663ba1fa6845`  
		Last Modified: Sat, 16 Oct 2021 03:11:19 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b757a2a0f02848b1254cbd8b54e1d3cd4651228ede9a8c75e127f91cb415c4`  
		Last Modified: Sat, 16 Oct 2021 03:11:20 GMT  
		Size: 5.5 MB (5489306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c37daf8b6b55859dc1f92dbe017858ae03bd5bf503a3cdbf317b0b4387b1383`  
		Last Modified: Sat, 16 Oct 2021 03:11:19 GMT  
		Size: 3.6 MB (3582632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4cd9409b0f69a0ebe270f43c3a217f05b4c326e5d7c9a4ffb0cb7852ecddc81`  
		Last Modified: Sat, 16 Oct 2021 03:11:18 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbcda06785eb5474250fd32695909199c0de3375a06cf66401d277da518f3da9`  
		Last Modified: Sat, 16 Oct 2021 03:11:17 GMT  
		Size: 2.3 MB (2276882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34cd90f184c404cd4ecd88ebe612e6f180f76836efd3c24a329a3b812c5c345`  
		Last Modified: Sat, 16 Oct 2021 03:11:16 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd6cef4ce4896ed34f82cdec0226170c9ec12e780095f39a268e4f4cd87be523`  
		Last Modified: Sat, 16 Oct 2021 03:11:16 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cb89a1550ea4efead895dec48626ae277912ca9eeffae1a3c1b8c3f0f9ed02d`  
		Last Modified: Sat, 16 Oct 2021 03:11:29 GMT  
		Size: 87.1 MB (87089805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df9f153bd93044efcf8d9cd1ea5266b32bf28df2ad72e5ce195428e8c81b917b`  
		Last Modified: Sat, 16 Oct 2021 03:11:16 GMT  
		Size: 5.6 KB (5611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:52b21e64bd048fb93b8a3ac5d36eaf3027bd5a7b1c71e833bc8ac0aa1c98c72b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.2 MB (124173665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6819e5d163d1d24d896d090e1f55c38bcb9e55db811196e3919f0707a86eff03`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:45:05 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 16 Oct 2021 03:45:15 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:45:15 GMT
ENV GOSU_VERSION=1.13
# Sat, 16 Oct 2021 03:45:29 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 16 Oct 2021 03:45:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 16 Oct 2021 03:45:37 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:45:37 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 16 Oct 2021 03:45:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 16 Oct 2021 03:45:42 GMT
ARG MARIADB_MAJOR=10.6
# Sat, 16 Oct 2021 03:45:43 GMT
ENV MARIADB_MAJOR=10.6
# Sat, 16 Oct 2021 03:45:44 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Sat, 16 Oct 2021 03:45:45 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Sat, 16 Oct 2021 03:45:46 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Sat, 16 Oct 2021 03:45:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 16 Oct 2021 03:46:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 16 Oct 2021 03:46:17 GMT
VOLUME [/var/lib/mysql]
# Sat, 16 Oct 2021 03:46:19 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Sat, 16 Oct 2021 03:46:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 03:46:20 GMT
EXPOSE 3306
# Sat, 16 Oct 2021 03:46:21 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c05479159a3de34e1aedf676cd1a6793673b2e223d06a85c1caeab97e08c15`  
		Last Modified: Sat, 16 Oct 2021 03:51:12 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3fae4be7ce6b0048b0994bc5bd1e2d202fb383de08c3f2b82896678b35e8d1`  
		Last Modified: Sat, 16 Oct 2021 03:51:12 GMT  
		Size: 5.3 MB (5320781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8ca9913d50b67d55691860d8b19e4e38456f1142af47d6ebd4e933757fb2b6`  
		Last Modified: Sat, 16 Oct 2021 03:51:12 GMT  
		Size: 3.4 MB (3368038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffbd8ed1ed1586e00f393ee1417f3bf2b1d83f13c20a5035a050af97e29b9d09`  
		Last Modified: Sat, 16 Oct 2021 03:51:11 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48e61cde050f1f52a8b54730fab5e7bc4db2d6a6303e8fa2ef4eab107076a9ba`  
		Last Modified: Sat, 16 Oct 2021 03:51:09 GMT  
		Size: 2.2 MB (2207084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0b524648b0e80b14e489493c061f52515d6e5791c7f356da3be691507607ce`  
		Last Modified: Sat, 16 Oct 2021 03:51:09 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a7bc5ea6462e7abeb995a46808ebc6c2f6d5afc6361c367235fc02909f95ff`  
		Last Modified: Sat, 16 Oct 2021 03:51:09 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70ea7fb2288eb8ce16b25989a901e5f6bc945315a86d749685f03dabde2bce5`  
		Last Modified: Sat, 16 Oct 2021 03:51:22 GMT  
		Size: 86.1 MB (86096615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:968494f5cebc0a5862440af69b49d4a863460de158a94c0f339b19d08ccf4ab6`  
		Last Modified: Sat, 16 Oct 2021 03:51:09 GMT  
		Size: 5.6 KB (5613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:aa3c316f88dd9537eeaa7201d6d3c5f8d8732196ee6c9cd5ce553816c7a060d9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137539722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a66b6be1b40e577fe733ec92528cf73ee97a8536e1fcddc9fe638aa9132f8173`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Oct 2021 00:36:38 GMT
ADD file:9246bf887411af1b286de95d779c11581dcef3c0d5a29e434162f0c085a7ce85 in / 
# Sat, 16 Oct 2021 00:36:44 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 01:34:00 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 16 Oct 2021 01:34:51 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:34:53 GMT
ENV GOSU_VERSION=1.13
# Sat, 16 Oct 2021 01:35:28 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 16 Oct 2021 01:35:36 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 16 Oct 2021 01:36:02 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:36:03 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 16 Oct 2021 01:36:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 16 Oct 2021 01:36:18 GMT
ARG MARIADB_MAJOR=10.6
# Sat, 16 Oct 2021 01:36:19 GMT
ENV MARIADB_MAJOR=10.6
# Sat, 16 Oct 2021 01:36:22 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Sat, 16 Oct 2021 01:36:24 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Sat, 16 Oct 2021 01:36:29 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Sat, 16 Oct 2021 01:36:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 16 Oct 2021 01:38:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 16 Oct 2021 01:39:01 GMT
VOLUME [/var/lib/mysql]
# Sat, 16 Oct 2021 01:39:03 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Sat, 16 Oct 2021 01:39:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 01:39:08 GMT
EXPOSE 3306
# Sat, 16 Oct 2021 01:39:15 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:77ba7971d651af68e20e7cbb6603a3f7acd8ef2893066767a93db104723556f2`  
		Last Modified: Sat, 16 Oct 2021 00:38:38 GMT  
		Size: 33.3 MB (33287238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a9c5581eb228ed7e984fa7a4e62a7f8b2a068039fde3d32fa3b208026a189d`  
		Last Modified: Sat, 16 Oct 2021 01:49:31 GMT  
		Size: 1.8 KB (1761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63d968d5ad046645779be85243a3db326487bc8905dabf68bb063ea79e1662c1`  
		Last Modified: Sat, 16 Oct 2021 01:49:32 GMT  
		Size: 6.7 MB (6667970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5bdbddf0ed762c90ab4fcfe1f42007a96e4f90ca4f0765dfcec52213a3f5c12`  
		Last Modified: Sat, 16 Oct 2021 01:49:31 GMT  
		Size: 3.7 MB (3670760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00cc95e86fb5ab1bda9839a1ecbd3c2d607bc6cfc5155f33bf32c9d7827ec98b`  
		Last Modified: Sat, 16 Oct 2021 01:49:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe2cefdba07cb9fc803227a545d4fcc196038c1020de7698bf4e333d9056cbd`  
		Last Modified: Sat, 16 Oct 2021 01:49:28 GMT  
		Size: 2.6 MB (2573066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab77c7b0e7b171541e9f7f813ef81190ef39151aea54bfe2b64f8c191ce672c`  
		Last Modified: Sat, 16 Oct 2021 01:49:27 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d188c1c418692bd6c05728f7b542eab7acbdf502f48eaf84c762ba6b27718c`  
		Last Modified: Sat, 16 Oct 2021 01:49:27 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288c0769408956c537d6b5b649bc2b69ffe5036157a0aa58dce6c17312680a33`  
		Last Modified: Sat, 16 Oct 2021 01:49:45 GMT  
		Size: 91.3 MB (91330343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d4c9a0a37f40daaa1c904e99bb499d11db46dd87bd94236295d1ad90603ba74`  
		Last Modified: Sat, 16 Oct 2021 01:49:27 GMT  
		Size: 5.6 KB (5613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:90bc202cc092060b6e454b7f2d06cbe792ffd3d7a2edefe42e30964c55d24dab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.0 MB (126014128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09b71468a7107bd097e1852fade221839dfd4b89ee873666b6f7beda44310b7a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Oct 2021 00:41:46 GMT
ADD file:cf3b6f9c395392eaf2c629969f59c48cde60ae1c74c3dbb13886481999a7a4d5 in / 
# Sat, 16 Oct 2021 00:41:48 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 01:02:36 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 16 Oct 2021 01:02:41 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:02:42 GMT
ENV GOSU_VERSION=1.13
# Sat, 16 Oct 2021 01:02:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 16 Oct 2021 01:02:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 16 Oct 2021 01:02:55 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:02:55 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 16 Oct 2021 01:03:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 16 Oct 2021 01:03:03 GMT
ARG MARIADB_MAJOR=10.6
# Sat, 16 Oct 2021 01:03:03 GMT
ENV MARIADB_MAJOR=10.6
# Sat, 16 Oct 2021 01:03:03 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Sat, 16 Oct 2021 01:03:04 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Sat, 16 Oct 2021 01:03:04 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Sat, 16 Oct 2021 01:03:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 16 Oct 2021 01:03:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 16 Oct 2021 01:03:26 GMT
VOLUME [/var/lib/mysql]
# Sat, 16 Oct 2021 01:03:26 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Sat, 16 Oct 2021 01:03:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 01:03:26 GMT
EXPOSE 3306
# Sat, 16 Oct 2021 01:03:26 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:1f0267805ccac7499fadaabf65e52d4564add2bc20ed25bcf77df24d8debb103`  
		Last Modified: Sat, 16 Oct 2021 00:42:57 GMT  
		Size: 27.1 MB (27120856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcc30a1fd200d10ce23e934b30e72d36ea131fb670d30afe697304591986fe1`  
		Last Modified: Sat, 16 Oct 2021 01:04:32 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:228a3fc0a9531bf3e9e08d9800daffbe33729ba8a16fb427b07a1a36fb047e02`  
		Last Modified: Sat, 16 Oct 2021 01:04:32 GMT  
		Size: 5.4 MB (5380980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e511a129710d7aa78451eebec778e60a256b2a9e60db59a9f6d09641bd4f96`  
		Last Modified: Sat, 16 Oct 2021 01:04:32 GMT  
		Size: 3.2 MB (3239822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a9cf411b6c206dca4cd2f493440c36781e332782682bb40969b6640e8e98e9`  
		Last Modified: Sat, 16 Oct 2021 01:04:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cac3f3cdb186c64fce6e0a7efc39abe96d0e6ab755d9193c981cc44c801cc51`  
		Last Modified: Sat, 16 Oct 2021 01:04:31 GMT  
		Size: 2.2 MB (2188905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd5f55dd4f1666fe90f4ca1b3b0cc36a9092c44ae19033a4d2b7b0e2ff3dddb`  
		Last Modified: Sat, 16 Oct 2021 01:04:30 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c0ae06775bbebbdaaf444830172bb614071d5d08004722e2ac0acc7dc0106c3`  
		Last Modified: Sat, 16 Oct 2021 01:04:30 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:362403b21b44d69858c7a816e3ddbbd7cb67dac62386727c8ce11d44891fc990`  
		Last Modified: Sat, 16 Oct 2021 01:04:48 GMT  
		Size: 88.1 MB (88073232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48196c9046fbbce7d43754945286d36794d5f7eb923e2501d8a9a4ddc88b3dd3`  
		Last Modified: Sat, 16 Oct 2021 01:04:30 GMT  
		Size: 5.6 KB (5614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2`

```console
$ docker pull mariadb@sha256:d2dc04db0abc5f74e07168874786190297a241c5e963a005aa4877e44fc5c8a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2` - linux; amd64

```console
$ docker pull mariadb@sha256:a528fb0b369f7dc138106ac7ff2d3500577d1be6cbee3a7261509bdbb7ee62d6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.3 MB (109274501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:354c935e3d016be16ddc8baaebc97205b8c78a89230b00f06333a2ce62c0f0d0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:22:09 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 01 Oct 2021 05:22:25 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:22:25 GMT
ENV GOSU_VERSION=1.13
# Fri, 01 Oct 2021 05:22:39 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 01 Oct 2021 05:22:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 01 Oct 2021 05:22:48 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:22:49 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 01 Oct 2021 05:22:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 01 Oct 2021 05:22:57 GMT
ARG MARIADB_MAJOR=10.2
# Fri, 01 Oct 2021 05:22:57 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 01 Oct 2021 05:22:57 GMT
ARG MARIADB_VERSION=1:10.2.40+maria~bionic
# Fri, 01 Oct 2021 05:22:58 GMT
ENV MARIADB_VERSION=1:10.2.40+maria~bionic
# Fri, 01 Oct 2021 05:22:58 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
# Fri, 01 Oct 2021 05:22:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 01 Oct 2021 05:23:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 01 Oct 2021 05:23:36 GMT
VOLUME [/var/lib/mysql]
# Fri, 01 Oct 2021 05:23:36 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Fri, 01 Oct 2021 05:23:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 01 Oct 2021 05:23:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Oct 2021 05:23:38 GMT
EXPOSE 3306
# Fri, 01 Oct 2021 05:23:38 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c939c6256f1f0a750da3d02b63d4aa63b9ac6f085a5b904ede35065e2f9074ad`  
		Last Modified: Fri, 01 Oct 2021 05:26:25 GMT  
		Size: 1.9 KB (1870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21b11a4bc2affe5918649c7ac2245c1ba21dc9f4ea8a536f01188e6e7a32bf30`  
		Last Modified: Fri, 01 Oct 2021 05:26:24 GMT  
		Size: 4.8 MB (4813381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec46f26e2520dcdcb3b1337a6f1d0324de5ca746cf496c2f58d1b3a999b0b3ee`  
		Last Modified: Fri, 01 Oct 2021 05:26:23 GMT  
		Size: 3.5 MB (3547363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98c10147eb944f79d9fbf87b70609cf920a464f53924f34d5e0e221a7a301474`  
		Last Modified: Fri, 01 Oct 2021 05:26:22 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02c518dbe68aa8249927d923eb729c649959ac6346fc141829fb1631d88a918d`  
		Last Modified: Fri, 01 Oct 2021 05:26:23 GMT  
		Size: 1.6 MB (1585830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2389b8a7dd566761cba6e2dc15b3fc69c13543880fc93dbf19d15619c461dad2`  
		Last Modified: Fri, 01 Oct 2021 05:26:20 GMT  
		Size: 5.2 KB (5173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4107cbdbc866a69764051c7aae57edbfaa8754f1ab814924f894fb24795bf0d2`  
		Last Modified: Fri, 01 Oct 2021 05:26:20 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1abc07c11569f5fdfc3bd41ab8584879a293c570c6d10e80240ba609fbe5918`  
		Last Modified: Fri, 01 Oct 2021 05:26:31 GMT  
		Size: 72.6 MB (72609605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b160c6de4e1da109323527158924e3ed20ee08ffbc35fa30f621da4e1842a63`  
		Last Modified: Fri, 01 Oct 2021 05:26:20 GMT  
		Size: 5.6 KB (5609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0543f573ce8402a676c92fe1ae461f34d772ae08698e463551812b0a2879babc`  
		Last Modified: Fri, 01 Oct 2021 05:26:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:c09020f7ca4505b6bd683de0805cc9e1fe4c14c9587574e638276f3e26519d9d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.2 MB (104224225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebba047d4094a727881cb732de6278b18c4acd55f72cb016b41c08a7f31055da`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:38 GMT
ADD file:35e2504756850fc1add00516fa89b0499b59c348457a96708eedb61313e7b25e in / 
# Sat, 16 Oct 2021 01:47:38 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:48:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 16 Oct 2021 03:49:08 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:49:09 GMT
ENV GOSU_VERSION=1.13
# Sat, 16 Oct 2021 03:49:24 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 16 Oct 2021 03:49:25 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 16 Oct 2021 03:49:32 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:49:33 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 16 Oct 2021 03:49:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 16 Oct 2021 03:49:38 GMT
ARG MARIADB_MAJOR=10.2
# Sat, 16 Oct 2021 03:49:39 GMT
ENV MARIADB_MAJOR=10.2
# Sat, 16 Oct 2021 03:49:40 GMT
ARG MARIADB_VERSION=1:10.2.40+maria~bionic
# Sat, 16 Oct 2021 03:49:41 GMT
ENV MARIADB_VERSION=1:10.2.40+maria~bionic
# Sat, 16 Oct 2021 03:49:42 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
# Sat, 16 Oct 2021 03:49:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 16 Oct 2021 03:50:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 16 Oct 2021 03:50:14 GMT
VOLUME [/var/lib/mysql]
# Sat, 16 Oct 2021 03:50:15 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Sat, 16 Oct 2021 03:50:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 16 Oct 2021 03:50:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 03:50:17 GMT
EXPOSE 3306
# Sat, 16 Oct 2021 03:50:18 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:f46992f278c2dd50c481ff60ce8528b6eb59016ac6243e1a7fb385c79c5944b9`  
		Last Modified: Fri, 01 Oct 2021 02:45:30 GMT  
		Size: 23.7 MB (23727476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5678889645a4645e6df6f5951b2faa756bcfc3a1c3a4d8b70126c8a381970e38`  
		Last Modified: Sat, 16 Oct 2021 03:53:30 GMT  
		Size: 1.9 KB (1858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11efc1be380cbc922ab4999aadde7b6c48c5228b757176209810d37554b2a056`  
		Last Modified: Sat, 16 Oct 2021 03:53:29 GMT  
		Size: 4.3 MB (4261579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edafeb64a60b41fcaeb64c8037a234ae753c0e0498bc680df42a45fa5f526bf7`  
		Last Modified: Sat, 16 Oct 2021 03:53:28 GMT  
		Size: 3.2 MB (3204113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f39c5af74372b97475cdbf4931359d2fcbeb6ba83f40e5be5c9ff9b20b8a6cf1`  
		Last Modified: Sat, 16 Oct 2021 03:53:27 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf0b072a7b86cf6569d8d3b0698fe518000c512c35400cf48881dfc6caa7f80`  
		Last Modified: Sat, 16 Oct 2021 03:53:28 GMT  
		Size: 1.5 MB (1532464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a388d5118a9b50f94be5b3e2591e454d893208caa3ac280441c02bf5bc948cc`  
		Last Modified: Sat, 16 Oct 2021 03:53:26 GMT  
		Size: 5.1 KB (5148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:170705872e9346973eb220e15746bc6097a59d74ddbb7cc2bb4a1f071f1cdc99`  
		Last Modified: Sat, 16 Oct 2021 03:53:25 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:625dd9916fe3332cf4517686c3573f7f9b2ed92b32dfe3a9d4998ce779586e67`  
		Last Modified: Sat, 16 Oct 2021 03:53:36 GMT  
		Size: 71.5 MB (71485410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41ddfbbaa1dbd3b8e0a64f88b4ec11adfda6bcf59dd2349eed5affa15a2deae`  
		Last Modified: Sat, 16 Oct 2021 03:53:25 GMT  
		Size: 5.6 KB (5614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1e8f42ac1ac41c28a8bd63b22cd03919c029b61acde90dea77d3da52b582c1`  
		Last Modified: Sat, 16 Oct 2021 03:53:25 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2` - linux; ppc64le

```console
$ docker pull mariadb@sha256:a87355bbfcd8c4d277b81f614a424ae07e75c61cd4f907771fafd75c95734f6d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117673902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e8c855f600de1dcf745c21fc2bad2a8c78a04b1b30e81059ceb8015b6831b98`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 05 Oct 2021 11:07:29 GMT
ADD file:fd96554dfb72307c3cf9292c343050a8b9f0848735b7555820f0068914ebd758 in / 
# Tue, 05 Oct 2021 11:07:35 GMT
CMD ["bash"]
# Wed, 06 Oct 2021 18:27:25 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 06 Oct 2021 18:28:04 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 06 Oct 2021 18:28:07 GMT
ENV GOSU_VERSION=1.13
# Wed, 06 Oct 2021 18:28:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 06 Oct 2021 18:28:56 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 06 Oct 2021 18:30:32 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 06 Oct 2021 18:30:36 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 06 Oct 2021 18:30:49 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 06 Oct 2021 18:30:51 GMT
ARG MARIADB_MAJOR=10.2
# Wed, 06 Oct 2021 18:30:54 GMT
ENV MARIADB_MAJOR=10.2
# Wed, 06 Oct 2021 18:30:56 GMT
ARG MARIADB_VERSION=1:10.2.40+maria~bionic
# Wed, 06 Oct 2021 18:30:58 GMT
ENV MARIADB_VERSION=1:10.2.40+maria~bionic
# Wed, 06 Oct 2021 18:31:01 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
# Wed, 06 Oct 2021 18:31:10 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 06 Oct 2021 18:32:52 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 06 Oct 2021 18:32:58 GMT
VOLUME [/var/lib/mysql]
# Wed, 06 Oct 2021 18:33:01 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Wed, 06 Oct 2021 18:33:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 06 Oct 2021 18:33:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Oct 2021 18:33:40 GMT
EXPOSE 3306
# Wed, 06 Oct 2021 18:33:41 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:db28fc1e594e5598e665c54ac1b7fd602d86dddaf8bb237a72303cec22a9185c`  
		Last Modified: Tue, 05 Oct 2021 11:10:31 GMT  
		Size: 30.4 MB (30432921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:508be09c006b6365ae7c5fc9b0593010a2d284d9b02e4f9ad77ee4f4209c8c0a`  
		Last Modified: Wed, 06 Oct 2021 18:37:35 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57bc7004e2371a404c5ff023b89e2ade70ef3581e3c7156807ac620fad13dbaf`  
		Last Modified: Wed, 06 Oct 2021 18:37:32 GMT  
		Size: 5.6 MB (5630476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0247b3a43e1d7479a934dd7064273de0a582a7b29cbbe3930976de3cdea14165`  
		Last Modified: Wed, 06 Oct 2021 18:37:32 GMT  
		Size: 3.5 MB (3529458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f36f80bf4a4eb1f224d050821b3697d447a6684a83bd5474d805d269be98738a`  
		Last Modified: Wed, 06 Oct 2021 18:37:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c8e01754107b9697fb72ecd295ce381ffdbf045d9af0e8434896bbdfb99589`  
		Last Modified: Wed, 06 Oct 2021 18:37:32 GMT  
		Size: 1.9 MB (1938899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d68c6f8634752aa2fad0a3bb47ecd3db12661c09a627f009b659af43d8b50693`  
		Last Modified: Wed, 06 Oct 2021 18:37:28 GMT  
		Size: 5.2 KB (5172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05753e4613d3ea1d36cd939dcb1df72b40d033867d856378e3bb83f4ab74f77e`  
		Last Modified: Wed, 06 Oct 2021 18:37:27 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02b48f20163eab27b9baf9ec26b3653fc71506f35970677fcab2ed9a46cf41ef`  
		Last Modified: Wed, 06 Oct 2021 18:37:42 GMT  
		Size: 76.1 MB (76128891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9e3e320fa8bc28bbfe5b93681ab8640f37280697cd105ce8b6687c1b48b9edc`  
		Last Modified: Wed, 06 Oct 2021 18:37:28 GMT  
		Size: 5.6 KB (5612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf75adc1fe0afd7e3946ed2ab76579aaa00cb5961dd57eb02fe88a7151ff240`  
		Last Modified: Wed, 06 Oct 2021 18:37:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2-bionic`

```console
$ docker pull mariadb@sha256:d2dc04db0abc5f74e07168874786190297a241c5e963a005aa4877e44fc5c8a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2-bionic` - linux; amd64

```console
$ docker pull mariadb@sha256:a528fb0b369f7dc138106ac7ff2d3500577d1be6cbee3a7261509bdbb7ee62d6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.3 MB (109274501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:354c935e3d016be16ddc8baaebc97205b8c78a89230b00f06333a2ce62c0f0d0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:22:09 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 01 Oct 2021 05:22:25 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:22:25 GMT
ENV GOSU_VERSION=1.13
# Fri, 01 Oct 2021 05:22:39 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 01 Oct 2021 05:22:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 01 Oct 2021 05:22:48 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:22:49 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 01 Oct 2021 05:22:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 01 Oct 2021 05:22:57 GMT
ARG MARIADB_MAJOR=10.2
# Fri, 01 Oct 2021 05:22:57 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 01 Oct 2021 05:22:57 GMT
ARG MARIADB_VERSION=1:10.2.40+maria~bionic
# Fri, 01 Oct 2021 05:22:58 GMT
ENV MARIADB_VERSION=1:10.2.40+maria~bionic
# Fri, 01 Oct 2021 05:22:58 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
# Fri, 01 Oct 2021 05:22:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 01 Oct 2021 05:23:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 01 Oct 2021 05:23:36 GMT
VOLUME [/var/lib/mysql]
# Fri, 01 Oct 2021 05:23:36 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Fri, 01 Oct 2021 05:23:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 01 Oct 2021 05:23:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Oct 2021 05:23:38 GMT
EXPOSE 3306
# Fri, 01 Oct 2021 05:23:38 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c939c6256f1f0a750da3d02b63d4aa63b9ac6f085a5b904ede35065e2f9074ad`  
		Last Modified: Fri, 01 Oct 2021 05:26:25 GMT  
		Size: 1.9 KB (1870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21b11a4bc2affe5918649c7ac2245c1ba21dc9f4ea8a536f01188e6e7a32bf30`  
		Last Modified: Fri, 01 Oct 2021 05:26:24 GMT  
		Size: 4.8 MB (4813381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec46f26e2520dcdcb3b1337a6f1d0324de5ca746cf496c2f58d1b3a999b0b3ee`  
		Last Modified: Fri, 01 Oct 2021 05:26:23 GMT  
		Size: 3.5 MB (3547363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98c10147eb944f79d9fbf87b70609cf920a464f53924f34d5e0e221a7a301474`  
		Last Modified: Fri, 01 Oct 2021 05:26:22 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02c518dbe68aa8249927d923eb729c649959ac6346fc141829fb1631d88a918d`  
		Last Modified: Fri, 01 Oct 2021 05:26:23 GMT  
		Size: 1.6 MB (1585830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2389b8a7dd566761cba6e2dc15b3fc69c13543880fc93dbf19d15619c461dad2`  
		Last Modified: Fri, 01 Oct 2021 05:26:20 GMT  
		Size: 5.2 KB (5173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4107cbdbc866a69764051c7aae57edbfaa8754f1ab814924f894fb24795bf0d2`  
		Last Modified: Fri, 01 Oct 2021 05:26:20 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1abc07c11569f5fdfc3bd41ab8584879a293c570c6d10e80240ba609fbe5918`  
		Last Modified: Fri, 01 Oct 2021 05:26:31 GMT  
		Size: 72.6 MB (72609605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b160c6de4e1da109323527158924e3ed20ee08ffbc35fa30f621da4e1842a63`  
		Last Modified: Fri, 01 Oct 2021 05:26:20 GMT  
		Size: 5.6 KB (5609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0543f573ce8402a676c92fe1ae461f34d772ae08698e463551812b0a2879babc`  
		Last Modified: Fri, 01 Oct 2021 05:26:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2-bionic` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:c09020f7ca4505b6bd683de0805cc9e1fe4c14c9587574e638276f3e26519d9d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.2 MB (104224225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebba047d4094a727881cb732de6278b18c4acd55f72cb016b41c08a7f31055da`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:38 GMT
ADD file:35e2504756850fc1add00516fa89b0499b59c348457a96708eedb61313e7b25e in / 
# Sat, 16 Oct 2021 01:47:38 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:48:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 16 Oct 2021 03:49:08 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:49:09 GMT
ENV GOSU_VERSION=1.13
# Sat, 16 Oct 2021 03:49:24 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 16 Oct 2021 03:49:25 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 16 Oct 2021 03:49:32 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:49:33 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 16 Oct 2021 03:49:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 16 Oct 2021 03:49:38 GMT
ARG MARIADB_MAJOR=10.2
# Sat, 16 Oct 2021 03:49:39 GMT
ENV MARIADB_MAJOR=10.2
# Sat, 16 Oct 2021 03:49:40 GMT
ARG MARIADB_VERSION=1:10.2.40+maria~bionic
# Sat, 16 Oct 2021 03:49:41 GMT
ENV MARIADB_VERSION=1:10.2.40+maria~bionic
# Sat, 16 Oct 2021 03:49:42 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
# Sat, 16 Oct 2021 03:49:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 16 Oct 2021 03:50:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 16 Oct 2021 03:50:14 GMT
VOLUME [/var/lib/mysql]
# Sat, 16 Oct 2021 03:50:15 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Sat, 16 Oct 2021 03:50:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 16 Oct 2021 03:50:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 03:50:17 GMT
EXPOSE 3306
# Sat, 16 Oct 2021 03:50:18 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:f46992f278c2dd50c481ff60ce8528b6eb59016ac6243e1a7fb385c79c5944b9`  
		Last Modified: Fri, 01 Oct 2021 02:45:30 GMT  
		Size: 23.7 MB (23727476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5678889645a4645e6df6f5951b2faa756bcfc3a1c3a4d8b70126c8a381970e38`  
		Last Modified: Sat, 16 Oct 2021 03:53:30 GMT  
		Size: 1.9 KB (1858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11efc1be380cbc922ab4999aadde7b6c48c5228b757176209810d37554b2a056`  
		Last Modified: Sat, 16 Oct 2021 03:53:29 GMT  
		Size: 4.3 MB (4261579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edafeb64a60b41fcaeb64c8037a234ae753c0e0498bc680df42a45fa5f526bf7`  
		Last Modified: Sat, 16 Oct 2021 03:53:28 GMT  
		Size: 3.2 MB (3204113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f39c5af74372b97475cdbf4931359d2fcbeb6ba83f40e5be5c9ff9b20b8a6cf1`  
		Last Modified: Sat, 16 Oct 2021 03:53:27 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf0b072a7b86cf6569d8d3b0698fe518000c512c35400cf48881dfc6caa7f80`  
		Last Modified: Sat, 16 Oct 2021 03:53:28 GMT  
		Size: 1.5 MB (1532464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a388d5118a9b50f94be5b3e2591e454d893208caa3ac280441c02bf5bc948cc`  
		Last Modified: Sat, 16 Oct 2021 03:53:26 GMT  
		Size: 5.1 KB (5148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:170705872e9346973eb220e15746bc6097a59d74ddbb7cc2bb4a1f071f1cdc99`  
		Last Modified: Sat, 16 Oct 2021 03:53:25 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:625dd9916fe3332cf4517686c3573f7f9b2ed92b32dfe3a9d4998ce779586e67`  
		Last Modified: Sat, 16 Oct 2021 03:53:36 GMT  
		Size: 71.5 MB (71485410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41ddfbbaa1dbd3b8e0a64f88b4ec11adfda6bcf59dd2349eed5affa15a2deae`  
		Last Modified: Sat, 16 Oct 2021 03:53:25 GMT  
		Size: 5.6 KB (5614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1e8f42ac1ac41c28a8bd63b22cd03919c029b61acde90dea77d3da52b582c1`  
		Last Modified: Sat, 16 Oct 2021 03:53:25 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2-bionic` - linux; ppc64le

```console
$ docker pull mariadb@sha256:a87355bbfcd8c4d277b81f614a424ae07e75c61cd4f907771fafd75c95734f6d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117673902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e8c855f600de1dcf745c21fc2bad2a8c78a04b1b30e81059ceb8015b6831b98`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 05 Oct 2021 11:07:29 GMT
ADD file:fd96554dfb72307c3cf9292c343050a8b9f0848735b7555820f0068914ebd758 in / 
# Tue, 05 Oct 2021 11:07:35 GMT
CMD ["bash"]
# Wed, 06 Oct 2021 18:27:25 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 06 Oct 2021 18:28:04 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 06 Oct 2021 18:28:07 GMT
ENV GOSU_VERSION=1.13
# Wed, 06 Oct 2021 18:28:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 06 Oct 2021 18:28:56 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 06 Oct 2021 18:30:32 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 06 Oct 2021 18:30:36 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 06 Oct 2021 18:30:49 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 06 Oct 2021 18:30:51 GMT
ARG MARIADB_MAJOR=10.2
# Wed, 06 Oct 2021 18:30:54 GMT
ENV MARIADB_MAJOR=10.2
# Wed, 06 Oct 2021 18:30:56 GMT
ARG MARIADB_VERSION=1:10.2.40+maria~bionic
# Wed, 06 Oct 2021 18:30:58 GMT
ENV MARIADB_VERSION=1:10.2.40+maria~bionic
# Wed, 06 Oct 2021 18:31:01 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
# Wed, 06 Oct 2021 18:31:10 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 06 Oct 2021 18:32:52 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 06 Oct 2021 18:32:58 GMT
VOLUME [/var/lib/mysql]
# Wed, 06 Oct 2021 18:33:01 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Wed, 06 Oct 2021 18:33:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.40/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 06 Oct 2021 18:33:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Oct 2021 18:33:40 GMT
EXPOSE 3306
# Wed, 06 Oct 2021 18:33:41 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:db28fc1e594e5598e665c54ac1b7fd602d86dddaf8bb237a72303cec22a9185c`  
		Last Modified: Tue, 05 Oct 2021 11:10:31 GMT  
		Size: 30.4 MB (30432921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:508be09c006b6365ae7c5fc9b0593010a2d284d9b02e4f9ad77ee4f4209c8c0a`  
		Last Modified: Wed, 06 Oct 2021 18:37:35 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57bc7004e2371a404c5ff023b89e2ade70ef3581e3c7156807ac620fad13dbaf`  
		Last Modified: Wed, 06 Oct 2021 18:37:32 GMT  
		Size: 5.6 MB (5630476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0247b3a43e1d7479a934dd7064273de0a582a7b29cbbe3930976de3cdea14165`  
		Last Modified: Wed, 06 Oct 2021 18:37:32 GMT  
		Size: 3.5 MB (3529458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f36f80bf4a4eb1f224d050821b3697d447a6684a83bd5474d805d269be98738a`  
		Last Modified: Wed, 06 Oct 2021 18:37:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c8e01754107b9697fb72ecd295ce381ffdbf045d9af0e8434896bbdfb99589`  
		Last Modified: Wed, 06 Oct 2021 18:37:32 GMT  
		Size: 1.9 MB (1938899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d68c6f8634752aa2fad0a3bb47ecd3db12661c09a627f009b659af43d8b50693`  
		Last Modified: Wed, 06 Oct 2021 18:37:28 GMT  
		Size: 5.2 KB (5172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05753e4613d3ea1d36cd939dcb1df72b40d033867d856378e3bb83f4ab74f77e`  
		Last Modified: Wed, 06 Oct 2021 18:37:27 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02b48f20163eab27b9baf9ec26b3653fc71506f35970677fcab2ed9a46cf41ef`  
		Last Modified: Wed, 06 Oct 2021 18:37:42 GMT  
		Size: 76.1 MB (76128891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9e3e320fa8bc28bbfe5b93681ab8640f37280697cd105ce8b6687c1b48b9edc`  
		Last Modified: Wed, 06 Oct 2021 18:37:28 GMT  
		Size: 5.6 KB (5612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf75adc1fe0afd7e3946ed2ab76579aaa00cb5961dd57eb02fe88a7151ff240`  
		Last Modified: Wed, 06 Oct 2021 18:37:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2.41`

**does not exist** (yet?)

## `mariadb:10.2.41-bionic`

**does not exist** (yet?)

## `mariadb:10.3`

```console
$ docker pull mariadb@sha256:22834b9671a1e89b74e0cc0bc285fd33425ba2641afe86cb3afd5d8617245b81
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3` - linux; amd64

```console
$ docker pull mariadb@sha256:7543801a78925a76f573263b976f4af96d97945cea96191bb66ae80152b7a52a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.0 MB (120017580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:439df5ac95824886b61e6060d35cdc1e29c8fb7fbb358f8770a6c2f86d717671`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:07:51 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 16 Oct 2021 03:07:59 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:07:59 GMT
ENV GOSU_VERSION=1.13
# Sat, 16 Oct 2021 03:08:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 16 Oct 2021 03:08:11 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 16 Oct 2021 03:08:19 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:08:19 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 16 Oct 2021 03:08:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 16 Oct 2021 03:10:15 GMT
ARG MARIADB_MAJOR=10.3
# Sat, 16 Oct 2021 03:10:15 GMT
ENV MARIADB_MAJOR=10.3
# Sat, 16 Oct 2021 03:10:16 GMT
ARG MARIADB_VERSION=1:10.3.31+maria~focal
# Sat, 16 Oct 2021 03:10:16 GMT
ENV MARIADB_VERSION=1:10.3.31+maria~focal
# Sat, 16 Oct 2021 03:10:16 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
# Sat, 16 Oct 2021 03:10:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 16 Oct 2021 03:10:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 16 Oct 2021 03:10:45 GMT
VOLUME [/var/lib/mysql]
# Sat, 16 Oct 2021 03:10:45 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Sat, 16 Oct 2021 03:10:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 16 Oct 2021 03:10:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 03:10:46 GMT
EXPOSE 3306
# Sat, 16 Oct 2021 03:10:46 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:034655750c88e076cbd516354371b6176d01179bf595d928444e663ba1fa6845`  
		Last Modified: Sat, 16 Oct 2021 03:11:19 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b757a2a0f02848b1254cbd8b54e1d3cd4651228ede9a8c75e127f91cb415c4`  
		Last Modified: Sat, 16 Oct 2021 03:11:20 GMT  
		Size: 5.5 MB (5489306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c37daf8b6b55859dc1f92dbe017858ae03bd5bf503a3cdbf317b0b4387b1383`  
		Last Modified: Sat, 16 Oct 2021 03:11:19 GMT  
		Size: 3.6 MB (3582632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4cd9409b0f69a0ebe270f43c3a217f05b4c326e5d7c9a4ffb0cb7852ecddc81`  
		Last Modified: Sat, 16 Oct 2021 03:11:18 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbcda06785eb5474250fd32695909199c0de3375a06cf66401d277da518f3da9`  
		Last Modified: Sat, 16 Oct 2021 03:11:17 GMT  
		Size: 2.3 MB (2276882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34cd90f184c404cd4ecd88ebe612e6f180f76836efd3c24a329a3b812c5c345`  
		Last Modified: Sat, 16 Oct 2021 03:11:16 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c0df9b2fca5488c3ae4bc7c8843d87ed1a2324bea90136eaafdbbc2b0f10cc`  
		Last Modified: Sat, 16 Oct 2021 03:12:51 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2a4d476ce21452a3d7898bf1ca3c9ab090ab9a76b9deb39d0059f648173bcc7`  
		Last Modified: Sat, 16 Oct 2021 03:13:04 GMT  
		Size: 80.1 MB (80091203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6592280ea5147460f99f4a42f891a1f3c46510547ac57ee49b23adf9ec73fbed`  
		Last Modified: Sat, 16 Oct 2021 03:12:52 GMT  
		Size: 5.6 KB (5612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ede5dfe32b4a731de65144f1fcc63ba296f46fb9eda5e4cb899db2d18af49e3`  
		Last Modified: Sat, 16 Oct 2021 03:12:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:f200ec45be8c937e80590f8605a4354f69e7f78126208c8942ef9f46d23ce0f8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.5 MB (117491220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7048d07a49847a32641e07f9ba10289a850b35cdf689c67db6a03a793a98baf3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:45:05 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 16 Oct 2021 03:45:15 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:45:15 GMT
ENV GOSU_VERSION=1.13
# Sat, 16 Oct 2021 03:45:29 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 16 Oct 2021 03:45:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 16 Oct 2021 03:45:37 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:45:37 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 16 Oct 2021 03:45:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 16 Oct 2021 03:48:06 GMT
ARG MARIADB_MAJOR=10.3
# Sat, 16 Oct 2021 03:48:06 GMT
ENV MARIADB_MAJOR=10.3
# Sat, 16 Oct 2021 03:48:07 GMT
ARG MARIADB_VERSION=1:10.3.31+maria~focal
# Sat, 16 Oct 2021 03:48:08 GMT
ENV MARIADB_VERSION=1:10.3.31+maria~focal
# Sat, 16 Oct 2021 03:48:09 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
# Sat, 16 Oct 2021 03:48:10 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 16 Oct 2021 03:48:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 16 Oct 2021 03:48:47 GMT
VOLUME [/var/lib/mysql]
# Sat, 16 Oct 2021 03:48:49 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Sat, 16 Oct 2021 03:48:49 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 16 Oct 2021 03:48:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 03:48:51 GMT
EXPOSE 3306
# Sat, 16 Oct 2021 03:48:52 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c05479159a3de34e1aedf676cd1a6793673b2e223d06a85c1caeab97e08c15`  
		Last Modified: Sat, 16 Oct 2021 03:51:12 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3fae4be7ce6b0048b0994bc5bd1e2d202fb383de08c3f2b82896678b35e8d1`  
		Last Modified: Sat, 16 Oct 2021 03:51:12 GMT  
		Size: 5.3 MB (5320781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8ca9913d50b67d55691860d8b19e4e38456f1142af47d6ebd4e933757fb2b6`  
		Last Modified: Sat, 16 Oct 2021 03:51:12 GMT  
		Size: 3.4 MB (3368038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffbd8ed1ed1586e00f393ee1417f3bf2b1d83f13c20a5035a050af97e29b9d09`  
		Last Modified: Sat, 16 Oct 2021 03:51:11 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48e61cde050f1f52a8b54730fab5e7bc4db2d6a6303e8fa2ef4eab107076a9ba`  
		Last Modified: Sat, 16 Oct 2021 03:51:09 GMT  
		Size: 2.2 MB (2207084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0b524648b0e80b14e489493c061f52515d6e5791c7f356da3be691507607ce`  
		Last Modified: Sat, 16 Oct 2021 03:51:09 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c568c49bc8e03b1a5d493c12bdbecb25a28ace4ba2896f0cbb34cf50ae669fe`  
		Last Modified: Sat, 16 Oct 2021 03:52:55 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc2b850a181accff6ee6dc3c16666aab87963e0bb5a21358f9fc4de7b8b7d76`  
		Last Modified: Sat, 16 Oct 2021 03:53:08 GMT  
		Size: 79.4 MB (79414050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22cd0a60f1c7a0dc039cb8da10405feeda9a8fe46934f3c49bd6474908405747`  
		Last Modified: Sat, 16 Oct 2021 03:52:55 GMT  
		Size: 5.6 KB (5612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51361d1004c07a2b37fce00584e31e8b4fc128083a536af0be0da1580721969a`  
		Last Modified: Sat, 16 Oct 2021 03:52:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3` - linux; ppc64le

```console
$ docker pull mariadb@sha256:eabb2e81a20381ca05c1eef2015ba97f7ad63de9a30d74add3c07174ceb70ab7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.9 MB (130878512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b14c8cd50591ce95eaff04590dcce413136bcdf53a1d7e29f4664791de54dfd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Oct 2021 00:36:38 GMT
ADD file:9246bf887411af1b286de95d779c11581dcef3c0d5a29e434162f0c085a7ce85 in / 
# Sat, 16 Oct 2021 00:36:44 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 01:34:00 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 16 Oct 2021 01:34:51 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:34:53 GMT
ENV GOSU_VERSION=1.13
# Sat, 16 Oct 2021 01:35:28 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 16 Oct 2021 01:35:36 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 16 Oct 2021 01:36:02 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:36:03 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 16 Oct 2021 01:36:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 16 Oct 2021 01:45:24 GMT
ARG MARIADB_MAJOR=10.3
# Sat, 16 Oct 2021 01:45:26 GMT
ENV MARIADB_MAJOR=10.3
# Sat, 16 Oct 2021 01:45:30 GMT
ARG MARIADB_VERSION=1:10.3.31+maria~focal
# Sat, 16 Oct 2021 01:45:31 GMT
ENV MARIADB_VERSION=1:10.3.31+maria~focal
# Sat, 16 Oct 2021 01:45:34 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
# Sat, 16 Oct 2021 01:45:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 16 Oct 2021 01:47:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 16 Oct 2021 01:48:00 GMT
VOLUME [/var/lib/mysql]
# Sat, 16 Oct 2021 01:48:01 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Sat, 16 Oct 2021 01:48:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 16 Oct 2021 01:48:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 01:48:17 GMT
EXPOSE 3306
# Sat, 16 Oct 2021 01:48:19 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:77ba7971d651af68e20e7cbb6603a3f7acd8ef2893066767a93db104723556f2`  
		Last Modified: Sat, 16 Oct 2021 00:38:38 GMT  
		Size: 33.3 MB (33287238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a9c5581eb228ed7e984fa7a4e62a7f8b2a068039fde3d32fa3b208026a189d`  
		Last Modified: Sat, 16 Oct 2021 01:49:31 GMT  
		Size: 1.8 KB (1761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63d968d5ad046645779be85243a3db326487bc8905dabf68bb063ea79e1662c1`  
		Last Modified: Sat, 16 Oct 2021 01:49:32 GMT  
		Size: 6.7 MB (6667970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5bdbddf0ed762c90ab4fcfe1f42007a96e4f90ca4f0765dfcec52213a3f5c12`  
		Last Modified: Sat, 16 Oct 2021 01:49:31 GMT  
		Size: 3.7 MB (3670760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00cc95e86fb5ab1bda9839a1ecbd3c2d607bc6cfc5155f33bf32c9d7827ec98b`  
		Last Modified: Sat, 16 Oct 2021 01:49:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe2cefdba07cb9fc803227a545d4fcc196038c1020de7698bf4e333d9056cbd`  
		Last Modified: Sat, 16 Oct 2021 01:49:28 GMT  
		Size: 2.6 MB (2573066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab77c7b0e7b171541e9f7f813ef81190ef39151aea54bfe2b64f8c191ce672c`  
		Last Modified: Sat, 16 Oct 2021 01:49:27 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94aeb2fd007f06d10435736a0bd9fae69670ff9c01bc11e62f75e5fea4653129`  
		Last Modified: Sat, 16 Oct 2021 01:51:28 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e393cff902c3ca290ce3dbad73eceaf35a4548496b5944e1fcd51253e5fcf022`  
		Last Modified: Sat, 16 Oct 2021 01:51:45 GMT  
		Size: 84.7 MB (84669015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9afc7f203a71d7290d7ab97ce69fc1691c8ef75f8582f449060a77a9ca89d1`  
		Last Modified: Sat, 16 Oct 2021 01:51:29 GMT  
		Size: 5.6 KB (5610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dc4f496ad3cc84a892fb9157e7341f3c85c2fd8d8a0251e3578987bc804d6a9`  
		Last Modified: Sat, 16 Oct 2021 01:51:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3-focal`

```console
$ docker pull mariadb@sha256:22834b9671a1e89b74e0cc0bc285fd33425ba2641afe86cb3afd5d8617245b81
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:7543801a78925a76f573263b976f4af96d97945cea96191bb66ae80152b7a52a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.0 MB (120017580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:439df5ac95824886b61e6060d35cdc1e29c8fb7fbb358f8770a6c2f86d717671`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:07:51 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 16 Oct 2021 03:07:59 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:07:59 GMT
ENV GOSU_VERSION=1.13
# Sat, 16 Oct 2021 03:08:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 16 Oct 2021 03:08:11 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 16 Oct 2021 03:08:19 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:08:19 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 16 Oct 2021 03:08:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 16 Oct 2021 03:10:15 GMT
ARG MARIADB_MAJOR=10.3
# Sat, 16 Oct 2021 03:10:15 GMT
ENV MARIADB_MAJOR=10.3
# Sat, 16 Oct 2021 03:10:16 GMT
ARG MARIADB_VERSION=1:10.3.31+maria~focal
# Sat, 16 Oct 2021 03:10:16 GMT
ENV MARIADB_VERSION=1:10.3.31+maria~focal
# Sat, 16 Oct 2021 03:10:16 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
# Sat, 16 Oct 2021 03:10:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 16 Oct 2021 03:10:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 16 Oct 2021 03:10:45 GMT
VOLUME [/var/lib/mysql]
# Sat, 16 Oct 2021 03:10:45 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Sat, 16 Oct 2021 03:10:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 16 Oct 2021 03:10:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 03:10:46 GMT
EXPOSE 3306
# Sat, 16 Oct 2021 03:10:46 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:034655750c88e076cbd516354371b6176d01179bf595d928444e663ba1fa6845`  
		Last Modified: Sat, 16 Oct 2021 03:11:19 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b757a2a0f02848b1254cbd8b54e1d3cd4651228ede9a8c75e127f91cb415c4`  
		Last Modified: Sat, 16 Oct 2021 03:11:20 GMT  
		Size: 5.5 MB (5489306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c37daf8b6b55859dc1f92dbe017858ae03bd5bf503a3cdbf317b0b4387b1383`  
		Last Modified: Sat, 16 Oct 2021 03:11:19 GMT  
		Size: 3.6 MB (3582632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4cd9409b0f69a0ebe270f43c3a217f05b4c326e5d7c9a4ffb0cb7852ecddc81`  
		Last Modified: Sat, 16 Oct 2021 03:11:18 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbcda06785eb5474250fd32695909199c0de3375a06cf66401d277da518f3da9`  
		Last Modified: Sat, 16 Oct 2021 03:11:17 GMT  
		Size: 2.3 MB (2276882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34cd90f184c404cd4ecd88ebe612e6f180f76836efd3c24a329a3b812c5c345`  
		Last Modified: Sat, 16 Oct 2021 03:11:16 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c0df9b2fca5488c3ae4bc7c8843d87ed1a2324bea90136eaafdbbc2b0f10cc`  
		Last Modified: Sat, 16 Oct 2021 03:12:51 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2a4d476ce21452a3d7898bf1ca3c9ab090ab9a76b9deb39d0059f648173bcc7`  
		Last Modified: Sat, 16 Oct 2021 03:13:04 GMT  
		Size: 80.1 MB (80091203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6592280ea5147460f99f4a42f891a1f3c46510547ac57ee49b23adf9ec73fbed`  
		Last Modified: Sat, 16 Oct 2021 03:12:52 GMT  
		Size: 5.6 KB (5612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ede5dfe32b4a731de65144f1fcc63ba296f46fb9eda5e4cb899db2d18af49e3`  
		Last Modified: Sat, 16 Oct 2021 03:12:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:f200ec45be8c937e80590f8605a4354f69e7f78126208c8942ef9f46d23ce0f8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.5 MB (117491220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7048d07a49847a32641e07f9ba10289a850b35cdf689c67db6a03a793a98baf3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:45:05 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 16 Oct 2021 03:45:15 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:45:15 GMT
ENV GOSU_VERSION=1.13
# Sat, 16 Oct 2021 03:45:29 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 16 Oct 2021 03:45:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 16 Oct 2021 03:45:37 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:45:37 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 16 Oct 2021 03:45:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 16 Oct 2021 03:48:06 GMT
ARG MARIADB_MAJOR=10.3
# Sat, 16 Oct 2021 03:48:06 GMT
ENV MARIADB_MAJOR=10.3
# Sat, 16 Oct 2021 03:48:07 GMT
ARG MARIADB_VERSION=1:10.3.31+maria~focal
# Sat, 16 Oct 2021 03:48:08 GMT
ENV MARIADB_VERSION=1:10.3.31+maria~focal
# Sat, 16 Oct 2021 03:48:09 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
# Sat, 16 Oct 2021 03:48:10 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 16 Oct 2021 03:48:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 16 Oct 2021 03:48:47 GMT
VOLUME [/var/lib/mysql]
# Sat, 16 Oct 2021 03:48:49 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Sat, 16 Oct 2021 03:48:49 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 16 Oct 2021 03:48:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 03:48:51 GMT
EXPOSE 3306
# Sat, 16 Oct 2021 03:48:52 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c05479159a3de34e1aedf676cd1a6793673b2e223d06a85c1caeab97e08c15`  
		Last Modified: Sat, 16 Oct 2021 03:51:12 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3fae4be7ce6b0048b0994bc5bd1e2d202fb383de08c3f2b82896678b35e8d1`  
		Last Modified: Sat, 16 Oct 2021 03:51:12 GMT  
		Size: 5.3 MB (5320781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8ca9913d50b67d55691860d8b19e4e38456f1142af47d6ebd4e933757fb2b6`  
		Last Modified: Sat, 16 Oct 2021 03:51:12 GMT  
		Size: 3.4 MB (3368038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffbd8ed1ed1586e00f393ee1417f3bf2b1d83f13c20a5035a050af97e29b9d09`  
		Last Modified: Sat, 16 Oct 2021 03:51:11 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48e61cde050f1f52a8b54730fab5e7bc4db2d6a6303e8fa2ef4eab107076a9ba`  
		Last Modified: Sat, 16 Oct 2021 03:51:09 GMT  
		Size: 2.2 MB (2207084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0b524648b0e80b14e489493c061f52515d6e5791c7f356da3be691507607ce`  
		Last Modified: Sat, 16 Oct 2021 03:51:09 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c568c49bc8e03b1a5d493c12bdbecb25a28ace4ba2896f0cbb34cf50ae669fe`  
		Last Modified: Sat, 16 Oct 2021 03:52:55 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc2b850a181accff6ee6dc3c16666aab87963e0bb5a21358f9fc4de7b8b7d76`  
		Last Modified: Sat, 16 Oct 2021 03:53:08 GMT  
		Size: 79.4 MB (79414050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22cd0a60f1c7a0dc039cb8da10405feeda9a8fe46934f3c49bd6474908405747`  
		Last Modified: Sat, 16 Oct 2021 03:52:55 GMT  
		Size: 5.6 KB (5612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51361d1004c07a2b37fce00584e31e8b4fc128083a536af0be0da1580721969a`  
		Last Modified: Sat, 16 Oct 2021 03:52:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:eabb2e81a20381ca05c1eef2015ba97f7ad63de9a30d74add3c07174ceb70ab7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.9 MB (130878512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b14c8cd50591ce95eaff04590dcce413136bcdf53a1d7e29f4664791de54dfd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Oct 2021 00:36:38 GMT
ADD file:9246bf887411af1b286de95d779c11581dcef3c0d5a29e434162f0c085a7ce85 in / 
# Sat, 16 Oct 2021 00:36:44 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 01:34:00 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 16 Oct 2021 01:34:51 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:34:53 GMT
ENV GOSU_VERSION=1.13
# Sat, 16 Oct 2021 01:35:28 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 16 Oct 2021 01:35:36 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 16 Oct 2021 01:36:02 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:36:03 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 16 Oct 2021 01:36:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 16 Oct 2021 01:45:24 GMT
ARG MARIADB_MAJOR=10.3
# Sat, 16 Oct 2021 01:45:26 GMT
ENV MARIADB_MAJOR=10.3
# Sat, 16 Oct 2021 01:45:30 GMT
ARG MARIADB_VERSION=1:10.3.31+maria~focal
# Sat, 16 Oct 2021 01:45:31 GMT
ENV MARIADB_VERSION=1:10.3.31+maria~focal
# Sat, 16 Oct 2021 01:45:34 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
# Sat, 16 Oct 2021 01:45:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 16 Oct 2021 01:47:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 16 Oct 2021 01:48:00 GMT
VOLUME [/var/lib/mysql]
# Sat, 16 Oct 2021 01:48:01 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Sat, 16 Oct 2021 01:48:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.31/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 16 Oct 2021 01:48:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 01:48:17 GMT
EXPOSE 3306
# Sat, 16 Oct 2021 01:48:19 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:77ba7971d651af68e20e7cbb6603a3f7acd8ef2893066767a93db104723556f2`  
		Last Modified: Sat, 16 Oct 2021 00:38:38 GMT  
		Size: 33.3 MB (33287238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a9c5581eb228ed7e984fa7a4e62a7f8b2a068039fde3d32fa3b208026a189d`  
		Last Modified: Sat, 16 Oct 2021 01:49:31 GMT  
		Size: 1.8 KB (1761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63d968d5ad046645779be85243a3db326487bc8905dabf68bb063ea79e1662c1`  
		Last Modified: Sat, 16 Oct 2021 01:49:32 GMT  
		Size: 6.7 MB (6667970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5bdbddf0ed762c90ab4fcfe1f42007a96e4f90ca4f0765dfcec52213a3f5c12`  
		Last Modified: Sat, 16 Oct 2021 01:49:31 GMT  
		Size: 3.7 MB (3670760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00cc95e86fb5ab1bda9839a1ecbd3c2d607bc6cfc5155f33bf32c9d7827ec98b`  
		Last Modified: Sat, 16 Oct 2021 01:49:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe2cefdba07cb9fc803227a545d4fcc196038c1020de7698bf4e333d9056cbd`  
		Last Modified: Sat, 16 Oct 2021 01:49:28 GMT  
		Size: 2.6 MB (2573066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab77c7b0e7b171541e9f7f813ef81190ef39151aea54bfe2b64f8c191ce672c`  
		Last Modified: Sat, 16 Oct 2021 01:49:27 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94aeb2fd007f06d10435736a0bd9fae69670ff9c01bc11e62f75e5fea4653129`  
		Last Modified: Sat, 16 Oct 2021 01:51:28 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e393cff902c3ca290ce3dbad73eceaf35a4548496b5944e1fcd51253e5fcf022`  
		Last Modified: Sat, 16 Oct 2021 01:51:45 GMT  
		Size: 84.7 MB (84669015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9afc7f203a71d7290d7ab97ce69fc1691c8ef75f8582f449060a77a9ca89d1`  
		Last Modified: Sat, 16 Oct 2021 01:51:29 GMT  
		Size: 5.6 KB (5610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dc4f496ad3cc84a892fb9157e7341f3c85c2fd8d8a0251e3578987bc804d6a9`  
		Last Modified: Sat, 16 Oct 2021 01:51:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3.32`

**does not exist** (yet?)

## `mariadb:10.3.32-focal`

**does not exist** (yet?)

## `mariadb:10.4`

```console
$ docker pull mariadb@sha256:65cdad364df07770a0da7da4183a78fefdcb202e146e541ea51b515ab26588de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4` - linux; amd64

```console
$ docker pull mariadb@sha256:439f7fa3d647ff354bd7b0883543ede691ab412d3cf722312f761de5116b728c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.7 MB (124740387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5f1527bdc85420e34baab9fa2467bc865342f43d0d11eb5b92c5b43063818a1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:07:51 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 16 Oct 2021 03:07:59 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:07:59 GMT
ENV GOSU_VERSION=1.13
# Sat, 16 Oct 2021 03:08:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 16 Oct 2021 03:08:11 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 16 Oct 2021 03:08:19 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:08:19 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 16 Oct 2021 03:08:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 16 Oct 2021 03:09:42 GMT
ARG MARIADB_MAJOR=10.4
# Sat, 16 Oct 2021 03:09:42 GMT
ENV MARIADB_MAJOR=10.4
# Sat, 16 Oct 2021 03:09:42 GMT
ARG MARIADB_VERSION=1:10.4.21+maria~focal
# Sat, 16 Oct 2021 03:09:42 GMT
ENV MARIADB_VERSION=1:10.4.21+maria~focal
# Sat, 16 Oct 2021 03:09:43 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
# Sat, 16 Oct 2021 03:09:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 16 Oct 2021 03:10:07 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 16 Oct 2021 03:10:08 GMT
VOLUME [/var/lib/mysql]
# Sat, 16 Oct 2021 03:10:08 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Sat, 16 Oct 2021 03:10:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 16 Oct 2021 03:10:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 03:10:10 GMT
EXPOSE 3306
# Sat, 16 Oct 2021 03:10:10 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:034655750c88e076cbd516354371b6176d01179bf595d928444e663ba1fa6845`  
		Last Modified: Sat, 16 Oct 2021 03:11:19 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b757a2a0f02848b1254cbd8b54e1d3cd4651228ede9a8c75e127f91cb415c4`  
		Last Modified: Sat, 16 Oct 2021 03:11:20 GMT  
		Size: 5.5 MB (5489306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c37daf8b6b55859dc1f92dbe017858ae03bd5bf503a3cdbf317b0b4387b1383`  
		Last Modified: Sat, 16 Oct 2021 03:11:19 GMT  
		Size: 3.6 MB (3582632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4cd9409b0f69a0ebe270f43c3a217f05b4c326e5d7c9a4ffb0cb7852ecddc81`  
		Last Modified: Sat, 16 Oct 2021 03:11:18 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbcda06785eb5474250fd32695909199c0de3375a06cf66401d277da518f3da9`  
		Last Modified: Sat, 16 Oct 2021 03:11:17 GMT  
		Size: 2.3 MB (2276882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34cd90f184c404cd4ecd88ebe612e6f180f76836efd3c24a329a3b812c5c345`  
		Last Modified: Sat, 16 Oct 2021 03:11:16 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6b213ac7f8a27abb0260723d8ab653adae1a5e6e1fa3c88d2d72e3823008a2a`  
		Last Modified: Sat, 16 Oct 2021 03:12:23 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac4568a963367b26c6c6c205b0cb775b5cf0812de8b44ba202309bbd7112592`  
		Last Modified: Sat, 16 Oct 2021 03:12:36 GMT  
		Size: 84.8 MB (84814009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5893a4f69042677decbadd989d4d1c7d3fb6f4fe92cc2986d6d26ac8ee8ceef`  
		Last Modified: Sat, 16 Oct 2021 03:12:23 GMT  
		Size: 5.6 KB (5613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d3849bbe75232c1320002f21633b2ae27d473117d5c43da4eee987fe3db34ae`  
		Last Modified: Sat, 16 Oct 2021 03:12:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:52d628b916bf43950ce0ce5632a623351eed6522f8e107a6eba6ea8963f37426
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.1 MB (122117980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7708994f226c0cefde734f08a20807dea8b65ba0ba73a751fcb7e1c29f89ac6b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:45:05 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 16 Oct 2021 03:45:15 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:45:15 GMT
ENV GOSU_VERSION=1.13
# Sat, 16 Oct 2021 03:45:29 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 16 Oct 2021 03:45:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 16 Oct 2021 03:45:37 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:45:37 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 16 Oct 2021 03:45:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 16 Oct 2021 03:47:14 GMT
ARG MARIADB_MAJOR=10.4
# Sat, 16 Oct 2021 03:47:15 GMT
ENV MARIADB_MAJOR=10.4
# Sat, 16 Oct 2021 03:47:16 GMT
ARG MARIADB_VERSION=1:10.4.21+maria~focal
# Sat, 16 Oct 2021 03:47:17 GMT
ENV MARIADB_VERSION=1:10.4.21+maria~focal
# Sat, 16 Oct 2021 03:47:18 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
# Sat, 16 Oct 2021 03:47:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 16 Oct 2021 03:47:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 16 Oct 2021 03:47:49 GMT
VOLUME [/var/lib/mysql]
# Sat, 16 Oct 2021 03:47:51 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Sat, 16 Oct 2021 03:47:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 16 Oct 2021 03:47:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 03:47:53 GMT
EXPOSE 3306
# Sat, 16 Oct 2021 03:47:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c05479159a3de34e1aedf676cd1a6793673b2e223d06a85c1caeab97e08c15`  
		Last Modified: Sat, 16 Oct 2021 03:51:12 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3fae4be7ce6b0048b0994bc5bd1e2d202fb383de08c3f2b82896678b35e8d1`  
		Last Modified: Sat, 16 Oct 2021 03:51:12 GMT  
		Size: 5.3 MB (5320781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8ca9913d50b67d55691860d8b19e4e38456f1142af47d6ebd4e933757fb2b6`  
		Last Modified: Sat, 16 Oct 2021 03:51:12 GMT  
		Size: 3.4 MB (3368038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffbd8ed1ed1586e00f393ee1417f3bf2b1d83f13c20a5035a050af97e29b9d09`  
		Last Modified: Sat, 16 Oct 2021 03:51:11 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48e61cde050f1f52a8b54730fab5e7bc4db2d6a6303e8fa2ef4eab107076a9ba`  
		Last Modified: Sat, 16 Oct 2021 03:51:09 GMT  
		Size: 2.2 MB (2207084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0b524648b0e80b14e489493c061f52515d6e5791c7f356da3be691507607ce`  
		Last Modified: Sat, 16 Oct 2021 03:51:09 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3dad55f85a67ac93ebeb8dad38d3c1c6500326134742d57fa9b76a98deb34ac`  
		Last Modified: Sat, 16 Oct 2021 03:52:24 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3097425ea97c6a8c8e3a11fcd692cf9b4acde246cc1dbee155184fdbf7e30d`  
		Last Modified: Sat, 16 Oct 2021 03:52:37 GMT  
		Size: 84.0 MB (84040811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b14d0cc23ba7e1016e58d13960b2d05c94a250584c8d2758d2506b03cef6ff`  
		Last Modified: Sat, 16 Oct 2021 03:52:24 GMT  
		Size: 5.6 KB (5611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce06bebf02092572d39ca9ee0adeca5b5967fb56f99c6391032c3f938b38bd83`  
		Last Modified: Sat, 16 Oct 2021 03:52:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4` - linux; ppc64le

```console
$ docker pull mariadb@sha256:db23ae4a8dc88c4e06fcd477bd8ec87388a4acd0562e8f1baeb9c16cd2e3d3a2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.5 MB (135463544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3acf37940c7d117f6000c53a107c6013f52d57d70afb7a47a667ea880124344b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Oct 2021 00:36:38 GMT
ADD file:9246bf887411af1b286de95d779c11581dcef3c0d5a29e434162f0c085a7ce85 in / 
# Sat, 16 Oct 2021 00:36:44 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 01:34:00 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 16 Oct 2021 01:34:51 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:34:53 GMT
ENV GOSU_VERSION=1.13
# Sat, 16 Oct 2021 01:35:28 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 16 Oct 2021 01:35:36 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 16 Oct 2021 01:36:02 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:36:03 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 16 Oct 2021 01:36:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 16 Oct 2021 01:42:17 GMT
ARG MARIADB_MAJOR=10.4
# Sat, 16 Oct 2021 01:42:19 GMT
ENV MARIADB_MAJOR=10.4
# Sat, 16 Oct 2021 01:42:22 GMT
ARG MARIADB_VERSION=1:10.4.21+maria~focal
# Sat, 16 Oct 2021 01:42:25 GMT
ENV MARIADB_VERSION=1:10.4.21+maria~focal
# Sat, 16 Oct 2021 01:42:27 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
# Sat, 16 Oct 2021 01:42:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 16 Oct 2021 01:44:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 16 Oct 2021 01:44:36 GMT
VOLUME [/var/lib/mysql]
# Sat, 16 Oct 2021 01:44:42 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Sat, 16 Oct 2021 01:44:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 16 Oct 2021 01:44:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 01:45:02 GMT
EXPOSE 3306
# Sat, 16 Oct 2021 01:45:07 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:77ba7971d651af68e20e7cbb6603a3f7acd8ef2893066767a93db104723556f2`  
		Last Modified: Sat, 16 Oct 2021 00:38:38 GMT  
		Size: 33.3 MB (33287238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a9c5581eb228ed7e984fa7a4e62a7f8b2a068039fde3d32fa3b208026a189d`  
		Last Modified: Sat, 16 Oct 2021 01:49:31 GMT  
		Size: 1.8 KB (1761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63d968d5ad046645779be85243a3db326487bc8905dabf68bb063ea79e1662c1`  
		Last Modified: Sat, 16 Oct 2021 01:49:32 GMT  
		Size: 6.7 MB (6667970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5bdbddf0ed762c90ab4fcfe1f42007a96e4f90ca4f0765dfcec52213a3f5c12`  
		Last Modified: Sat, 16 Oct 2021 01:49:31 GMT  
		Size: 3.7 MB (3670760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00cc95e86fb5ab1bda9839a1ecbd3c2d607bc6cfc5155f33bf32c9d7827ec98b`  
		Last Modified: Sat, 16 Oct 2021 01:49:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe2cefdba07cb9fc803227a545d4fcc196038c1020de7698bf4e333d9056cbd`  
		Last Modified: Sat, 16 Oct 2021 01:49:28 GMT  
		Size: 2.6 MB (2573066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab77c7b0e7b171541e9f7f813ef81190ef39151aea54bfe2b64f8c191ce672c`  
		Last Modified: Sat, 16 Oct 2021 01:49:27 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e32cfb63425b3d801b33babc5bccf0ef736e4a9c7dd5e04fe577798daedc1634`  
		Last Modified: Sat, 16 Oct 2021 01:50:51 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb5c5072f86749780a8a81ebfe4aa7ca737f4f74bb3f6a69febc5eb2924e89cf`  
		Last Modified: Sat, 16 Oct 2021 01:51:09 GMT  
		Size: 89.3 MB (89254045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a45b7223486b0ec48518eefd709259162497aa7fa00c4ffd87b23d69b694143e`  
		Last Modified: Sat, 16 Oct 2021 01:50:51 GMT  
		Size: 5.6 KB (5612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89d460edc3fbc58f5e1daccef6ff69244bbed3674513cc88cc95a9b7ea0e4421`  
		Last Modified: Sat, 16 Oct 2021 01:50:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4-focal`

```console
$ docker pull mariadb@sha256:65cdad364df07770a0da7da4183a78fefdcb202e146e541ea51b515ab26588de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:439f7fa3d647ff354bd7b0883543ede691ab412d3cf722312f761de5116b728c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.7 MB (124740387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5f1527bdc85420e34baab9fa2467bc865342f43d0d11eb5b92c5b43063818a1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:07:51 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 16 Oct 2021 03:07:59 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:07:59 GMT
ENV GOSU_VERSION=1.13
# Sat, 16 Oct 2021 03:08:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 16 Oct 2021 03:08:11 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 16 Oct 2021 03:08:19 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:08:19 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 16 Oct 2021 03:08:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 16 Oct 2021 03:09:42 GMT
ARG MARIADB_MAJOR=10.4
# Sat, 16 Oct 2021 03:09:42 GMT
ENV MARIADB_MAJOR=10.4
# Sat, 16 Oct 2021 03:09:42 GMT
ARG MARIADB_VERSION=1:10.4.21+maria~focal
# Sat, 16 Oct 2021 03:09:42 GMT
ENV MARIADB_VERSION=1:10.4.21+maria~focal
# Sat, 16 Oct 2021 03:09:43 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
# Sat, 16 Oct 2021 03:09:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 16 Oct 2021 03:10:07 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 16 Oct 2021 03:10:08 GMT
VOLUME [/var/lib/mysql]
# Sat, 16 Oct 2021 03:10:08 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Sat, 16 Oct 2021 03:10:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 16 Oct 2021 03:10:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 03:10:10 GMT
EXPOSE 3306
# Sat, 16 Oct 2021 03:10:10 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:034655750c88e076cbd516354371b6176d01179bf595d928444e663ba1fa6845`  
		Last Modified: Sat, 16 Oct 2021 03:11:19 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b757a2a0f02848b1254cbd8b54e1d3cd4651228ede9a8c75e127f91cb415c4`  
		Last Modified: Sat, 16 Oct 2021 03:11:20 GMT  
		Size: 5.5 MB (5489306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c37daf8b6b55859dc1f92dbe017858ae03bd5bf503a3cdbf317b0b4387b1383`  
		Last Modified: Sat, 16 Oct 2021 03:11:19 GMT  
		Size: 3.6 MB (3582632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4cd9409b0f69a0ebe270f43c3a217f05b4c326e5d7c9a4ffb0cb7852ecddc81`  
		Last Modified: Sat, 16 Oct 2021 03:11:18 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbcda06785eb5474250fd32695909199c0de3375a06cf66401d277da518f3da9`  
		Last Modified: Sat, 16 Oct 2021 03:11:17 GMT  
		Size: 2.3 MB (2276882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34cd90f184c404cd4ecd88ebe612e6f180f76836efd3c24a329a3b812c5c345`  
		Last Modified: Sat, 16 Oct 2021 03:11:16 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6b213ac7f8a27abb0260723d8ab653adae1a5e6e1fa3c88d2d72e3823008a2a`  
		Last Modified: Sat, 16 Oct 2021 03:12:23 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac4568a963367b26c6c6c205b0cb775b5cf0812de8b44ba202309bbd7112592`  
		Last Modified: Sat, 16 Oct 2021 03:12:36 GMT  
		Size: 84.8 MB (84814009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5893a4f69042677decbadd989d4d1c7d3fb6f4fe92cc2986d6d26ac8ee8ceef`  
		Last Modified: Sat, 16 Oct 2021 03:12:23 GMT  
		Size: 5.6 KB (5613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d3849bbe75232c1320002f21633b2ae27d473117d5c43da4eee987fe3db34ae`  
		Last Modified: Sat, 16 Oct 2021 03:12:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:52d628b916bf43950ce0ce5632a623351eed6522f8e107a6eba6ea8963f37426
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.1 MB (122117980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7708994f226c0cefde734f08a20807dea8b65ba0ba73a751fcb7e1c29f89ac6b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:45:05 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 16 Oct 2021 03:45:15 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:45:15 GMT
ENV GOSU_VERSION=1.13
# Sat, 16 Oct 2021 03:45:29 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 16 Oct 2021 03:45:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 16 Oct 2021 03:45:37 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:45:37 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 16 Oct 2021 03:45:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 16 Oct 2021 03:47:14 GMT
ARG MARIADB_MAJOR=10.4
# Sat, 16 Oct 2021 03:47:15 GMT
ENV MARIADB_MAJOR=10.4
# Sat, 16 Oct 2021 03:47:16 GMT
ARG MARIADB_VERSION=1:10.4.21+maria~focal
# Sat, 16 Oct 2021 03:47:17 GMT
ENV MARIADB_VERSION=1:10.4.21+maria~focal
# Sat, 16 Oct 2021 03:47:18 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
# Sat, 16 Oct 2021 03:47:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 16 Oct 2021 03:47:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 16 Oct 2021 03:47:49 GMT
VOLUME [/var/lib/mysql]
# Sat, 16 Oct 2021 03:47:51 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Sat, 16 Oct 2021 03:47:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 16 Oct 2021 03:47:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 03:47:53 GMT
EXPOSE 3306
# Sat, 16 Oct 2021 03:47:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c05479159a3de34e1aedf676cd1a6793673b2e223d06a85c1caeab97e08c15`  
		Last Modified: Sat, 16 Oct 2021 03:51:12 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3fae4be7ce6b0048b0994bc5bd1e2d202fb383de08c3f2b82896678b35e8d1`  
		Last Modified: Sat, 16 Oct 2021 03:51:12 GMT  
		Size: 5.3 MB (5320781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8ca9913d50b67d55691860d8b19e4e38456f1142af47d6ebd4e933757fb2b6`  
		Last Modified: Sat, 16 Oct 2021 03:51:12 GMT  
		Size: 3.4 MB (3368038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffbd8ed1ed1586e00f393ee1417f3bf2b1d83f13c20a5035a050af97e29b9d09`  
		Last Modified: Sat, 16 Oct 2021 03:51:11 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48e61cde050f1f52a8b54730fab5e7bc4db2d6a6303e8fa2ef4eab107076a9ba`  
		Last Modified: Sat, 16 Oct 2021 03:51:09 GMT  
		Size: 2.2 MB (2207084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0b524648b0e80b14e489493c061f52515d6e5791c7f356da3be691507607ce`  
		Last Modified: Sat, 16 Oct 2021 03:51:09 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3dad55f85a67ac93ebeb8dad38d3c1c6500326134742d57fa9b76a98deb34ac`  
		Last Modified: Sat, 16 Oct 2021 03:52:24 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3097425ea97c6a8c8e3a11fcd692cf9b4acde246cc1dbee155184fdbf7e30d`  
		Last Modified: Sat, 16 Oct 2021 03:52:37 GMT  
		Size: 84.0 MB (84040811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b14d0cc23ba7e1016e58d13960b2d05c94a250584c8d2758d2506b03cef6ff`  
		Last Modified: Sat, 16 Oct 2021 03:52:24 GMT  
		Size: 5.6 KB (5611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce06bebf02092572d39ca9ee0adeca5b5967fb56f99c6391032c3f938b38bd83`  
		Last Modified: Sat, 16 Oct 2021 03:52:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:db23ae4a8dc88c4e06fcd477bd8ec87388a4acd0562e8f1baeb9c16cd2e3d3a2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.5 MB (135463544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3acf37940c7d117f6000c53a107c6013f52d57d70afb7a47a667ea880124344b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Oct 2021 00:36:38 GMT
ADD file:9246bf887411af1b286de95d779c11581dcef3c0d5a29e434162f0c085a7ce85 in / 
# Sat, 16 Oct 2021 00:36:44 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 01:34:00 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 16 Oct 2021 01:34:51 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:34:53 GMT
ENV GOSU_VERSION=1.13
# Sat, 16 Oct 2021 01:35:28 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 16 Oct 2021 01:35:36 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 16 Oct 2021 01:36:02 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:36:03 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 16 Oct 2021 01:36:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 16 Oct 2021 01:42:17 GMT
ARG MARIADB_MAJOR=10.4
# Sat, 16 Oct 2021 01:42:19 GMT
ENV MARIADB_MAJOR=10.4
# Sat, 16 Oct 2021 01:42:22 GMT
ARG MARIADB_VERSION=1:10.4.21+maria~focal
# Sat, 16 Oct 2021 01:42:25 GMT
ENV MARIADB_VERSION=1:10.4.21+maria~focal
# Sat, 16 Oct 2021 01:42:27 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
# Sat, 16 Oct 2021 01:42:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 16 Oct 2021 01:44:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 16 Oct 2021 01:44:36 GMT
VOLUME [/var/lib/mysql]
# Sat, 16 Oct 2021 01:44:42 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Sat, 16 Oct 2021 01:44:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.21/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 16 Oct 2021 01:44:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 01:45:02 GMT
EXPOSE 3306
# Sat, 16 Oct 2021 01:45:07 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:77ba7971d651af68e20e7cbb6603a3f7acd8ef2893066767a93db104723556f2`  
		Last Modified: Sat, 16 Oct 2021 00:38:38 GMT  
		Size: 33.3 MB (33287238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a9c5581eb228ed7e984fa7a4e62a7f8b2a068039fde3d32fa3b208026a189d`  
		Last Modified: Sat, 16 Oct 2021 01:49:31 GMT  
		Size: 1.8 KB (1761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63d968d5ad046645779be85243a3db326487bc8905dabf68bb063ea79e1662c1`  
		Last Modified: Sat, 16 Oct 2021 01:49:32 GMT  
		Size: 6.7 MB (6667970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5bdbddf0ed762c90ab4fcfe1f42007a96e4f90ca4f0765dfcec52213a3f5c12`  
		Last Modified: Sat, 16 Oct 2021 01:49:31 GMT  
		Size: 3.7 MB (3670760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00cc95e86fb5ab1bda9839a1ecbd3c2d607bc6cfc5155f33bf32c9d7827ec98b`  
		Last Modified: Sat, 16 Oct 2021 01:49:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe2cefdba07cb9fc803227a545d4fcc196038c1020de7698bf4e333d9056cbd`  
		Last Modified: Sat, 16 Oct 2021 01:49:28 GMT  
		Size: 2.6 MB (2573066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab77c7b0e7b171541e9f7f813ef81190ef39151aea54bfe2b64f8c191ce672c`  
		Last Modified: Sat, 16 Oct 2021 01:49:27 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e32cfb63425b3d801b33babc5bccf0ef736e4a9c7dd5e04fe577798daedc1634`  
		Last Modified: Sat, 16 Oct 2021 01:50:51 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb5c5072f86749780a8a81ebfe4aa7ca737f4f74bb3f6a69febc5eb2924e89cf`  
		Last Modified: Sat, 16 Oct 2021 01:51:09 GMT  
		Size: 89.3 MB (89254045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a45b7223486b0ec48518eefd709259162497aa7fa00c4ffd87b23d69b694143e`  
		Last Modified: Sat, 16 Oct 2021 01:50:51 GMT  
		Size: 5.6 KB (5612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89d460edc3fbc58f5e1daccef6ff69244bbed3674513cc88cc95a9b7ea0e4421`  
		Last Modified: Sat, 16 Oct 2021 01:50:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4.22`

**does not exist** (yet?)

## `mariadb:10.4.22-focal`

**does not exist** (yet?)

## `mariadb:10.5`

```console
$ docker pull mariadb@sha256:f0e9a95a715f5f1233f0513b6ccc83e2d5692cd787bc9425e11cef667cf086ec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.5` - linux; amd64

```console
$ docker pull mariadb@sha256:a5ebad8f03ea9352ccf1ec3c84d91c2112ba86bbface1b57091f37aa7899d6c9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.9 MB (126863845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a2e250ac49189e065785b9744b87ec79472c9fa20766aafd25af62a40953316`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:07:51 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 16 Oct 2021 03:07:59 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:07:59 GMT
ENV GOSU_VERSION=1.13
# Sat, 16 Oct 2021 03:08:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 16 Oct 2021 03:08:11 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 16 Oct 2021 03:08:19 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:08:19 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 16 Oct 2021 03:08:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 16 Oct 2021 03:09:13 GMT
ARG MARIADB_MAJOR=10.5
# Sat, 16 Oct 2021 03:09:13 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 16 Oct 2021 03:09:14 GMT
ARG MARIADB_VERSION=1:10.5.12+maria~focal
# Sat, 16 Oct 2021 03:09:14 GMT
ENV MARIADB_VERSION=1:10.5.12+maria~focal
# Sat, 16 Oct 2021 03:09:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
# Sat, 16 Oct 2021 03:09:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 16 Oct 2021 03:09:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 16 Oct 2021 03:09:38 GMT
VOLUME [/var/lib/mysql]
# Sat, 16 Oct 2021 03:09:39 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Sat, 16 Oct 2021 03:09:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 03:09:39 GMT
EXPOSE 3306
# Sat, 16 Oct 2021 03:09:39 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:034655750c88e076cbd516354371b6176d01179bf595d928444e663ba1fa6845`  
		Last Modified: Sat, 16 Oct 2021 03:11:19 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b757a2a0f02848b1254cbd8b54e1d3cd4651228ede9a8c75e127f91cb415c4`  
		Last Modified: Sat, 16 Oct 2021 03:11:20 GMT  
		Size: 5.5 MB (5489306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c37daf8b6b55859dc1f92dbe017858ae03bd5bf503a3cdbf317b0b4387b1383`  
		Last Modified: Sat, 16 Oct 2021 03:11:19 GMT  
		Size: 3.6 MB (3582632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4cd9409b0f69a0ebe270f43c3a217f05b4c326e5d7c9a4ffb0cb7852ecddc81`  
		Last Modified: Sat, 16 Oct 2021 03:11:18 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbcda06785eb5474250fd32695909199c0de3375a06cf66401d277da518f3da9`  
		Last Modified: Sat, 16 Oct 2021 03:11:17 GMT  
		Size: 2.3 MB (2276882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34cd90f184c404cd4ecd88ebe612e6f180f76836efd3c24a329a3b812c5c345`  
		Last Modified: Sat, 16 Oct 2021 03:11:16 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cb5c0007d2fe89812d4cab07fd14f2180576945a7f84eb9723a1eeb62b4f983`  
		Last Modified: Sat, 16 Oct 2021 03:11:55 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4047e305dff1b8644f8f4e095c1b7394bf5fe9fc439f0959684843c2126a80e`  
		Last Modified: Sat, 16 Oct 2021 03:12:08 GMT  
		Size: 86.9 MB (86937589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c06a7a5e1d44c26cd13b9ee12e04ddfc816bd24b95fbcea9a99ec9a3bce27b`  
		Last Modified: Sat, 16 Oct 2021 03:11:55 GMT  
		Size: 5.6 KB (5613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:5d7ae1ffed53e6531aa0fb9ddb63d1362807cbd4a7d54c01224ca7c7e7cdf5c6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.2 MB (124176932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0242d993b4d4a83d1c97258f477e78652669739adbd76a6d69e0fdac42901c1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:45:05 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 16 Oct 2021 03:45:15 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:45:15 GMT
ENV GOSU_VERSION=1.13
# Sat, 16 Oct 2021 03:45:29 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 16 Oct 2021 03:45:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 16 Oct 2021 03:45:37 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:45:37 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 16 Oct 2021 03:45:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 16 Oct 2021 03:46:31 GMT
ARG MARIADB_MAJOR=10.5
# Sat, 16 Oct 2021 03:46:31 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 16 Oct 2021 03:46:32 GMT
ARG MARIADB_VERSION=1:10.5.12+maria~focal
# Sat, 16 Oct 2021 03:46:33 GMT
ENV MARIADB_VERSION=1:10.5.12+maria~focal
# Sat, 16 Oct 2021 03:46:34 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
# Sat, 16 Oct 2021 03:46:35 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 16 Oct 2021 03:47:01 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 16 Oct 2021 03:47:02 GMT
VOLUME [/var/lib/mysql]
# Sat, 16 Oct 2021 03:47:03 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Sat, 16 Oct 2021 03:47:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 03:47:04 GMT
EXPOSE 3306
# Sat, 16 Oct 2021 03:47:05 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c05479159a3de34e1aedf676cd1a6793673b2e223d06a85c1caeab97e08c15`  
		Last Modified: Sat, 16 Oct 2021 03:51:12 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3fae4be7ce6b0048b0994bc5bd1e2d202fb383de08c3f2b82896678b35e8d1`  
		Last Modified: Sat, 16 Oct 2021 03:51:12 GMT  
		Size: 5.3 MB (5320781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8ca9913d50b67d55691860d8b19e4e38456f1142af47d6ebd4e933757fb2b6`  
		Last Modified: Sat, 16 Oct 2021 03:51:12 GMT  
		Size: 3.4 MB (3368038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffbd8ed1ed1586e00f393ee1417f3bf2b1d83f13c20a5035a050af97e29b9d09`  
		Last Modified: Sat, 16 Oct 2021 03:51:11 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48e61cde050f1f52a8b54730fab5e7bc4db2d6a6303e8fa2ef4eab107076a9ba`  
		Last Modified: Sat, 16 Oct 2021 03:51:09 GMT  
		Size: 2.2 MB (2207084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0b524648b0e80b14e489493c061f52515d6e5791c7f356da3be691507607ce`  
		Last Modified: Sat, 16 Oct 2021 03:51:09 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4421aafc4bd3436ba25f6032d603338713d5fd3f4f9302121aedda7dfe79f45`  
		Last Modified: Sat, 16 Oct 2021 03:51:54 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:285fe8e564567de7094996713252296e8452a75d7658bb0dacd90829a0ef939c`  
		Last Modified: Sat, 16 Oct 2021 03:52:08 GMT  
		Size: 86.1 MB (86099886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39261fd21fcbcb21e50326a01037fc758fd7e1671b02d6f5589520bea7fb0c16`  
		Last Modified: Sat, 16 Oct 2021 03:51:54 GMT  
		Size: 5.6 KB (5609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; ppc64le

```console
$ docker pull mariadb@sha256:4f8d9dd96a6dbef3deb6138d39cfc38f8d0277a783db2e39a34d7a054b674684
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.6 MB (137580279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ea3573cf742f38dedaa04d69169803bfa123f2c4d59e9b3c0c592ab22381be5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Oct 2021 00:36:38 GMT
ADD file:9246bf887411af1b286de95d779c11581dcef3c0d5a29e434162f0c085a7ce85 in / 
# Sat, 16 Oct 2021 00:36:44 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 01:34:00 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 16 Oct 2021 01:34:51 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:34:53 GMT
ENV GOSU_VERSION=1.13
# Sat, 16 Oct 2021 01:35:28 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 16 Oct 2021 01:35:36 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 16 Oct 2021 01:36:02 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:36:03 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 16 Oct 2021 01:36:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 16 Oct 2021 01:39:39 GMT
ARG MARIADB_MAJOR=10.5
# Sat, 16 Oct 2021 01:39:42 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 16 Oct 2021 01:39:45 GMT
ARG MARIADB_VERSION=1:10.5.12+maria~focal
# Sat, 16 Oct 2021 01:39:47 GMT
ENV MARIADB_VERSION=1:10.5.12+maria~focal
# Sat, 16 Oct 2021 01:39:49 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
# Sat, 16 Oct 2021 01:39:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 16 Oct 2021 01:41:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 16 Oct 2021 01:41:52 GMT
VOLUME [/var/lib/mysql]
# Sat, 16 Oct 2021 01:41:54 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Sat, 16 Oct 2021 01:41:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 01:42:00 GMT
EXPOSE 3306
# Sat, 16 Oct 2021 01:42:03 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:77ba7971d651af68e20e7cbb6603a3f7acd8ef2893066767a93db104723556f2`  
		Last Modified: Sat, 16 Oct 2021 00:38:38 GMT  
		Size: 33.3 MB (33287238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a9c5581eb228ed7e984fa7a4e62a7f8b2a068039fde3d32fa3b208026a189d`  
		Last Modified: Sat, 16 Oct 2021 01:49:31 GMT  
		Size: 1.8 KB (1761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63d968d5ad046645779be85243a3db326487bc8905dabf68bb063ea79e1662c1`  
		Last Modified: Sat, 16 Oct 2021 01:49:32 GMT  
		Size: 6.7 MB (6667970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5bdbddf0ed762c90ab4fcfe1f42007a96e4f90ca4f0765dfcec52213a3f5c12`  
		Last Modified: Sat, 16 Oct 2021 01:49:31 GMT  
		Size: 3.7 MB (3670760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00cc95e86fb5ab1bda9839a1ecbd3c2d607bc6cfc5155f33bf32c9d7827ec98b`  
		Last Modified: Sat, 16 Oct 2021 01:49:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe2cefdba07cb9fc803227a545d4fcc196038c1020de7698bf4e333d9056cbd`  
		Last Modified: Sat, 16 Oct 2021 01:49:28 GMT  
		Size: 2.6 MB (2573066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab77c7b0e7b171541e9f7f813ef81190ef39151aea54bfe2b64f8c191ce672c`  
		Last Modified: Sat, 16 Oct 2021 01:49:27 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec67cba87144a745f61e6d90badf06dd6518c512a3b7a067623cdeb4b9cec79`  
		Last Modified: Sat, 16 Oct 2021 01:50:16 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:def963c9f47e8420d77e6cd15e6dc91a13dd6a6505af461e51c341d383391007`  
		Last Modified: Sat, 16 Oct 2021 01:50:34 GMT  
		Size: 91.4 MB (91370902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec1682d32f1d61eec73e062f876c8ea7b60b2bbd1ca6c8517026f735a72bf88`  
		Last Modified: Sat, 16 Oct 2021 01:50:16 GMT  
		Size: 5.6 KB (5611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; s390x

```console
$ docker pull mariadb@sha256:7f7a7b0832e1b134a141c55274c96532dd995cc1ae0e963b6a928dc890847d2b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.0 MB (126048014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f672fd796e85e5a330f1f56ebd53ff3b67f962c269decf39128ae22f9ab408f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Oct 2021 00:41:46 GMT
ADD file:cf3b6f9c395392eaf2c629969f59c48cde60ae1c74c3dbb13886481999a7a4d5 in / 
# Sat, 16 Oct 2021 00:41:48 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 01:02:36 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 16 Oct 2021 01:02:41 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:02:42 GMT
ENV GOSU_VERSION=1.13
# Sat, 16 Oct 2021 01:02:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 16 Oct 2021 01:02:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 16 Oct 2021 01:02:55 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:02:55 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 16 Oct 2021 01:03:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 16 Oct 2021 01:03:35 GMT
ARG MARIADB_MAJOR=10.5
# Sat, 16 Oct 2021 01:03:35 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 16 Oct 2021 01:03:35 GMT
ARG MARIADB_VERSION=1:10.5.12+maria~focal
# Sat, 16 Oct 2021 01:03:35 GMT
ENV MARIADB_VERSION=1:10.5.12+maria~focal
# Sat, 16 Oct 2021 01:03:35 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
# Sat, 16 Oct 2021 01:03:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 16 Oct 2021 01:03:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 16 Oct 2021 01:03:58 GMT
VOLUME [/var/lib/mysql]
# Sat, 16 Oct 2021 01:03:58 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Sat, 16 Oct 2021 01:03:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 01:03:58 GMT
EXPOSE 3306
# Sat, 16 Oct 2021 01:03:58 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:1f0267805ccac7499fadaabf65e52d4564add2bc20ed25bcf77df24d8debb103`  
		Last Modified: Sat, 16 Oct 2021 00:42:57 GMT  
		Size: 27.1 MB (27120856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcc30a1fd200d10ce23e934b30e72d36ea131fb670d30afe697304591986fe1`  
		Last Modified: Sat, 16 Oct 2021 01:04:32 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:228a3fc0a9531bf3e9e08d9800daffbe33729ba8a16fb427b07a1a36fb047e02`  
		Last Modified: Sat, 16 Oct 2021 01:04:32 GMT  
		Size: 5.4 MB (5380980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e511a129710d7aa78451eebec778e60a256b2a9e60db59a9f6d09641bd4f96`  
		Last Modified: Sat, 16 Oct 2021 01:04:32 GMT  
		Size: 3.2 MB (3239822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a9cf411b6c206dca4cd2f493440c36781e332782682bb40969b6640e8e98e9`  
		Last Modified: Sat, 16 Oct 2021 01:04:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cac3f3cdb186c64fce6e0a7efc39abe96d0e6ab755d9193c981cc44c801cc51`  
		Last Modified: Sat, 16 Oct 2021 01:04:31 GMT  
		Size: 2.2 MB (2188905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd5f55dd4f1666fe90f4ca1b3b0cc36a9092c44ae19033a4d2b7b0e2ff3dddb`  
		Last Modified: Sat, 16 Oct 2021 01:04:30 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba27885bcb0e790f7990ad6b69669737ee44b5902deec85e48298b05b09835c`  
		Last Modified: Sat, 16 Oct 2021 01:05:06 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4814429007deb3858bf50326ba8c969e2a7b313c61ad7c5c387ed893d9d1f743`  
		Last Modified: Sat, 16 Oct 2021 01:05:18 GMT  
		Size: 88.1 MB (88107119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0aac5e8a79c251782a156851ac4e82652f50218e26b06c096f762d33782377c`  
		Last Modified: Sat, 16 Oct 2021 01:05:06 GMT  
		Size: 5.6 KB (5610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5-focal`

```console
$ docker pull mariadb@sha256:f0e9a95a715f5f1233f0513b6ccc83e2d5692cd787bc9425e11cef667cf086ec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.5-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:a5ebad8f03ea9352ccf1ec3c84d91c2112ba86bbface1b57091f37aa7899d6c9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.9 MB (126863845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a2e250ac49189e065785b9744b87ec79472c9fa20766aafd25af62a40953316`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:07:51 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 16 Oct 2021 03:07:59 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:07:59 GMT
ENV GOSU_VERSION=1.13
# Sat, 16 Oct 2021 03:08:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 16 Oct 2021 03:08:11 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 16 Oct 2021 03:08:19 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:08:19 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 16 Oct 2021 03:08:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 16 Oct 2021 03:09:13 GMT
ARG MARIADB_MAJOR=10.5
# Sat, 16 Oct 2021 03:09:13 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 16 Oct 2021 03:09:14 GMT
ARG MARIADB_VERSION=1:10.5.12+maria~focal
# Sat, 16 Oct 2021 03:09:14 GMT
ENV MARIADB_VERSION=1:10.5.12+maria~focal
# Sat, 16 Oct 2021 03:09:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
# Sat, 16 Oct 2021 03:09:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 16 Oct 2021 03:09:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 16 Oct 2021 03:09:38 GMT
VOLUME [/var/lib/mysql]
# Sat, 16 Oct 2021 03:09:39 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Sat, 16 Oct 2021 03:09:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 03:09:39 GMT
EXPOSE 3306
# Sat, 16 Oct 2021 03:09:39 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:034655750c88e076cbd516354371b6176d01179bf595d928444e663ba1fa6845`  
		Last Modified: Sat, 16 Oct 2021 03:11:19 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b757a2a0f02848b1254cbd8b54e1d3cd4651228ede9a8c75e127f91cb415c4`  
		Last Modified: Sat, 16 Oct 2021 03:11:20 GMT  
		Size: 5.5 MB (5489306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c37daf8b6b55859dc1f92dbe017858ae03bd5bf503a3cdbf317b0b4387b1383`  
		Last Modified: Sat, 16 Oct 2021 03:11:19 GMT  
		Size: 3.6 MB (3582632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4cd9409b0f69a0ebe270f43c3a217f05b4c326e5d7c9a4ffb0cb7852ecddc81`  
		Last Modified: Sat, 16 Oct 2021 03:11:18 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbcda06785eb5474250fd32695909199c0de3375a06cf66401d277da518f3da9`  
		Last Modified: Sat, 16 Oct 2021 03:11:17 GMT  
		Size: 2.3 MB (2276882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34cd90f184c404cd4ecd88ebe612e6f180f76836efd3c24a329a3b812c5c345`  
		Last Modified: Sat, 16 Oct 2021 03:11:16 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cb5c0007d2fe89812d4cab07fd14f2180576945a7f84eb9723a1eeb62b4f983`  
		Last Modified: Sat, 16 Oct 2021 03:11:55 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4047e305dff1b8644f8f4e095c1b7394bf5fe9fc439f0959684843c2126a80e`  
		Last Modified: Sat, 16 Oct 2021 03:12:08 GMT  
		Size: 86.9 MB (86937589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c06a7a5e1d44c26cd13b9ee12e04ddfc816bd24b95fbcea9a99ec9a3bce27b`  
		Last Modified: Sat, 16 Oct 2021 03:11:55 GMT  
		Size: 5.6 KB (5613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:5d7ae1ffed53e6531aa0fb9ddb63d1362807cbd4a7d54c01224ca7c7e7cdf5c6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.2 MB (124176932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0242d993b4d4a83d1c97258f477e78652669739adbd76a6d69e0fdac42901c1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:45:05 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 16 Oct 2021 03:45:15 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:45:15 GMT
ENV GOSU_VERSION=1.13
# Sat, 16 Oct 2021 03:45:29 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 16 Oct 2021 03:45:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 16 Oct 2021 03:45:37 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:45:37 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 16 Oct 2021 03:45:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 16 Oct 2021 03:46:31 GMT
ARG MARIADB_MAJOR=10.5
# Sat, 16 Oct 2021 03:46:31 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 16 Oct 2021 03:46:32 GMT
ARG MARIADB_VERSION=1:10.5.12+maria~focal
# Sat, 16 Oct 2021 03:46:33 GMT
ENV MARIADB_VERSION=1:10.5.12+maria~focal
# Sat, 16 Oct 2021 03:46:34 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
# Sat, 16 Oct 2021 03:46:35 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 16 Oct 2021 03:47:01 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 16 Oct 2021 03:47:02 GMT
VOLUME [/var/lib/mysql]
# Sat, 16 Oct 2021 03:47:03 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Sat, 16 Oct 2021 03:47:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 03:47:04 GMT
EXPOSE 3306
# Sat, 16 Oct 2021 03:47:05 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c05479159a3de34e1aedf676cd1a6793673b2e223d06a85c1caeab97e08c15`  
		Last Modified: Sat, 16 Oct 2021 03:51:12 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3fae4be7ce6b0048b0994bc5bd1e2d202fb383de08c3f2b82896678b35e8d1`  
		Last Modified: Sat, 16 Oct 2021 03:51:12 GMT  
		Size: 5.3 MB (5320781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8ca9913d50b67d55691860d8b19e4e38456f1142af47d6ebd4e933757fb2b6`  
		Last Modified: Sat, 16 Oct 2021 03:51:12 GMT  
		Size: 3.4 MB (3368038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffbd8ed1ed1586e00f393ee1417f3bf2b1d83f13c20a5035a050af97e29b9d09`  
		Last Modified: Sat, 16 Oct 2021 03:51:11 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48e61cde050f1f52a8b54730fab5e7bc4db2d6a6303e8fa2ef4eab107076a9ba`  
		Last Modified: Sat, 16 Oct 2021 03:51:09 GMT  
		Size: 2.2 MB (2207084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0b524648b0e80b14e489493c061f52515d6e5791c7f356da3be691507607ce`  
		Last Modified: Sat, 16 Oct 2021 03:51:09 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4421aafc4bd3436ba25f6032d603338713d5fd3f4f9302121aedda7dfe79f45`  
		Last Modified: Sat, 16 Oct 2021 03:51:54 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:285fe8e564567de7094996713252296e8452a75d7658bb0dacd90829a0ef939c`  
		Last Modified: Sat, 16 Oct 2021 03:52:08 GMT  
		Size: 86.1 MB (86099886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39261fd21fcbcb21e50326a01037fc758fd7e1671b02d6f5589520bea7fb0c16`  
		Last Modified: Sat, 16 Oct 2021 03:51:54 GMT  
		Size: 5.6 KB (5609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:4f8d9dd96a6dbef3deb6138d39cfc38f8d0277a783db2e39a34d7a054b674684
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.6 MB (137580279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ea3573cf742f38dedaa04d69169803bfa123f2c4d59e9b3c0c592ab22381be5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Oct 2021 00:36:38 GMT
ADD file:9246bf887411af1b286de95d779c11581dcef3c0d5a29e434162f0c085a7ce85 in / 
# Sat, 16 Oct 2021 00:36:44 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 01:34:00 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 16 Oct 2021 01:34:51 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:34:53 GMT
ENV GOSU_VERSION=1.13
# Sat, 16 Oct 2021 01:35:28 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 16 Oct 2021 01:35:36 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 16 Oct 2021 01:36:02 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:36:03 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 16 Oct 2021 01:36:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 16 Oct 2021 01:39:39 GMT
ARG MARIADB_MAJOR=10.5
# Sat, 16 Oct 2021 01:39:42 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 16 Oct 2021 01:39:45 GMT
ARG MARIADB_VERSION=1:10.5.12+maria~focal
# Sat, 16 Oct 2021 01:39:47 GMT
ENV MARIADB_VERSION=1:10.5.12+maria~focal
# Sat, 16 Oct 2021 01:39:49 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
# Sat, 16 Oct 2021 01:39:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 16 Oct 2021 01:41:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 16 Oct 2021 01:41:52 GMT
VOLUME [/var/lib/mysql]
# Sat, 16 Oct 2021 01:41:54 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Sat, 16 Oct 2021 01:41:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 01:42:00 GMT
EXPOSE 3306
# Sat, 16 Oct 2021 01:42:03 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:77ba7971d651af68e20e7cbb6603a3f7acd8ef2893066767a93db104723556f2`  
		Last Modified: Sat, 16 Oct 2021 00:38:38 GMT  
		Size: 33.3 MB (33287238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a9c5581eb228ed7e984fa7a4e62a7f8b2a068039fde3d32fa3b208026a189d`  
		Last Modified: Sat, 16 Oct 2021 01:49:31 GMT  
		Size: 1.8 KB (1761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63d968d5ad046645779be85243a3db326487bc8905dabf68bb063ea79e1662c1`  
		Last Modified: Sat, 16 Oct 2021 01:49:32 GMT  
		Size: 6.7 MB (6667970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5bdbddf0ed762c90ab4fcfe1f42007a96e4f90ca4f0765dfcec52213a3f5c12`  
		Last Modified: Sat, 16 Oct 2021 01:49:31 GMT  
		Size: 3.7 MB (3670760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00cc95e86fb5ab1bda9839a1ecbd3c2d607bc6cfc5155f33bf32c9d7827ec98b`  
		Last Modified: Sat, 16 Oct 2021 01:49:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe2cefdba07cb9fc803227a545d4fcc196038c1020de7698bf4e333d9056cbd`  
		Last Modified: Sat, 16 Oct 2021 01:49:28 GMT  
		Size: 2.6 MB (2573066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab77c7b0e7b171541e9f7f813ef81190ef39151aea54bfe2b64f8c191ce672c`  
		Last Modified: Sat, 16 Oct 2021 01:49:27 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec67cba87144a745f61e6d90badf06dd6518c512a3b7a067623cdeb4b9cec79`  
		Last Modified: Sat, 16 Oct 2021 01:50:16 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:def963c9f47e8420d77e6cd15e6dc91a13dd6a6505af461e51c341d383391007`  
		Last Modified: Sat, 16 Oct 2021 01:50:34 GMT  
		Size: 91.4 MB (91370902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec1682d32f1d61eec73e062f876c8ea7b60b2bbd1ca6c8517026f735a72bf88`  
		Last Modified: Sat, 16 Oct 2021 01:50:16 GMT  
		Size: 5.6 KB (5611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:7f7a7b0832e1b134a141c55274c96532dd995cc1ae0e963b6a928dc890847d2b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.0 MB (126048014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f672fd796e85e5a330f1f56ebd53ff3b67f962c269decf39128ae22f9ab408f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Oct 2021 00:41:46 GMT
ADD file:cf3b6f9c395392eaf2c629969f59c48cde60ae1c74c3dbb13886481999a7a4d5 in / 
# Sat, 16 Oct 2021 00:41:48 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 01:02:36 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 16 Oct 2021 01:02:41 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:02:42 GMT
ENV GOSU_VERSION=1.13
# Sat, 16 Oct 2021 01:02:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 16 Oct 2021 01:02:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 16 Oct 2021 01:02:55 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:02:55 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 16 Oct 2021 01:03:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 16 Oct 2021 01:03:35 GMT
ARG MARIADB_MAJOR=10.5
# Sat, 16 Oct 2021 01:03:35 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 16 Oct 2021 01:03:35 GMT
ARG MARIADB_VERSION=1:10.5.12+maria~focal
# Sat, 16 Oct 2021 01:03:35 GMT
ENV MARIADB_VERSION=1:10.5.12+maria~focal
# Sat, 16 Oct 2021 01:03:35 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
# Sat, 16 Oct 2021 01:03:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 16 Oct 2021 01:03:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.12/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 16 Oct 2021 01:03:58 GMT
VOLUME [/var/lib/mysql]
# Sat, 16 Oct 2021 01:03:58 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Sat, 16 Oct 2021 01:03:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 01:03:58 GMT
EXPOSE 3306
# Sat, 16 Oct 2021 01:03:58 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:1f0267805ccac7499fadaabf65e52d4564add2bc20ed25bcf77df24d8debb103`  
		Last Modified: Sat, 16 Oct 2021 00:42:57 GMT  
		Size: 27.1 MB (27120856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcc30a1fd200d10ce23e934b30e72d36ea131fb670d30afe697304591986fe1`  
		Last Modified: Sat, 16 Oct 2021 01:04:32 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:228a3fc0a9531bf3e9e08d9800daffbe33729ba8a16fb427b07a1a36fb047e02`  
		Last Modified: Sat, 16 Oct 2021 01:04:32 GMT  
		Size: 5.4 MB (5380980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e511a129710d7aa78451eebec778e60a256b2a9e60db59a9f6d09641bd4f96`  
		Last Modified: Sat, 16 Oct 2021 01:04:32 GMT  
		Size: 3.2 MB (3239822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a9cf411b6c206dca4cd2f493440c36781e332782682bb40969b6640e8e98e9`  
		Last Modified: Sat, 16 Oct 2021 01:04:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cac3f3cdb186c64fce6e0a7efc39abe96d0e6ab755d9193c981cc44c801cc51`  
		Last Modified: Sat, 16 Oct 2021 01:04:31 GMT  
		Size: 2.2 MB (2188905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd5f55dd4f1666fe90f4ca1b3b0cc36a9092c44ae19033a4d2b7b0e2ff3dddb`  
		Last Modified: Sat, 16 Oct 2021 01:04:30 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba27885bcb0e790f7990ad6b69669737ee44b5902deec85e48298b05b09835c`  
		Last Modified: Sat, 16 Oct 2021 01:05:06 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4814429007deb3858bf50326ba8c969e2a7b313c61ad7c5c387ed893d9d1f743`  
		Last Modified: Sat, 16 Oct 2021 01:05:18 GMT  
		Size: 88.1 MB (88107119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0aac5e8a79c251782a156851ac4e82652f50218e26b06c096f762d33782377c`  
		Last Modified: Sat, 16 Oct 2021 01:05:06 GMT  
		Size: 5.6 KB (5610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5.13`

**does not exist** (yet?)

## `mariadb:10.5.13-focal`

**does not exist** (yet?)

## `mariadb:10.6`

```console
$ docker pull mariadb@sha256:c014ba1efc5dbd711d0520c7762d57807f35549de3414eb31e942a420c8a2ed2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.6` - linux; amd64

```console
$ docker pull mariadb@sha256:dd08274a61f912b78facb7d144f898c0fd53da4f0c2fcf8ea80cd05f22577221
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.0 MB (127016059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12e05d5da3c5223e9877e8eb90d68560ff66cedcb955131061d60d093a908f0c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:07:51 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 16 Oct 2021 03:07:59 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:07:59 GMT
ENV GOSU_VERSION=1.13
# Sat, 16 Oct 2021 03:08:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 16 Oct 2021 03:08:11 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 16 Oct 2021 03:08:19 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:08:19 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 16 Oct 2021 03:08:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 16 Oct 2021 03:08:27 GMT
ARG MARIADB_MAJOR=10.6
# Sat, 16 Oct 2021 03:08:27 GMT
ENV MARIADB_MAJOR=10.6
# Sat, 16 Oct 2021 03:08:27 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Sat, 16 Oct 2021 03:08:27 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Sat, 16 Oct 2021 03:08:27 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Sat, 16 Oct 2021 03:08:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 16 Oct 2021 03:09:01 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 16 Oct 2021 03:09:02 GMT
VOLUME [/var/lib/mysql]
# Sat, 16 Oct 2021 03:09:02 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Sat, 16 Oct 2021 03:09:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 03:09:02 GMT
EXPOSE 3306
# Sat, 16 Oct 2021 03:09:02 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:034655750c88e076cbd516354371b6176d01179bf595d928444e663ba1fa6845`  
		Last Modified: Sat, 16 Oct 2021 03:11:19 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b757a2a0f02848b1254cbd8b54e1d3cd4651228ede9a8c75e127f91cb415c4`  
		Last Modified: Sat, 16 Oct 2021 03:11:20 GMT  
		Size: 5.5 MB (5489306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c37daf8b6b55859dc1f92dbe017858ae03bd5bf503a3cdbf317b0b4387b1383`  
		Last Modified: Sat, 16 Oct 2021 03:11:19 GMT  
		Size: 3.6 MB (3582632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4cd9409b0f69a0ebe270f43c3a217f05b4c326e5d7c9a4ffb0cb7852ecddc81`  
		Last Modified: Sat, 16 Oct 2021 03:11:18 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbcda06785eb5474250fd32695909199c0de3375a06cf66401d277da518f3da9`  
		Last Modified: Sat, 16 Oct 2021 03:11:17 GMT  
		Size: 2.3 MB (2276882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34cd90f184c404cd4ecd88ebe612e6f180f76836efd3c24a329a3b812c5c345`  
		Last Modified: Sat, 16 Oct 2021 03:11:16 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd6cef4ce4896ed34f82cdec0226170c9ec12e780095f39a268e4f4cd87be523`  
		Last Modified: Sat, 16 Oct 2021 03:11:16 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cb89a1550ea4efead895dec48626ae277912ca9eeffae1a3c1b8c3f0f9ed02d`  
		Last Modified: Sat, 16 Oct 2021 03:11:29 GMT  
		Size: 87.1 MB (87089805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df9f153bd93044efcf8d9cd1ea5266b32bf28df2ad72e5ce195428e8c81b917b`  
		Last Modified: Sat, 16 Oct 2021 03:11:16 GMT  
		Size: 5.6 KB (5611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:52b21e64bd048fb93b8a3ac5d36eaf3027bd5a7b1c71e833bc8ac0aa1c98c72b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.2 MB (124173665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6819e5d163d1d24d896d090e1f55c38bcb9e55db811196e3919f0707a86eff03`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:45:05 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 16 Oct 2021 03:45:15 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:45:15 GMT
ENV GOSU_VERSION=1.13
# Sat, 16 Oct 2021 03:45:29 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 16 Oct 2021 03:45:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 16 Oct 2021 03:45:37 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:45:37 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 16 Oct 2021 03:45:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 16 Oct 2021 03:45:42 GMT
ARG MARIADB_MAJOR=10.6
# Sat, 16 Oct 2021 03:45:43 GMT
ENV MARIADB_MAJOR=10.6
# Sat, 16 Oct 2021 03:45:44 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Sat, 16 Oct 2021 03:45:45 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Sat, 16 Oct 2021 03:45:46 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Sat, 16 Oct 2021 03:45:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 16 Oct 2021 03:46:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 16 Oct 2021 03:46:17 GMT
VOLUME [/var/lib/mysql]
# Sat, 16 Oct 2021 03:46:19 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Sat, 16 Oct 2021 03:46:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 03:46:20 GMT
EXPOSE 3306
# Sat, 16 Oct 2021 03:46:21 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c05479159a3de34e1aedf676cd1a6793673b2e223d06a85c1caeab97e08c15`  
		Last Modified: Sat, 16 Oct 2021 03:51:12 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3fae4be7ce6b0048b0994bc5bd1e2d202fb383de08c3f2b82896678b35e8d1`  
		Last Modified: Sat, 16 Oct 2021 03:51:12 GMT  
		Size: 5.3 MB (5320781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8ca9913d50b67d55691860d8b19e4e38456f1142af47d6ebd4e933757fb2b6`  
		Last Modified: Sat, 16 Oct 2021 03:51:12 GMT  
		Size: 3.4 MB (3368038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffbd8ed1ed1586e00f393ee1417f3bf2b1d83f13c20a5035a050af97e29b9d09`  
		Last Modified: Sat, 16 Oct 2021 03:51:11 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48e61cde050f1f52a8b54730fab5e7bc4db2d6a6303e8fa2ef4eab107076a9ba`  
		Last Modified: Sat, 16 Oct 2021 03:51:09 GMT  
		Size: 2.2 MB (2207084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0b524648b0e80b14e489493c061f52515d6e5791c7f356da3be691507607ce`  
		Last Modified: Sat, 16 Oct 2021 03:51:09 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a7bc5ea6462e7abeb995a46808ebc6c2f6d5afc6361c367235fc02909f95ff`  
		Last Modified: Sat, 16 Oct 2021 03:51:09 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70ea7fb2288eb8ce16b25989a901e5f6bc945315a86d749685f03dabde2bce5`  
		Last Modified: Sat, 16 Oct 2021 03:51:22 GMT  
		Size: 86.1 MB (86096615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:968494f5cebc0a5862440af69b49d4a863460de158a94c0f339b19d08ccf4ab6`  
		Last Modified: Sat, 16 Oct 2021 03:51:09 GMT  
		Size: 5.6 KB (5613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6` - linux; ppc64le

```console
$ docker pull mariadb@sha256:aa3c316f88dd9537eeaa7201d6d3c5f8d8732196ee6c9cd5ce553816c7a060d9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137539722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a66b6be1b40e577fe733ec92528cf73ee97a8536e1fcddc9fe638aa9132f8173`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Oct 2021 00:36:38 GMT
ADD file:9246bf887411af1b286de95d779c11581dcef3c0d5a29e434162f0c085a7ce85 in / 
# Sat, 16 Oct 2021 00:36:44 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 01:34:00 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 16 Oct 2021 01:34:51 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:34:53 GMT
ENV GOSU_VERSION=1.13
# Sat, 16 Oct 2021 01:35:28 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 16 Oct 2021 01:35:36 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 16 Oct 2021 01:36:02 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:36:03 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 16 Oct 2021 01:36:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 16 Oct 2021 01:36:18 GMT
ARG MARIADB_MAJOR=10.6
# Sat, 16 Oct 2021 01:36:19 GMT
ENV MARIADB_MAJOR=10.6
# Sat, 16 Oct 2021 01:36:22 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Sat, 16 Oct 2021 01:36:24 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Sat, 16 Oct 2021 01:36:29 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Sat, 16 Oct 2021 01:36:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 16 Oct 2021 01:38:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 16 Oct 2021 01:39:01 GMT
VOLUME [/var/lib/mysql]
# Sat, 16 Oct 2021 01:39:03 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Sat, 16 Oct 2021 01:39:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 01:39:08 GMT
EXPOSE 3306
# Sat, 16 Oct 2021 01:39:15 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:77ba7971d651af68e20e7cbb6603a3f7acd8ef2893066767a93db104723556f2`  
		Last Modified: Sat, 16 Oct 2021 00:38:38 GMT  
		Size: 33.3 MB (33287238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a9c5581eb228ed7e984fa7a4e62a7f8b2a068039fde3d32fa3b208026a189d`  
		Last Modified: Sat, 16 Oct 2021 01:49:31 GMT  
		Size: 1.8 KB (1761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63d968d5ad046645779be85243a3db326487bc8905dabf68bb063ea79e1662c1`  
		Last Modified: Sat, 16 Oct 2021 01:49:32 GMT  
		Size: 6.7 MB (6667970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5bdbddf0ed762c90ab4fcfe1f42007a96e4f90ca4f0765dfcec52213a3f5c12`  
		Last Modified: Sat, 16 Oct 2021 01:49:31 GMT  
		Size: 3.7 MB (3670760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00cc95e86fb5ab1bda9839a1ecbd3c2d607bc6cfc5155f33bf32c9d7827ec98b`  
		Last Modified: Sat, 16 Oct 2021 01:49:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe2cefdba07cb9fc803227a545d4fcc196038c1020de7698bf4e333d9056cbd`  
		Last Modified: Sat, 16 Oct 2021 01:49:28 GMT  
		Size: 2.6 MB (2573066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab77c7b0e7b171541e9f7f813ef81190ef39151aea54bfe2b64f8c191ce672c`  
		Last Modified: Sat, 16 Oct 2021 01:49:27 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d188c1c418692bd6c05728f7b542eab7acbdf502f48eaf84c762ba6b27718c`  
		Last Modified: Sat, 16 Oct 2021 01:49:27 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288c0769408956c537d6b5b649bc2b69ffe5036157a0aa58dce6c17312680a33`  
		Last Modified: Sat, 16 Oct 2021 01:49:45 GMT  
		Size: 91.3 MB (91330343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d4c9a0a37f40daaa1c904e99bb499d11db46dd87bd94236295d1ad90603ba74`  
		Last Modified: Sat, 16 Oct 2021 01:49:27 GMT  
		Size: 5.6 KB (5613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6` - linux; s390x

```console
$ docker pull mariadb@sha256:90bc202cc092060b6e454b7f2d06cbe792ffd3d7a2edefe42e30964c55d24dab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.0 MB (126014128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09b71468a7107bd097e1852fade221839dfd4b89ee873666b6f7beda44310b7a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Oct 2021 00:41:46 GMT
ADD file:cf3b6f9c395392eaf2c629969f59c48cde60ae1c74c3dbb13886481999a7a4d5 in / 
# Sat, 16 Oct 2021 00:41:48 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 01:02:36 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 16 Oct 2021 01:02:41 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:02:42 GMT
ENV GOSU_VERSION=1.13
# Sat, 16 Oct 2021 01:02:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 16 Oct 2021 01:02:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 16 Oct 2021 01:02:55 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:02:55 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 16 Oct 2021 01:03:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 16 Oct 2021 01:03:03 GMT
ARG MARIADB_MAJOR=10.6
# Sat, 16 Oct 2021 01:03:03 GMT
ENV MARIADB_MAJOR=10.6
# Sat, 16 Oct 2021 01:03:03 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Sat, 16 Oct 2021 01:03:04 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Sat, 16 Oct 2021 01:03:04 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Sat, 16 Oct 2021 01:03:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 16 Oct 2021 01:03:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 16 Oct 2021 01:03:26 GMT
VOLUME [/var/lib/mysql]
# Sat, 16 Oct 2021 01:03:26 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Sat, 16 Oct 2021 01:03:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 01:03:26 GMT
EXPOSE 3306
# Sat, 16 Oct 2021 01:03:26 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:1f0267805ccac7499fadaabf65e52d4564add2bc20ed25bcf77df24d8debb103`  
		Last Modified: Sat, 16 Oct 2021 00:42:57 GMT  
		Size: 27.1 MB (27120856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcc30a1fd200d10ce23e934b30e72d36ea131fb670d30afe697304591986fe1`  
		Last Modified: Sat, 16 Oct 2021 01:04:32 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:228a3fc0a9531bf3e9e08d9800daffbe33729ba8a16fb427b07a1a36fb047e02`  
		Last Modified: Sat, 16 Oct 2021 01:04:32 GMT  
		Size: 5.4 MB (5380980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e511a129710d7aa78451eebec778e60a256b2a9e60db59a9f6d09641bd4f96`  
		Last Modified: Sat, 16 Oct 2021 01:04:32 GMT  
		Size: 3.2 MB (3239822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a9cf411b6c206dca4cd2f493440c36781e332782682bb40969b6640e8e98e9`  
		Last Modified: Sat, 16 Oct 2021 01:04:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cac3f3cdb186c64fce6e0a7efc39abe96d0e6ab755d9193c981cc44c801cc51`  
		Last Modified: Sat, 16 Oct 2021 01:04:31 GMT  
		Size: 2.2 MB (2188905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd5f55dd4f1666fe90f4ca1b3b0cc36a9092c44ae19033a4d2b7b0e2ff3dddb`  
		Last Modified: Sat, 16 Oct 2021 01:04:30 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c0ae06775bbebbdaaf444830172bb614071d5d08004722e2ac0acc7dc0106c3`  
		Last Modified: Sat, 16 Oct 2021 01:04:30 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:362403b21b44d69858c7a816e3ddbbd7cb67dac62386727c8ce11d44891fc990`  
		Last Modified: Sat, 16 Oct 2021 01:04:48 GMT  
		Size: 88.1 MB (88073232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48196c9046fbbce7d43754945286d36794d5f7eb923e2501d8a9a4ddc88b3dd3`  
		Last Modified: Sat, 16 Oct 2021 01:04:30 GMT  
		Size: 5.6 KB (5614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.6-focal`

```console
$ docker pull mariadb@sha256:c014ba1efc5dbd711d0520c7762d57807f35549de3414eb31e942a420c8a2ed2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.6-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:dd08274a61f912b78facb7d144f898c0fd53da4f0c2fcf8ea80cd05f22577221
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.0 MB (127016059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12e05d5da3c5223e9877e8eb90d68560ff66cedcb955131061d60d093a908f0c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:07:51 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 16 Oct 2021 03:07:59 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:07:59 GMT
ENV GOSU_VERSION=1.13
# Sat, 16 Oct 2021 03:08:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 16 Oct 2021 03:08:11 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 16 Oct 2021 03:08:19 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:08:19 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 16 Oct 2021 03:08:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 16 Oct 2021 03:08:27 GMT
ARG MARIADB_MAJOR=10.6
# Sat, 16 Oct 2021 03:08:27 GMT
ENV MARIADB_MAJOR=10.6
# Sat, 16 Oct 2021 03:08:27 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Sat, 16 Oct 2021 03:08:27 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Sat, 16 Oct 2021 03:08:27 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Sat, 16 Oct 2021 03:08:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 16 Oct 2021 03:09:01 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 16 Oct 2021 03:09:02 GMT
VOLUME [/var/lib/mysql]
# Sat, 16 Oct 2021 03:09:02 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Sat, 16 Oct 2021 03:09:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 03:09:02 GMT
EXPOSE 3306
# Sat, 16 Oct 2021 03:09:02 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:034655750c88e076cbd516354371b6176d01179bf595d928444e663ba1fa6845`  
		Last Modified: Sat, 16 Oct 2021 03:11:19 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b757a2a0f02848b1254cbd8b54e1d3cd4651228ede9a8c75e127f91cb415c4`  
		Last Modified: Sat, 16 Oct 2021 03:11:20 GMT  
		Size: 5.5 MB (5489306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c37daf8b6b55859dc1f92dbe017858ae03bd5bf503a3cdbf317b0b4387b1383`  
		Last Modified: Sat, 16 Oct 2021 03:11:19 GMT  
		Size: 3.6 MB (3582632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4cd9409b0f69a0ebe270f43c3a217f05b4c326e5d7c9a4ffb0cb7852ecddc81`  
		Last Modified: Sat, 16 Oct 2021 03:11:18 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbcda06785eb5474250fd32695909199c0de3375a06cf66401d277da518f3da9`  
		Last Modified: Sat, 16 Oct 2021 03:11:17 GMT  
		Size: 2.3 MB (2276882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34cd90f184c404cd4ecd88ebe612e6f180f76836efd3c24a329a3b812c5c345`  
		Last Modified: Sat, 16 Oct 2021 03:11:16 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd6cef4ce4896ed34f82cdec0226170c9ec12e780095f39a268e4f4cd87be523`  
		Last Modified: Sat, 16 Oct 2021 03:11:16 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cb89a1550ea4efead895dec48626ae277912ca9eeffae1a3c1b8c3f0f9ed02d`  
		Last Modified: Sat, 16 Oct 2021 03:11:29 GMT  
		Size: 87.1 MB (87089805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df9f153bd93044efcf8d9cd1ea5266b32bf28df2ad72e5ce195428e8c81b917b`  
		Last Modified: Sat, 16 Oct 2021 03:11:16 GMT  
		Size: 5.6 KB (5611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:52b21e64bd048fb93b8a3ac5d36eaf3027bd5a7b1c71e833bc8ac0aa1c98c72b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.2 MB (124173665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6819e5d163d1d24d896d090e1f55c38bcb9e55db811196e3919f0707a86eff03`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:45:05 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 16 Oct 2021 03:45:15 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:45:15 GMT
ENV GOSU_VERSION=1.13
# Sat, 16 Oct 2021 03:45:29 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 16 Oct 2021 03:45:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 16 Oct 2021 03:45:37 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:45:37 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 16 Oct 2021 03:45:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 16 Oct 2021 03:45:42 GMT
ARG MARIADB_MAJOR=10.6
# Sat, 16 Oct 2021 03:45:43 GMT
ENV MARIADB_MAJOR=10.6
# Sat, 16 Oct 2021 03:45:44 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Sat, 16 Oct 2021 03:45:45 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Sat, 16 Oct 2021 03:45:46 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Sat, 16 Oct 2021 03:45:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 16 Oct 2021 03:46:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 16 Oct 2021 03:46:17 GMT
VOLUME [/var/lib/mysql]
# Sat, 16 Oct 2021 03:46:19 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Sat, 16 Oct 2021 03:46:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 03:46:20 GMT
EXPOSE 3306
# Sat, 16 Oct 2021 03:46:21 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c05479159a3de34e1aedf676cd1a6793673b2e223d06a85c1caeab97e08c15`  
		Last Modified: Sat, 16 Oct 2021 03:51:12 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3fae4be7ce6b0048b0994bc5bd1e2d202fb383de08c3f2b82896678b35e8d1`  
		Last Modified: Sat, 16 Oct 2021 03:51:12 GMT  
		Size: 5.3 MB (5320781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8ca9913d50b67d55691860d8b19e4e38456f1142af47d6ebd4e933757fb2b6`  
		Last Modified: Sat, 16 Oct 2021 03:51:12 GMT  
		Size: 3.4 MB (3368038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffbd8ed1ed1586e00f393ee1417f3bf2b1d83f13c20a5035a050af97e29b9d09`  
		Last Modified: Sat, 16 Oct 2021 03:51:11 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48e61cde050f1f52a8b54730fab5e7bc4db2d6a6303e8fa2ef4eab107076a9ba`  
		Last Modified: Sat, 16 Oct 2021 03:51:09 GMT  
		Size: 2.2 MB (2207084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0b524648b0e80b14e489493c061f52515d6e5791c7f356da3be691507607ce`  
		Last Modified: Sat, 16 Oct 2021 03:51:09 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a7bc5ea6462e7abeb995a46808ebc6c2f6d5afc6361c367235fc02909f95ff`  
		Last Modified: Sat, 16 Oct 2021 03:51:09 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70ea7fb2288eb8ce16b25989a901e5f6bc945315a86d749685f03dabde2bce5`  
		Last Modified: Sat, 16 Oct 2021 03:51:22 GMT  
		Size: 86.1 MB (86096615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:968494f5cebc0a5862440af69b49d4a863460de158a94c0f339b19d08ccf4ab6`  
		Last Modified: Sat, 16 Oct 2021 03:51:09 GMT  
		Size: 5.6 KB (5613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:aa3c316f88dd9537eeaa7201d6d3c5f8d8732196ee6c9cd5ce553816c7a060d9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137539722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a66b6be1b40e577fe733ec92528cf73ee97a8536e1fcddc9fe638aa9132f8173`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Oct 2021 00:36:38 GMT
ADD file:9246bf887411af1b286de95d779c11581dcef3c0d5a29e434162f0c085a7ce85 in / 
# Sat, 16 Oct 2021 00:36:44 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 01:34:00 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 16 Oct 2021 01:34:51 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:34:53 GMT
ENV GOSU_VERSION=1.13
# Sat, 16 Oct 2021 01:35:28 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 16 Oct 2021 01:35:36 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 16 Oct 2021 01:36:02 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:36:03 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 16 Oct 2021 01:36:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 16 Oct 2021 01:36:18 GMT
ARG MARIADB_MAJOR=10.6
# Sat, 16 Oct 2021 01:36:19 GMT
ENV MARIADB_MAJOR=10.6
# Sat, 16 Oct 2021 01:36:22 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Sat, 16 Oct 2021 01:36:24 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Sat, 16 Oct 2021 01:36:29 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Sat, 16 Oct 2021 01:36:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 16 Oct 2021 01:38:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 16 Oct 2021 01:39:01 GMT
VOLUME [/var/lib/mysql]
# Sat, 16 Oct 2021 01:39:03 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Sat, 16 Oct 2021 01:39:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 01:39:08 GMT
EXPOSE 3306
# Sat, 16 Oct 2021 01:39:15 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:77ba7971d651af68e20e7cbb6603a3f7acd8ef2893066767a93db104723556f2`  
		Last Modified: Sat, 16 Oct 2021 00:38:38 GMT  
		Size: 33.3 MB (33287238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a9c5581eb228ed7e984fa7a4e62a7f8b2a068039fde3d32fa3b208026a189d`  
		Last Modified: Sat, 16 Oct 2021 01:49:31 GMT  
		Size: 1.8 KB (1761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63d968d5ad046645779be85243a3db326487bc8905dabf68bb063ea79e1662c1`  
		Last Modified: Sat, 16 Oct 2021 01:49:32 GMT  
		Size: 6.7 MB (6667970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5bdbddf0ed762c90ab4fcfe1f42007a96e4f90ca4f0765dfcec52213a3f5c12`  
		Last Modified: Sat, 16 Oct 2021 01:49:31 GMT  
		Size: 3.7 MB (3670760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00cc95e86fb5ab1bda9839a1ecbd3c2d607bc6cfc5155f33bf32c9d7827ec98b`  
		Last Modified: Sat, 16 Oct 2021 01:49:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe2cefdba07cb9fc803227a545d4fcc196038c1020de7698bf4e333d9056cbd`  
		Last Modified: Sat, 16 Oct 2021 01:49:28 GMT  
		Size: 2.6 MB (2573066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab77c7b0e7b171541e9f7f813ef81190ef39151aea54bfe2b64f8c191ce672c`  
		Last Modified: Sat, 16 Oct 2021 01:49:27 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d188c1c418692bd6c05728f7b542eab7acbdf502f48eaf84c762ba6b27718c`  
		Last Modified: Sat, 16 Oct 2021 01:49:27 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288c0769408956c537d6b5b649bc2b69ffe5036157a0aa58dce6c17312680a33`  
		Last Modified: Sat, 16 Oct 2021 01:49:45 GMT  
		Size: 91.3 MB (91330343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d4c9a0a37f40daaa1c904e99bb499d11db46dd87bd94236295d1ad90603ba74`  
		Last Modified: Sat, 16 Oct 2021 01:49:27 GMT  
		Size: 5.6 KB (5613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:90bc202cc092060b6e454b7f2d06cbe792ffd3d7a2edefe42e30964c55d24dab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.0 MB (126014128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09b71468a7107bd097e1852fade221839dfd4b89ee873666b6f7beda44310b7a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Oct 2021 00:41:46 GMT
ADD file:cf3b6f9c395392eaf2c629969f59c48cde60ae1c74c3dbb13886481999a7a4d5 in / 
# Sat, 16 Oct 2021 00:41:48 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 01:02:36 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 16 Oct 2021 01:02:41 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:02:42 GMT
ENV GOSU_VERSION=1.13
# Sat, 16 Oct 2021 01:02:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 16 Oct 2021 01:02:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 16 Oct 2021 01:02:55 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:02:55 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 16 Oct 2021 01:03:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 16 Oct 2021 01:03:03 GMT
ARG MARIADB_MAJOR=10.6
# Sat, 16 Oct 2021 01:03:03 GMT
ENV MARIADB_MAJOR=10.6
# Sat, 16 Oct 2021 01:03:03 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Sat, 16 Oct 2021 01:03:04 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Sat, 16 Oct 2021 01:03:04 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Sat, 16 Oct 2021 01:03:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 16 Oct 2021 01:03:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 16 Oct 2021 01:03:26 GMT
VOLUME [/var/lib/mysql]
# Sat, 16 Oct 2021 01:03:26 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Sat, 16 Oct 2021 01:03:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 01:03:26 GMT
EXPOSE 3306
# Sat, 16 Oct 2021 01:03:26 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:1f0267805ccac7499fadaabf65e52d4564add2bc20ed25bcf77df24d8debb103`  
		Last Modified: Sat, 16 Oct 2021 00:42:57 GMT  
		Size: 27.1 MB (27120856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcc30a1fd200d10ce23e934b30e72d36ea131fb670d30afe697304591986fe1`  
		Last Modified: Sat, 16 Oct 2021 01:04:32 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:228a3fc0a9531bf3e9e08d9800daffbe33729ba8a16fb427b07a1a36fb047e02`  
		Last Modified: Sat, 16 Oct 2021 01:04:32 GMT  
		Size: 5.4 MB (5380980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e511a129710d7aa78451eebec778e60a256b2a9e60db59a9f6d09641bd4f96`  
		Last Modified: Sat, 16 Oct 2021 01:04:32 GMT  
		Size: 3.2 MB (3239822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a9cf411b6c206dca4cd2f493440c36781e332782682bb40969b6640e8e98e9`  
		Last Modified: Sat, 16 Oct 2021 01:04:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cac3f3cdb186c64fce6e0a7efc39abe96d0e6ab755d9193c981cc44c801cc51`  
		Last Modified: Sat, 16 Oct 2021 01:04:31 GMT  
		Size: 2.2 MB (2188905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd5f55dd4f1666fe90f4ca1b3b0cc36a9092c44ae19033a4d2b7b0e2ff3dddb`  
		Last Modified: Sat, 16 Oct 2021 01:04:30 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c0ae06775bbebbdaaf444830172bb614071d5d08004722e2ac0acc7dc0106c3`  
		Last Modified: Sat, 16 Oct 2021 01:04:30 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:362403b21b44d69858c7a816e3ddbbd7cb67dac62386727c8ce11d44891fc990`  
		Last Modified: Sat, 16 Oct 2021 01:04:48 GMT  
		Size: 88.1 MB (88073232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48196c9046fbbce7d43754945286d36794d5f7eb923e2501d8a9a4ddc88b3dd3`  
		Last Modified: Sat, 16 Oct 2021 01:04:30 GMT  
		Size: 5.6 KB (5614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.6.5`

**does not exist** (yet?)

## `mariadb:10.6.5-focal`

**does not exist** (yet?)

## `mariadb:10.7`

**does not exist** (yet?)

## `mariadb:10.7-focal`

**does not exist** (yet?)

## `mariadb:10.7.1`

**does not exist** (yet?)

## `mariadb:10.7.1-focal`

**does not exist** (yet?)

## `mariadb:focal`

```console
$ docker pull mariadb@sha256:c014ba1efc5dbd711d0520c7762d57807f35549de3414eb31e942a420c8a2ed2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:focal` - linux; amd64

```console
$ docker pull mariadb@sha256:dd08274a61f912b78facb7d144f898c0fd53da4f0c2fcf8ea80cd05f22577221
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.0 MB (127016059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12e05d5da3c5223e9877e8eb90d68560ff66cedcb955131061d60d093a908f0c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:07:51 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 16 Oct 2021 03:07:59 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:07:59 GMT
ENV GOSU_VERSION=1.13
# Sat, 16 Oct 2021 03:08:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 16 Oct 2021 03:08:11 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 16 Oct 2021 03:08:19 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:08:19 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 16 Oct 2021 03:08:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 16 Oct 2021 03:08:27 GMT
ARG MARIADB_MAJOR=10.6
# Sat, 16 Oct 2021 03:08:27 GMT
ENV MARIADB_MAJOR=10.6
# Sat, 16 Oct 2021 03:08:27 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Sat, 16 Oct 2021 03:08:27 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Sat, 16 Oct 2021 03:08:27 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Sat, 16 Oct 2021 03:08:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 16 Oct 2021 03:09:01 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 16 Oct 2021 03:09:02 GMT
VOLUME [/var/lib/mysql]
# Sat, 16 Oct 2021 03:09:02 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Sat, 16 Oct 2021 03:09:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 03:09:02 GMT
EXPOSE 3306
# Sat, 16 Oct 2021 03:09:02 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:034655750c88e076cbd516354371b6176d01179bf595d928444e663ba1fa6845`  
		Last Modified: Sat, 16 Oct 2021 03:11:19 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b757a2a0f02848b1254cbd8b54e1d3cd4651228ede9a8c75e127f91cb415c4`  
		Last Modified: Sat, 16 Oct 2021 03:11:20 GMT  
		Size: 5.5 MB (5489306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c37daf8b6b55859dc1f92dbe017858ae03bd5bf503a3cdbf317b0b4387b1383`  
		Last Modified: Sat, 16 Oct 2021 03:11:19 GMT  
		Size: 3.6 MB (3582632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4cd9409b0f69a0ebe270f43c3a217f05b4c326e5d7c9a4ffb0cb7852ecddc81`  
		Last Modified: Sat, 16 Oct 2021 03:11:18 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbcda06785eb5474250fd32695909199c0de3375a06cf66401d277da518f3da9`  
		Last Modified: Sat, 16 Oct 2021 03:11:17 GMT  
		Size: 2.3 MB (2276882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34cd90f184c404cd4ecd88ebe612e6f180f76836efd3c24a329a3b812c5c345`  
		Last Modified: Sat, 16 Oct 2021 03:11:16 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd6cef4ce4896ed34f82cdec0226170c9ec12e780095f39a268e4f4cd87be523`  
		Last Modified: Sat, 16 Oct 2021 03:11:16 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cb89a1550ea4efead895dec48626ae277912ca9eeffae1a3c1b8c3f0f9ed02d`  
		Last Modified: Sat, 16 Oct 2021 03:11:29 GMT  
		Size: 87.1 MB (87089805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df9f153bd93044efcf8d9cd1ea5266b32bf28df2ad72e5ce195428e8c81b917b`  
		Last Modified: Sat, 16 Oct 2021 03:11:16 GMT  
		Size: 5.6 KB (5611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:52b21e64bd048fb93b8a3ac5d36eaf3027bd5a7b1c71e833bc8ac0aa1c98c72b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.2 MB (124173665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6819e5d163d1d24d896d090e1f55c38bcb9e55db811196e3919f0707a86eff03`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:45:05 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 16 Oct 2021 03:45:15 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:45:15 GMT
ENV GOSU_VERSION=1.13
# Sat, 16 Oct 2021 03:45:29 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 16 Oct 2021 03:45:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 16 Oct 2021 03:45:37 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:45:37 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 16 Oct 2021 03:45:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 16 Oct 2021 03:45:42 GMT
ARG MARIADB_MAJOR=10.6
# Sat, 16 Oct 2021 03:45:43 GMT
ENV MARIADB_MAJOR=10.6
# Sat, 16 Oct 2021 03:45:44 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Sat, 16 Oct 2021 03:45:45 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Sat, 16 Oct 2021 03:45:46 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Sat, 16 Oct 2021 03:45:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 16 Oct 2021 03:46:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 16 Oct 2021 03:46:17 GMT
VOLUME [/var/lib/mysql]
# Sat, 16 Oct 2021 03:46:19 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Sat, 16 Oct 2021 03:46:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 03:46:20 GMT
EXPOSE 3306
# Sat, 16 Oct 2021 03:46:21 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c05479159a3de34e1aedf676cd1a6793673b2e223d06a85c1caeab97e08c15`  
		Last Modified: Sat, 16 Oct 2021 03:51:12 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3fae4be7ce6b0048b0994bc5bd1e2d202fb383de08c3f2b82896678b35e8d1`  
		Last Modified: Sat, 16 Oct 2021 03:51:12 GMT  
		Size: 5.3 MB (5320781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8ca9913d50b67d55691860d8b19e4e38456f1142af47d6ebd4e933757fb2b6`  
		Last Modified: Sat, 16 Oct 2021 03:51:12 GMT  
		Size: 3.4 MB (3368038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffbd8ed1ed1586e00f393ee1417f3bf2b1d83f13c20a5035a050af97e29b9d09`  
		Last Modified: Sat, 16 Oct 2021 03:51:11 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48e61cde050f1f52a8b54730fab5e7bc4db2d6a6303e8fa2ef4eab107076a9ba`  
		Last Modified: Sat, 16 Oct 2021 03:51:09 GMT  
		Size: 2.2 MB (2207084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0b524648b0e80b14e489493c061f52515d6e5791c7f356da3be691507607ce`  
		Last Modified: Sat, 16 Oct 2021 03:51:09 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a7bc5ea6462e7abeb995a46808ebc6c2f6d5afc6361c367235fc02909f95ff`  
		Last Modified: Sat, 16 Oct 2021 03:51:09 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70ea7fb2288eb8ce16b25989a901e5f6bc945315a86d749685f03dabde2bce5`  
		Last Modified: Sat, 16 Oct 2021 03:51:22 GMT  
		Size: 86.1 MB (86096615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:968494f5cebc0a5862440af69b49d4a863460de158a94c0f339b19d08ccf4ab6`  
		Last Modified: Sat, 16 Oct 2021 03:51:09 GMT  
		Size: 5.6 KB (5613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:aa3c316f88dd9537eeaa7201d6d3c5f8d8732196ee6c9cd5ce553816c7a060d9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137539722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a66b6be1b40e577fe733ec92528cf73ee97a8536e1fcddc9fe638aa9132f8173`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Oct 2021 00:36:38 GMT
ADD file:9246bf887411af1b286de95d779c11581dcef3c0d5a29e434162f0c085a7ce85 in / 
# Sat, 16 Oct 2021 00:36:44 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 01:34:00 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 16 Oct 2021 01:34:51 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:34:53 GMT
ENV GOSU_VERSION=1.13
# Sat, 16 Oct 2021 01:35:28 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 16 Oct 2021 01:35:36 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 16 Oct 2021 01:36:02 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:36:03 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 16 Oct 2021 01:36:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 16 Oct 2021 01:36:18 GMT
ARG MARIADB_MAJOR=10.6
# Sat, 16 Oct 2021 01:36:19 GMT
ENV MARIADB_MAJOR=10.6
# Sat, 16 Oct 2021 01:36:22 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Sat, 16 Oct 2021 01:36:24 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Sat, 16 Oct 2021 01:36:29 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Sat, 16 Oct 2021 01:36:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 16 Oct 2021 01:38:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 16 Oct 2021 01:39:01 GMT
VOLUME [/var/lib/mysql]
# Sat, 16 Oct 2021 01:39:03 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Sat, 16 Oct 2021 01:39:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 01:39:08 GMT
EXPOSE 3306
# Sat, 16 Oct 2021 01:39:15 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:77ba7971d651af68e20e7cbb6603a3f7acd8ef2893066767a93db104723556f2`  
		Last Modified: Sat, 16 Oct 2021 00:38:38 GMT  
		Size: 33.3 MB (33287238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a9c5581eb228ed7e984fa7a4e62a7f8b2a068039fde3d32fa3b208026a189d`  
		Last Modified: Sat, 16 Oct 2021 01:49:31 GMT  
		Size: 1.8 KB (1761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63d968d5ad046645779be85243a3db326487bc8905dabf68bb063ea79e1662c1`  
		Last Modified: Sat, 16 Oct 2021 01:49:32 GMT  
		Size: 6.7 MB (6667970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5bdbddf0ed762c90ab4fcfe1f42007a96e4f90ca4f0765dfcec52213a3f5c12`  
		Last Modified: Sat, 16 Oct 2021 01:49:31 GMT  
		Size: 3.7 MB (3670760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00cc95e86fb5ab1bda9839a1ecbd3c2d607bc6cfc5155f33bf32c9d7827ec98b`  
		Last Modified: Sat, 16 Oct 2021 01:49:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe2cefdba07cb9fc803227a545d4fcc196038c1020de7698bf4e333d9056cbd`  
		Last Modified: Sat, 16 Oct 2021 01:49:28 GMT  
		Size: 2.6 MB (2573066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab77c7b0e7b171541e9f7f813ef81190ef39151aea54bfe2b64f8c191ce672c`  
		Last Modified: Sat, 16 Oct 2021 01:49:27 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d188c1c418692bd6c05728f7b542eab7acbdf502f48eaf84c762ba6b27718c`  
		Last Modified: Sat, 16 Oct 2021 01:49:27 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288c0769408956c537d6b5b649bc2b69ffe5036157a0aa58dce6c17312680a33`  
		Last Modified: Sat, 16 Oct 2021 01:49:45 GMT  
		Size: 91.3 MB (91330343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d4c9a0a37f40daaa1c904e99bb499d11db46dd87bd94236295d1ad90603ba74`  
		Last Modified: Sat, 16 Oct 2021 01:49:27 GMT  
		Size: 5.6 KB (5613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:focal` - linux; s390x

```console
$ docker pull mariadb@sha256:90bc202cc092060b6e454b7f2d06cbe792ffd3d7a2edefe42e30964c55d24dab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.0 MB (126014128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09b71468a7107bd097e1852fade221839dfd4b89ee873666b6f7beda44310b7a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Oct 2021 00:41:46 GMT
ADD file:cf3b6f9c395392eaf2c629969f59c48cde60ae1c74c3dbb13886481999a7a4d5 in / 
# Sat, 16 Oct 2021 00:41:48 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 01:02:36 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 16 Oct 2021 01:02:41 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:02:42 GMT
ENV GOSU_VERSION=1.13
# Sat, 16 Oct 2021 01:02:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 16 Oct 2021 01:02:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 16 Oct 2021 01:02:55 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:02:55 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 16 Oct 2021 01:03:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 16 Oct 2021 01:03:03 GMT
ARG MARIADB_MAJOR=10.6
# Sat, 16 Oct 2021 01:03:03 GMT
ENV MARIADB_MAJOR=10.6
# Sat, 16 Oct 2021 01:03:03 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Sat, 16 Oct 2021 01:03:04 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Sat, 16 Oct 2021 01:03:04 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Sat, 16 Oct 2021 01:03:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 16 Oct 2021 01:03:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 16 Oct 2021 01:03:26 GMT
VOLUME [/var/lib/mysql]
# Sat, 16 Oct 2021 01:03:26 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Sat, 16 Oct 2021 01:03:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 01:03:26 GMT
EXPOSE 3306
# Sat, 16 Oct 2021 01:03:26 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:1f0267805ccac7499fadaabf65e52d4564add2bc20ed25bcf77df24d8debb103`  
		Last Modified: Sat, 16 Oct 2021 00:42:57 GMT  
		Size: 27.1 MB (27120856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcc30a1fd200d10ce23e934b30e72d36ea131fb670d30afe697304591986fe1`  
		Last Modified: Sat, 16 Oct 2021 01:04:32 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:228a3fc0a9531bf3e9e08d9800daffbe33729ba8a16fb427b07a1a36fb047e02`  
		Last Modified: Sat, 16 Oct 2021 01:04:32 GMT  
		Size: 5.4 MB (5380980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e511a129710d7aa78451eebec778e60a256b2a9e60db59a9f6d09641bd4f96`  
		Last Modified: Sat, 16 Oct 2021 01:04:32 GMT  
		Size: 3.2 MB (3239822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a9cf411b6c206dca4cd2f493440c36781e332782682bb40969b6640e8e98e9`  
		Last Modified: Sat, 16 Oct 2021 01:04:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cac3f3cdb186c64fce6e0a7efc39abe96d0e6ab755d9193c981cc44c801cc51`  
		Last Modified: Sat, 16 Oct 2021 01:04:31 GMT  
		Size: 2.2 MB (2188905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd5f55dd4f1666fe90f4ca1b3b0cc36a9092c44ae19033a4d2b7b0e2ff3dddb`  
		Last Modified: Sat, 16 Oct 2021 01:04:30 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c0ae06775bbebbdaaf444830172bb614071d5d08004722e2ac0acc7dc0106c3`  
		Last Modified: Sat, 16 Oct 2021 01:04:30 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:362403b21b44d69858c7a816e3ddbbd7cb67dac62386727c8ce11d44891fc990`  
		Last Modified: Sat, 16 Oct 2021 01:04:48 GMT  
		Size: 88.1 MB (88073232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48196c9046fbbce7d43754945286d36794d5f7eb923e2501d8a9a4ddc88b3dd3`  
		Last Modified: Sat, 16 Oct 2021 01:04:30 GMT  
		Size: 5.6 KB (5614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:latest`

```console
$ docker pull mariadb@sha256:c014ba1efc5dbd711d0520c7762d57807f35549de3414eb31e942a420c8a2ed2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:latest` - linux; amd64

```console
$ docker pull mariadb@sha256:dd08274a61f912b78facb7d144f898c0fd53da4f0c2fcf8ea80cd05f22577221
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.0 MB (127016059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12e05d5da3c5223e9877e8eb90d68560ff66cedcb955131061d60d093a908f0c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:07:51 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 16 Oct 2021 03:07:59 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:07:59 GMT
ENV GOSU_VERSION=1.13
# Sat, 16 Oct 2021 03:08:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 16 Oct 2021 03:08:11 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 16 Oct 2021 03:08:19 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:08:19 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 16 Oct 2021 03:08:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 16 Oct 2021 03:08:27 GMT
ARG MARIADB_MAJOR=10.6
# Sat, 16 Oct 2021 03:08:27 GMT
ENV MARIADB_MAJOR=10.6
# Sat, 16 Oct 2021 03:08:27 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Sat, 16 Oct 2021 03:08:27 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Sat, 16 Oct 2021 03:08:27 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Sat, 16 Oct 2021 03:08:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 16 Oct 2021 03:09:01 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 16 Oct 2021 03:09:02 GMT
VOLUME [/var/lib/mysql]
# Sat, 16 Oct 2021 03:09:02 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Sat, 16 Oct 2021 03:09:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 03:09:02 GMT
EXPOSE 3306
# Sat, 16 Oct 2021 03:09:02 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:034655750c88e076cbd516354371b6176d01179bf595d928444e663ba1fa6845`  
		Last Modified: Sat, 16 Oct 2021 03:11:19 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b757a2a0f02848b1254cbd8b54e1d3cd4651228ede9a8c75e127f91cb415c4`  
		Last Modified: Sat, 16 Oct 2021 03:11:20 GMT  
		Size: 5.5 MB (5489306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c37daf8b6b55859dc1f92dbe017858ae03bd5bf503a3cdbf317b0b4387b1383`  
		Last Modified: Sat, 16 Oct 2021 03:11:19 GMT  
		Size: 3.6 MB (3582632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4cd9409b0f69a0ebe270f43c3a217f05b4c326e5d7c9a4ffb0cb7852ecddc81`  
		Last Modified: Sat, 16 Oct 2021 03:11:18 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbcda06785eb5474250fd32695909199c0de3375a06cf66401d277da518f3da9`  
		Last Modified: Sat, 16 Oct 2021 03:11:17 GMT  
		Size: 2.3 MB (2276882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34cd90f184c404cd4ecd88ebe612e6f180f76836efd3c24a329a3b812c5c345`  
		Last Modified: Sat, 16 Oct 2021 03:11:16 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd6cef4ce4896ed34f82cdec0226170c9ec12e780095f39a268e4f4cd87be523`  
		Last Modified: Sat, 16 Oct 2021 03:11:16 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cb89a1550ea4efead895dec48626ae277912ca9eeffae1a3c1b8c3f0f9ed02d`  
		Last Modified: Sat, 16 Oct 2021 03:11:29 GMT  
		Size: 87.1 MB (87089805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df9f153bd93044efcf8d9cd1ea5266b32bf28df2ad72e5ce195428e8c81b917b`  
		Last Modified: Sat, 16 Oct 2021 03:11:16 GMT  
		Size: 5.6 KB (5611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:52b21e64bd048fb93b8a3ac5d36eaf3027bd5a7b1c71e833bc8ac0aa1c98c72b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.2 MB (124173665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6819e5d163d1d24d896d090e1f55c38bcb9e55db811196e3919f0707a86eff03`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:45:05 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 16 Oct 2021 03:45:15 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:45:15 GMT
ENV GOSU_VERSION=1.13
# Sat, 16 Oct 2021 03:45:29 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 16 Oct 2021 03:45:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 16 Oct 2021 03:45:37 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:45:37 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 16 Oct 2021 03:45:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 16 Oct 2021 03:45:42 GMT
ARG MARIADB_MAJOR=10.6
# Sat, 16 Oct 2021 03:45:43 GMT
ENV MARIADB_MAJOR=10.6
# Sat, 16 Oct 2021 03:45:44 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Sat, 16 Oct 2021 03:45:45 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Sat, 16 Oct 2021 03:45:46 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Sat, 16 Oct 2021 03:45:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 16 Oct 2021 03:46:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 16 Oct 2021 03:46:17 GMT
VOLUME [/var/lib/mysql]
# Sat, 16 Oct 2021 03:46:19 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Sat, 16 Oct 2021 03:46:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 03:46:20 GMT
EXPOSE 3306
# Sat, 16 Oct 2021 03:46:21 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c05479159a3de34e1aedf676cd1a6793673b2e223d06a85c1caeab97e08c15`  
		Last Modified: Sat, 16 Oct 2021 03:51:12 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3fae4be7ce6b0048b0994bc5bd1e2d202fb383de08c3f2b82896678b35e8d1`  
		Last Modified: Sat, 16 Oct 2021 03:51:12 GMT  
		Size: 5.3 MB (5320781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8ca9913d50b67d55691860d8b19e4e38456f1142af47d6ebd4e933757fb2b6`  
		Last Modified: Sat, 16 Oct 2021 03:51:12 GMT  
		Size: 3.4 MB (3368038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffbd8ed1ed1586e00f393ee1417f3bf2b1d83f13c20a5035a050af97e29b9d09`  
		Last Modified: Sat, 16 Oct 2021 03:51:11 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48e61cde050f1f52a8b54730fab5e7bc4db2d6a6303e8fa2ef4eab107076a9ba`  
		Last Modified: Sat, 16 Oct 2021 03:51:09 GMT  
		Size: 2.2 MB (2207084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0b524648b0e80b14e489493c061f52515d6e5791c7f356da3be691507607ce`  
		Last Modified: Sat, 16 Oct 2021 03:51:09 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a7bc5ea6462e7abeb995a46808ebc6c2f6d5afc6361c367235fc02909f95ff`  
		Last Modified: Sat, 16 Oct 2021 03:51:09 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70ea7fb2288eb8ce16b25989a901e5f6bc945315a86d749685f03dabde2bce5`  
		Last Modified: Sat, 16 Oct 2021 03:51:22 GMT  
		Size: 86.1 MB (86096615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:968494f5cebc0a5862440af69b49d4a863460de158a94c0f339b19d08ccf4ab6`  
		Last Modified: Sat, 16 Oct 2021 03:51:09 GMT  
		Size: 5.6 KB (5613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; ppc64le

```console
$ docker pull mariadb@sha256:aa3c316f88dd9537eeaa7201d6d3c5f8d8732196ee6c9cd5ce553816c7a060d9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137539722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a66b6be1b40e577fe733ec92528cf73ee97a8536e1fcddc9fe638aa9132f8173`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Oct 2021 00:36:38 GMT
ADD file:9246bf887411af1b286de95d779c11581dcef3c0d5a29e434162f0c085a7ce85 in / 
# Sat, 16 Oct 2021 00:36:44 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 01:34:00 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 16 Oct 2021 01:34:51 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:34:53 GMT
ENV GOSU_VERSION=1.13
# Sat, 16 Oct 2021 01:35:28 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 16 Oct 2021 01:35:36 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 16 Oct 2021 01:36:02 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:36:03 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 16 Oct 2021 01:36:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 16 Oct 2021 01:36:18 GMT
ARG MARIADB_MAJOR=10.6
# Sat, 16 Oct 2021 01:36:19 GMT
ENV MARIADB_MAJOR=10.6
# Sat, 16 Oct 2021 01:36:22 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Sat, 16 Oct 2021 01:36:24 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Sat, 16 Oct 2021 01:36:29 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Sat, 16 Oct 2021 01:36:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 16 Oct 2021 01:38:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 16 Oct 2021 01:39:01 GMT
VOLUME [/var/lib/mysql]
# Sat, 16 Oct 2021 01:39:03 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Sat, 16 Oct 2021 01:39:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 01:39:08 GMT
EXPOSE 3306
# Sat, 16 Oct 2021 01:39:15 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:77ba7971d651af68e20e7cbb6603a3f7acd8ef2893066767a93db104723556f2`  
		Last Modified: Sat, 16 Oct 2021 00:38:38 GMT  
		Size: 33.3 MB (33287238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a9c5581eb228ed7e984fa7a4e62a7f8b2a068039fde3d32fa3b208026a189d`  
		Last Modified: Sat, 16 Oct 2021 01:49:31 GMT  
		Size: 1.8 KB (1761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63d968d5ad046645779be85243a3db326487bc8905dabf68bb063ea79e1662c1`  
		Last Modified: Sat, 16 Oct 2021 01:49:32 GMT  
		Size: 6.7 MB (6667970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5bdbddf0ed762c90ab4fcfe1f42007a96e4f90ca4f0765dfcec52213a3f5c12`  
		Last Modified: Sat, 16 Oct 2021 01:49:31 GMT  
		Size: 3.7 MB (3670760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00cc95e86fb5ab1bda9839a1ecbd3c2d607bc6cfc5155f33bf32c9d7827ec98b`  
		Last Modified: Sat, 16 Oct 2021 01:49:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe2cefdba07cb9fc803227a545d4fcc196038c1020de7698bf4e333d9056cbd`  
		Last Modified: Sat, 16 Oct 2021 01:49:28 GMT  
		Size: 2.6 MB (2573066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab77c7b0e7b171541e9f7f813ef81190ef39151aea54bfe2b64f8c191ce672c`  
		Last Modified: Sat, 16 Oct 2021 01:49:27 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d188c1c418692bd6c05728f7b542eab7acbdf502f48eaf84c762ba6b27718c`  
		Last Modified: Sat, 16 Oct 2021 01:49:27 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288c0769408956c537d6b5b649bc2b69ffe5036157a0aa58dce6c17312680a33`  
		Last Modified: Sat, 16 Oct 2021 01:49:45 GMT  
		Size: 91.3 MB (91330343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d4c9a0a37f40daaa1c904e99bb499d11db46dd87bd94236295d1ad90603ba74`  
		Last Modified: Sat, 16 Oct 2021 01:49:27 GMT  
		Size: 5.6 KB (5613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; s390x

```console
$ docker pull mariadb@sha256:90bc202cc092060b6e454b7f2d06cbe792ffd3d7a2edefe42e30964c55d24dab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.0 MB (126014128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09b71468a7107bd097e1852fade221839dfd4b89ee873666b6f7beda44310b7a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Oct 2021 00:41:46 GMT
ADD file:cf3b6f9c395392eaf2c629969f59c48cde60ae1c74c3dbb13886481999a7a4d5 in / 
# Sat, 16 Oct 2021 00:41:48 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 01:02:36 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 16 Oct 2021 01:02:41 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:02:42 GMT
ENV GOSU_VERSION=1.13
# Sat, 16 Oct 2021 01:02:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 16 Oct 2021 01:02:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 16 Oct 2021 01:02:55 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:02:55 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 16 Oct 2021 01:03:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 16 Oct 2021 01:03:03 GMT
ARG MARIADB_MAJOR=10.6
# Sat, 16 Oct 2021 01:03:03 GMT
ENV MARIADB_MAJOR=10.6
# Sat, 16 Oct 2021 01:03:03 GMT
ARG MARIADB_VERSION=1:10.6.4+maria~focal
# Sat, 16 Oct 2021 01:03:04 GMT
ENV MARIADB_VERSION=1:10.6.4+maria~focal
# Sat, 16 Oct 2021 01:03:04 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
# Sat, 16 Oct 2021 01:03:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 16 Oct 2021 01:03:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 16 Oct 2021 01:03:26 GMT
VOLUME [/var/lib/mysql]
# Sat, 16 Oct 2021 01:03:26 GMT
COPY file:12b2a6a332e2002415e548cd024d4bdcdc90745b28f202869ff2d205d7a8c8cc in /usr/local/bin/ 
# Sat, 16 Oct 2021 01:03:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 01:03:26 GMT
EXPOSE 3306
# Sat, 16 Oct 2021 01:03:26 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:1f0267805ccac7499fadaabf65e52d4564add2bc20ed25bcf77df24d8debb103`  
		Last Modified: Sat, 16 Oct 2021 00:42:57 GMT  
		Size: 27.1 MB (27120856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcc30a1fd200d10ce23e934b30e72d36ea131fb670d30afe697304591986fe1`  
		Last Modified: Sat, 16 Oct 2021 01:04:32 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:228a3fc0a9531bf3e9e08d9800daffbe33729ba8a16fb427b07a1a36fb047e02`  
		Last Modified: Sat, 16 Oct 2021 01:04:32 GMT  
		Size: 5.4 MB (5380980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e511a129710d7aa78451eebec778e60a256b2a9e60db59a9f6d09641bd4f96`  
		Last Modified: Sat, 16 Oct 2021 01:04:32 GMT  
		Size: 3.2 MB (3239822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a9cf411b6c206dca4cd2f493440c36781e332782682bb40969b6640e8e98e9`  
		Last Modified: Sat, 16 Oct 2021 01:04:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cac3f3cdb186c64fce6e0a7efc39abe96d0e6ab755d9193c981cc44c801cc51`  
		Last Modified: Sat, 16 Oct 2021 01:04:31 GMT  
		Size: 2.2 MB (2188905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd5f55dd4f1666fe90f4ca1b3b0cc36a9092c44ae19033a4d2b7b0e2ff3dddb`  
		Last Modified: Sat, 16 Oct 2021 01:04:30 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c0ae06775bbebbdaaf444830172bb614071d5d08004722e2ac0acc7dc0106c3`  
		Last Modified: Sat, 16 Oct 2021 01:04:30 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:362403b21b44d69858c7a816e3ddbbd7cb67dac62386727c8ce11d44891fc990`  
		Last Modified: Sat, 16 Oct 2021 01:04:48 GMT  
		Size: 88.1 MB (88073232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48196c9046fbbce7d43754945286d36794d5f7eb923e2501d8a9a4ddc88b3dd3`  
		Last Modified: Sat, 16 Oct 2021 01:04:30 GMT  
		Size: 5.6 KB (5614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
