<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mariadb`

-	[`mariadb:10`](#mariadb10)
-	[`mariadb:10-focal`](#mariadb10-focal)
-	[`mariadb:10.2`](#mariadb102)
-	[`mariadb:10.2-bionic`](#mariadb102-bionic)
-	[`mariadb:10.2.43`](#mariadb10243)
-	[`mariadb:10.2.43-bionic`](#mariadb10243-bionic)
-	[`mariadb:10.3`](#mariadb103)
-	[`mariadb:10.3-focal`](#mariadb103-focal)
-	[`mariadb:10.3.34`](#mariadb10334)
-	[`mariadb:10.3.34-focal`](#mariadb10334-focal)
-	[`mariadb:10.4`](#mariadb104)
-	[`mariadb:10.4-focal`](#mariadb104-focal)
-	[`mariadb:10.4.24`](#mariadb10424)
-	[`mariadb:10.4.24-focal`](#mariadb10424-focal)
-	[`mariadb:10.5`](#mariadb105)
-	[`mariadb:10.5-focal`](#mariadb105-focal)
-	[`mariadb:10.5.15`](#mariadb10515)
-	[`mariadb:10.5.15-focal`](#mariadb10515-focal)
-	[`mariadb:10.6`](#mariadb106)
-	[`mariadb:10.6-focal`](#mariadb106-focal)
-	[`mariadb:10.6.7`](#mariadb1067)
-	[`mariadb:10.6.7-focal`](#mariadb1067-focal)
-	[`mariadb:10.7`](#mariadb107)
-	[`mariadb:10.7-focal`](#mariadb107-focal)
-	[`mariadb:10.7.3`](#mariadb1073)
-	[`mariadb:10.7.3-focal`](#mariadb1073-focal)
-	[`mariadb:10.8-rc`](#mariadb108-rc)
-	[`mariadb:10.8-rc-focal`](#mariadb108-rc-focal)
-	[`mariadb:10.8.2-rc`](#mariadb1082-rc)
-	[`mariadb:10.8.2-rc-focal`](#mariadb1082-rc-focal)
-	[`mariadb:focal`](#mariadbfocal)
-	[`mariadb:latest`](#mariadblatest)

## `mariadb:10`

```console
$ docker pull mariadb@sha256:3a557616cccfbe3fa9dbcd31086511b907498dbf2526888977c87c1c8a952694
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10` - linux; amd64

```console
$ docker pull mariadb@sha256:c5cefb5639e0f9360734406cb0f8b7a119c29083705059a1c4509cf31b6f1dbe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128668138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a1ace59b072bf4850281c7a3262a76f762ef97d774a38f5a5cddda9514dd811`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:51:07 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 02:51:07 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 02:51:07 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 02:51:07 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 02:51:07 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:51:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:51:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:51:29 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:51:29 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:51:30 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:51:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:51:30 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:51:30 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8f6c64a8fa57732c8eb3db48d751c40e0795aa5ca42f05d27c2e9ab31075bc`  
		Last Modified: Fri, 22 Apr 2022 02:55:43 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9817bd990fc72a53340f7dfdda9343811b5a6f4cbc914369c092d3994a044a`  
		Last Modified: Fri, 22 Apr 2022 02:55:56 GMT  
		Size: 88.7 MB (88741666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14828b87067569c6589bb8a62987321b440e088af17c5e8a0163841f3bba2e26`  
		Last Modified: Fri, 22 Apr 2022 02:55:42 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233be9bdce04aeae1b3a83158f299fccc9e8ef3535617d5ea40ebe5b9dcac8c6`  
		Last Modified: Fri, 22 Apr 2022 02:55:42 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:de0cb4b23ef923f913d2c4a2dc8164cd85c679fbc0b0f152188e7b0b59cc2805
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125721225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a812ba80dab1b9376c209ff5bfa06ee2d1fe4fd7382cff8b7dd05b2e02ab103`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:29:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 03:29:22 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:23 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 03:29:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 03:29:39 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 03:29:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:48 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 03:29:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 03:30:37 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 03:30:38 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 03:30:39 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 03:30:40 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 03:30:41 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 03:30:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 03:31:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 03:31:05 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 03:31:07 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 03:31:08 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 03:31:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 03:31:09 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 03:31:10 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7061769dfb44ec758f6d367a5d4ea0ae9e6f03ca107b7f4ee4b2419e2ae693b`  
		Last Modified: Fri, 22 Apr 2022 03:36:31 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc0a8ec71ebae8e12eafc6106df54088463cc344135ebd19dc41f331e0ed6f2`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 5.3 MB (5320310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87bc30abcdec1bcda27933f56dac195031b448391d01eb7ed27fe77b389117e7`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 3.4 MB (3370037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c05e5ca55fe31dfae11772d53c4dd507f38b7e27ba3b7b878954b5c1d9697f87`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617ab90f9424ca5c02f763590888d7804d6be962990b9f82717351743533c8f0`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 2.2 MB (2202477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bbb7ad258365e117ef11517dc6c0beadccf14acb57fba68848b61d4e0044111`  
		Last Modified: Fri, 22 Apr 2022 03:36:26 GMT  
		Size: 2.5 KB (2469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adee1bd260a8e20308d2463b97fdf304e75ff2a03259cb9b597295f8a899488d`  
		Last Modified: Fri, 22 Apr 2022 03:37:00 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600d1c5c23efadd0b4f5b2716ca3d427db04d06648bf9eeeffdca772ee584382`  
		Last Modified: Fri, 22 Apr 2022 03:37:13 GMT  
		Size: 87.6 MB (87644354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c9f5ecbe579c7837ce9f148319eb5dc065bedde53ae1ac35e0a124523c39ee`  
		Last Modified: Fri, 22 Apr 2022 03:37:00 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59eb437ecaf54263722ed5022a76bed608412ab4f94fc2aa7666d1653ddf23ce`  
		Last Modified: Fri, 22 Apr 2022 03:37:00 GMT  
		Size: 6.8 KB (6777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10` - linux; ppc64le

```console
$ docker pull mariadb@sha256:e66b201216b5bebbd358365e3b3c977f306720c2dcd66dad04da85aeeb1ac9ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.5 MB (139536731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ff5e20d4ebd7fe8753ba3d0e7907e1a21a78868e5672e580c4951ab3f27b484`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:34:08 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 10:34:09 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 10:34:11 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 10:34:12 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 10:34:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:34:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:36:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:36:14 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:36:15 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:36:16 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:36:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:36:19 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:36:21 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa16fdd8f2b7ed887c119c9ca942715f9f1d4e3d0704344fe671cb921c3df6e6`  
		Last Modified: Fri, 22 Apr 2022 10:52:43 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc7852c7cfc5a89e8ec199e80be577caf5cb6278d52334b86888dad8b9a5d19`  
		Last Modified: Fri, 22 Apr 2022 10:53:01 GMT  
		Size: 93.3 MB (93323480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90b1dfdfe9bb649c7f4ce895a13e16f1cefed0bd1dca47c742a8dbb7f7ecd33`  
		Last Modified: Fri, 22 Apr 2022 10:52:43 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf93f3686f15dba104bc6ae5f4303b33340d33a2d4244c00f76ef218d9ded2d`  
		Last Modified: Fri, 22 Apr 2022 10:52:43 GMT  
		Size: 6.8 KB (6778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10` - linux; s390x

```console
$ docker pull mariadb@sha256:b2805c726caa7af5fe4e44a3ade5afbbb7f7c780567c147cb36b5c7a363464b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127722709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a8b068ba5353d198e5fd7c34100da7ebc6771c257d75e23b80a211925de86aa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 00:39:34 GMT
ADD file:a5fe3b5fef5d5d99022e3a45894edf18c9e5f79c4be8020d61724cdc164256b3 in / 
# Fri, 22 Apr 2022 00:39:39 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:19:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:19:18 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:19:19 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:19:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:19:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:19:48 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:19:50 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:19:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:21:06 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 02:21:06 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 02:21:07 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 02:21:07 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 02:21:08 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:21:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:21:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:21:56 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:21:56 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:21:56 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:21:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:21:57 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:21:57 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:716ba34a9a0241d7bed3fa68865e745000f025af68d21dab7d692215c5074a58`  
		Last Modified: Tue, 19 Apr 2022 13:16:37 GMT  
		Size: 27.1 MB (27085718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bc8f5833a8cfe0537845df0a5d311b211ef889ed5d5e12ace1bd3eb30834c6`  
		Last Modified: Fri, 22 Apr 2022 02:25:50 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f4186175df1fdbe352452d13a8d94670ff3446432648e7b163e9a1c6a94d88`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 5.4 MB (5378760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea503bea58815ffe61d67ad911ffab94ad5a57e364db2126c3cb11e8f732d37`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 3.2 MB (3244218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76eb02e31628a4e2997c0f38de59eb7d09325086dd65b6b511c1e63c7fdd1692`  
		Last Modified: Fri, 22 Apr 2022 02:25:48 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34da960e123e0d72767a541ecf7347f03dfad9502e82a54cd713eb6c1e2d294b`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 2.2 MB (2183672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0ddf5cdd828e8ea2c4c69fedbb30d4aebf50bbc1c279fae4855faec077ae98`  
		Last Modified: Fri, 22 Apr 2022 02:25:47 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e906a7a4ca515f29ae2f9d042b9d50795a7722dff0e54711609032ab009449`  
		Last Modified: Fri, 22 Apr 2022 02:26:13 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8aa65ca376e03fed74f419a6a903362e83d6d4e1e1773ad67ad7183de7bbdf2`  
		Last Modified: Fri, 22 Apr 2022 02:26:26 GMT  
		Size: 89.8 MB (89815355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d48c43c28d400d613cd154b3e3182816a6e8b669d1fd7254e80bd5c51ae5f17`  
		Last Modified: Fri, 22 Apr 2022 02:26:13 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b5541b27b08286050b0bfd633e5710b2273e67032af256ca1137c955ccbd51`  
		Last Modified: Fri, 22 Apr 2022 02:26:13 GMT  
		Size: 6.8 KB (6775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10-focal`

```console
$ docker pull mariadb@sha256:3a557616cccfbe3fa9dbcd31086511b907498dbf2526888977c87c1c8a952694
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:c5cefb5639e0f9360734406cb0f8b7a119c29083705059a1c4509cf31b6f1dbe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128668138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a1ace59b072bf4850281c7a3262a76f762ef97d774a38f5a5cddda9514dd811`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:51:07 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 02:51:07 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 02:51:07 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 02:51:07 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 02:51:07 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:51:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:51:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:51:29 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:51:29 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:51:30 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:51:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:51:30 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:51:30 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8f6c64a8fa57732c8eb3db48d751c40e0795aa5ca42f05d27c2e9ab31075bc`  
		Last Modified: Fri, 22 Apr 2022 02:55:43 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9817bd990fc72a53340f7dfdda9343811b5a6f4cbc914369c092d3994a044a`  
		Last Modified: Fri, 22 Apr 2022 02:55:56 GMT  
		Size: 88.7 MB (88741666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14828b87067569c6589bb8a62987321b440e088af17c5e8a0163841f3bba2e26`  
		Last Modified: Fri, 22 Apr 2022 02:55:42 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233be9bdce04aeae1b3a83158f299fccc9e8ef3535617d5ea40ebe5b9dcac8c6`  
		Last Modified: Fri, 22 Apr 2022 02:55:42 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:de0cb4b23ef923f913d2c4a2dc8164cd85c679fbc0b0f152188e7b0b59cc2805
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125721225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a812ba80dab1b9376c209ff5bfa06ee2d1fe4fd7382cff8b7dd05b2e02ab103`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:29:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 03:29:22 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:23 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 03:29:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 03:29:39 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 03:29:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:48 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 03:29:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 03:30:37 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 03:30:38 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 03:30:39 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 03:30:40 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 03:30:41 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 03:30:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 03:31:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 03:31:05 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 03:31:07 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 03:31:08 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 03:31:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 03:31:09 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 03:31:10 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7061769dfb44ec758f6d367a5d4ea0ae9e6f03ca107b7f4ee4b2419e2ae693b`  
		Last Modified: Fri, 22 Apr 2022 03:36:31 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc0a8ec71ebae8e12eafc6106df54088463cc344135ebd19dc41f331e0ed6f2`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 5.3 MB (5320310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87bc30abcdec1bcda27933f56dac195031b448391d01eb7ed27fe77b389117e7`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 3.4 MB (3370037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c05e5ca55fe31dfae11772d53c4dd507f38b7e27ba3b7b878954b5c1d9697f87`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617ab90f9424ca5c02f763590888d7804d6be962990b9f82717351743533c8f0`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 2.2 MB (2202477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bbb7ad258365e117ef11517dc6c0beadccf14acb57fba68848b61d4e0044111`  
		Last Modified: Fri, 22 Apr 2022 03:36:26 GMT  
		Size: 2.5 KB (2469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adee1bd260a8e20308d2463b97fdf304e75ff2a03259cb9b597295f8a899488d`  
		Last Modified: Fri, 22 Apr 2022 03:37:00 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600d1c5c23efadd0b4f5b2716ca3d427db04d06648bf9eeeffdca772ee584382`  
		Last Modified: Fri, 22 Apr 2022 03:37:13 GMT  
		Size: 87.6 MB (87644354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c9f5ecbe579c7837ce9f148319eb5dc065bedde53ae1ac35e0a124523c39ee`  
		Last Modified: Fri, 22 Apr 2022 03:37:00 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59eb437ecaf54263722ed5022a76bed608412ab4f94fc2aa7666d1653ddf23ce`  
		Last Modified: Fri, 22 Apr 2022 03:37:00 GMT  
		Size: 6.8 KB (6777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:e66b201216b5bebbd358365e3b3c977f306720c2dcd66dad04da85aeeb1ac9ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.5 MB (139536731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ff5e20d4ebd7fe8753ba3d0e7907e1a21a78868e5672e580c4951ab3f27b484`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:34:08 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 10:34:09 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 10:34:11 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 10:34:12 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 10:34:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:34:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:36:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:36:14 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:36:15 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:36:16 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:36:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:36:19 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:36:21 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa16fdd8f2b7ed887c119c9ca942715f9f1d4e3d0704344fe671cb921c3df6e6`  
		Last Modified: Fri, 22 Apr 2022 10:52:43 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc7852c7cfc5a89e8ec199e80be577caf5cb6278d52334b86888dad8b9a5d19`  
		Last Modified: Fri, 22 Apr 2022 10:53:01 GMT  
		Size: 93.3 MB (93323480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90b1dfdfe9bb649c7f4ce895a13e16f1cefed0bd1dca47c742a8dbb7f7ecd33`  
		Last Modified: Fri, 22 Apr 2022 10:52:43 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf93f3686f15dba104bc6ae5f4303b33340d33a2d4244c00f76ef218d9ded2d`  
		Last Modified: Fri, 22 Apr 2022 10:52:43 GMT  
		Size: 6.8 KB (6778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:b2805c726caa7af5fe4e44a3ade5afbbb7f7c780567c147cb36b5c7a363464b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127722709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a8b068ba5353d198e5fd7c34100da7ebc6771c257d75e23b80a211925de86aa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 00:39:34 GMT
ADD file:a5fe3b5fef5d5d99022e3a45894edf18c9e5f79c4be8020d61724cdc164256b3 in / 
# Fri, 22 Apr 2022 00:39:39 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:19:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:19:18 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:19:19 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:19:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:19:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:19:48 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:19:50 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:19:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:21:06 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 02:21:06 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 02:21:07 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 02:21:07 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 02:21:08 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:21:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:21:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:21:56 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:21:56 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:21:56 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:21:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:21:57 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:21:57 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:716ba34a9a0241d7bed3fa68865e745000f025af68d21dab7d692215c5074a58`  
		Last Modified: Tue, 19 Apr 2022 13:16:37 GMT  
		Size: 27.1 MB (27085718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bc8f5833a8cfe0537845df0a5d311b211ef889ed5d5e12ace1bd3eb30834c6`  
		Last Modified: Fri, 22 Apr 2022 02:25:50 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f4186175df1fdbe352452d13a8d94670ff3446432648e7b163e9a1c6a94d88`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 5.4 MB (5378760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea503bea58815ffe61d67ad911ffab94ad5a57e364db2126c3cb11e8f732d37`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 3.2 MB (3244218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76eb02e31628a4e2997c0f38de59eb7d09325086dd65b6b511c1e63c7fdd1692`  
		Last Modified: Fri, 22 Apr 2022 02:25:48 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34da960e123e0d72767a541ecf7347f03dfad9502e82a54cd713eb6c1e2d294b`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 2.2 MB (2183672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0ddf5cdd828e8ea2c4c69fedbb30d4aebf50bbc1c279fae4855faec077ae98`  
		Last Modified: Fri, 22 Apr 2022 02:25:47 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e906a7a4ca515f29ae2f9d042b9d50795a7722dff0e54711609032ab009449`  
		Last Modified: Fri, 22 Apr 2022 02:26:13 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8aa65ca376e03fed74f419a6a903362e83d6d4e1e1773ad67ad7183de7bbdf2`  
		Last Modified: Fri, 22 Apr 2022 02:26:26 GMT  
		Size: 89.8 MB (89815355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d48c43c28d400d613cd154b3e3182816a6e8b669d1fd7254e80bd5c51ae5f17`  
		Last Modified: Fri, 22 Apr 2022 02:26:13 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b5541b27b08286050b0bfd633e5710b2273e67032af256ca1137c955ccbd51`  
		Last Modified: Fri, 22 Apr 2022 02:26:13 GMT  
		Size: 6.8 KB (6775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2`

```console
$ docker pull mariadb@sha256:d56d83407f000dac7ad1f6229fcbb418cbd6e82c559943b657c606a5a6731f70
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2` - linux; amd64

```console
$ docker pull mariadb@sha256:8fcefbc6900276beaf7355e091c097ef57d2016e710fd202d325caeaae76d0a9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.3 MB (109317051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e64d2ba5ee25d4a070b1d24ef9e9ff239efce9a68854eef75e6bad1bd14d115`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Apr 2022 22:59:58 GMT
ADD file:5131314b62b7386e388b173018be7058491e96459344f78e6a2220771a65a2cd in / 
# Thu, 21 Apr 2022 22:59:58 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:53:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:53:40 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:53:40 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:53:53 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:53:53 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:54:01 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:54:01 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:54:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:54:02 GMT
ARG MARIADB_MAJOR=10.2
# Fri, 22 Apr 2022 02:54:02 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 22 Apr 2022 02:54:02 GMT
ARG MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 22 Apr 2022 02:54:03 GMT
ENV MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 22 Apr 2022 02:54:03 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
# Fri, 22 Apr 2022 02:54:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:54:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:54:37 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:54:38 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:54:38 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:54:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 02:54:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:54:38 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:54:38 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:88736512a147458c580cd28c969698561f236abba2ef04dbf0d7940cb3d7375e`  
		Last Modified: Tue, 19 Apr 2022 13:10:00 GMT  
		Size: 26.7 MB (26709883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2b6021c87a182e98ffd2863b419bb79abb17cbe79278678bd9fe625af2fdf0`  
		Last Modified: Fri, 22 Apr 2022 02:58:25 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:765f601f0e14bf00b76a7c869dda18bb82726fb91ec363e01da58c1c7b443a3c`  
		Last Modified: Fri, 22 Apr 2022 02:58:25 GMT  
		Size: 4.8 MB (4813346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01afffc2780257e621ca877a11e714b4a7c5c410f53d54498085dc40d6bfbc5`  
		Last Modified: Fri, 22 Apr 2022 02:58:23 GMT  
		Size: 3.6 MB (3553293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3da9b715df5cce68601eb2b10a167f2a0fce8580873de81baa04625b3630777`  
		Last Modified: Fri, 22 Apr 2022 02:58:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a2f060b97f61c909fac29a13ed6566d3582398b8aad97229e9cc5e8ff1b932`  
		Last Modified: Fri, 22 Apr 2022 02:58:23 GMT  
		Size: 1.6 MB (1583545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd15d91ff5e8df79d2baef2f494b7a3630ab71ff3873ffa33312779f13c2221`  
		Last Modified: Fri, 22 Apr 2022 02:58:22 GMT  
		Size: 5.2 KB (5171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbe407eaad30abd7fa7ea03f254a904ee2124fc3f320b3847677be56343ffb4`  
		Last Modified: Fri, 22 Apr 2022 02:58:20 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:866119df23a1053b37cbcf551ce1817f59f56a5201e1cefe3af83ac98b4fccfd`  
		Last Modified: Fri, 22 Apr 2022 02:58:31 GMT  
		Size: 72.6 MB (72639071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f565937cba773bda59caa0bfc5797250dedf1cbf2794053575300e6c8a306ffd`  
		Last Modified: Fri, 22 Apr 2022 02:58:20 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9d560a16832325d66ddca5bcd9b1e7d6026434f572a5965d8f6ff235e17bcdc`  
		Last Modified: Fri, 22 Apr 2022 02:58:20 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e6b018aab576555b6e0bfd1b1b382e6ef1eed43e7c6956456e42bf5acf235c`  
		Last Modified: Fri, 22 Apr 2022 02:58:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:1c9f0fcb1eb1ba416c80996780437b2ce79e7fe35a7181b19c215a709357e057
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.3 MB (104256493 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ac67686df123e98ac100937f16351e2ed91379fa2b020f53717143419040771`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:01 GMT
ADD file:5c0ff944739f8966900c55d6a77ba4ba6031b585962994b1684845dcd411c2fb in / 
# Fri, 22 Apr 2022 00:54:02 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:34:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 03:34:13 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:34:14 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 03:34:30 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 03:34:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 03:34:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:34:41 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 03:34:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 03:34:44 GMT
ARG MARIADB_MAJOR=10.2
# Fri, 22 Apr 2022 03:34:45 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 22 Apr 2022 03:34:46 GMT
ARG MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 22 Apr 2022 03:34:47 GMT
ENV MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 22 Apr 2022 03:34:48 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
# Fri, 22 Apr 2022 03:34:49 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 03:35:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 03:35:16 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 03:35:17 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 03:35:18 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 03:35:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 03:35:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 03:35:20 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 03:35:21 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:945d527fe80d536e4da70ea808f70d90bc97d7930c7ae2c61b5dabd1dba19e07`  
		Last Modified: Tue, 19 Apr 2022 13:10:40 GMT  
		Size: 23.7 MB (23734459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:526688af7e2add13ae8d736fa6943df49e915b287b820c3ecc1a4eaadd634771`  
		Last Modified: Fri, 22 Apr 2022 03:39:56 GMT  
		Size: 1.9 KB (1852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5e585d8b18453fd40b1abddebed16f2d4c7a8888b784b16cbfbfb113ea593c`  
		Last Modified: Fri, 22 Apr 2022 03:39:57 GMT  
		Size: 4.3 MB (4261564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b41ed4c94b830d808a09906d9ef6b5bcbcf061f2d8de544f31038c6669f81048`  
		Last Modified: Fri, 22 Apr 2022 03:39:55 GMT  
		Size: 3.2 MB (3207318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7564588601d09221509677911f1948155c0b8fbe3c826e97b5f8fd330ba6fa88`  
		Last Modified: Fri, 22 Apr 2022 03:39:54 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc302d085a4cbe3e8aead085ed4c551cf4f1a721a2ab643e21699d6e6ab950f`  
		Last Modified: Fri, 22 Apr 2022 03:39:55 GMT  
		Size: 1.5 MB (1530359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8104dd1631fc10394deef46910add4eee0c9dbf157957655deaeef04f92e57b9`  
		Last Modified: Fri, 22 Apr 2022 03:39:54 GMT  
		Size: 5.1 KB (5148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b5be6088cee7c79f8e6e6bbd83903fdbf83a85e86912f76b44b5b69f748518`  
		Last Modified: Fri, 22 Apr 2022 03:39:52 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7e84380d53b6a33f5bcde93311b2f87047c25a84d72f03e7f1886ef7780afa5`  
		Last Modified: Fri, 22 Apr 2022 03:40:03 GMT  
		Size: 71.5 MB (71504959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66e2f45215648b75332404bb488ea92aefed9ffbc25b913b78b4d29519855296`  
		Last Modified: Fri, 22 Apr 2022 03:39:52 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0575e7adbe8581a6c1ded4f9a6a6a2a2d277d63dad3031f1aeafd4bf9569e6f8`  
		Last Modified: Fri, 22 Apr 2022 03:39:51 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c606fbbd4f83d3117ebb71c3b5868f56232588156292d925c5938812f3cf7b4`  
		Last Modified: Fri, 22 Apr 2022 03:39:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2` - linux; ppc64le

```console
$ docker pull mariadb@sha256:dbc2601a0da428fc25e3d403550a438bfcc8fd9cfd1a781a09cd93a184437f38
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117723741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ea9e8a354784e1f553b08a6a4844b6ea7270601ceac2d5d2612d78f261b2bcf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 22 Apr 2022 08:07:45 GMT
ADD file:d5447cb8fcc4a12030e43cda74f87e1bec09c6d1093307e25164127500f5e0d9 in / 
# Fri, 22 Apr 2022 08:07:52 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:46:40 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:47:20 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:47:23 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:48:02 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:48:10 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:48:33 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:48:35 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:48:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:48:44 GMT
ARG MARIADB_MAJOR=10.2
# Fri, 22 Apr 2022 10:48:46 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 22 Apr 2022 10:48:48 GMT
ARG MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 22 Apr 2022 10:48:53 GMT
ENV MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 22 Apr 2022 10:48:56 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
# Fri, 22 Apr 2022 10:49:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:50:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:50:31 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:50:33 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:50:35 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:50:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 10:50:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:50:47 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:50:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:00422cde8b22ee0ff419263739625132280d08ffe78075ad3fb44dd003fab8e2`  
		Last Modified: Tue, 19 Apr 2022 13:12:05 GMT  
		Size: 30.4 MB (30442273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d73a75b263aa5a8efa4063fe2cb0f0d32acae619cdc553734e3417e30d6b27bd`  
		Last Modified: Fri, 22 Apr 2022 10:56:17 GMT  
		Size: 1.9 KB (1889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e177e7220472e4fb95ebe55fc7c4df30f6f8e906eedcf2b2de96ee46427ddb27`  
		Last Modified: Fri, 22 Apr 2022 10:56:17 GMT  
		Size: 5.6 MB (5630370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83f94b997942bb04b6262987f676f71c4fcb3405275aaffa1d93cb2761cd992`  
		Last Modified: Fri, 22 Apr 2022 10:56:17 GMT  
		Size: 3.5 MB (3533576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcaaa83e354a55bc8695e97ccbe18ad1983635ddffc077397d9dcab59232a6ca`  
		Last Modified: Fri, 22 Apr 2022 10:56:13 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0acb42415ce918b2ef55aa6ca28ff68811a35afd6397ddfad2745e9304fd51`  
		Last Modified: Fri, 22 Apr 2022 10:56:14 GMT  
		Size: 1.9 MB (1940450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37da9d58fff4c88201a1f7e6ca49ee9196e8ca997be6fe3f1fd8746e5c86e555`  
		Last Modified: Fri, 22 Apr 2022 10:56:13 GMT  
		Size: 5.2 KB (5172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d52f49a6d22ef0cdb764bed90008e3bb404704dd3a9d79bfb8553294c037909`  
		Last Modified: Fri, 22 Apr 2022 10:56:11 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e181baf563e9972873f24b1166c5a0da1afe97ef128d2bab41ef59b7443f9cf0`  
		Last Modified: Fri, 22 Apr 2022 10:56:25 GMT  
		Size: 76.2 MB (76159138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b11feb102b797ccfad139daa6fb6e80ad9b042348e827b5f259bd2a9c0e25fe3`  
		Last Modified: Fri, 22 Apr 2022 10:56:11 GMT  
		Size: 3.5 KB (3499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a56146d487a5b8c4b9b6e79fdf91674d8c023a9bef40ff2639db425f8000ac0`  
		Last Modified: Fri, 22 Apr 2022 10:56:11 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2563b23b40b5850bb08c2404b1e6ec15774ac8815fbba0b60d731bd0597820`  
		Last Modified: Fri, 22 Apr 2022 10:56:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2-bionic`

```console
$ docker pull mariadb@sha256:d56d83407f000dac7ad1f6229fcbb418cbd6e82c559943b657c606a5a6731f70
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2-bionic` - linux; amd64

```console
$ docker pull mariadb@sha256:8fcefbc6900276beaf7355e091c097ef57d2016e710fd202d325caeaae76d0a9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.3 MB (109317051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e64d2ba5ee25d4a070b1d24ef9e9ff239efce9a68854eef75e6bad1bd14d115`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Apr 2022 22:59:58 GMT
ADD file:5131314b62b7386e388b173018be7058491e96459344f78e6a2220771a65a2cd in / 
# Thu, 21 Apr 2022 22:59:58 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:53:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:53:40 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:53:40 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:53:53 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:53:53 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:54:01 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:54:01 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:54:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:54:02 GMT
ARG MARIADB_MAJOR=10.2
# Fri, 22 Apr 2022 02:54:02 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 22 Apr 2022 02:54:02 GMT
ARG MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 22 Apr 2022 02:54:03 GMT
ENV MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 22 Apr 2022 02:54:03 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
# Fri, 22 Apr 2022 02:54:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:54:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:54:37 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:54:38 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:54:38 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:54:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 02:54:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:54:38 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:54:38 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:88736512a147458c580cd28c969698561f236abba2ef04dbf0d7940cb3d7375e`  
		Last Modified: Tue, 19 Apr 2022 13:10:00 GMT  
		Size: 26.7 MB (26709883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2b6021c87a182e98ffd2863b419bb79abb17cbe79278678bd9fe625af2fdf0`  
		Last Modified: Fri, 22 Apr 2022 02:58:25 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:765f601f0e14bf00b76a7c869dda18bb82726fb91ec363e01da58c1c7b443a3c`  
		Last Modified: Fri, 22 Apr 2022 02:58:25 GMT  
		Size: 4.8 MB (4813346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01afffc2780257e621ca877a11e714b4a7c5c410f53d54498085dc40d6bfbc5`  
		Last Modified: Fri, 22 Apr 2022 02:58:23 GMT  
		Size: 3.6 MB (3553293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3da9b715df5cce68601eb2b10a167f2a0fce8580873de81baa04625b3630777`  
		Last Modified: Fri, 22 Apr 2022 02:58:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a2f060b97f61c909fac29a13ed6566d3582398b8aad97229e9cc5e8ff1b932`  
		Last Modified: Fri, 22 Apr 2022 02:58:23 GMT  
		Size: 1.6 MB (1583545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd15d91ff5e8df79d2baef2f494b7a3630ab71ff3873ffa33312779f13c2221`  
		Last Modified: Fri, 22 Apr 2022 02:58:22 GMT  
		Size: 5.2 KB (5171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbe407eaad30abd7fa7ea03f254a904ee2124fc3f320b3847677be56343ffb4`  
		Last Modified: Fri, 22 Apr 2022 02:58:20 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:866119df23a1053b37cbcf551ce1817f59f56a5201e1cefe3af83ac98b4fccfd`  
		Last Modified: Fri, 22 Apr 2022 02:58:31 GMT  
		Size: 72.6 MB (72639071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f565937cba773bda59caa0bfc5797250dedf1cbf2794053575300e6c8a306ffd`  
		Last Modified: Fri, 22 Apr 2022 02:58:20 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9d560a16832325d66ddca5bcd9b1e7d6026434f572a5965d8f6ff235e17bcdc`  
		Last Modified: Fri, 22 Apr 2022 02:58:20 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e6b018aab576555b6e0bfd1b1b382e6ef1eed43e7c6956456e42bf5acf235c`  
		Last Modified: Fri, 22 Apr 2022 02:58:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2-bionic` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:1c9f0fcb1eb1ba416c80996780437b2ce79e7fe35a7181b19c215a709357e057
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.3 MB (104256493 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ac67686df123e98ac100937f16351e2ed91379fa2b020f53717143419040771`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:01 GMT
ADD file:5c0ff944739f8966900c55d6a77ba4ba6031b585962994b1684845dcd411c2fb in / 
# Fri, 22 Apr 2022 00:54:02 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:34:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 03:34:13 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:34:14 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 03:34:30 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 03:34:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 03:34:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:34:41 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 03:34:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 03:34:44 GMT
ARG MARIADB_MAJOR=10.2
# Fri, 22 Apr 2022 03:34:45 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 22 Apr 2022 03:34:46 GMT
ARG MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 22 Apr 2022 03:34:47 GMT
ENV MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 22 Apr 2022 03:34:48 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
# Fri, 22 Apr 2022 03:34:49 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 03:35:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 03:35:16 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 03:35:17 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 03:35:18 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 03:35:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 03:35:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 03:35:20 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 03:35:21 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:945d527fe80d536e4da70ea808f70d90bc97d7930c7ae2c61b5dabd1dba19e07`  
		Last Modified: Tue, 19 Apr 2022 13:10:40 GMT  
		Size: 23.7 MB (23734459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:526688af7e2add13ae8d736fa6943df49e915b287b820c3ecc1a4eaadd634771`  
		Last Modified: Fri, 22 Apr 2022 03:39:56 GMT  
		Size: 1.9 KB (1852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5e585d8b18453fd40b1abddebed16f2d4c7a8888b784b16cbfbfb113ea593c`  
		Last Modified: Fri, 22 Apr 2022 03:39:57 GMT  
		Size: 4.3 MB (4261564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b41ed4c94b830d808a09906d9ef6b5bcbcf061f2d8de544f31038c6669f81048`  
		Last Modified: Fri, 22 Apr 2022 03:39:55 GMT  
		Size: 3.2 MB (3207318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7564588601d09221509677911f1948155c0b8fbe3c826e97b5f8fd330ba6fa88`  
		Last Modified: Fri, 22 Apr 2022 03:39:54 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc302d085a4cbe3e8aead085ed4c551cf4f1a721a2ab643e21699d6e6ab950f`  
		Last Modified: Fri, 22 Apr 2022 03:39:55 GMT  
		Size: 1.5 MB (1530359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8104dd1631fc10394deef46910add4eee0c9dbf157957655deaeef04f92e57b9`  
		Last Modified: Fri, 22 Apr 2022 03:39:54 GMT  
		Size: 5.1 KB (5148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b5be6088cee7c79f8e6e6bbd83903fdbf83a85e86912f76b44b5b69f748518`  
		Last Modified: Fri, 22 Apr 2022 03:39:52 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7e84380d53b6a33f5bcde93311b2f87047c25a84d72f03e7f1886ef7780afa5`  
		Last Modified: Fri, 22 Apr 2022 03:40:03 GMT  
		Size: 71.5 MB (71504959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66e2f45215648b75332404bb488ea92aefed9ffbc25b913b78b4d29519855296`  
		Last Modified: Fri, 22 Apr 2022 03:39:52 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0575e7adbe8581a6c1ded4f9a6a6a2a2d277d63dad3031f1aeafd4bf9569e6f8`  
		Last Modified: Fri, 22 Apr 2022 03:39:51 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c606fbbd4f83d3117ebb71c3b5868f56232588156292d925c5938812f3cf7b4`  
		Last Modified: Fri, 22 Apr 2022 03:39:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2-bionic` - linux; ppc64le

```console
$ docker pull mariadb@sha256:dbc2601a0da428fc25e3d403550a438bfcc8fd9cfd1a781a09cd93a184437f38
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117723741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ea9e8a354784e1f553b08a6a4844b6ea7270601ceac2d5d2612d78f261b2bcf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 22 Apr 2022 08:07:45 GMT
ADD file:d5447cb8fcc4a12030e43cda74f87e1bec09c6d1093307e25164127500f5e0d9 in / 
# Fri, 22 Apr 2022 08:07:52 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:46:40 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:47:20 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:47:23 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:48:02 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:48:10 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:48:33 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:48:35 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:48:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:48:44 GMT
ARG MARIADB_MAJOR=10.2
# Fri, 22 Apr 2022 10:48:46 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 22 Apr 2022 10:48:48 GMT
ARG MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 22 Apr 2022 10:48:53 GMT
ENV MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 22 Apr 2022 10:48:56 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
# Fri, 22 Apr 2022 10:49:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:50:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:50:31 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:50:33 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:50:35 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:50:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 10:50:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:50:47 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:50:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:00422cde8b22ee0ff419263739625132280d08ffe78075ad3fb44dd003fab8e2`  
		Last Modified: Tue, 19 Apr 2022 13:12:05 GMT  
		Size: 30.4 MB (30442273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d73a75b263aa5a8efa4063fe2cb0f0d32acae619cdc553734e3417e30d6b27bd`  
		Last Modified: Fri, 22 Apr 2022 10:56:17 GMT  
		Size: 1.9 KB (1889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e177e7220472e4fb95ebe55fc7c4df30f6f8e906eedcf2b2de96ee46427ddb27`  
		Last Modified: Fri, 22 Apr 2022 10:56:17 GMT  
		Size: 5.6 MB (5630370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83f94b997942bb04b6262987f676f71c4fcb3405275aaffa1d93cb2761cd992`  
		Last Modified: Fri, 22 Apr 2022 10:56:17 GMT  
		Size: 3.5 MB (3533576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcaaa83e354a55bc8695e97ccbe18ad1983635ddffc077397d9dcab59232a6ca`  
		Last Modified: Fri, 22 Apr 2022 10:56:13 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0acb42415ce918b2ef55aa6ca28ff68811a35afd6397ddfad2745e9304fd51`  
		Last Modified: Fri, 22 Apr 2022 10:56:14 GMT  
		Size: 1.9 MB (1940450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37da9d58fff4c88201a1f7e6ca49ee9196e8ca997be6fe3f1fd8746e5c86e555`  
		Last Modified: Fri, 22 Apr 2022 10:56:13 GMT  
		Size: 5.2 KB (5172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d52f49a6d22ef0cdb764bed90008e3bb404704dd3a9d79bfb8553294c037909`  
		Last Modified: Fri, 22 Apr 2022 10:56:11 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e181baf563e9972873f24b1166c5a0da1afe97ef128d2bab41ef59b7443f9cf0`  
		Last Modified: Fri, 22 Apr 2022 10:56:25 GMT  
		Size: 76.2 MB (76159138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b11feb102b797ccfad139daa6fb6e80ad9b042348e827b5f259bd2a9c0e25fe3`  
		Last Modified: Fri, 22 Apr 2022 10:56:11 GMT  
		Size: 3.5 KB (3499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a56146d487a5b8c4b9b6e79fdf91674d8c023a9bef40ff2639db425f8000ac0`  
		Last Modified: Fri, 22 Apr 2022 10:56:11 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2563b23b40b5850bb08c2404b1e6ec15774ac8815fbba0b60d731bd0597820`  
		Last Modified: Fri, 22 Apr 2022 10:56:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2.43`

```console
$ docker pull mariadb@sha256:d56d83407f000dac7ad1f6229fcbb418cbd6e82c559943b657c606a5a6731f70
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2.43` - linux; amd64

```console
$ docker pull mariadb@sha256:8fcefbc6900276beaf7355e091c097ef57d2016e710fd202d325caeaae76d0a9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.3 MB (109317051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e64d2ba5ee25d4a070b1d24ef9e9ff239efce9a68854eef75e6bad1bd14d115`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Apr 2022 22:59:58 GMT
ADD file:5131314b62b7386e388b173018be7058491e96459344f78e6a2220771a65a2cd in / 
# Thu, 21 Apr 2022 22:59:58 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:53:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:53:40 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:53:40 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:53:53 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:53:53 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:54:01 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:54:01 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:54:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:54:02 GMT
ARG MARIADB_MAJOR=10.2
# Fri, 22 Apr 2022 02:54:02 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 22 Apr 2022 02:54:02 GMT
ARG MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 22 Apr 2022 02:54:03 GMT
ENV MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 22 Apr 2022 02:54:03 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
# Fri, 22 Apr 2022 02:54:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:54:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:54:37 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:54:38 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:54:38 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:54:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 02:54:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:54:38 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:54:38 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:88736512a147458c580cd28c969698561f236abba2ef04dbf0d7940cb3d7375e`  
		Last Modified: Tue, 19 Apr 2022 13:10:00 GMT  
		Size: 26.7 MB (26709883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2b6021c87a182e98ffd2863b419bb79abb17cbe79278678bd9fe625af2fdf0`  
		Last Modified: Fri, 22 Apr 2022 02:58:25 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:765f601f0e14bf00b76a7c869dda18bb82726fb91ec363e01da58c1c7b443a3c`  
		Last Modified: Fri, 22 Apr 2022 02:58:25 GMT  
		Size: 4.8 MB (4813346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01afffc2780257e621ca877a11e714b4a7c5c410f53d54498085dc40d6bfbc5`  
		Last Modified: Fri, 22 Apr 2022 02:58:23 GMT  
		Size: 3.6 MB (3553293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3da9b715df5cce68601eb2b10a167f2a0fce8580873de81baa04625b3630777`  
		Last Modified: Fri, 22 Apr 2022 02:58:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a2f060b97f61c909fac29a13ed6566d3582398b8aad97229e9cc5e8ff1b932`  
		Last Modified: Fri, 22 Apr 2022 02:58:23 GMT  
		Size: 1.6 MB (1583545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd15d91ff5e8df79d2baef2f494b7a3630ab71ff3873ffa33312779f13c2221`  
		Last Modified: Fri, 22 Apr 2022 02:58:22 GMT  
		Size: 5.2 KB (5171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbe407eaad30abd7fa7ea03f254a904ee2124fc3f320b3847677be56343ffb4`  
		Last Modified: Fri, 22 Apr 2022 02:58:20 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:866119df23a1053b37cbcf551ce1817f59f56a5201e1cefe3af83ac98b4fccfd`  
		Last Modified: Fri, 22 Apr 2022 02:58:31 GMT  
		Size: 72.6 MB (72639071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f565937cba773bda59caa0bfc5797250dedf1cbf2794053575300e6c8a306ffd`  
		Last Modified: Fri, 22 Apr 2022 02:58:20 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9d560a16832325d66ddca5bcd9b1e7d6026434f572a5965d8f6ff235e17bcdc`  
		Last Modified: Fri, 22 Apr 2022 02:58:20 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e6b018aab576555b6e0bfd1b1b382e6ef1eed43e7c6956456e42bf5acf235c`  
		Last Modified: Fri, 22 Apr 2022 02:58:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2.43` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:1c9f0fcb1eb1ba416c80996780437b2ce79e7fe35a7181b19c215a709357e057
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.3 MB (104256493 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ac67686df123e98ac100937f16351e2ed91379fa2b020f53717143419040771`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:01 GMT
ADD file:5c0ff944739f8966900c55d6a77ba4ba6031b585962994b1684845dcd411c2fb in / 
# Fri, 22 Apr 2022 00:54:02 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:34:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 03:34:13 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:34:14 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 03:34:30 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 03:34:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 03:34:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:34:41 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 03:34:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 03:34:44 GMT
ARG MARIADB_MAJOR=10.2
# Fri, 22 Apr 2022 03:34:45 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 22 Apr 2022 03:34:46 GMT
ARG MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 22 Apr 2022 03:34:47 GMT
ENV MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 22 Apr 2022 03:34:48 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
# Fri, 22 Apr 2022 03:34:49 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 03:35:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 03:35:16 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 03:35:17 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 03:35:18 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 03:35:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 03:35:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 03:35:20 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 03:35:21 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:945d527fe80d536e4da70ea808f70d90bc97d7930c7ae2c61b5dabd1dba19e07`  
		Last Modified: Tue, 19 Apr 2022 13:10:40 GMT  
		Size: 23.7 MB (23734459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:526688af7e2add13ae8d736fa6943df49e915b287b820c3ecc1a4eaadd634771`  
		Last Modified: Fri, 22 Apr 2022 03:39:56 GMT  
		Size: 1.9 KB (1852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5e585d8b18453fd40b1abddebed16f2d4c7a8888b784b16cbfbfb113ea593c`  
		Last Modified: Fri, 22 Apr 2022 03:39:57 GMT  
		Size: 4.3 MB (4261564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b41ed4c94b830d808a09906d9ef6b5bcbcf061f2d8de544f31038c6669f81048`  
		Last Modified: Fri, 22 Apr 2022 03:39:55 GMT  
		Size: 3.2 MB (3207318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7564588601d09221509677911f1948155c0b8fbe3c826e97b5f8fd330ba6fa88`  
		Last Modified: Fri, 22 Apr 2022 03:39:54 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc302d085a4cbe3e8aead085ed4c551cf4f1a721a2ab643e21699d6e6ab950f`  
		Last Modified: Fri, 22 Apr 2022 03:39:55 GMT  
		Size: 1.5 MB (1530359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8104dd1631fc10394deef46910add4eee0c9dbf157957655deaeef04f92e57b9`  
		Last Modified: Fri, 22 Apr 2022 03:39:54 GMT  
		Size: 5.1 KB (5148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b5be6088cee7c79f8e6e6bbd83903fdbf83a85e86912f76b44b5b69f748518`  
		Last Modified: Fri, 22 Apr 2022 03:39:52 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7e84380d53b6a33f5bcde93311b2f87047c25a84d72f03e7f1886ef7780afa5`  
		Last Modified: Fri, 22 Apr 2022 03:40:03 GMT  
		Size: 71.5 MB (71504959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66e2f45215648b75332404bb488ea92aefed9ffbc25b913b78b4d29519855296`  
		Last Modified: Fri, 22 Apr 2022 03:39:52 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0575e7adbe8581a6c1ded4f9a6a6a2a2d277d63dad3031f1aeafd4bf9569e6f8`  
		Last Modified: Fri, 22 Apr 2022 03:39:51 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c606fbbd4f83d3117ebb71c3b5868f56232588156292d925c5938812f3cf7b4`  
		Last Modified: Fri, 22 Apr 2022 03:39:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2.43` - linux; ppc64le

```console
$ docker pull mariadb@sha256:dbc2601a0da428fc25e3d403550a438bfcc8fd9cfd1a781a09cd93a184437f38
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117723741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ea9e8a354784e1f553b08a6a4844b6ea7270601ceac2d5d2612d78f261b2bcf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 22 Apr 2022 08:07:45 GMT
ADD file:d5447cb8fcc4a12030e43cda74f87e1bec09c6d1093307e25164127500f5e0d9 in / 
# Fri, 22 Apr 2022 08:07:52 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:46:40 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:47:20 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:47:23 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:48:02 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:48:10 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:48:33 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:48:35 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:48:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:48:44 GMT
ARG MARIADB_MAJOR=10.2
# Fri, 22 Apr 2022 10:48:46 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 22 Apr 2022 10:48:48 GMT
ARG MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 22 Apr 2022 10:48:53 GMT
ENV MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 22 Apr 2022 10:48:56 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
# Fri, 22 Apr 2022 10:49:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:50:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:50:31 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:50:33 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:50:35 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:50:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 10:50:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:50:47 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:50:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:00422cde8b22ee0ff419263739625132280d08ffe78075ad3fb44dd003fab8e2`  
		Last Modified: Tue, 19 Apr 2022 13:12:05 GMT  
		Size: 30.4 MB (30442273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d73a75b263aa5a8efa4063fe2cb0f0d32acae619cdc553734e3417e30d6b27bd`  
		Last Modified: Fri, 22 Apr 2022 10:56:17 GMT  
		Size: 1.9 KB (1889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e177e7220472e4fb95ebe55fc7c4df30f6f8e906eedcf2b2de96ee46427ddb27`  
		Last Modified: Fri, 22 Apr 2022 10:56:17 GMT  
		Size: 5.6 MB (5630370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83f94b997942bb04b6262987f676f71c4fcb3405275aaffa1d93cb2761cd992`  
		Last Modified: Fri, 22 Apr 2022 10:56:17 GMT  
		Size: 3.5 MB (3533576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcaaa83e354a55bc8695e97ccbe18ad1983635ddffc077397d9dcab59232a6ca`  
		Last Modified: Fri, 22 Apr 2022 10:56:13 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0acb42415ce918b2ef55aa6ca28ff68811a35afd6397ddfad2745e9304fd51`  
		Last Modified: Fri, 22 Apr 2022 10:56:14 GMT  
		Size: 1.9 MB (1940450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37da9d58fff4c88201a1f7e6ca49ee9196e8ca997be6fe3f1fd8746e5c86e555`  
		Last Modified: Fri, 22 Apr 2022 10:56:13 GMT  
		Size: 5.2 KB (5172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d52f49a6d22ef0cdb764bed90008e3bb404704dd3a9d79bfb8553294c037909`  
		Last Modified: Fri, 22 Apr 2022 10:56:11 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e181baf563e9972873f24b1166c5a0da1afe97ef128d2bab41ef59b7443f9cf0`  
		Last Modified: Fri, 22 Apr 2022 10:56:25 GMT  
		Size: 76.2 MB (76159138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b11feb102b797ccfad139daa6fb6e80ad9b042348e827b5f259bd2a9c0e25fe3`  
		Last Modified: Fri, 22 Apr 2022 10:56:11 GMT  
		Size: 3.5 KB (3499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a56146d487a5b8c4b9b6e79fdf91674d8c023a9bef40ff2639db425f8000ac0`  
		Last Modified: Fri, 22 Apr 2022 10:56:11 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2563b23b40b5850bb08c2404b1e6ec15774ac8815fbba0b60d731bd0597820`  
		Last Modified: Fri, 22 Apr 2022 10:56:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2.43-bionic`

```console
$ docker pull mariadb@sha256:d56d83407f000dac7ad1f6229fcbb418cbd6e82c559943b657c606a5a6731f70
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2.43-bionic` - linux; amd64

```console
$ docker pull mariadb@sha256:8fcefbc6900276beaf7355e091c097ef57d2016e710fd202d325caeaae76d0a9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.3 MB (109317051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e64d2ba5ee25d4a070b1d24ef9e9ff239efce9a68854eef75e6bad1bd14d115`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Apr 2022 22:59:58 GMT
ADD file:5131314b62b7386e388b173018be7058491e96459344f78e6a2220771a65a2cd in / 
# Thu, 21 Apr 2022 22:59:58 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:53:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:53:40 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:53:40 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:53:53 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:53:53 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:54:01 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:54:01 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:54:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:54:02 GMT
ARG MARIADB_MAJOR=10.2
# Fri, 22 Apr 2022 02:54:02 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 22 Apr 2022 02:54:02 GMT
ARG MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 22 Apr 2022 02:54:03 GMT
ENV MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 22 Apr 2022 02:54:03 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
# Fri, 22 Apr 2022 02:54:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:54:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:54:37 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:54:38 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:54:38 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:54:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 02:54:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:54:38 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:54:38 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:88736512a147458c580cd28c969698561f236abba2ef04dbf0d7940cb3d7375e`  
		Last Modified: Tue, 19 Apr 2022 13:10:00 GMT  
		Size: 26.7 MB (26709883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2b6021c87a182e98ffd2863b419bb79abb17cbe79278678bd9fe625af2fdf0`  
		Last Modified: Fri, 22 Apr 2022 02:58:25 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:765f601f0e14bf00b76a7c869dda18bb82726fb91ec363e01da58c1c7b443a3c`  
		Last Modified: Fri, 22 Apr 2022 02:58:25 GMT  
		Size: 4.8 MB (4813346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01afffc2780257e621ca877a11e714b4a7c5c410f53d54498085dc40d6bfbc5`  
		Last Modified: Fri, 22 Apr 2022 02:58:23 GMT  
		Size: 3.6 MB (3553293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3da9b715df5cce68601eb2b10a167f2a0fce8580873de81baa04625b3630777`  
		Last Modified: Fri, 22 Apr 2022 02:58:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a2f060b97f61c909fac29a13ed6566d3582398b8aad97229e9cc5e8ff1b932`  
		Last Modified: Fri, 22 Apr 2022 02:58:23 GMT  
		Size: 1.6 MB (1583545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd15d91ff5e8df79d2baef2f494b7a3630ab71ff3873ffa33312779f13c2221`  
		Last Modified: Fri, 22 Apr 2022 02:58:22 GMT  
		Size: 5.2 KB (5171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbe407eaad30abd7fa7ea03f254a904ee2124fc3f320b3847677be56343ffb4`  
		Last Modified: Fri, 22 Apr 2022 02:58:20 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:866119df23a1053b37cbcf551ce1817f59f56a5201e1cefe3af83ac98b4fccfd`  
		Last Modified: Fri, 22 Apr 2022 02:58:31 GMT  
		Size: 72.6 MB (72639071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f565937cba773bda59caa0bfc5797250dedf1cbf2794053575300e6c8a306ffd`  
		Last Modified: Fri, 22 Apr 2022 02:58:20 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9d560a16832325d66ddca5bcd9b1e7d6026434f572a5965d8f6ff235e17bcdc`  
		Last Modified: Fri, 22 Apr 2022 02:58:20 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e6b018aab576555b6e0bfd1b1b382e6ef1eed43e7c6956456e42bf5acf235c`  
		Last Modified: Fri, 22 Apr 2022 02:58:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2.43-bionic` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:1c9f0fcb1eb1ba416c80996780437b2ce79e7fe35a7181b19c215a709357e057
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.3 MB (104256493 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ac67686df123e98ac100937f16351e2ed91379fa2b020f53717143419040771`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:01 GMT
ADD file:5c0ff944739f8966900c55d6a77ba4ba6031b585962994b1684845dcd411c2fb in / 
# Fri, 22 Apr 2022 00:54:02 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:34:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 03:34:13 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:34:14 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 03:34:30 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 03:34:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 03:34:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:34:41 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 03:34:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 03:34:44 GMT
ARG MARIADB_MAJOR=10.2
# Fri, 22 Apr 2022 03:34:45 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 22 Apr 2022 03:34:46 GMT
ARG MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 22 Apr 2022 03:34:47 GMT
ENV MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 22 Apr 2022 03:34:48 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
# Fri, 22 Apr 2022 03:34:49 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 03:35:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 03:35:16 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 03:35:17 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 03:35:18 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 03:35:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 03:35:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 03:35:20 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 03:35:21 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:945d527fe80d536e4da70ea808f70d90bc97d7930c7ae2c61b5dabd1dba19e07`  
		Last Modified: Tue, 19 Apr 2022 13:10:40 GMT  
		Size: 23.7 MB (23734459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:526688af7e2add13ae8d736fa6943df49e915b287b820c3ecc1a4eaadd634771`  
		Last Modified: Fri, 22 Apr 2022 03:39:56 GMT  
		Size: 1.9 KB (1852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5e585d8b18453fd40b1abddebed16f2d4c7a8888b784b16cbfbfb113ea593c`  
		Last Modified: Fri, 22 Apr 2022 03:39:57 GMT  
		Size: 4.3 MB (4261564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b41ed4c94b830d808a09906d9ef6b5bcbcf061f2d8de544f31038c6669f81048`  
		Last Modified: Fri, 22 Apr 2022 03:39:55 GMT  
		Size: 3.2 MB (3207318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7564588601d09221509677911f1948155c0b8fbe3c826e97b5f8fd330ba6fa88`  
		Last Modified: Fri, 22 Apr 2022 03:39:54 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc302d085a4cbe3e8aead085ed4c551cf4f1a721a2ab643e21699d6e6ab950f`  
		Last Modified: Fri, 22 Apr 2022 03:39:55 GMT  
		Size: 1.5 MB (1530359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8104dd1631fc10394deef46910add4eee0c9dbf157957655deaeef04f92e57b9`  
		Last Modified: Fri, 22 Apr 2022 03:39:54 GMT  
		Size: 5.1 KB (5148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b5be6088cee7c79f8e6e6bbd83903fdbf83a85e86912f76b44b5b69f748518`  
		Last Modified: Fri, 22 Apr 2022 03:39:52 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7e84380d53b6a33f5bcde93311b2f87047c25a84d72f03e7f1886ef7780afa5`  
		Last Modified: Fri, 22 Apr 2022 03:40:03 GMT  
		Size: 71.5 MB (71504959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66e2f45215648b75332404bb488ea92aefed9ffbc25b913b78b4d29519855296`  
		Last Modified: Fri, 22 Apr 2022 03:39:52 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0575e7adbe8581a6c1ded4f9a6a6a2a2d277d63dad3031f1aeafd4bf9569e6f8`  
		Last Modified: Fri, 22 Apr 2022 03:39:51 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c606fbbd4f83d3117ebb71c3b5868f56232588156292d925c5938812f3cf7b4`  
		Last Modified: Fri, 22 Apr 2022 03:39:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2.43-bionic` - linux; ppc64le

```console
$ docker pull mariadb@sha256:dbc2601a0da428fc25e3d403550a438bfcc8fd9cfd1a781a09cd93a184437f38
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117723741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ea9e8a354784e1f553b08a6a4844b6ea7270601ceac2d5d2612d78f261b2bcf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 22 Apr 2022 08:07:45 GMT
ADD file:d5447cb8fcc4a12030e43cda74f87e1bec09c6d1093307e25164127500f5e0d9 in / 
# Fri, 22 Apr 2022 08:07:52 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:46:40 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:47:20 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:47:23 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:48:02 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:48:10 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:48:33 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:48:35 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:48:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:48:44 GMT
ARG MARIADB_MAJOR=10.2
# Fri, 22 Apr 2022 10:48:46 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 22 Apr 2022 10:48:48 GMT
ARG MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 22 Apr 2022 10:48:53 GMT
ENV MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 22 Apr 2022 10:48:56 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
# Fri, 22 Apr 2022 10:49:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:50:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:50:31 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:50:33 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:50:35 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:50:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 10:50:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:50:47 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:50:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:00422cde8b22ee0ff419263739625132280d08ffe78075ad3fb44dd003fab8e2`  
		Last Modified: Tue, 19 Apr 2022 13:12:05 GMT  
		Size: 30.4 MB (30442273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d73a75b263aa5a8efa4063fe2cb0f0d32acae619cdc553734e3417e30d6b27bd`  
		Last Modified: Fri, 22 Apr 2022 10:56:17 GMT  
		Size: 1.9 KB (1889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e177e7220472e4fb95ebe55fc7c4df30f6f8e906eedcf2b2de96ee46427ddb27`  
		Last Modified: Fri, 22 Apr 2022 10:56:17 GMT  
		Size: 5.6 MB (5630370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83f94b997942bb04b6262987f676f71c4fcb3405275aaffa1d93cb2761cd992`  
		Last Modified: Fri, 22 Apr 2022 10:56:17 GMT  
		Size: 3.5 MB (3533576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcaaa83e354a55bc8695e97ccbe18ad1983635ddffc077397d9dcab59232a6ca`  
		Last Modified: Fri, 22 Apr 2022 10:56:13 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0acb42415ce918b2ef55aa6ca28ff68811a35afd6397ddfad2745e9304fd51`  
		Last Modified: Fri, 22 Apr 2022 10:56:14 GMT  
		Size: 1.9 MB (1940450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37da9d58fff4c88201a1f7e6ca49ee9196e8ca997be6fe3f1fd8746e5c86e555`  
		Last Modified: Fri, 22 Apr 2022 10:56:13 GMT  
		Size: 5.2 KB (5172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d52f49a6d22ef0cdb764bed90008e3bb404704dd3a9d79bfb8553294c037909`  
		Last Modified: Fri, 22 Apr 2022 10:56:11 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e181baf563e9972873f24b1166c5a0da1afe97ef128d2bab41ef59b7443f9cf0`  
		Last Modified: Fri, 22 Apr 2022 10:56:25 GMT  
		Size: 76.2 MB (76159138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b11feb102b797ccfad139daa6fb6e80ad9b042348e827b5f259bd2a9c0e25fe3`  
		Last Modified: Fri, 22 Apr 2022 10:56:11 GMT  
		Size: 3.5 KB (3499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a56146d487a5b8c4b9b6e79fdf91674d8c023a9bef40ff2639db425f8000ac0`  
		Last Modified: Fri, 22 Apr 2022 10:56:11 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2563b23b40b5850bb08c2404b1e6ec15774ac8815fbba0b60d731bd0597820`  
		Last Modified: Fri, 22 Apr 2022 10:56:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3`

```console
$ docker pull mariadb@sha256:114febf5009acb4f4f777b21ff2097c572ded2120a95d6a7aafb7e72d849e17c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3` - linux; amd64

```console
$ docker pull mariadb@sha256:3fadf7ebd60b5b879e6f9e2cd46c782e18c64ec78a5e1ddd5e587a779364933d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.1 MB (120117709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82643bd90d5e12d8dcc3923c5037bace1b14063504a971ec0498cf5e162bf61f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:52:58 GMT
ARG MARIADB_MAJOR=10.3
# Fri, 22 Apr 2022 02:52:58 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 22 Apr 2022 02:52:59 GMT
ARG MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 22 Apr 2022 02:52:59 GMT
ENV MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 22 Apr 2022 02:52:59 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:52:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:53:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:53:26 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:53:26 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:53:26 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:53:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 02:53:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:53:27 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:53:27 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7801d5a27d87a0a14725087a02be10adf3637adbacf9636d809795ed70a34ce`  
		Last Modified: Fri, 22 Apr 2022 02:57:52 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa7f812281a340552e5374feef34fd9a2563c703d0193aad89c90cf3fe9fe39a`  
		Last Modified: Fri, 22 Apr 2022 02:58:04 GMT  
		Size: 80.2 MB (80191115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b0502732e9ee8013217b08ed97cb6199c16b413212459861470162d7a1ea6d`  
		Last Modified: Fri, 22 Apr 2022 02:57:53 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38fba0e3193601cd73bca932f9f778413d041e214ebad8a4a0b24f5ce35ec76d`  
		Last Modified: Fri, 22 Apr 2022 02:57:53 GMT  
		Size: 6.8 KB (6772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22c2c705d6abdc6c36ec9ad28a43a47c9d00d5c2aa196ceee150b34001faaad4`  
		Last Modified: Fri, 22 Apr 2022 02:57:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:b0a3468d4dde2bcc2c7999df4171d3103fe48ca55ceb859595bc017605245b37
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117607783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8114a9faba606cea1bb35dd16d5898781167d329e63deacd215a765ee19fc419`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:29:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 03:29:22 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:23 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 03:29:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 03:29:39 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 03:29:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:48 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 03:29:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 03:33:18 GMT
ARG MARIADB_MAJOR=10.3
# Fri, 22 Apr 2022 03:33:19 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 22 Apr 2022 03:33:20 GMT
ARG MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 22 Apr 2022 03:33:21 GMT
ENV MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 22 Apr 2022 03:33:22 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 03:33:23 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 03:33:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 03:33:49 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 03:33:50 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 03:33:51 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 03:33:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 03:33:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 03:33:53 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 03:33:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7061769dfb44ec758f6d367a5d4ea0ae9e6f03ca107b7f4ee4b2419e2ae693b`  
		Last Modified: Fri, 22 Apr 2022 03:36:31 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc0a8ec71ebae8e12eafc6106df54088463cc344135ebd19dc41f331e0ed6f2`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 5.3 MB (5320310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87bc30abcdec1bcda27933f56dac195031b448391d01eb7ed27fe77b389117e7`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 3.4 MB (3370037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c05e5ca55fe31dfae11772d53c4dd507f38b7e27ba3b7b878954b5c1d9697f87`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617ab90f9424ca5c02f763590888d7804d6be962990b9f82717351743533c8f0`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 2.2 MB (2202477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bbb7ad258365e117ef11517dc6c0beadccf14acb57fba68848b61d4e0044111`  
		Last Modified: Fri, 22 Apr 2022 03:36:26 GMT  
		Size: 2.5 KB (2469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75d58a2e8d323795646bfacabb25905ae6059f68898ba6a1b4e2bc54dc38d56d`  
		Last Modified: Fri, 22 Apr 2022 03:39:21 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1384173381c8a4fb5181fa3fbb0064e82bbcd4f030ec1b3aaa1e4f5316093b9c`  
		Last Modified: Fri, 22 Apr 2022 03:39:34 GMT  
		Size: 79.5 MB (79530796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3aab6dbbd81fafbc2878c10cf601c0a59dd4b03e482f90844e4af59db46a1f1`  
		Last Modified: Fri, 22 Apr 2022 03:39:21 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93d0ae64b3b2dabde027d3920bfbd5c50903fab69b84da305a3f69e8b9e0bd70`  
		Last Modified: Fri, 22 Apr 2022 03:39:21 GMT  
		Size: 6.8 KB (6769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b800dfda623d3ab156ad3e143ce76e259219c0c69e171b41dbb1e465655a6dc3`  
		Last Modified: Fri, 22 Apr 2022 03:39:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3` - linux; ppc64le

```console
$ docker pull mariadb@sha256:87b61f8379eb65a704fd612759413f1078a26d40e8d2bea31075c10e8e5c64c1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.0 MB (131005136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23d224c4121a61e5b5ed36485d24161c66509f7d3e5726444beca6059032c3a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:43:50 GMT
ARG MARIADB_MAJOR=10.3
# Fri, 22 Apr 2022 10:43:52 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 22 Apr 2022 10:43:55 GMT
ARG MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 22 Apr 2022 10:43:58 GMT
ENV MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 22 Apr 2022 10:44:01 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:44:07 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:45:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:45:50 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:45:54 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:45:56 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:46:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 10:46:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:46:18 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:46:21 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e69825db8399a8e8531089312f836140b3c2e202cd9e9f8d3e33f2862140bf7`  
		Last Modified: Fri, 22 Apr 2022 10:55:34 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f3a5eacd4b3852d2a6df25f3dcdbe1a2350a97ac7a75e7f6fef19cc6ce125d`  
		Last Modified: Fri, 22 Apr 2022 10:55:50 GMT  
		Size: 84.8 MB (84791769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3127a0e21401b0104caee55b024a479dcacb37031f547853f5f157d65bb3afe1`  
		Last Modified: Fri, 22 Apr 2022 10:55:34 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a468c88d3fc33c46a0b0bfc86b2251de989fffa4efb7f03fddd35192bd88acd`  
		Last Modified: Fri, 22 Apr 2022 10:55:34 GMT  
		Size: 6.8 KB (6772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413ee9ba3b320da907982067cc2460e9ae78998da3271ca620f0e122a465d7c5`  
		Last Modified: Fri, 22 Apr 2022 10:55:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3-focal`

```console
$ docker pull mariadb@sha256:114febf5009acb4f4f777b21ff2097c572ded2120a95d6a7aafb7e72d849e17c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:3fadf7ebd60b5b879e6f9e2cd46c782e18c64ec78a5e1ddd5e587a779364933d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.1 MB (120117709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82643bd90d5e12d8dcc3923c5037bace1b14063504a971ec0498cf5e162bf61f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:52:58 GMT
ARG MARIADB_MAJOR=10.3
# Fri, 22 Apr 2022 02:52:58 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 22 Apr 2022 02:52:59 GMT
ARG MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 22 Apr 2022 02:52:59 GMT
ENV MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 22 Apr 2022 02:52:59 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:52:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:53:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:53:26 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:53:26 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:53:26 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:53:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 02:53:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:53:27 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:53:27 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7801d5a27d87a0a14725087a02be10adf3637adbacf9636d809795ed70a34ce`  
		Last Modified: Fri, 22 Apr 2022 02:57:52 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa7f812281a340552e5374feef34fd9a2563c703d0193aad89c90cf3fe9fe39a`  
		Last Modified: Fri, 22 Apr 2022 02:58:04 GMT  
		Size: 80.2 MB (80191115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b0502732e9ee8013217b08ed97cb6199c16b413212459861470162d7a1ea6d`  
		Last Modified: Fri, 22 Apr 2022 02:57:53 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38fba0e3193601cd73bca932f9f778413d041e214ebad8a4a0b24f5ce35ec76d`  
		Last Modified: Fri, 22 Apr 2022 02:57:53 GMT  
		Size: 6.8 KB (6772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22c2c705d6abdc6c36ec9ad28a43a47c9d00d5c2aa196ceee150b34001faaad4`  
		Last Modified: Fri, 22 Apr 2022 02:57:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:b0a3468d4dde2bcc2c7999df4171d3103fe48ca55ceb859595bc017605245b37
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117607783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8114a9faba606cea1bb35dd16d5898781167d329e63deacd215a765ee19fc419`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:29:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 03:29:22 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:23 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 03:29:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 03:29:39 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 03:29:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:48 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 03:29:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 03:33:18 GMT
ARG MARIADB_MAJOR=10.3
# Fri, 22 Apr 2022 03:33:19 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 22 Apr 2022 03:33:20 GMT
ARG MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 22 Apr 2022 03:33:21 GMT
ENV MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 22 Apr 2022 03:33:22 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 03:33:23 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 03:33:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 03:33:49 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 03:33:50 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 03:33:51 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 03:33:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 03:33:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 03:33:53 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 03:33:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7061769dfb44ec758f6d367a5d4ea0ae9e6f03ca107b7f4ee4b2419e2ae693b`  
		Last Modified: Fri, 22 Apr 2022 03:36:31 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc0a8ec71ebae8e12eafc6106df54088463cc344135ebd19dc41f331e0ed6f2`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 5.3 MB (5320310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87bc30abcdec1bcda27933f56dac195031b448391d01eb7ed27fe77b389117e7`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 3.4 MB (3370037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c05e5ca55fe31dfae11772d53c4dd507f38b7e27ba3b7b878954b5c1d9697f87`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617ab90f9424ca5c02f763590888d7804d6be962990b9f82717351743533c8f0`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 2.2 MB (2202477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bbb7ad258365e117ef11517dc6c0beadccf14acb57fba68848b61d4e0044111`  
		Last Modified: Fri, 22 Apr 2022 03:36:26 GMT  
		Size: 2.5 KB (2469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75d58a2e8d323795646bfacabb25905ae6059f68898ba6a1b4e2bc54dc38d56d`  
		Last Modified: Fri, 22 Apr 2022 03:39:21 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1384173381c8a4fb5181fa3fbb0064e82bbcd4f030ec1b3aaa1e4f5316093b9c`  
		Last Modified: Fri, 22 Apr 2022 03:39:34 GMT  
		Size: 79.5 MB (79530796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3aab6dbbd81fafbc2878c10cf601c0a59dd4b03e482f90844e4af59db46a1f1`  
		Last Modified: Fri, 22 Apr 2022 03:39:21 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93d0ae64b3b2dabde027d3920bfbd5c50903fab69b84da305a3f69e8b9e0bd70`  
		Last Modified: Fri, 22 Apr 2022 03:39:21 GMT  
		Size: 6.8 KB (6769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b800dfda623d3ab156ad3e143ce76e259219c0c69e171b41dbb1e465655a6dc3`  
		Last Modified: Fri, 22 Apr 2022 03:39:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:87b61f8379eb65a704fd612759413f1078a26d40e8d2bea31075c10e8e5c64c1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.0 MB (131005136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23d224c4121a61e5b5ed36485d24161c66509f7d3e5726444beca6059032c3a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:43:50 GMT
ARG MARIADB_MAJOR=10.3
# Fri, 22 Apr 2022 10:43:52 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 22 Apr 2022 10:43:55 GMT
ARG MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 22 Apr 2022 10:43:58 GMT
ENV MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 22 Apr 2022 10:44:01 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:44:07 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:45:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:45:50 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:45:54 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:45:56 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:46:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 10:46:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:46:18 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:46:21 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e69825db8399a8e8531089312f836140b3c2e202cd9e9f8d3e33f2862140bf7`  
		Last Modified: Fri, 22 Apr 2022 10:55:34 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f3a5eacd4b3852d2a6df25f3dcdbe1a2350a97ac7a75e7f6fef19cc6ce125d`  
		Last Modified: Fri, 22 Apr 2022 10:55:50 GMT  
		Size: 84.8 MB (84791769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3127a0e21401b0104caee55b024a479dcacb37031f547853f5f157d65bb3afe1`  
		Last Modified: Fri, 22 Apr 2022 10:55:34 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a468c88d3fc33c46a0b0bfc86b2251de989fffa4efb7f03fddd35192bd88acd`  
		Last Modified: Fri, 22 Apr 2022 10:55:34 GMT  
		Size: 6.8 KB (6772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413ee9ba3b320da907982067cc2460e9ae78998da3271ca620f0e122a465d7c5`  
		Last Modified: Fri, 22 Apr 2022 10:55:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3.34`

```console
$ docker pull mariadb@sha256:114febf5009acb4f4f777b21ff2097c572ded2120a95d6a7aafb7e72d849e17c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3.34` - linux; amd64

```console
$ docker pull mariadb@sha256:3fadf7ebd60b5b879e6f9e2cd46c782e18c64ec78a5e1ddd5e587a779364933d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.1 MB (120117709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82643bd90d5e12d8dcc3923c5037bace1b14063504a971ec0498cf5e162bf61f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:52:58 GMT
ARG MARIADB_MAJOR=10.3
# Fri, 22 Apr 2022 02:52:58 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 22 Apr 2022 02:52:59 GMT
ARG MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 22 Apr 2022 02:52:59 GMT
ENV MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 22 Apr 2022 02:52:59 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:52:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:53:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:53:26 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:53:26 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:53:26 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:53:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 02:53:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:53:27 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:53:27 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7801d5a27d87a0a14725087a02be10adf3637adbacf9636d809795ed70a34ce`  
		Last Modified: Fri, 22 Apr 2022 02:57:52 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa7f812281a340552e5374feef34fd9a2563c703d0193aad89c90cf3fe9fe39a`  
		Last Modified: Fri, 22 Apr 2022 02:58:04 GMT  
		Size: 80.2 MB (80191115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b0502732e9ee8013217b08ed97cb6199c16b413212459861470162d7a1ea6d`  
		Last Modified: Fri, 22 Apr 2022 02:57:53 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38fba0e3193601cd73bca932f9f778413d041e214ebad8a4a0b24f5ce35ec76d`  
		Last Modified: Fri, 22 Apr 2022 02:57:53 GMT  
		Size: 6.8 KB (6772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22c2c705d6abdc6c36ec9ad28a43a47c9d00d5c2aa196ceee150b34001faaad4`  
		Last Modified: Fri, 22 Apr 2022 02:57:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.34` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:b0a3468d4dde2bcc2c7999df4171d3103fe48ca55ceb859595bc017605245b37
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117607783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8114a9faba606cea1bb35dd16d5898781167d329e63deacd215a765ee19fc419`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:29:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 03:29:22 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:23 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 03:29:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 03:29:39 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 03:29:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:48 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 03:29:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 03:33:18 GMT
ARG MARIADB_MAJOR=10.3
# Fri, 22 Apr 2022 03:33:19 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 22 Apr 2022 03:33:20 GMT
ARG MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 22 Apr 2022 03:33:21 GMT
ENV MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 22 Apr 2022 03:33:22 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 03:33:23 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 03:33:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 03:33:49 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 03:33:50 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 03:33:51 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 03:33:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 03:33:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 03:33:53 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 03:33:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7061769dfb44ec758f6d367a5d4ea0ae9e6f03ca107b7f4ee4b2419e2ae693b`  
		Last Modified: Fri, 22 Apr 2022 03:36:31 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc0a8ec71ebae8e12eafc6106df54088463cc344135ebd19dc41f331e0ed6f2`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 5.3 MB (5320310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87bc30abcdec1bcda27933f56dac195031b448391d01eb7ed27fe77b389117e7`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 3.4 MB (3370037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c05e5ca55fe31dfae11772d53c4dd507f38b7e27ba3b7b878954b5c1d9697f87`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617ab90f9424ca5c02f763590888d7804d6be962990b9f82717351743533c8f0`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 2.2 MB (2202477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bbb7ad258365e117ef11517dc6c0beadccf14acb57fba68848b61d4e0044111`  
		Last Modified: Fri, 22 Apr 2022 03:36:26 GMT  
		Size: 2.5 KB (2469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75d58a2e8d323795646bfacabb25905ae6059f68898ba6a1b4e2bc54dc38d56d`  
		Last Modified: Fri, 22 Apr 2022 03:39:21 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1384173381c8a4fb5181fa3fbb0064e82bbcd4f030ec1b3aaa1e4f5316093b9c`  
		Last Modified: Fri, 22 Apr 2022 03:39:34 GMT  
		Size: 79.5 MB (79530796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3aab6dbbd81fafbc2878c10cf601c0a59dd4b03e482f90844e4af59db46a1f1`  
		Last Modified: Fri, 22 Apr 2022 03:39:21 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93d0ae64b3b2dabde027d3920bfbd5c50903fab69b84da305a3f69e8b9e0bd70`  
		Last Modified: Fri, 22 Apr 2022 03:39:21 GMT  
		Size: 6.8 KB (6769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b800dfda623d3ab156ad3e143ce76e259219c0c69e171b41dbb1e465655a6dc3`  
		Last Modified: Fri, 22 Apr 2022 03:39:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.34` - linux; ppc64le

```console
$ docker pull mariadb@sha256:87b61f8379eb65a704fd612759413f1078a26d40e8d2bea31075c10e8e5c64c1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.0 MB (131005136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23d224c4121a61e5b5ed36485d24161c66509f7d3e5726444beca6059032c3a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:43:50 GMT
ARG MARIADB_MAJOR=10.3
# Fri, 22 Apr 2022 10:43:52 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 22 Apr 2022 10:43:55 GMT
ARG MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 22 Apr 2022 10:43:58 GMT
ENV MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 22 Apr 2022 10:44:01 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:44:07 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:45:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:45:50 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:45:54 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:45:56 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:46:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 10:46:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:46:18 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:46:21 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e69825db8399a8e8531089312f836140b3c2e202cd9e9f8d3e33f2862140bf7`  
		Last Modified: Fri, 22 Apr 2022 10:55:34 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f3a5eacd4b3852d2a6df25f3dcdbe1a2350a97ac7a75e7f6fef19cc6ce125d`  
		Last Modified: Fri, 22 Apr 2022 10:55:50 GMT  
		Size: 84.8 MB (84791769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3127a0e21401b0104caee55b024a479dcacb37031f547853f5f157d65bb3afe1`  
		Last Modified: Fri, 22 Apr 2022 10:55:34 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a468c88d3fc33c46a0b0bfc86b2251de989fffa4efb7f03fddd35192bd88acd`  
		Last Modified: Fri, 22 Apr 2022 10:55:34 GMT  
		Size: 6.8 KB (6772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413ee9ba3b320da907982067cc2460e9ae78998da3271ca620f0e122a465d7c5`  
		Last Modified: Fri, 22 Apr 2022 10:55:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3.34-focal`

```console
$ docker pull mariadb@sha256:114febf5009acb4f4f777b21ff2097c572ded2120a95d6a7aafb7e72d849e17c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3.34-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:3fadf7ebd60b5b879e6f9e2cd46c782e18c64ec78a5e1ddd5e587a779364933d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.1 MB (120117709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82643bd90d5e12d8dcc3923c5037bace1b14063504a971ec0498cf5e162bf61f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:52:58 GMT
ARG MARIADB_MAJOR=10.3
# Fri, 22 Apr 2022 02:52:58 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 22 Apr 2022 02:52:59 GMT
ARG MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 22 Apr 2022 02:52:59 GMT
ENV MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 22 Apr 2022 02:52:59 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:52:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:53:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:53:26 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:53:26 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:53:26 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:53:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 02:53:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:53:27 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:53:27 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7801d5a27d87a0a14725087a02be10adf3637adbacf9636d809795ed70a34ce`  
		Last Modified: Fri, 22 Apr 2022 02:57:52 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa7f812281a340552e5374feef34fd9a2563c703d0193aad89c90cf3fe9fe39a`  
		Last Modified: Fri, 22 Apr 2022 02:58:04 GMT  
		Size: 80.2 MB (80191115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b0502732e9ee8013217b08ed97cb6199c16b413212459861470162d7a1ea6d`  
		Last Modified: Fri, 22 Apr 2022 02:57:53 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38fba0e3193601cd73bca932f9f778413d041e214ebad8a4a0b24f5ce35ec76d`  
		Last Modified: Fri, 22 Apr 2022 02:57:53 GMT  
		Size: 6.8 KB (6772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22c2c705d6abdc6c36ec9ad28a43a47c9d00d5c2aa196ceee150b34001faaad4`  
		Last Modified: Fri, 22 Apr 2022 02:57:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.34-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:b0a3468d4dde2bcc2c7999df4171d3103fe48ca55ceb859595bc017605245b37
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117607783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8114a9faba606cea1bb35dd16d5898781167d329e63deacd215a765ee19fc419`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:29:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 03:29:22 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:23 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 03:29:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 03:29:39 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 03:29:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:48 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 03:29:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 03:33:18 GMT
ARG MARIADB_MAJOR=10.3
# Fri, 22 Apr 2022 03:33:19 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 22 Apr 2022 03:33:20 GMT
ARG MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 22 Apr 2022 03:33:21 GMT
ENV MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 22 Apr 2022 03:33:22 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 03:33:23 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 03:33:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 03:33:49 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 03:33:50 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 03:33:51 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 03:33:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 03:33:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 03:33:53 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 03:33:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7061769dfb44ec758f6d367a5d4ea0ae9e6f03ca107b7f4ee4b2419e2ae693b`  
		Last Modified: Fri, 22 Apr 2022 03:36:31 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc0a8ec71ebae8e12eafc6106df54088463cc344135ebd19dc41f331e0ed6f2`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 5.3 MB (5320310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87bc30abcdec1bcda27933f56dac195031b448391d01eb7ed27fe77b389117e7`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 3.4 MB (3370037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c05e5ca55fe31dfae11772d53c4dd507f38b7e27ba3b7b878954b5c1d9697f87`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617ab90f9424ca5c02f763590888d7804d6be962990b9f82717351743533c8f0`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 2.2 MB (2202477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bbb7ad258365e117ef11517dc6c0beadccf14acb57fba68848b61d4e0044111`  
		Last Modified: Fri, 22 Apr 2022 03:36:26 GMT  
		Size: 2.5 KB (2469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75d58a2e8d323795646bfacabb25905ae6059f68898ba6a1b4e2bc54dc38d56d`  
		Last Modified: Fri, 22 Apr 2022 03:39:21 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1384173381c8a4fb5181fa3fbb0064e82bbcd4f030ec1b3aaa1e4f5316093b9c`  
		Last Modified: Fri, 22 Apr 2022 03:39:34 GMT  
		Size: 79.5 MB (79530796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3aab6dbbd81fafbc2878c10cf601c0a59dd4b03e482f90844e4af59db46a1f1`  
		Last Modified: Fri, 22 Apr 2022 03:39:21 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93d0ae64b3b2dabde027d3920bfbd5c50903fab69b84da305a3f69e8b9e0bd70`  
		Last Modified: Fri, 22 Apr 2022 03:39:21 GMT  
		Size: 6.8 KB (6769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b800dfda623d3ab156ad3e143ce76e259219c0c69e171b41dbb1e465655a6dc3`  
		Last Modified: Fri, 22 Apr 2022 03:39:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.34-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:87b61f8379eb65a704fd612759413f1078a26d40e8d2bea31075c10e8e5c64c1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.0 MB (131005136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23d224c4121a61e5b5ed36485d24161c66509f7d3e5726444beca6059032c3a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:43:50 GMT
ARG MARIADB_MAJOR=10.3
# Fri, 22 Apr 2022 10:43:52 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 22 Apr 2022 10:43:55 GMT
ARG MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 22 Apr 2022 10:43:58 GMT
ENV MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 22 Apr 2022 10:44:01 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:44:07 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:45:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:45:50 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:45:54 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:45:56 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:46:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 10:46:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:46:18 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:46:21 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e69825db8399a8e8531089312f836140b3c2e202cd9e9f8d3e33f2862140bf7`  
		Last Modified: Fri, 22 Apr 2022 10:55:34 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f3a5eacd4b3852d2a6df25f3dcdbe1a2350a97ac7a75e7f6fef19cc6ce125d`  
		Last Modified: Fri, 22 Apr 2022 10:55:50 GMT  
		Size: 84.8 MB (84791769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3127a0e21401b0104caee55b024a479dcacb37031f547853f5f157d65bb3afe1`  
		Last Modified: Fri, 22 Apr 2022 10:55:34 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a468c88d3fc33c46a0b0bfc86b2251de989fffa4efb7f03fddd35192bd88acd`  
		Last Modified: Fri, 22 Apr 2022 10:55:34 GMT  
		Size: 6.8 KB (6772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413ee9ba3b320da907982067cc2460e9ae78998da3271ca620f0e122a465d7c5`  
		Last Modified: Fri, 22 Apr 2022 10:55:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4`

```console
$ docker pull mariadb@sha256:3407ca0c62adb53486a951981a1d4b5abdc1a085302800536f950ab6cc195ef9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4` - linux; amd64

```console
$ docker pull mariadb@sha256:819963937619a1891b4e1f4c6125d4ea4f3bb6195d72042307ae2cd68071b1ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125679716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ad3c8256a516f93654aed599432527de806b5da9c2088233c692591c291a9a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:52:31 GMT
ARG MARIADB_MAJOR=10.4
# Fri, 22 Apr 2022 02:52:31 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 22 Apr 2022 02:52:31 GMT
ARG MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 22 Apr 2022 02:52:31 GMT
ENV MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 22 Apr 2022 02:52:31 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:52:31 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:52:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:52:54 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:52:54 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:52:54 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:52:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 02:52:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:52:55 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:52:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b744c9184d699263c8a3ef44c0767a0429db8c6892701eef91c0237b61421e5`  
		Last Modified: Fri, 22 Apr 2022 02:57:23 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d15a78b4ec63a31d0349185788c72af768e99002fcbb2a6a46c3a8a6fd263eb`  
		Last Modified: Fri, 22 Apr 2022 02:57:36 GMT  
		Size: 85.8 MB (85753125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76088cf45319c739b3d59169b2c599481218be04824f4aadb20657eb83c43f1b`  
		Last Modified: Fri, 22 Apr 2022 02:57:23 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4519dcc8d4be31b8246d8f666c1db6c7eab0ff35ade6ece88c6b7f39a784d29`  
		Last Modified: Fri, 22 Apr 2022 02:57:23 GMT  
		Size: 6.8 KB (6769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2f902b376b26e5290db3e69f9cfadc24be1001705c68c97205619cd98b2a00d`  
		Last Modified: Fri, 22 Apr 2022 02:57:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:5d236398b97b1b21bc59bfe04347c7d5e9a7c25262c9d689f252a5564db6ac75
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (123003440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:415471e389e03c9a46cc26a19f15d17851980a7d462e7dc6ccd0b31176ce962d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:29:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 03:29:22 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:23 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 03:29:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 03:29:39 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 03:29:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:48 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 03:29:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 03:32:34 GMT
ARG MARIADB_MAJOR=10.4
# Fri, 22 Apr 2022 03:32:35 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 22 Apr 2022 03:32:36 GMT
ARG MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 22 Apr 2022 03:32:37 GMT
ENV MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 22 Apr 2022 03:32:38 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 03:32:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 03:33:00 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 03:33:01 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 03:33:03 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 03:33:04 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 03:33:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 03:33:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 03:33:06 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 03:33:07 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7061769dfb44ec758f6d367a5d4ea0ae9e6f03ca107b7f4ee4b2419e2ae693b`  
		Last Modified: Fri, 22 Apr 2022 03:36:31 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc0a8ec71ebae8e12eafc6106df54088463cc344135ebd19dc41f331e0ed6f2`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 5.3 MB (5320310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87bc30abcdec1bcda27933f56dac195031b448391d01eb7ed27fe77b389117e7`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 3.4 MB (3370037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c05e5ca55fe31dfae11772d53c4dd507f38b7e27ba3b7b878954b5c1d9697f87`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617ab90f9424ca5c02f763590888d7804d6be962990b9f82717351743533c8f0`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 2.2 MB (2202477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bbb7ad258365e117ef11517dc6c0beadccf14acb57fba68848b61d4e0044111`  
		Last Modified: Fri, 22 Apr 2022 03:36:26 GMT  
		Size: 2.5 KB (2469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6621bd87de585f05ea51a6b3598bfa29f0ff3951b60d0c5606c91502870b0958`  
		Last Modified: Fri, 22 Apr 2022 03:38:49 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddbe366c1c96a19178e87a62b0a9c494e2782a803c372f61633274f19888a000`  
		Last Modified: Fri, 22 Apr 2022 03:39:03 GMT  
		Size: 84.9 MB (84926449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59355c48a61f996a696a7908746cda2d53f0b218e25e728d79f8f4fa04bf62c9`  
		Last Modified: Fri, 22 Apr 2022 03:38:49 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b3631a62bc5e2a6c28a270dd40a8147335467a507a82369e9df194f28dd990e`  
		Last Modified: Fri, 22 Apr 2022 03:38:49 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46603c22a95530e6b7bccdaff42e56804c79dd3518e83b728ede90af78421ba6`  
		Last Modified: Fri, 22 Apr 2022 03:38:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4` - linux; ppc64le

```console
$ docker pull mariadb@sha256:2a66bce22b31b71f3e4c5ca55d1344053c2405d40cbd5cd2d6db8583f8b498d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.6 MB (136559157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e3ed094c127c558d29be417acf0ef28f516f3c6ce0059d914ad23b1dd1e0abc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:41:09 GMT
ARG MARIADB_MAJOR=10.4
# Fri, 22 Apr 2022 10:41:11 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 22 Apr 2022 10:41:13 GMT
ARG MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 22 Apr 2022 10:41:15 GMT
ENV MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 22 Apr 2022 10:41:17 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:41:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:43:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:43:16 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:43:18 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:43:18 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:43:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 10:43:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:43:29 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:43:32 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7f41e21911d9adde7defbce93577afcf701ee7053f4465df314a9652f54872`  
		Last Modified: Fri, 22 Apr 2022 10:54:55 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e15a11cf0a1e0548f3cca3664f091c4b1b78d83e51c62656c5e57113914280b`  
		Last Modified: Fri, 22 Apr 2022 10:55:12 GMT  
		Size: 90.3 MB (90345786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9773723ca77bed5f552c2e35fb43ee9cc4c3c575340c8d985ae91428a19f15a0`  
		Last Modified: Fri, 22 Apr 2022 10:54:55 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6560ee8fe30273309437e97324852b4d11e1d5d9190e485cf4f44ac6d50320b3`  
		Last Modified: Fri, 22 Apr 2022 10:54:55 GMT  
		Size: 6.8 KB (6775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab7263353b18e3000afe4ce89fc5a3eb2462783f322c68298b0c7a90fc76acc8`  
		Last Modified: Fri, 22 Apr 2022 10:54:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4-focal`

```console
$ docker pull mariadb@sha256:3407ca0c62adb53486a951981a1d4b5abdc1a085302800536f950ab6cc195ef9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:819963937619a1891b4e1f4c6125d4ea4f3bb6195d72042307ae2cd68071b1ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125679716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ad3c8256a516f93654aed599432527de806b5da9c2088233c692591c291a9a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:52:31 GMT
ARG MARIADB_MAJOR=10.4
# Fri, 22 Apr 2022 02:52:31 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 22 Apr 2022 02:52:31 GMT
ARG MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 22 Apr 2022 02:52:31 GMT
ENV MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 22 Apr 2022 02:52:31 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:52:31 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:52:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:52:54 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:52:54 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:52:54 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:52:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 02:52:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:52:55 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:52:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b744c9184d699263c8a3ef44c0767a0429db8c6892701eef91c0237b61421e5`  
		Last Modified: Fri, 22 Apr 2022 02:57:23 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d15a78b4ec63a31d0349185788c72af768e99002fcbb2a6a46c3a8a6fd263eb`  
		Last Modified: Fri, 22 Apr 2022 02:57:36 GMT  
		Size: 85.8 MB (85753125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76088cf45319c739b3d59169b2c599481218be04824f4aadb20657eb83c43f1b`  
		Last Modified: Fri, 22 Apr 2022 02:57:23 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4519dcc8d4be31b8246d8f666c1db6c7eab0ff35ade6ece88c6b7f39a784d29`  
		Last Modified: Fri, 22 Apr 2022 02:57:23 GMT  
		Size: 6.8 KB (6769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2f902b376b26e5290db3e69f9cfadc24be1001705c68c97205619cd98b2a00d`  
		Last Modified: Fri, 22 Apr 2022 02:57:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:5d236398b97b1b21bc59bfe04347c7d5e9a7c25262c9d689f252a5564db6ac75
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (123003440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:415471e389e03c9a46cc26a19f15d17851980a7d462e7dc6ccd0b31176ce962d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:29:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 03:29:22 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:23 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 03:29:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 03:29:39 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 03:29:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:48 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 03:29:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 03:32:34 GMT
ARG MARIADB_MAJOR=10.4
# Fri, 22 Apr 2022 03:32:35 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 22 Apr 2022 03:32:36 GMT
ARG MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 22 Apr 2022 03:32:37 GMT
ENV MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 22 Apr 2022 03:32:38 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 03:32:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 03:33:00 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 03:33:01 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 03:33:03 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 03:33:04 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 03:33:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 03:33:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 03:33:06 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 03:33:07 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7061769dfb44ec758f6d367a5d4ea0ae9e6f03ca107b7f4ee4b2419e2ae693b`  
		Last Modified: Fri, 22 Apr 2022 03:36:31 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc0a8ec71ebae8e12eafc6106df54088463cc344135ebd19dc41f331e0ed6f2`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 5.3 MB (5320310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87bc30abcdec1bcda27933f56dac195031b448391d01eb7ed27fe77b389117e7`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 3.4 MB (3370037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c05e5ca55fe31dfae11772d53c4dd507f38b7e27ba3b7b878954b5c1d9697f87`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617ab90f9424ca5c02f763590888d7804d6be962990b9f82717351743533c8f0`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 2.2 MB (2202477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bbb7ad258365e117ef11517dc6c0beadccf14acb57fba68848b61d4e0044111`  
		Last Modified: Fri, 22 Apr 2022 03:36:26 GMT  
		Size: 2.5 KB (2469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6621bd87de585f05ea51a6b3598bfa29f0ff3951b60d0c5606c91502870b0958`  
		Last Modified: Fri, 22 Apr 2022 03:38:49 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddbe366c1c96a19178e87a62b0a9c494e2782a803c372f61633274f19888a000`  
		Last Modified: Fri, 22 Apr 2022 03:39:03 GMT  
		Size: 84.9 MB (84926449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59355c48a61f996a696a7908746cda2d53f0b218e25e728d79f8f4fa04bf62c9`  
		Last Modified: Fri, 22 Apr 2022 03:38:49 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b3631a62bc5e2a6c28a270dd40a8147335467a507a82369e9df194f28dd990e`  
		Last Modified: Fri, 22 Apr 2022 03:38:49 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46603c22a95530e6b7bccdaff42e56804c79dd3518e83b728ede90af78421ba6`  
		Last Modified: Fri, 22 Apr 2022 03:38:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:2a66bce22b31b71f3e4c5ca55d1344053c2405d40cbd5cd2d6db8583f8b498d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.6 MB (136559157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e3ed094c127c558d29be417acf0ef28f516f3c6ce0059d914ad23b1dd1e0abc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:41:09 GMT
ARG MARIADB_MAJOR=10.4
# Fri, 22 Apr 2022 10:41:11 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 22 Apr 2022 10:41:13 GMT
ARG MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 22 Apr 2022 10:41:15 GMT
ENV MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 22 Apr 2022 10:41:17 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:41:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:43:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:43:16 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:43:18 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:43:18 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:43:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 10:43:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:43:29 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:43:32 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7f41e21911d9adde7defbce93577afcf701ee7053f4465df314a9652f54872`  
		Last Modified: Fri, 22 Apr 2022 10:54:55 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e15a11cf0a1e0548f3cca3664f091c4b1b78d83e51c62656c5e57113914280b`  
		Last Modified: Fri, 22 Apr 2022 10:55:12 GMT  
		Size: 90.3 MB (90345786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9773723ca77bed5f552c2e35fb43ee9cc4c3c575340c8d985ae91428a19f15a0`  
		Last Modified: Fri, 22 Apr 2022 10:54:55 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6560ee8fe30273309437e97324852b4d11e1d5d9190e485cf4f44ac6d50320b3`  
		Last Modified: Fri, 22 Apr 2022 10:54:55 GMT  
		Size: 6.8 KB (6775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab7263353b18e3000afe4ce89fc5a3eb2462783f322c68298b0c7a90fc76acc8`  
		Last Modified: Fri, 22 Apr 2022 10:54:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4.24`

```console
$ docker pull mariadb@sha256:3407ca0c62adb53486a951981a1d4b5abdc1a085302800536f950ab6cc195ef9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4.24` - linux; amd64

```console
$ docker pull mariadb@sha256:819963937619a1891b4e1f4c6125d4ea4f3bb6195d72042307ae2cd68071b1ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125679716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ad3c8256a516f93654aed599432527de806b5da9c2088233c692591c291a9a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:52:31 GMT
ARG MARIADB_MAJOR=10.4
# Fri, 22 Apr 2022 02:52:31 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 22 Apr 2022 02:52:31 GMT
ARG MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 22 Apr 2022 02:52:31 GMT
ENV MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 22 Apr 2022 02:52:31 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:52:31 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:52:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:52:54 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:52:54 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:52:54 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:52:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 02:52:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:52:55 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:52:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b744c9184d699263c8a3ef44c0767a0429db8c6892701eef91c0237b61421e5`  
		Last Modified: Fri, 22 Apr 2022 02:57:23 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d15a78b4ec63a31d0349185788c72af768e99002fcbb2a6a46c3a8a6fd263eb`  
		Last Modified: Fri, 22 Apr 2022 02:57:36 GMT  
		Size: 85.8 MB (85753125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76088cf45319c739b3d59169b2c599481218be04824f4aadb20657eb83c43f1b`  
		Last Modified: Fri, 22 Apr 2022 02:57:23 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4519dcc8d4be31b8246d8f666c1db6c7eab0ff35ade6ece88c6b7f39a784d29`  
		Last Modified: Fri, 22 Apr 2022 02:57:23 GMT  
		Size: 6.8 KB (6769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2f902b376b26e5290db3e69f9cfadc24be1001705c68c97205619cd98b2a00d`  
		Last Modified: Fri, 22 Apr 2022 02:57:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.24` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:5d236398b97b1b21bc59bfe04347c7d5e9a7c25262c9d689f252a5564db6ac75
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (123003440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:415471e389e03c9a46cc26a19f15d17851980a7d462e7dc6ccd0b31176ce962d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:29:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 03:29:22 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:23 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 03:29:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 03:29:39 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 03:29:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:48 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 03:29:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 03:32:34 GMT
ARG MARIADB_MAJOR=10.4
# Fri, 22 Apr 2022 03:32:35 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 22 Apr 2022 03:32:36 GMT
ARG MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 22 Apr 2022 03:32:37 GMT
ENV MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 22 Apr 2022 03:32:38 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 03:32:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 03:33:00 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 03:33:01 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 03:33:03 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 03:33:04 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 03:33:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 03:33:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 03:33:06 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 03:33:07 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7061769dfb44ec758f6d367a5d4ea0ae9e6f03ca107b7f4ee4b2419e2ae693b`  
		Last Modified: Fri, 22 Apr 2022 03:36:31 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc0a8ec71ebae8e12eafc6106df54088463cc344135ebd19dc41f331e0ed6f2`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 5.3 MB (5320310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87bc30abcdec1bcda27933f56dac195031b448391d01eb7ed27fe77b389117e7`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 3.4 MB (3370037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c05e5ca55fe31dfae11772d53c4dd507f38b7e27ba3b7b878954b5c1d9697f87`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617ab90f9424ca5c02f763590888d7804d6be962990b9f82717351743533c8f0`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 2.2 MB (2202477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bbb7ad258365e117ef11517dc6c0beadccf14acb57fba68848b61d4e0044111`  
		Last Modified: Fri, 22 Apr 2022 03:36:26 GMT  
		Size: 2.5 KB (2469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6621bd87de585f05ea51a6b3598bfa29f0ff3951b60d0c5606c91502870b0958`  
		Last Modified: Fri, 22 Apr 2022 03:38:49 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddbe366c1c96a19178e87a62b0a9c494e2782a803c372f61633274f19888a000`  
		Last Modified: Fri, 22 Apr 2022 03:39:03 GMT  
		Size: 84.9 MB (84926449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59355c48a61f996a696a7908746cda2d53f0b218e25e728d79f8f4fa04bf62c9`  
		Last Modified: Fri, 22 Apr 2022 03:38:49 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b3631a62bc5e2a6c28a270dd40a8147335467a507a82369e9df194f28dd990e`  
		Last Modified: Fri, 22 Apr 2022 03:38:49 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46603c22a95530e6b7bccdaff42e56804c79dd3518e83b728ede90af78421ba6`  
		Last Modified: Fri, 22 Apr 2022 03:38:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.24` - linux; ppc64le

```console
$ docker pull mariadb@sha256:2a66bce22b31b71f3e4c5ca55d1344053c2405d40cbd5cd2d6db8583f8b498d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.6 MB (136559157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e3ed094c127c558d29be417acf0ef28f516f3c6ce0059d914ad23b1dd1e0abc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:41:09 GMT
ARG MARIADB_MAJOR=10.4
# Fri, 22 Apr 2022 10:41:11 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 22 Apr 2022 10:41:13 GMT
ARG MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 22 Apr 2022 10:41:15 GMT
ENV MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 22 Apr 2022 10:41:17 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:41:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:43:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:43:16 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:43:18 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:43:18 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:43:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 10:43:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:43:29 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:43:32 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7f41e21911d9adde7defbce93577afcf701ee7053f4465df314a9652f54872`  
		Last Modified: Fri, 22 Apr 2022 10:54:55 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e15a11cf0a1e0548f3cca3664f091c4b1b78d83e51c62656c5e57113914280b`  
		Last Modified: Fri, 22 Apr 2022 10:55:12 GMT  
		Size: 90.3 MB (90345786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9773723ca77bed5f552c2e35fb43ee9cc4c3c575340c8d985ae91428a19f15a0`  
		Last Modified: Fri, 22 Apr 2022 10:54:55 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6560ee8fe30273309437e97324852b4d11e1d5d9190e485cf4f44ac6d50320b3`  
		Last Modified: Fri, 22 Apr 2022 10:54:55 GMT  
		Size: 6.8 KB (6775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab7263353b18e3000afe4ce89fc5a3eb2462783f322c68298b0c7a90fc76acc8`  
		Last Modified: Fri, 22 Apr 2022 10:54:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4.24-focal`

```console
$ docker pull mariadb@sha256:3407ca0c62adb53486a951981a1d4b5abdc1a085302800536f950ab6cc195ef9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4.24-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:819963937619a1891b4e1f4c6125d4ea4f3bb6195d72042307ae2cd68071b1ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125679716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ad3c8256a516f93654aed599432527de806b5da9c2088233c692591c291a9a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:52:31 GMT
ARG MARIADB_MAJOR=10.4
# Fri, 22 Apr 2022 02:52:31 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 22 Apr 2022 02:52:31 GMT
ARG MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 22 Apr 2022 02:52:31 GMT
ENV MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 22 Apr 2022 02:52:31 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:52:31 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:52:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:52:54 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:52:54 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:52:54 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:52:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 02:52:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:52:55 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:52:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b744c9184d699263c8a3ef44c0767a0429db8c6892701eef91c0237b61421e5`  
		Last Modified: Fri, 22 Apr 2022 02:57:23 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d15a78b4ec63a31d0349185788c72af768e99002fcbb2a6a46c3a8a6fd263eb`  
		Last Modified: Fri, 22 Apr 2022 02:57:36 GMT  
		Size: 85.8 MB (85753125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76088cf45319c739b3d59169b2c599481218be04824f4aadb20657eb83c43f1b`  
		Last Modified: Fri, 22 Apr 2022 02:57:23 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4519dcc8d4be31b8246d8f666c1db6c7eab0ff35ade6ece88c6b7f39a784d29`  
		Last Modified: Fri, 22 Apr 2022 02:57:23 GMT  
		Size: 6.8 KB (6769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2f902b376b26e5290db3e69f9cfadc24be1001705c68c97205619cd98b2a00d`  
		Last Modified: Fri, 22 Apr 2022 02:57:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.24-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:5d236398b97b1b21bc59bfe04347c7d5e9a7c25262c9d689f252a5564db6ac75
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (123003440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:415471e389e03c9a46cc26a19f15d17851980a7d462e7dc6ccd0b31176ce962d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:29:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 03:29:22 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:23 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 03:29:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 03:29:39 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 03:29:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:48 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 03:29:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 03:32:34 GMT
ARG MARIADB_MAJOR=10.4
# Fri, 22 Apr 2022 03:32:35 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 22 Apr 2022 03:32:36 GMT
ARG MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 22 Apr 2022 03:32:37 GMT
ENV MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 22 Apr 2022 03:32:38 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 03:32:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 03:33:00 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 03:33:01 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 03:33:03 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 03:33:04 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 03:33:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 03:33:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 03:33:06 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 03:33:07 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7061769dfb44ec758f6d367a5d4ea0ae9e6f03ca107b7f4ee4b2419e2ae693b`  
		Last Modified: Fri, 22 Apr 2022 03:36:31 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc0a8ec71ebae8e12eafc6106df54088463cc344135ebd19dc41f331e0ed6f2`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 5.3 MB (5320310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87bc30abcdec1bcda27933f56dac195031b448391d01eb7ed27fe77b389117e7`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 3.4 MB (3370037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c05e5ca55fe31dfae11772d53c4dd507f38b7e27ba3b7b878954b5c1d9697f87`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617ab90f9424ca5c02f763590888d7804d6be962990b9f82717351743533c8f0`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 2.2 MB (2202477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bbb7ad258365e117ef11517dc6c0beadccf14acb57fba68848b61d4e0044111`  
		Last Modified: Fri, 22 Apr 2022 03:36:26 GMT  
		Size: 2.5 KB (2469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6621bd87de585f05ea51a6b3598bfa29f0ff3951b60d0c5606c91502870b0958`  
		Last Modified: Fri, 22 Apr 2022 03:38:49 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddbe366c1c96a19178e87a62b0a9c494e2782a803c372f61633274f19888a000`  
		Last Modified: Fri, 22 Apr 2022 03:39:03 GMT  
		Size: 84.9 MB (84926449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59355c48a61f996a696a7908746cda2d53f0b218e25e728d79f8f4fa04bf62c9`  
		Last Modified: Fri, 22 Apr 2022 03:38:49 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b3631a62bc5e2a6c28a270dd40a8147335467a507a82369e9df194f28dd990e`  
		Last Modified: Fri, 22 Apr 2022 03:38:49 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46603c22a95530e6b7bccdaff42e56804c79dd3518e83b728ede90af78421ba6`  
		Last Modified: Fri, 22 Apr 2022 03:38:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.24-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:2a66bce22b31b71f3e4c5ca55d1344053c2405d40cbd5cd2d6db8583f8b498d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.6 MB (136559157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e3ed094c127c558d29be417acf0ef28f516f3c6ce0059d914ad23b1dd1e0abc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:41:09 GMT
ARG MARIADB_MAJOR=10.4
# Fri, 22 Apr 2022 10:41:11 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 22 Apr 2022 10:41:13 GMT
ARG MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 22 Apr 2022 10:41:15 GMT
ENV MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 22 Apr 2022 10:41:17 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:41:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:43:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:43:16 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:43:18 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:43:18 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:43:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 10:43:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:43:29 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:43:32 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7f41e21911d9adde7defbce93577afcf701ee7053f4465df314a9652f54872`  
		Last Modified: Fri, 22 Apr 2022 10:54:55 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e15a11cf0a1e0548f3cca3664f091c4b1b78d83e51c62656c5e57113914280b`  
		Last Modified: Fri, 22 Apr 2022 10:55:12 GMT  
		Size: 90.3 MB (90345786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9773723ca77bed5f552c2e35fb43ee9cc4c3c575340c8d985ae91428a19f15a0`  
		Last Modified: Fri, 22 Apr 2022 10:54:55 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6560ee8fe30273309437e97324852b4d11e1d5d9190e485cf4f44ac6d50320b3`  
		Last Modified: Fri, 22 Apr 2022 10:54:55 GMT  
		Size: 6.8 KB (6775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab7263353b18e3000afe4ce89fc5a3eb2462783f322c68298b0c7a90fc76acc8`  
		Last Modified: Fri, 22 Apr 2022 10:54:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5`

```console
$ docker pull mariadb@sha256:78fb679e1155f656443d0c68f4510cd50f4473cd1b0b8af6e9308f945d3728d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.5` - linux; amd64

```console
$ docker pull mariadb@sha256:5d5daf7e35f3b1e8dc54b7f279bf8d0fabdc5489f329b9e4af289e92c692abd4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.9 MB (127923752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8247f649c1ad0ed98bded330f521a2114583f7d253dcb91228d0f865e76ac90`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:52:03 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 22 Apr 2022 02:52:03 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 22 Apr 2022 02:52:03 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 22 Apr 2022 02:52:03 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 22 Apr 2022 02:52:03 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:52:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:52:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:52:25 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:52:25 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:52:25 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:52:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:52:25 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:52:25 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:490dd7915b8002205becea23f1301b54b93df661098f49fb349100eace3c473d`  
		Last Modified: Fri, 22 Apr 2022 02:56:54 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0791622d551403008eaaa8a55b8c2ce888d9cf059518ffec3789cef789c4c987`  
		Last Modified: Fri, 22 Apr 2022 02:57:07 GMT  
		Size: 88.0 MB (87997283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f43c35539e9763ffe7ff15d83e7fe71d078c83207758e1114050595ca29ecfc9`  
		Last Modified: Fri, 22 Apr 2022 02:56:54 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42c10e4d1ed516fbfdc6e0848f37064f65ff78b2638f1c30002dbd8850e140d`  
		Last Modified: Fri, 22 Apr 2022 02:56:54 GMT  
		Size: 6.8 KB (6769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:625c0474316639388207ded0869b44f175076eab236114bda81b667d2b213257
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.2 MB (125185078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f5fb172364c7f183ad023a938202e2dc83ac228a56b65d707f5b05cbfa6e107`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:29:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 03:29:22 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:23 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 03:29:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 03:29:39 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 03:29:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:48 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 03:29:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 03:31:57 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 22 Apr 2022 03:31:58 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 22 Apr 2022 03:31:59 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 22 Apr 2022 03:32:00 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 22 Apr 2022 03:32:01 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 03:32:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 03:32:23 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 03:32:23 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 03:32:25 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 03:32:26 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 03:32:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 03:32:27 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 03:32:28 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7061769dfb44ec758f6d367a5d4ea0ae9e6f03ca107b7f4ee4b2419e2ae693b`  
		Last Modified: Fri, 22 Apr 2022 03:36:31 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc0a8ec71ebae8e12eafc6106df54088463cc344135ebd19dc41f331e0ed6f2`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 5.3 MB (5320310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87bc30abcdec1bcda27933f56dac195031b448391d01eb7ed27fe77b389117e7`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 3.4 MB (3370037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c05e5ca55fe31dfae11772d53c4dd507f38b7e27ba3b7b878954b5c1d9697f87`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617ab90f9424ca5c02f763590888d7804d6be962990b9f82717351743533c8f0`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 2.2 MB (2202477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bbb7ad258365e117ef11517dc6c0beadccf14acb57fba68848b61d4e0044111`  
		Last Modified: Fri, 22 Apr 2022 03:36:26 GMT  
		Size: 2.5 KB (2469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8091a565556e50b1f2a61e037a3cc54b74e533130f1ce65c6cb658a4b2c1d3ad`  
		Last Modified: Fri, 22 Apr 2022 03:38:17 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9267378c56cd36856faf39e7034a58ac75280075f26fa6b62c4682f123dbe82d`  
		Last Modified: Fri, 22 Apr 2022 03:38:32 GMT  
		Size: 87.1 MB (87108212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ddfbbb4c59339bd121747dd3678278eacdebba57051c29a81543b2a51d33e7f`  
		Last Modified: Fri, 22 Apr 2022 03:38:17 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb66f97861c0444691a7d546c9cb81cc12d54c77d7c7a68ce08a5b79ef86633`  
		Last Modified: Fri, 22 Apr 2022 03:38:17 GMT  
		Size: 6.8 KB (6770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; ppc64le

```console
$ docker pull mariadb@sha256:7253c8bbce09ad62f4aedb92fb4ece6de9a8a6b9389b70fd915a2630bc910810
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.8 MB (138780434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82b5ae0af269fec9ab843a97f38af5e144f1d13e845da7729991e23afb6c4820`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:38:45 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 22 Apr 2022 10:38:48 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 22 Apr 2022 10:38:50 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 22 Apr 2022 10:38:53 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 22 Apr 2022 10:38:56 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:39:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:40:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:40:39 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:40:41 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:40:42 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:40:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:40:47 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:40:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8585fdfb939ad59fe43800e8258791cae1a48fe19fc82bc5b28ee7cea88e25a6`  
		Last Modified: Fri, 22 Apr 2022 10:54:17 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d55c8c0f19134ea3f4e78d7db234e964e8f9b8a28d596ebe4a625594319f9159`  
		Last Modified: Fri, 22 Apr 2022 10:54:35 GMT  
		Size: 92.6 MB (92567188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6cd4f314b64534547b791600e31d8158b548b2fe4e79ecc4da4285aea8a8741`  
		Last Modified: Fri, 22 Apr 2022 10:54:17 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47740fd99121c3a1f7c4c4125a8beb046167869d84ae7ed84c2f6ea1ae329ee8`  
		Last Modified: Fri, 22 Apr 2022 10:54:17 GMT  
		Size: 6.8 KB (6772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; s390x

```console
$ docker pull mariadb@sha256:04652e28b66023a0295a84be62aefb6f5b2ab32171e314175a3f63a78c6aeef3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127198159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bc3c5916525d13560f4b4b25b0e8151e47a8bc455aae8a0f0a3ae03a19b2f45`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 22 Apr 2022 00:39:34 GMT
ADD file:a5fe3b5fef5d5d99022e3a45894edf18c9e5f79c4be8020d61724cdc164256b3 in / 
# Fri, 22 Apr 2022 00:39:39 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:19:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:19:18 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:19:19 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:19:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:19:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:19:48 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:19:50 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:19:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:23:41 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 22 Apr 2022 02:23:41 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 22 Apr 2022 02:23:42 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 22 Apr 2022 02:23:42 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 22 Apr 2022 02:23:43 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:23:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:24:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:24:42 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:24:42 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:24:42 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:24:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:24:44 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:24:44 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:716ba34a9a0241d7bed3fa68865e745000f025af68d21dab7d692215c5074a58`  
		Last Modified: Tue, 19 Apr 2022 13:16:37 GMT  
		Size: 27.1 MB (27085718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bc8f5833a8cfe0537845df0a5d311b211ef889ed5d5e12ace1bd3eb30834c6`  
		Last Modified: Fri, 22 Apr 2022 02:25:50 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f4186175df1fdbe352452d13a8d94670ff3446432648e7b163e9a1c6a94d88`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 5.4 MB (5378760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea503bea58815ffe61d67ad911ffab94ad5a57e364db2126c3cb11e8f732d37`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 3.2 MB (3244218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76eb02e31628a4e2997c0f38de59eb7d09325086dd65b6b511c1e63c7fdd1692`  
		Last Modified: Fri, 22 Apr 2022 02:25:48 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34da960e123e0d72767a541ecf7347f03dfad9502e82a54cd713eb6c1e2d294b`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 2.2 MB (2183672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0ddf5cdd828e8ea2c4c69fedbb30d4aebf50bbc1c279fae4855faec077ae98`  
		Last Modified: Fri, 22 Apr 2022 02:25:47 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05fb65dfb7bfadd22596171fe5454faeb610cc39920fc6fcddd3f99715b6594f`  
		Last Modified: Fri, 22 Apr 2022 02:27:15 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c4360a6f8123f6f8730826efa42bc162a0abfc6cc4d3e762db3f61c3f98848`  
		Last Modified: Fri, 22 Apr 2022 02:27:28 GMT  
		Size: 89.3 MB (89290810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a851624fbd4c0981e63aabd6bbfdb07b44616bed75da2079b3b7d6b78803f734`  
		Last Modified: Fri, 22 Apr 2022 02:27:16 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066be019881a416b3163e98a409f5313e4b468558f7a3c363d947312515c2d44`  
		Last Modified: Fri, 22 Apr 2022 02:27:15 GMT  
		Size: 6.8 KB (6771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5-focal`

```console
$ docker pull mariadb@sha256:78fb679e1155f656443d0c68f4510cd50f4473cd1b0b8af6e9308f945d3728d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.5-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:5d5daf7e35f3b1e8dc54b7f279bf8d0fabdc5489f329b9e4af289e92c692abd4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.9 MB (127923752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8247f649c1ad0ed98bded330f521a2114583f7d253dcb91228d0f865e76ac90`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:52:03 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 22 Apr 2022 02:52:03 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 22 Apr 2022 02:52:03 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 22 Apr 2022 02:52:03 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 22 Apr 2022 02:52:03 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:52:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:52:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:52:25 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:52:25 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:52:25 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:52:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:52:25 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:52:25 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:490dd7915b8002205becea23f1301b54b93df661098f49fb349100eace3c473d`  
		Last Modified: Fri, 22 Apr 2022 02:56:54 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0791622d551403008eaaa8a55b8c2ce888d9cf059518ffec3789cef789c4c987`  
		Last Modified: Fri, 22 Apr 2022 02:57:07 GMT  
		Size: 88.0 MB (87997283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f43c35539e9763ffe7ff15d83e7fe71d078c83207758e1114050595ca29ecfc9`  
		Last Modified: Fri, 22 Apr 2022 02:56:54 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42c10e4d1ed516fbfdc6e0848f37064f65ff78b2638f1c30002dbd8850e140d`  
		Last Modified: Fri, 22 Apr 2022 02:56:54 GMT  
		Size: 6.8 KB (6769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:625c0474316639388207ded0869b44f175076eab236114bda81b667d2b213257
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.2 MB (125185078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f5fb172364c7f183ad023a938202e2dc83ac228a56b65d707f5b05cbfa6e107`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:29:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 03:29:22 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:23 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 03:29:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 03:29:39 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 03:29:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:48 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 03:29:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 03:31:57 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 22 Apr 2022 03:31:58 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 22 Apr 2022 03:31:59 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 22 Apr 2022 03:32:00 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 22 Apr 2022 03:32:01 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 03:32:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 03:32:23 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 03:32:23 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 03:32:25 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 03:32:26 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 03:32:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 03:32:27 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 03:32:28 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7061769dfb44ec758f6d367a5d4ea0ae9e6f03ca107b7f4ee4b2419e2ae693b`  
		Last Modified: Fri, 22 Apr 2022 03:36:31 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc0a8ec71ebae8e12eafc6106df54088463cc344135ebd19dc41f331e0ed6f2`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 5.3 MB (5320310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87bc30abcdec1bcda27933f56dac195031b448391d01eb7ed27fe77b389117e7`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 3.4 MB (3370037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c05e5ca55fe31dfae11772d53c4dd507f38b7e27ba3b7b878954b5c1d9697f87`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617ab90f9424ca5c02f763590888d7804d6be962990b9f82717351743533c8f0`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 2.2 MB (2202477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bbb7ad258365e117ef11517dc6c0beadccf14acb57fba68848b61d4e0044111`  
		Last Modified: Fri, 22 Apr 2022 03:36:26 GMT  
		Size: 2.5 KB (2469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8091a565556e50b1f2a61e037a3cc54b74e533130f1ce65c6cb658a4b2c1d3ad`  
		Last Modified: Fri, 22 Apr 2022 03:38:17 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9267378c56cd36856faf39e7034a58ac75280075f26fa6b62c4682f123dbe82d`  
		Last Modified: Fri, 22 Apr 2022 03:38:32 GMT  
		Size: 87.1 MB (87108212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ddfbbb4c59339bd121747dd3678278eacdebba57051c29a81543b2a51d33e7f`  
		Last Modified: Fri, 22 Apr 2022 03:38:17 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb66f97861c0444691a7d546c9cb81cc12d54c77d7c7a68ce08a5b79ef86633`  
		Last Modified: Fri, 22 Apr 2022 03:38:17 GMT  
		Size: 6.8 KB (6770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:7253c8bbce09ad62f4aedb92fb4ece6de9a8a6b9389b70fd915a2630bc910810
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.8 MB (138780434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82b5ae0af269fec9ab843a97f38af5e144f1d13e845da7729991e23afb6c4820`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:38:45 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 22 Apr 2022 10:38:48 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 22 Apr 2022 10:38:50 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 22 Apr 2022 10:38:53 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 22 Apr 2022 10:38:56 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:39:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:40:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:40:39 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:40:41 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:40:42 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:40:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:40:47 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:40:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8585fdfb939ad59fe43800e8258791cae1a48fe19fc82bc5b28ee7cea88e25a6`  
		Last Modified: Fri, 22 Apr 2022 10:54:17 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d55c8c0f19134ea3f4e78d7db234e964e8f9b8a28d596ebe4a625594319f9159`  
		Last Modified: Fri, 22 Apr 2022 10:54:35 GMT  
		Size: 92.6 MB (92567188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6cd4f314b64534547b791600e31d8158b548b2fe4e79ecc4da4285aea8a8741`  
		Last Modified: Fri, 22 Apr 2022 10:54:17 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47740fd99121c3a1f7c4c4125a8beb046167869d84ae7ed84c2f6ea1ae329ee8`  
		Last Modified: Fri, 22 Apr 2022 10:54:17 GMT  
		Size: 6.8 KB (6772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:04652e28b66023a0295a84be62aefb6f5b2ab32171e314175a3f63a78c6aeef3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127198159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bc3c5916525d13560f4b4b25b0e8151e47a8bc455aae8a0f0a3ae03a19b2f45`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 22 Apr 2022 00:39:34 GMT
ADD file:a5fe3b5fef5d5d99022e3a45894edf18c9e5f79c4be8020d61724cdc164256b3 in / 
# Fri, 22 Apr 2022 00:39:39 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:19:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:19:18 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:19:19 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:19:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:19:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:19:48 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:19:50 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:19:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:23:41 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 22 Apr 2022 02:23:41 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 22 Apr 2022 02:23:42 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 22 Apr 2022 02:23:42 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 22 Apr 2022 02:23:43 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:23:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:24:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:24:42 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:24:42 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:24:42 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:24:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:24:44 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:24:44 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:716ba34a9a0241d7bed3fa68865e745000f025af68d21dab7d692215c5074a58`  
		Last Modified: Tue, 19 Apr 2022 13:16:37 GMT  
		Size: 27.1 MB (27085718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bc8f5833a8cfe0537845df0a5d311b211ef889ed5d5e12ace1bd3eb30834c6`  
		Last Modified: Fri, 22 Apr 2022 02:25:50 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f4186175df1fdbe352452d13a8d94670ff3446432648e7b163e9a1c6a94d88`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 5.4 MB (5378760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea503bea58815ffe61d67ad911ffab94ad5a57e364db2126c3cb11e8f732d37`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 3.2 MB (3244218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76eb02e31628a4e2997c0f38de59eb7d09325086dd65b6b511c1e63c7fdd1692`  
		Last Modified: Fri, 22 Apr 2022 02:25:48 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34da960e123e0d72767a541ecf7347f03dfad9502e82a54cd713eb6c1e2d294b`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 2.2 MB (2183672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0ddf5cdd828e8ea2c4c69fedbb30d4aebf50bbc1c279fae4855faec077ae98`  
		Last Modified: Fri, 22 Apr 2022 02:25:47 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05fb65dfb7bfadd22596171fe5454faeb610cc39920fc6fcddd3f99715b6594f`  
		Last Modified: Fri, 22 Apr 2022 02:27:15 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c4360a6f8123f6f8730826efa42bc162a0abfc6cc4d3e762db3f61c3f98848`  
		Last Modified: Fri, 22 Apr 2022 02:27:28 GMT  
		Size: 89.3 MB (89290810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a851624fbd4c0981e63aabd6bbfdb07b44616bed75da2079b3b7d6b78803f734`  
		Last Modified: Fri, 22 Apr 2022 02:27:16 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066be019881a416b3163e98a409f5313e4b468558f7a3c363d947312515c2d44`  
		Last Modified: Fri, 22 Apr 2022 02:27:15 GMT  
		Size: 6.8 KB (6771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5.15`

```console
$ docker pull mariadb@sha256:78fb679e1155f656443d0c68f4510cd50f4473cd1b0b8af6e9308f945d3728d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.5.15` - linux; amd64

```console
$ docker pull mariadb@sha256:5d5daf7e35f3b1e8dc54b7f279bf8d0fabdc5489f329b9e4af289e92c692abd4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.9 MB (127923752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8247f649c1ad0ed98bded330f521a2114583f7d253dcb91228d0f865e76ac90`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:52:03 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 22 Apr 2022 02:52:03 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 22 Apr 2022 02:52:03 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 22 Apr 2022 02:52:03 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 22 Apr 2022 02:52:03 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:52:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:52:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:52:25 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:52:25 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:52:25 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:52:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:52:25 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:52:25 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:490dd7915b8002205becea23f1301b54b93df661098f49fb349100eace3c473d`  
		Last Modified: Fri, 22 Apr 2022 02:56:54 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0791622d551403008eaaa8a55b8c2ce888d9cf059518ffec3789cef789c4c987`  
		Last Modified: Fri, 22 Apr 2022 02:57:07 GMT  
		Size: 88.0 MB (87997283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f43c35539e9763ffe7ff15d83e7fe71d078c83207758e1114050595ca29ecfc9`  
		Last Modified: Fri, 22 Apr 2022 02:56:54 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42c10e4d1ed516fbfdc6e0848f37064f65ff78b2638f1c30002dbd8850e140d`  
		Last Modified: Fri, 22 Apr 2022 02:56:54 GMT  
		Size: 6.8 KB (6769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.15` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:625c0474316639388207ded0869b44f175076eab236114bda81b667d2b213257
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.2 MB (125185078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f5fb172364c7f183ad023a938202e2dc83ac228a56b65d707f5b05cbfa6e107`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:29:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 03:29:22 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:23 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 03:29:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 03:29:39 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 03:29:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:48 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 03:29:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 03:31:57 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 22 Apr 2022 03:31:58 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 22 Apr 2022 03:31:59 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 22 Apr 2022 03:32:00 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 22 Apr 2022 03:32:01 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 03:32:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 03:32:23 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 03:32:23 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 03:32:25 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 03:32:26 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 03:32:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 03:32:27 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 03:32:28 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7061769dfb44ec758f6d367a5d4ea0ae9e6f03ca107b7f4ee4b2419e2ae693b`  
		Last Modified: Fri, 22 Apr 2022 03:36:31 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc0a8ec71ebae8e12eafc6106df54088463cc344135ebd19dc41f331e0ed6f2`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 5.3 MB (5320310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87bc30abcdec1bcda27933f56dac195031b448391d01eb7ed27fe77b389117e7`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 3.4 MB (3370037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c05e5ca55fe31dfae11772d53c4dd507f38b7e27ba3b7b878954b5c1d9697f87`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617ab90f9424ca5c02f763590888d7804d6be962990b9f82717351743533c8f0`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 2.2 MB (2202477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bbb7ad258365e117ef11517dc6c0beadccf14acb57fba68848b61d4e0044111`  
		Last Modified: Fri, 22 Apr 2022 03:36:26 GMT  
		Size: 2.5 KB (2469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8091a565556e50b1f2a61e037a3cc54b74e533130f1ce65c6cb658a4b2c1d3ad`  
		Last Modified: Fri, 22 Apr 2022 03:38:17 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9267378c56cd36856faf39e7034a58ac75280075f26fa6b62c4682f123dbe82d`  
		Last Modified: Fri, 22 Apr 2022 03:38:32 GMT  
		Size: 87.1 MB (87108212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ddfbbb4c59339bd121747dd3678278eacdebba57051c29a81543b2a51d33e7f`  
		Last Modified: Fri, 22 Apr 2022 03:38:17 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb66f97861c0444691a7d546c9cb81cc12d54c77d7c7a68ce08a5b79ef86633`  
		Last Modified: Fri, 22 Apr 2022 03:38:17 GMT  
		Size: 6.8 KB (6770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.15` - linux; ppc64le

```console
$ docker pull mariadb@sha256:7253c8bbce09ad62f4aedb92fb4ece6de9a8a6b9389b70fd915a2630bc910810
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.8 MB (138780434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82b5ae0af269fec9ab843a97f38af5e144f1d13e845da7729991e23afb6c4820`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:38:45 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 22 Apr 2022 10:38:48 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 22 Apr 2022 10:38:50 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 22 Apr 2022 10:38:53 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 22 Apr 2022 10:38:56 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:39:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:40:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:40:39 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:40:41 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:40:42 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:40:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:40:47 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:40:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8585fdfb939ad59fe43800e8258791cae1a48fe19fc82bc5b28ee7cea88e25a6`  
		Last Modified: Fri, 22 Apr 2022 10:54:17 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d55c8c0f19134ea3f4e78d7db234e964e8f9b8a28d596ebe4a625594319f9159`  
		Last Modified: Fri, 22 Apr 2022 10:54:35 GMT  
		Size: 92.6 MB (92567188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6cd4f314b64534547b791600e31d8158b548b2fe4e79ecc4da4285aea8a8741`  
		Last Modified: Fri, 22 Apr 2022 10:54:17 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47740fd99121c3a1f7c4c4125a8beb046167869d84ae7ed84c2f6ea1ae329ee8`  
		Last Modified: Fri, 22 Apr 2022 10:54:17 GMT  
		Size: 6.8 KB (6772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.15` - linux; s390x

```console
$ docker pull mariadb@sha256:04652e28b66023a0295a84be62aefb6f5b2ab32171e314175a3f63a78c6aeef3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127198159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bc3c5916525d13560f4b4b25b0e8151e47a8bc455aae8a0f0a3ae03a19b2f45`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 22 Apr 2022 00:39:34 GMT
ADD file:a5fe3b5fef5d5d99022e3a45894edf18c9e5f79c4be8020d61724cdc164256b3 in / 
# Fri, 22 Apr 2022 00:39:39 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:19:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:19:18 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:19:19 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:19:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:19:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:19:48 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:19:50 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:19:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:23:41 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 22 Apr 2022 02:23:41 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 22 Apr 2022 02:23:42 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 22 Apr 2022 02:23:42 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 22 Apr 2022 02:23:43 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:23:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:24:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:24:42 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:24:42 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:24:42 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:24:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:24:44 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:24:44 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:716ba34a9a0241d7bed3fa68865e745000f025af68d21dab7d692215c5074a58`  
		Last Modified: Tue, 19 Apr 2022 13:16:37 GMT  
		Size: 27.1 MB (27085718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bc8f5833a8cfe0537845df0a5d311b211ef889ed5d5e12ace1bd3eb30834c6`  
		Last Modified: Fri, 22 Apr 2022 02:25:50 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f4186175df1fdbe352452d13a8d94670ff3446432648e7b163e9a1c6a94d88`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 5.4 MB (5378760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea503bea58815ffe61d67ad911ffab94ad5a57e364db2126c3cb11e8f732d37`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 3.2 MB (3244218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76eb02e31628a4e2997c0f38de59eb7d09325086dd65b6b511c1e63c7fdd1692`  
		Last Modified: Fri, 22 Apr 2022 02:25:48 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34da960e123e0d72767a541ecf7347f03dfad9502e82a54cd713eb6c1e2d294b`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 2.2 MB (2183672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0ddf5cdd828e8ea2c4c69fedbb30d4aebf50bbc1c279fae4855faec077ae98`  
		Last Modified: Fri, 22 Apr 2022 02:25:47 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05fb65dfb7bfadd22596171fe5454faeb610cc39920fc6fcddd3f99715b6594f`  
		Last Modified: Fri, 22 Apr 2022 02:27:15 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c4360a6f8123f6f8730826efa42bc162a0abfc6cc4d3e762db3f61c3f98848`  
		Last Modified: Fri, 22 Apr 2022 02:27:28 GMT  
		Size: 89.3 MB (89290810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a851624fbd4c0981e63aabd6bbfdb07b44616bed75da2079b3b7d6b78803f734`  
		Last Modified: Fri, 22 Apr 2022 02:27:16 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066be019881a416b3163e98a409f5313e4b468558f7a3c363d947312515c2d44`  
		Last Modified: Fri, 22 Apr 2022 02:27:15 GMT  
		Size: 6.8 KB (6771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5.15-focal`

```console
$ docker pull mariadb@sha256:78fb679e1155f656443d0c68f4510cd50f4473cd1b0b8af6e9308f945d3728d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.5.15-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:5d5daf7e35f3b1e8dc54b7f279bf8d0fabdc5489f329b9e4af289e92c692abd4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.9 MB (127923752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8247f649c1ad0ed98bded330f521a2114583f7d253dcb91228d0f865e76ac90`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:52:03 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 22 Apr 2022 02:52:03 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 22 Apr 2022 02:52:03 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 22 Apr 2022 02:52:03 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 22 Apr 2022 02:52:03 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:52:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:52:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:52:25 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:52:25 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:52:25 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:52:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:52:25 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:52:25 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:490dd7915b8002205becea23f1301b54b93df661098f49fb349100eace3c473d`  
		Last Modified: Fri, 22 Apr 2022 02:56:54 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0791622d551403008eaaa8a55b8c2ce888d9cf059518ffec3789cef789c4c987`  
		Last Modified: Fri, 22 Apr 2022 02:57:07 GMT  
		Size: 88.0 MB (87997283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f43c35539e9763ffe7ff15d83e7fe71d078c83207758e1114050595ca29ecfc9`  
		Last Modified: Fri, 22 Apr 2022 02:56:54 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42c10e4d1ed516fbfdc6e0848f37064f65ff78b2638f1c30002dbd8850e140d`  
		Last Modified: Fri, 22 Apr 2022 02:56:54 GMT  
		Size: 6.8 KB (6769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.15-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:625c0474316639388207ded0869b44f175076eab236114bda81b667d2b213257
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.2 MB (125185078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f5fb172364c7f183ad023a938202e2dc83ac228a56b65d707f5b05cbfa6e107`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:29:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 03:29:22 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:23 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 03:29:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 03:29:39 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 03:29:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:48 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 03:29:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 03:31:57 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 22 Apr 2022 03:31:58 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 22 Apr 2022 03:31:59 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 22 Apr 2022 03:32:00 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 22 Apr 2022 03:32:01 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 03:32:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 03:32:23 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 03:32:23 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 03:32:25 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 03:32:26 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 03:32:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 03:32:27 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 03:32:28 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7061769dfb44ec758f6d367a5d4ea0ae9e6f03ca107b7f4ee4b2419e2ae693b`  
		Last Modified: Fri, 22 Apr 2022 03:36:31 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc0a8ec71ebae8e12eafc6106df54088463cc344135ebd19dc41f331e0ed6f2`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 5.3 MB (5320310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87bc30abcdec1bcda27933f56dac195031b448391d01eb7ed27fe77b389117e7`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 3.4 MB (3370037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c05e5ca55fe31dfae11772d53c4dd507f38b7e27ba3b7b878954b5c1d9697f87`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617ab90f9424ca5c02f763590888d7804d6be962990b9f82717351743533c8f0`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 2.2 MB (2202477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bbb7ad258365e117ef11517dc6c0beadccf14acb57fba68848b61d4e0044111`  
		Last Modified: Fri, 22 Apr 2022 03:36:26 GMT  
		Size: 2.5 KB (2469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8091a565556e50b1f2a61e037a3cc54b74e533130f1ce65c6cb658a4b2c1d3ad`  
		Last Modified: Fri, 22 Apr 2022 03:38:17 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9267378c56cd36856faf39e7034a58ac75280075f26fa6b62c4682f123dbe82d`  
		Last Modified: Fri, 22 Apr 2022 03:38:32 GMT  
		Size: 87.1 MB (87108212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ddfbbb4c59339bd121747dd3678278eacdebba57051c29a81543b2a51d33e7f`  
		Last Modified: Fri, 22 Apr 2022 03:38:17 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb66f97861c0444691a7d546c9cb81cc12d54c77d7c7a68ce08a5b79ef86633`  
		Last Modified: Fri, 22 Apr 2022 03:38:17 GMT  
		Size: 6.8 KB (6770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.15-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:7253c8bbce09ad62f4aedb92fb4ece6de9a8a6b9389b70fd915a2630bc910810
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.8 MB (138780434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82b5ae0af269fec9ab843a97f38af5e144f1d13e845da7729991e23afb6c4820`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:38:45 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 22 Apr 2022 10:38:48 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 22 Apr 2022 10:38:50 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 22 Apr 2022 10:38:53 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 22 Apr 2022 10:38:56 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:39:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:40:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:40:39 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:40:41 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:40:42 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:40:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:40:47 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:40:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8585fdfb939ad59fe43800e8258791cae1a48fe19fc82bc5b28ee7cea88e25a6`  
		Last Modified: Fri, 22 Apr 2022 10:54:17 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d55c8c0f19134ea3f4e78d7db234e964e8f9b8a28d596ebe4a625594319f9159`  
		Last Modified: Fri, 22 Apr 2022 10:54:35 GMT  
		Size: 92.6 MB (92567188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6cd4f314b64534547b791600e31d8158b548b2fe4e79ecc4da4285aea8a8741`  
		Last Modified: Fri, 22 Apr 2022 10:54:17 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47740fd99121c3a1f7c4c4125a8beb046167869d84ae7ed84c2f6ea1ae329ee8`  
		Last Modified: Fri, 22 Apr 2022 10:54:17 GMT  
		Size: 6.8 KB (6772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.15-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:04652e28b66023a0295a84be62aefb6f5b2ab32171e314175a3f63a78c6aeef3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127198159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bc3c5916525d13560f4b4b25b0e8151e47a8bc455aae8a0f0a3ae03a19b2f45`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 22 Apr 2022 00:39:34 GMT
ADD file:a5fe3b5fef5d5d99022e3a45894edf18c9e5f79c4be8020d61724cdc164256b3 in / 
# Fri, 22 Apr 2022 00:39:39 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:19:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:19:18 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:19:19 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:19:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:19:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:19:48 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:19:50 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:19:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:23:41 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 22 Apr 2022 02:23:41 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 22 Apr 2022 02:23:42 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 22 Apr 2022 02:23:42 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 22 Apr 2022 02:23:43 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:23:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:24:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:24:42 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:24:42 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:24:42 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:24:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:24:44 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:24:44 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:716ba34a9a0241d7bed3fa68865e745000f025af68d21dab7d692215c5074a58`  
		Last Modified: Tue, 19 Apr 2022 13:16:37 GMT  
		Size: 27.1 MB (27085718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bc8f5833a8cfe0537845df0a5d311b211ef889ed5d5e12ace1bd3eb30834c6`  
		Last Modified: Fri, 22 Apr 2022 02:25:50 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f4186175df1fdbe352452d13a8d94670ff3446432648e7b163e9a1c6a94d88`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 5.4 MB (5378760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea503bea58815ffe61d67ad911ffab94ad5a57e364db2126c3cb11e8f732d37`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 3.2 MB (3244218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76eb02e31628a4e2997c0f38de59eb7d09325086dd65b6b511c1e63c7fdd1692`  
		Last Modified: Fri, 22 Apr 2022 02:25:48 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34da960e123e0d72767a541ecf7347f03dfad9502e82a54cd713eb6c1e2d294b`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 2.2 MB (2183672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0ddf5cdd828e8ea2c4c69fedbb30d4aebf50bbc1c279fae4855faec077ae98`  
		Last Modified: Fri, 22 Apr 2022 02:25:47 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05fb65dfb7bfadd22596171fe5454faeb610cc39920fc6fcddd3f99715b6594f`  
		Last Modified: Fri, 22 Apr 2022 02:27:15 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c4360a6f8123f6f8730826efa42bc162a0abfc6cc4d3e762db3f61c3f98848`  
		Last Modified: Fri, 22 Apr 2022 02:27:28 GMT  
		Size: 89.3 MB (89290810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a851624fbd4c0981e63aabd6bbfdb07b44616bed75da2079b3b7d6b78803f734`  
		Last Modified: Fri, 22 Apr 2022 02:27:16 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066be019881a416b3163e98a409f5313e4b468558f7a3c363d947312515c2d44`  
		Last Modified: Fri, 22 Apr 2022 02:27:15 GMT  
		Size: 6.8 KB (6771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.6`

```console
$ docker pull mariadb@sha256:67cc5029c18c5743c089357a9e391d69b95b25d0ffc82c8b2ab5716f3d6411fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.6` - linux; amd64

```console
$ docker pull mariadb@sha256:50f7f199fb81c7cc4a3b367ee8a25f18ce83439a565d094d1d55d25924b195a4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.2 MB (128169667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00b1a894e91d2f10ceabfce4375d818c5ca907add9dfbaf8d5954c717baa1d5b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:51:35 GMT
ARG MARIADB_MAJOR=10.6
# Fri, 22 Apr 2022 02:51:35 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 22 Apr 2022 02:51:35 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 22 Apr 2022 02:51:35 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 22 Apr 2022 02:51:35 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:51:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:51:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:51:57 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:51:58 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:51:58 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:51:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:51:58 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:51:58 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585fa6ed9f9263b79c20959c2e25d32d6523ac4267f3f4b450311c77bbfc30ff`  
		Last Modified: Fri, 22 Apr 2022 02:56:24 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c4c29c67dbd6b0c81f43ef62d78d3a581ab7f158f68716c49129209ce26140`  
		Last Modified: Fri, 22 Apr 2022 02:56:37 GMT  
		Size: 88.2 MB (88243195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e60110958fb03947e33902acb382866ef3dc70a9dd00ec275c738ccf39c525`  
		Last Modified: Fri, 22 Apr 2022 02:56:24 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505d73d050133db6e682e04624cbd8a35f21434a6abfe41a42acf3d86f2a8be2`  
		Last Modified: Fri, 22 Apr 2022 02:56:24 GMT  
		Size: 6.8 KB (6773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:0f69dd7135467c758eaf38b002040f755b56d3f113206ad2fb619a816f892e04
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.3 MB (125269986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:954363dc348daab30d0d80cb879fadd367bf4682300fb1184cb20758ef9b4d8e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:29:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 03:29:22 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:23 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 03:29:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 03:29:39 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 03:29:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:48 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 03:29:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 03:31:21 GMT
ARG MARIADB_MAJOR=10.6
# Fri, 22 Apr 2022 03:31:21 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 22 Apr 2022 03:31:22 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 22 Apr 2022 03:31:23 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 22 Apr 2022 03:31:24 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 03:31:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 03:31:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 03:31:47 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 03:31:48 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 03:31:49 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 03:31:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 03:31:50 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 03:31:51 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7061769dfb44ec758f6d367a5d4ea0ae9e6f03ca107b7f4ee4b2419e2ae693b`  
		Last Modified: Fri, 22 Apr 2022 03:36:31 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc0a8ec71ebae8e12eafc6106df54088463cc344135ebd19dc41f331e0ed6f2`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 5.3 MB (5320310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87bc30abcdec1bcda27933f56dac195031b448391d01eb7ed27fe77b389117e7`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 3.4 MB (3370037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c05e5ca55fe31dfae11772d53c4dd507f38b7e27ba3b7b878954b5c1d9697f87`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617ab90f9424ca5c02f763590888d7804d6be962990b9f82717351743533c8f0`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 2.2 MB (2202477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bbb7ad258365e117ef11517dc6c0beadccf14acb57fba68848b61d4e0044111`  
		Last Modified: Fri, 22 Apr 2022 03:36:26 GMT  
		Size: 2.5 KB (2469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:917a0556bc96fc86ba4247ad14c91eff07a51b4c11c2b7312f359fa4952b65ab`  
		Last Modified: Fri, 22 Apr 2022 03:37:45 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:401e41504b0610c7c515f1e87b58f6a4f76b0efb434265ac79cdb26338418fcb`  
		Last Modified: Fri, 22 Apr 2022 03:37:59 GMT  
		Size: 87.2 MB (87193119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2973475b99cf2ecc2e641d21187a8b95509d5fa450da668a084548009bd61d`  
		Last Modified: Fri, 22 Apr 2022 03:37:45 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:806758339109fe9a41d7989bbe6b865c949aad6d89548ba294755aeb918fcbd1`  
		Last Modified: Fri, 22 Apr 2022 03:37:45 GMT  
		Size: 6.8 KB (6775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6` - linux; ppc64le

```console
$ docker pull mariadb@sha256:a39a7f33def5844756a0716e2080b6541f8d3be2fb462c15b689cda1bc4e516c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.8 MB (138840617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a07018cb70d1cbe1cfba60fa5297c5e412d15a54ecd11ab0f4b9888774bf1f7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:36:35 GMT
ARG MARIADB_MAJOR=10.6
# Fri, 22 Apr 2022 10:36:37 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 22 Apr 2022 10:36:39 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 22 Apr 2022 10:36:41 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 22 Apr 2022 10:36:43 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:36:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:38:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:38:16 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:38:18 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:38:20 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:38:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:38:25 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:38:28 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f321db739686e112b38409c1a2f57546c06f622fde87d19ca5f556414f96c55e`  
		Last Modified: Fri, 22 Apr 2022 10:53:38 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:587f01c1085fb65e86c6b1592a8d8fe53e2e5abc56f331aa8d55c6be5756deb4`  
		Last Modified: Fri, 22 Apr 2022 10:53:56 GMT  
		Size: 92.6 MB (92627369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f02d948139d8d0e091f50c2b98b6fafa25be9aaf1088eeabb89fa1b80bcaed34`  
		Last Modified: Fri, 22 Apr 2022 10:53:38 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:259eabdc6f306e8fc1339696c7d86f65dfae8a68f5bf05b76f16ceba8f12b2c1`  
		Last Modified: Fri, 22 Apr 2022 10:53:38 GMT  
		Size: 6.8 KB (6777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6` - linux; s390x

```console
$ docker pull mariadb@sha256:f3145aec7ef88c78b5e58998c5533b612c4340b7653db9e515771788921372de
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127224189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a5299ca6cc5d9abc9540158598205030ffb81fc77ef90715c497be93c07a78a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 00:39:34 GMT
ADD file:a5fe3b5fef5d5d99022e3a45894edf18c9e5f79c4be8020d61724cdc164256b3 in / 
# Fri, 22 Apr 2022 00:39:39 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:19:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:19:18 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:19:19 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:19:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:19:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:19:48 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:19:50 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:19:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:22:07 GMT
ARG MARIADB_MAJOR=10.6
# Fri, 22 Apr 2022 02:22:08 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 22 Apr 2022 02:22:08 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 22 Apr 2022 02:22:08 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 22 Apr 2022 02:22:08 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:22:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:23:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:23:24 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:23:25 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:23:25 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:23:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:23:26 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:23:27 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:716ba34a9a0241d7bed3fa68865e745000f025af68d21dab7d692215c5074a58`  
		Last Modified: Tue, 19 Apr 2022 13:16:37 GMT  
		Size: 27.1 MB (27085718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bc8f5833a8cfe0537845df0a5d311b211ef889ed5d5e12ace1bd3eb30834c6`  
		Last Modified: Fri, 22 Apr 2022 02:25:50 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f4186175df1fdbe352452d13a8d94670ff3446432648e7b163e9a1c6a94d88`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 5.4 MB (5378760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea503bea58815ffe61d67ad911ffab94ad5a57e364db2126c3cb11e8f732d37`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 3.2 MB (3244218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76eb02e31628a4e2997c0f38de59eb7d09325086dd65b6b511c1e63c7fdd1692`  
		Last Modified: Fri, 22 Apr 2022 02:25:48 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34da960e123e0d72767a541ecf7347f03dfad9502e82a54cd713eb6c1e2d294b`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 2.2 MB (2183672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0ddf5cdd828e8ea2c4c69fedbb30d4aebf50bbc1c279fae4855faec077ae98`  
		Last Modified: Fri, 22 Apr 2022 02:25:47 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e35c54487aecc070dabfd10f05fea192997a924c40f34ce639efb014e680c9`  
		Last Modified: Fri, 22 Apr 2022 02:26:50 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3c9680acb91618fb11946acb1d0ffe3b786aa0dca839e443807bdf8c602bf7`  
		Last Modified: Fri, 22 Apr 2022 02:27:02 GMT  
		Size: 89.3 MB (89316836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2f75131c8fca54541218624eb65a78cd5a644e59d8d26d299f25ee5de9145b`  
		Last Modified: Fri, 22 Apr 2022 02:26:49 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:452e2c047542abc87ef70ff67d163f63116cd3ffe1eadc207a6ec96b27099743`  
		Last Modified: Fri, 22 Apr 2022 02:26:50 GMT  
		Size: 6.8 KB (6775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.6-focal`

```console
$ docker pull mariadb@sha256:67cc5029c18c5743c089357a9e391d69b95b25d0ffc82c8b2ab5716f3d6411fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.6-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:50f7f199fb81c7cc4a3b367ee8a25f18ce83439a565d094d1d55d25924b195a4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.2 MB (128169667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00b1a894e91d2f10ceabfce4375d818c5ca907add9dfbaf8d5954c717baa1d5b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:51:35 GMT
ARG MARIADB_MAJOR=10.6
# Fri, 22 Apr 2022 02:51:35 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 22 Apr 2022 02:51:35 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 22 Apr 2022 02:51:35 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 22 Apr 2022 02:51:35 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:51:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:51:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:51:57 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:51:58 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:51:58 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:51:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:51:58 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:51:58 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585fa6ed9f9263b79c20959c2e25d32d6523ac4267f3f4b450311c77bbfc30ff`  
		Last Modified: Fri, 22 Apr 2022 02:56:24 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c4c29c67dbd6b0c81f43ef62d78d3a581ab7f158f68716c49129209ce26140`  
		Last Modified: Fri, 22 Apr 2022 02:56:37 GMT  
		Size: 88.2 MB (88243195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e60110958fb03947e33902acb382866ef3dc70a9dd00ec275c738ccf39c525`  
		Last Modified: Fri, 22 Apr 2022 02:56:24 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505d73d050133db6e682e04624cbd8a35f21434a6abfe41a42acf3d86f2a8be2`  
		Last Modified: Fri, 22 Apr 2022 02:56:24 GMT  
		Size: 6.8 KB (6773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:0f69dd7135467c758eaf38b002040f755b56d3f113206ad2fb619a816f892e04
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.3 MB (125269986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:954363dc348daab30d0d80cb879fadd367bf4682300fb1184cb20758ef9b4d8e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:29:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 03:29:22 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:23 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 03:29:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 03:29:39 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 03:29:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:48 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 03:29:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 03:31:21 GMT
ARG MARIADB_MAJOR=10.6
# Fri, 22 Apr 2022 03:31:21 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 22 Apr 2022 03:31:22 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 22 Apr 2022 03:31:23 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 22 Apr 2022 03:31:24 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 03:31:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 03:31:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 03:31:47 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 03:31:48 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 03:31:49 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 03:31:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 03:31:50 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 03:31:51 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7061769dfb44ec758f6d367a5d4ea0ae9e6f03ca107b7f4ee4b2419e2ae693b`  
		Last Modified: Fri, 22 Apr 2022 03:36:31 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc0a8ec71ebae8e12eafc6106df54088463cc344135ebd19dc41f331e0ed6f2`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 5.3 MB (5320310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87bc30abcdec1bcda27933f56dac195031b448391d01eb7ed27fe77b389117e7`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 3.4 MB (3370037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c05e5ca55fe31dfae11772d53c4dd507f38b7e27ba3b7b878954b5c1d9697f87`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617ab90f9424ca5c02f763590888d7804d6be962990b9f82717351743533c8f0`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 2.2 MB (2202477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bbb7ad258365e117ef11517dc6c0beadccf14acb57fba68848b61d4e0044111`  
		Last Modified: Fri, 22 Apr 2022 03:36:26 GMT  
		Size: 2.5 KB (2469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:917a0556bc96fc86ba4247ad14c91eff07a51b4c11c2b7312f359fa4952b65ab`  
		Last Modified: Fri, 22 Apr 2022 03:37:45 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:401e41504b0610c7c515f1e87b58f6a4f76b0efb434265ac79cdb26338418fcb`  
		Last Modified: Fri, 22 Apr 2022 03:37:59 GMT  
		Size: 87.2 MB (87193119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2973475b99cf2ecc2e641d21187a8b95509d5fa450da668a084548009bd61d`  
		Last Modified: Fri, 22 Apr 2022 03:37:45 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:806758339109fe9a41d7989bbe6b865c949aad6d89548ba294755aeb918fcbd1`  
		Last Modified: Fri, 22 Apr 2022 03:37:45 GMT  
		Size: 6.8 KB (6775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:a39a7f33def5844756a0716e2080b6541f8d3be2fb462c15b689cda1bc4e516c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.8 MB (138840617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a07018cb70d1cbe1cfba60fa5297c5e412d15a54ecd11ab0f4b9888774bf1f7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:36:35 GMT
ARG MARIADB_MAJOR=10.6
# Fri, 22 Apr 2022 10:36:37 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 22 Apr 2022 10:36:39 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 22 Apr 2022 10:36:41 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 22 Apr 2022 10:36:43 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:36:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:38:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:38:16 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:38:18 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:38:20 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:38:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:38:25 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:38:28 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f321db739686e112b38409c1a2f57546c06f622fde87d19ca5f556414f96c55e`  
		Last Modified: Fri, 22 Apr 2022 10:53:38 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:587f01c1085fb65e86c6b1592a8d8fe53e2e5abc56f331aa8d55c6be5756deb4`  
		Last Modified: Fri, 22 Apr 2022 10:53:56 GMT  
		Size: 92.6 MB (92627369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f02d948139d8d0e091f50c2b98b6fafa25be9aaf1088eeabb89fa1b80bcaed34`  
		Last Modified: Fri, 22 Apr 2022 10:53:38 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:259eabdc6f306e8fc1339696c7d86f65dfae8a68f5bf05b76f16ceba8f12b2c1`  
		Last Modified: Fri, 22 Apr 2022 10:53:38 GMT  
		Size: 6.8 KB (6777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:f3145aec7ef88c78b5e58998c5533b612c4340b7653db9e515771788921372de
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127224189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a5299ca6cc5d9abc9540158598205030ffb81fc77ef90715c497be93c07a78a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 00:39:34 GMT
ADD file:a5fe3b5fef5d5d99022e3a45894edf18c9e5f79c4be8020d61724cdc164256b3 in / 
# Fri, 22 Apr 2022 00:39:39 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:19:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:19:18 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:19:19 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:19:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:19:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:19:48 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:19:50 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:19:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:22:07 GMT
ARG MARIADB_MAJOR=10.6
# Fri, 22 Apr 2022 02:22:08 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 22 Apr 2022 02:22:08 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 22 Apr 2022 02:22:08 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 22 Apr 2022 02:22:08 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:22:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:23:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:23:24 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:23:25 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:23:25 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:23:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:23:26 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:23:27 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:716ba34a9a0241d7bed3fa68865e745000f025af68d21dab7d692215c5074a58`  
		Last Modified: Tue, 19 Apr 2022 13:16:37 GMT  
		Size: 27.1 MB (27085718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bc8f5833a8cfe0537845df0a5d311b211ef889ed5d5e12ace1bd3eb30834c6`  
		Last Modified: Fri, 22 Apr 2022 02:25:50 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f4186175df1fdbe352452d13a8d94670ff3446432648e7b163e9a1c6a94d88`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 5.4 MB (5378760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea503bea58815ffe61d67ad911ffab94ad5a57e364db2126c3cb11e8f732d37`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 3.2 MB (3244218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76eb02e31628a4e2997c0f38de59eb7d09325086dd65b6b511c1e63c7fdd1692`  
		Last Modified: Fri, 22 Apr 2022 02:25:48 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34da960e123e0d72767a541ecf7347f03dfad9502e82a54cd713eb6c1e2d294b`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 2.2 MB (2183672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0ddf5cdd828e8ea2c4c69fedbb30d4aebf50bbc1c279fae4855faec077ae98`  
		Last Modified: Fri, 22 Apr 2022 02:25:47 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e35c54487aecc070dabfd10f05fea192997a924c40f34ce639efb014e680c9`  
		Last Modified: Fri, 22 Apr 2022 02:26:50 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3c9680acb91618fb11946acb1d0ffe3b786aa0dca839e443807bdf8c602bf7`  
		Last Modified: Fri, 22 Apr 2022 02:27:02 GMT  
		Size: 89.3 MB (89316836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2f75131c8fca54541218624eb65a78cd5a644e59d8d26d299f25ee5de9145b`  
		Last Modified: Fri, 22 Apr 2022 02:26:49 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:452e2c047542abc87ef70ff67d163f63116cd3ffe1eadc207a6ec96b27099743`  
		Last Modified: Fri, 22 Apr 2022 02:26:50 GMT  
		Size: 6.8 KB (6775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.6.7`

```console
$ docker pull mariadb@sha256:67cc5029c18c5743c089357a9e391d69b95b25d0ffc82c8b2ab5716f3d6411fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.6.7` - linux; amd64

```console
$ docker pull mariadb@sha256:50f7f199fb81c7cc4a3b367ee8a25f18ce83439a565d094d1d55d25924b195a4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.2 MB (128169667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00b1a894e91d2f10ceabfce4375d818c5ca907add9dfbaf8d5954c717baa1d5b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:51:35 GMT
ARG MARIADB_MAJOR=10.6
# Fri, 22 Apr 2022 02:51:35 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 22 Apr 2022 02:51:35 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 22 Apr 2022 02:51:35 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 22 Apr 2022 02:51:35 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:51:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:51:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:51:57 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:51:58 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:51:58 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:51:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:51:58 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:51:58 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585fa6ed9f9263b79c20959c2e25d32d6523ac4267f3f4b450311c77bbfc30ff`  
		Last Modified: Fri, 22 Apr 2022 02:56:24 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c4c29c67dbd6b0c81f43ef62d78d3a581ab7f158f68716c49129209ce26140`  
		Last Modified: Fri, 22 Apr 2022 02:56:37 GMT  
		Size: 88.2 MB (88243195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e60110958fb03947e33902acb382866ef3dc70a9dd00ec275c738ccf39c525`  
		Last Modified: Fri, 22 Apr 2022 02:56:24 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505d73d050133db6e682e04624cbd8a35f21434a6abfe41a42acf3d86f2a8be2`  
		Last Modified: Fri, 22 Apr 2022 02:56:24 GMT  
		Size: 6.8 KB (6773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6.7` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:0f69dd7135467c758eaf38b002040f755b56d3f113206ad2fb619a816f892e04
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.3 MB (125269986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:954363dc348daab30d0d80cb879fadd367bf4682300fb1184cb20758ef9b4d8e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:29:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 03:29:22 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:23 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 03:29:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 03:29:39 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 03:29:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:48 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 03:29:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 03:31:21 GMT
ARG MARIADB_MAJOR=10.6
# Fri, 22 Apr 2022 03:31:21 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 22 Apr 2022 03:31:22 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 22 Apr 2022 03:31:23 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 22 Apr 2022 03:31:24 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 03:31:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 03:31:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 03:31:47 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 03:31:48 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 03:31:49 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 03:31:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 03:31:50 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 03:31:51 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7061769dfb44ec758f6d367a5d4ea0ae9e6f03ca107b7f4ee4b2419e2ae693b`  
		Last Modified: Fri, 22 Apr 2022 03:36:31 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc0a8ec71ebae8e12eafc6106df54088463cc344135ebd19dc41f331e0ed6f2`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 5.3 MB (5320310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87bc30abcdec1bcda27933f56dac195031b448391d01eb7ed27fe77b389117e7`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 3.4 MB (3370037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c05e5ca55fe31dfae11772d53c4dd507f38b7e27ba3b7b878954b5c1d9697f87`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617ab90f9424ca5c02f763590888d7804d6be962990b9f82717351743533c8f0`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 2.2 MB (2202477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bbb7ad258365e117ef11517dc6c0beadccf14acb57fba68848b61d4e0044111`  
		Last Modified: Fri, 22 Apr 2022 03:36:26 GMT  
		Size: 2.5 KB (2469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:917a0556bc96fc86ba4247ad14c91eff07a51b4c11c2b7312f359fa4952b65ab`  
		Last Modified: Fri, 22 Apr 2022 03:37:45 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:401e41504b0610c7c515f1e87b58f6a4f76b0efb434265ac79cdb26338418fcb`  
		Last Modified: Fri, 22 Apr 2022 03:37:59 GMT  
		Size: 87.2 MB (87193119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2973475b99cf2ecc2e641d21187a8b95509d5fa450da668a084548009bd61d`  
		Last Modified: Fri, 22 Apr 2022 03:37:45 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:806758339109fe9a41d7989bbe6b865c949aad6d89548ba294755aeb918fcbd1`  
		Last Modified: Fri, 22 Apr 2022 03:37:45 GMT  
		Size: 6.8 KB (6775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6.7` - linux; ppc64le

```console
$ docker pull mariadb@sha256:a39a7f33def5844756a0716e2080b6541f8d3be2fb462c15b689cda1bc4e516c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.8 MB (138840617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a07018cb70d1cbe1cfba60fa5297c5e412d15a54ecd11ab0f4b9888774bf1f7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:36:35 GMT
ARG MARIADB_MAJOR=10.6
# Fri, 22 Apr 2022 10:36:37 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 22 Apr 2022 10:36:39 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 22 Apr 2022 10:36:41 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 22 Apr 2022 10:36:43 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:36:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:38:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:38:16 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:38:18 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:38:20 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:38:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:38:25 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:38:28 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f321db739686e112b38409c1a2f57546c06f622fde87d19ca5f556414f96c55e`  
		Last Modified: Fri, 22 Apr 2022 10:53:38 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:587f01c1085fb65e86c6b1592a8d8fe53e2e5abc56f331aa8d55c6be5756deb4`  
		Last Modified: Fri, 22 Apr 2022 10:53:56 GMT  
		Size: 92.6 MB (92627369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f02d948139d8d0e091f50c2b98b6fafa25be9aaf1088eeabb89fa1b80bcaed34`  
		Last Modified: Fri, 22 Apr 2022 10:53:38 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:259eabdc6f306e8fc1339696c7d86f65dfae8a68f5bf05b76f16ceba8f12b2c1`  
		Last Modified: Fri, 22 Apr 2022 10:53:38 GMT  
		Size: 6.8 KB (6777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6.7` - linux; s390x

```console
$ docker pull mariadb@sha256:f3145aec7ef88c78b5e58998c5533b612c4340b7653db9e515771788921372de
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127224189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a5299ca6cc5d9abc9540158598205030ffb81fc77ef90715c497be93c07a78a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 00:39:34 GMT
ADD file:a5fe3b5fef5d5d99022e3a45894edf18c9e5f79c4be8020d61724cdc164256b3 in / 
# Fri, 22 Apr 2022 00:39:39 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:19:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:19:18 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:19:19 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:19:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:19:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:19:48 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:19:50 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:19:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:22:07 GMT
ARG MARIADB_MAJOR=10.6
# Fri, 22 Apr 2022 02:22:08 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 22 Apr 2022 02:22:08 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 22 Apr 2022 02:22:08 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 22 Apr 2022 02:22:08 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:22:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:23:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:23:24 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:23:25 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:23:25 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:23:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:23:26 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:23:27 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:716ba34a9a0241d7bed3fa68865e745000f025af68d21dab7d692215c5074a58`  
		Last Modified: Tue, 19 Apr 2022 13:16:37 GMT  
		Size: 27.1 MB (27085718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bc8f5833a8cfe0537845df0a5d311b211ef889ed5d5e12ace1bd3eb30834c6`  
		Last Modified: Fri, 22 Apr 2022 02:25:50 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f4186175df1fdbe352452d13a8d94670ff3446432648e7b163e9a1c6a94d88`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 5.4 MB (5378760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea503bea58815ffe61d67ad911ffab94ad5a57e364db2126c3cb11e8f732d37`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 3.2 MB (3244218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76eb02e31628a4e2997c0f38de59eb7d09325086dd65b6b511c1e63c7fdd1692`  
		Last Modified: Fri, 22 Apr 2022 02:25:48 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34da960e123e0d72767a541ecf7347f03dfad9502e82a54cd713eb6c1e2d294b`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 2.2 MB (2183672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0ddf5cdd828e8ea2c4c69fedbb30d4aebf50bbc1c279fae4855faec077ae98`  
		Last Modified: Fri, 22 Apr 2022 02:25:47 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e35c54487aecc070dabfd10f05fea192997a924c40f34ce639efb014e680c9`  
		Last Modified: Fri, 22 Apr 2022 02:26:50 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3c9680acb91618fb11946acb1d0ffe3b786aa0dca839e443807bdf8c602bf7`  
		Last Modified: Fri, 22 Apr 2022 02:27:02 GMT  
		Size: 89.3 MB (89316836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2f75131c8fca54541218624eb65a78cd5a644e59d8d26d299f25ee5de9145b`  
		Last Modified: Fri, 22 Apr 2022 02:26:49 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:452e2c047542abc87ef70ff67d163f63116cd3ffe1eadc207a6ec96b27099743`  
		Last Modified: Fri, 22 Apr 2022 02:26:50 GMT  
		Size: 6.8 KB (6775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.6.7-focal`

```console
$ docker pull mariadb@sha256:67cc5029c18c5743c089357a9e391d69b95b25d0ffc82c8b2ab5716f3d6411fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.6.7-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:50f7f199fb81c7cc4a3b367ee8a25f18ce83439a565d094d1d55d25924b195a4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.2 MB (128169667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00b1a894e91d2f10ceabfce4375d818c5ca907add9dfbaf8d5954c717baa1d5b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:51:35 GMT
ARG MARIADB_MAJOR=10.6
# Fri, 22 Apr 2022 02:51:35 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 22 Apr 2022 02:51:35 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 22 Apr 2022 02:51:35 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 22 Apr 2022 02:51:35 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:51:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:51:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:51:57 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:51:58 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:51:58 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:51:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:51:58 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:51:58 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585fa6ed9f9263b79c20959c2e25d32d6523ac4267f3f4b450311c77bbfc30ff`  
		Last Modified: Fri, 22 Apr 2022 02:56:24 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c4c29c67dbd6b0c81f43ef62d78d3a581ab7f158f68716c49129209ce26140`  
		Last Modified: Fri, 22 Apr 2022 02:56:37 GMT  
		Size: 88.2 MB (88243195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e60110958fb03947e33902acb382866ef3dc70a9dd00ec275c738ccf39c525`  
		Last Modified: Fri, 22 Apr 2022 02:56:24 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505d73d050133db6e682e04624cbd8a35f21434a6abfe41a42acf3d86f2a8be2`  
		Last Modified: Fri, 22 Apr 2022 02:56:24 GMT  
		Size: 6.8 KB (6773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6.7-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:0f69dd7135467c758eaf38b002040f755b56d3f113206ad2fb619a816f892e04
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.3 MB (125269986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:954363dc348daab30d0d80cb879fadd367bf4682300fb1184cb20758ef9b4d8e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:29:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 03:29:22 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:23 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 03:29:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 03:29:39 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 03:29:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:48 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 03:29:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 03:31:21 GMT
ARG MARIADB_MAJOR=10.6
# Fri, 22 Apr 2022 03:31:21 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 22 Apr 2022 03:31:22 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 22 Apr 2022 03:31:23 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 22 Apr 2022 03:31:24 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 03:31:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 03:31:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 03:31:47 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 03:31:48 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 03:31:49 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 03:31:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 03:31:50 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 03:31:51 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7061769dfb44ec758f6d367a5d4ea0ae9e6f03ca107b7f4ee4b2419e2ae693b`  
		Last Modified: Fri, 22 Apr 2022 03:36:31 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc0a8ec71ebae8e12eafc6106df54088463cc344135ebd19dc41f331e0ed6f2`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 5.3 MB (5320310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87bc30abcdec1bcda27933f56dac195031b448391d01eb7ed27fe77b389117e7`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 3.4 MB (3370037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c05e5ca55fe31dfae11772d53c4dd507f38b7e27ba3b7b878954b5c1d9697f87`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617ab90f9424ca5c02f763590888d7804d6be962990b9f82717351743533c8f0`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 2.2 MB (2202477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bbb7ad258365e117ef11517dc6c0beadccf14acb57fba68848b61d4e0044111`  
		Last Modified: Fri, 22 Apr 2022 03:36:26 GMT  
		Size: 2.5 KB (2469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:917a0556bc96fc86ba4247ad14c91eff07a51b4c11c2b7312f359fa4952b65ab`  
		Last Modified: Fri, 22 Apr 2022 03:37:45 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:401e41504b0610c7c515f1e87b58f6a4f76b0efb434265ac79cdb26338418fcb`  
		Last Modified: Fri, 22 Apr 2022 03:37:59 GMT  
		Size: 87.2 MB (87193119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2973475b99cf2ecc2e641d21187a8b95509d5fa450da668a084548009bd61d`  
		Last Modified: Fri, 22 Apr 2022 03:37:45 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:806758339109fe9a41d7989bbe6b865c949aad6d89548ba294755aeb918fcbd1`  
		Last Modified: Fri, 22 Apr 2022 03:37:45 GMT  
		Size: 6.8 KB (6775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6.7-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:a39a7f33def5844756a0716e2080b6541f8d3be2fb462c15b689cda1bc4e516c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.8 MB (138840617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a07018cb70d1cbe1cfba60fa5297c5e412d15a54ecd11ab0f4b9888774bf1f7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:36:35 GMT
ARG MARIADB_MAJOR=10.6
# Fri, 22 Apr 2022 10:36:37 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 22 Apr 2022 10:36:39 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 22 Apr 2022 10:36:41 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 22 Apr 2022 10:36:43 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:36:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:38:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:38:16 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:38:18 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:38:20 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:38:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:38:25 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:38:28 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f321db739686e112b38409c1a2f57546c06f622fde87d19ca5f556414f96c55e`  
		Last Modified: Fri, 22 Apr 2022 10:53:38 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:587f01c1085fb65e86c6b1592a8d8fe53e2e5abc56f331aa8d55c6be5756deb4`  
		Last Modified: Fri, 22 Apr 2022 10:53:56 GMT  
		Size: 92.6 MB (92627369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f02d948139d8d0e091f50c2b98b6fafa25be9aaf1088eeabb89fa1b80bcaed34`  
		Last Modified: Fri, 22 Apr 2022 10:53:38 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:259eabdc6f306e8fc1339696c7d86f65dfae8a68f5bf05b76f16ceba8f12b2c1`  
		Last Modified: Fri, 22 Apr 2022 10:53:38 GMT  
		Size: 6.8 KB (6777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6.7-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:f3145aec7ef88c78b5e58998c5533b612c4340b7653db9e515771788921372de
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127224189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a5299ca6cc5d9abc9540158598205030ffb81fc77ef90715c497be93c07a78a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 00:39:34 GMT
ADD file:a5fe3b5fef5d5d99022e3a45894edf18c9e5f79c4be8020d61724cdc164256b3 in / 
# Fri, 22 Apr 2022 00:39:39 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:19:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:19:18 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:19:19 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:19:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:19:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:19:48 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:19:50 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:19:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:22:07 GMT
ARG MARIADB_MAJOR=10.6
# Fri, 22 Apr 2022 02:22:08 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 22 Apr 2022 02:22:08 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 22 Apr 2022 02:22:08 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 22 Apr 2022 02:22:08 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:22:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:23:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:23:24 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:23:25 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:23:25 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:23:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:23:26 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:23:27 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:716ba34a9a0241d7bed3fa68865e745000f025af68d21dab7d692215c5074a58`  
		Last Modified: Tue, 19 Apr 2022 13:16:37 GMT  
		Size: 27.1 MB (27085718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bc8f5833a8cfe0537845df0a5d311b211ef889ed5d5e12ace1bd3eb30834c6`  
		Last Modified: Fri, 22 Apr 2022 02:25:50 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f4186175df1fdbe352452d13a8d94670ff3446432648e7b163e9a1c6a94d88`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 5.4 MB (5378760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea503bea58815ffe61d67ad911ffab94ad5a57e364db2126c3cb11e8f732d37`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 3.2 MB (3244218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76eb02e31628a4e2997c0f38de59eb7d09325086dd65b6b511c1e63c7fdd1692`  
		Last Modified: Fri, 22 Apr 2022 02:25:48 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34da960e123e0d72767a541ecf7347f03dfad9502e82a54cd713eb6c1e2d294b`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 2.2 MB (2183672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0ddf5cdd828e8ea2c4c69fedbb30d4aebf50bbc1c279fae4855faec077ae98`  
		Last Modified: Fri, 22 Apr 2022 02:25:47 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e35c54487aecc070dabfd10f05fea192997a924c40f34ce639efb014e680c9`  
		Last Modified: Fri, 22 Apr 2022 02:26:50 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3c9680acb91618fb11946acb1d0ffe3b786aa0dca839e443807bdf8c602bf7`  
		Last Modified: Fri, 22 Apr 2022 02:27:02 GMT  
		Size: 89.3 MB (89316836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2f75131c8fca54541218624eb65a78cd5a644e59d8d26d299f25ee5de9145b`  
		Last Modified: Fri, 22 Apr 2022 02:26:49 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:452e2c047542abc87ef70ff67d163f63116cd3ffe1eadc207a6ec96b27099743`  
		Last Modified: Fri, 22 Apr 2022 02:26:50 GMT  
		Size: 6.8 KB (6775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.7`

```console
$ docker pull mariadb@sha256:3a557616cccfbe3fa9dbcd31086511b907498dbf2526888977c87c1c8a952694
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.7` - linux; amd64

```console
$ docker pull mariadb@sha256:c5cefb5639e0f9360734406cb0f8b7a119c29083705059a1c4509cf31b6f1dbe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128668138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a1ace59b072bf4850281c7a3262a76f762ef97d774a38f5a5cddda9514dd811`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:51:07 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 02:51:07 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 02:51:07 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 02:51:07 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 02:51:07 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:51:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:51:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:51:29 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:51:29 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:51:30 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:51:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:51:30 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:51:30 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8f6c64a8fa57732c8eb3db48d751c40e0795aa5ca42f05d27c2e9ab31075bc`  
		Last Modified: Fri, 22 Apr 2022 02:55:43 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9817bd990fc72a53340f7dfdda9343811b5a6f4cbc914369c092d3994a044a`  
		Last Modified: Fri, 22 Apr 2022 02:55:56 GMT  
		Size: 88.7 MB (88741666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14828b87067569c6589bb8a62987321b440e088af17c5e8a0163841f3bba2e26`  
		Last Modified: Fri, 22 Apr 2022 02:55:42 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233be9bdce04aeae1b3a83158f299fccc9e8ef3535617d5ea40ebe5b9dcac8c6`  
		Last Modified: Fri, 22 Apr 2022 02:55:42 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:de0cb4b23ef923f913d2c4a2dc8164cd85c679fbc0b0f152188e7b0b59cc2805
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125721225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a812ba80dab1b9376c209ff5bfa06ee2d1fe4fd7382cff8b7dd05b2e02ab103`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:29:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 03:29:22 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:23 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 03:29:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 03:29:39 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 03:29:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:48 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 03:29:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 03:30:37 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 03:30:38 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 03:30:39 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 03:30:40 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 03:30:41 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 03:30:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 03:31:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 03:31:05 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 03:31:07 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 03:31:08 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 03:31:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 03:31:09 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 03:31:10 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7061769dfb44ec758f6d367a5d4ea0ae9e6f03ca107b7f4ee4b2419e2ae693b`  
		Last Modified: Fri, 22 Apr 2022 03:36:31 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc0a8ec71ebae8e12eafc6106df54088463cc344135ebd19dc41f331e0ed6f2`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 5.3 MB (5320310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87bc30abcdec1bcda27933f56dac195031b448391d01eb7ed27fe77b389117e7`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 3.4 MB (3370037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c05e5ca55fe31dfae11772d53c4dd507f38b7e27ba3b7b878954b5c1d9697f87`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617ab90f9424ca5c02f763590888d7804d6be962990b9f82717351743533c8f0`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 2.2 MB (2202477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bbb7ad258365e117ef11517dc6c0beadccf14acb57fba68848b61d4e0044111`  
		Last Modified: Fri, 22 Apr 2022 03:36:26 GMT  
		Size: 2.5 KB (2469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adee1bd260a8e20308d2463b97fdf304e75ff2a03259cb9b597295f8a899488d`  
		Last Modified: Fri, 22 Apr 2022 03:37:00 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600d1c5c23efadd0b4f5b2716ca3d427db04d06648bf9eeeffdca772ee584382`  
		Last Modified: Fri, 22 Apr 2022 03:37:13 GMT  
		Size: 87.6 MB (87644354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c9f5ecbe579c7837ce9f148319eb5dc065bedde53ae1ac35e0a124523c39ee`  
		Last Modified: Fri, 22 Apr 2022 03:37:00 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59eb437ecaf54263722ed5022a76bed608412ab4f94fc2aa7666d1653ddf23ce`  
		Last Modified: Fri, 22 Apr 2022 03:37:00 GMT  
		Size: 6.8 KB (6777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7` - linux; ppc64le

```console
$ docker pull mariadb@sha256:e66b201216b5bebbd358365e3b3c977f306720c2dcd66dad04da85aeeb1ac9ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.5 MB (139536731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ff5e20d4ebd7fe8753ba3d0e7907e1a21a78868e5672e580c4951ab3f27b484`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:34:08 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 10:34:09 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 10:34:11 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 10:34:12 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 10:34:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:34:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:36:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:36:14 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:36:15 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:36:16 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:36:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:36:19 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:36:21 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa16fdd8f2b7ed887c119c9ca942715f9f1d4e3d0704344fe671cb921c3df6e6`  
		Last Modified: Fri, 22 Apr 2022 10:52:43 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc7852c7cfc5a89e8ec199e80be577caf5cb6278d52334b86888dad8b9a5d19`  
		Last Modified: Fri, 22 Apr 2022 10:53:01 GMT  
		Size: 93.3 MB (93323480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90b1dfdfe9bb649c7f4ce895a13e16f1cefed0bd1dca47c742a8dbb7f7ecd33`  
		Last Modified: Fri, 22 Apr 2022 10:52:43 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf93f3686f15dba104bc6ae5f4303b33340d33a2d4244c00f76ef218d9ded2d`  
		Last Modified: Fri, 22 Apr 2022 10:52:43 GMT  
		Size: 6.8 KB (6778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7` - linux; s390x

```console
$ docker pull mariadb@sha256:b2805c726caa7af5fe4e44a3ade5afbbb7f7c780567c147cb36b5c7a363464b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127722709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a8b068ba5353d198e5fd7c34100da7ebc6771c257d75e23b80a211925de86aa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 00:39:34 GMT
ADD file:a5fe3b5fef5d5d99022e3a45894edf18c9e5f79c4be8020d61724cdc164256b3 in / 
# Fri, 22 Apr 2022 00:39:39 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:19:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:19:18 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:19:19 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:19:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:19:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:19:48 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:19:50 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:19:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:21:06 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 02:21:06 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 02:21:07 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 02:21:07 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 02:21:08 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:21:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:21:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:21:56 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:21:56 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:21:56 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:21:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:21:57 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:21:57 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:716ba34a9a0241d7bed3fa68865e745000f025af68d21dab7d692215c5074a58`  
		Last Modified: Tue, 19 Apr 2022 13:16:37 GMT  
		Size: 27.1 MB (27085718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bc8f5833a8cfe0537845df0a5d311b211ef889ed5d5e12ace1bd3eb30834c6`  
		Last Modified: Fri, 22 Apr 2022 02:25:50 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f4186175df1fdbe352452d13a8d94670ff3446432648e7b163e9a1c6a94d88`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 5.4 MB (5378760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea503bea58815ffe61d67ad911ffab94ad5a57e364db2126c3cb11e8f732d37`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 3.2 MB (3244218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76eb02e31628a4e2997c0f38de59eb7d09325086dd65b6b511c1e63c7fdd1692`  
		Last Modified: Fri, 22 Apr 2022 02:25:48 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34da960e123e0d72767a541ecf7347f03dfad9502e82a54cd713eb6c1e2d294b`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 2.2 MB (2183672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0ddf5cdd828e8ea2c4c69fedbb30d4aebf50bbc1c279fae4855faec077ae98`  
		Last Modified: Fri, 22 Apr 2022 02:25:47 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e906a7a4ca515f29ae2f9d042b9d50795a7722dff0e54711609032ab009449`  
		Last Modified: Fri, 22 Apr 2022 02:26:13 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8aa65ca376e03fed74f419a6a903362e83d6d4e1e1773ad67ad7183de7bbdf2`  
		Last Modified: Fri, 22 Apr 2022 02:26:26 GMT  
		Size: 89.8 MB (89815355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d48c43c28d400d613cd154b3e3182816a6e8b669d1fd7254e80bd5c51ae5f17`  
		Last Modified: Fri, 22 Apr 2022 02:26:13 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b5541b27b08286050b0bfd633e5710b2273e67032af256ca1137c955ccbd51`  
		Last Modified: Fri, 22 Apr 2022 02:26:13 GMT  
		Size: 6.8 KB (6775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.7-focal`

```console
$ docker pull mariadb@sha256:3a557616cccfbe3fa9dbcd31086511b907498dbf2526888977c87c1c8a952694
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.7-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:c5cefb5639e0f9360734406cb0f8b7a119c29083705059a1c4509cf31b6f1dbe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128668138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a1ace59b072bf4850281c7a3262a76f762ef97d774a38f5a5cddda9514dd811`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:51:07 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 02:51:07 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 02:51:07 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 02:51:07 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 02:51:07 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:51:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:51:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:51:29 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:51:29 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:51:30 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:51:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:51:30 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:51:30 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8f6c64a8fa57732c8eb3db48d751c40e0795aa5ca42f05d27c2e9ab31075bc`  
		Last Modified: Fri, 22 Apr 2022 02:55:43 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9817bd990fc72a53340f7dfdda9343811b5a6f4cbc914369c092d3994a044a`  
		Last Modified: Fri, 22 Apr 2022 02:55:56 GMT  
		Size: 88.7 MB (88741666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14828b87067569c6589bb8a62987321b440e088af17c5e8a0163841f3bba2e26`  
		Last Modified: Fri, 22 Apr 2022 02:55:42 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233be9bdce04aeae1b3a83158f299fccc9e8ef3535617d5ea40ebe5b9dcac8c6`  
		Last Modified: Fri, 22 Apr 2022 02:55:42 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:de0cb4b23ef923f913d2c4a2dc8164cd85c679fbc0b0f152188e7b0b59cc2805
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125721225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a812ba80dab1b9376c209ff5bfa06ee2d1fe4fd7382cff8b7dd05b2e02ab103`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:29:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 03:29:22 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:23 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 03:29:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 03:29:39 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 03:29:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:48 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 03:29:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 03:30:37 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 03:30:38 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 03:30:39 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 03:30:40 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 03:30:41 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 03:30:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 03:31:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 03:31:05 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 03:31:07 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 03:31:08 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 03:31:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 03:31:09 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 03:31:10 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7061769dfb44ec758f6d367a5d4ea0ae9e6f03ca107b7f4ee4b2419e2ae693b`  
		Last Modified: Fri, 22 Apr 2022 03:36:31 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc0a8ec71ebae8e12eafc6106df54088463cc344135ebd19dc41f331e0ed6f2`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 5.3 MB (5320310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87bc30abcdec1bcda27933f56dac195031b448391d01eb7ed27fe77b389117e7`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 3.4 MB (3370037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c05e5ca55fe31dfae11772d53c4dd507f38b7e27ba3b7b878954b5c1d9697f87`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617ab90f9424ca5c02f763590888d7804d6be962990b9f82717351743533c8f0`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 2.2 MB (2202477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bbb7ad258365e117ef11517dc6c0beadccf14acb57fba68848b61d4e0044111`  
		Last Modified: Fri, 22 Apr 2022 03:36:26 GMT  
		Size: 2.5 KB (2469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adee1bd260a8e20308d2463b97fdf304e75ff2a03259cb9b597295f8a899488d`  
		Last Modified: Fri, 22 Apr 2022 03:37:00 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600d1c5c23efadd0b4f5b2716ca3d427db04d06648bf9eeeffdca772ee584382`  
		Last Modified: Fri, 22 Apr 2022 03:37:13 GMT  
		Size: 87.6 MB (87644354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c9f5ecbe579c7837ce9f148319eb5dc065bedde53ae1ac35e0a124523c39ee`  
		Last Modified: Fri, 22 Apr 2022 03:37:00 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59eb437ecaf54263722ed5022a76bed608412ab4f94fc2aa7666d1653ddf23ce`  
		Last Modified: Fri, 22 Apr 2022 03:37:00 GMT  
		Size: 6.8 KB (6777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:e66b201216b5bebbd358365e3b3c977f306720c2dcd66dad04da85aeeb1ac9ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.5 MB (139536731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ff5e20d4ebd7fe8753ba3d0e7907e1a21a78868e5672e580c4951ab3f27b484`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:34:08 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 10:34:09 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 10:34:11 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 10:34:12 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 10:34:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:34:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:36:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:36:14 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:36:15 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:36:16 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:36:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:36:19 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:36:21 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa16fdd8f2b7ed887c119c9ca942715f9f1d4e3d0704344fe671cb921c3df6e6`  
		Last Modified: Fri, 22 Apr 2022 10:52:43 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc7852c7cfc5a89e8ec199e80be577caf5cb6278d52334b86888dad8b9a5d19`  
		Last Modified: Fri, 22 Apr 2022 10:53:01 GMT  
		Size: 93.3 MB (93323480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90b1dfdfe9bb649c7f4ce895a13e16f1cefed0bd1dca47c742a8dbb7f7ecd33`  
		Last Modified: Fri, 22 Apr 2022 10:52:43 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf93f3686f15dba104bc6ae5f4303b33340d33a2d4244c00f76ef218d9ded2d`  
		Last Modified: Fri, 22 Apr 2022 10:52:43 GMT  
		Size: 6.8 KB (6778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:b2805c726caa7af5fe4e44a3ade5afbbb7f7c780567c147cb36b5c7a363464b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127722709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a8b068ba5353d198e5fd7c34100da7ebc6771c257d75e23b80a211925de86aa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 00:39:34 GMT
ADD file:a5fe3b5fef5d5d99022e3a45894edf18c9e5f79c4be8020d61724cdc164256b3 in / 
# Fri, 22 Apr 2022 00:39:39 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:19:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:19:18 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:19:19 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:19:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:19:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:19:48 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:19:50 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:19:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:21:06 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 02:21:06 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 02:21:07 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 02:21:07 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 02:21:08 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:21:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:21:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:21:56 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:21:56 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:21:56 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:21:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:21:57 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:21:57 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:716ba34a9a0241d7bed3fa68865e745000f025af68d21dab7d692215c5074a58`  
		Last Modified: Tue, 19 Apr 2022 13:16:37 GMT  
		Size: 27.1 MB (27085718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bc8f5833a8cfe0537845df0a5d311b211ef889ed5d5e12ace1bd3eb30834c6`  
		Last Modified: Fri, 22 Apr 2022 02:25:50 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f4186175df1fdbe352452d13a8d94670ff3446432648e7b163e9a1c6a94d88`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 5.4 MB (5378760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea503bea58815ffe61d67ad911ffab94ad5a57e364db2126c3cb11e8f732d37`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 3.2 MB (3244218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76eb02e31628a4e2997c0f38de59eb7d09325086dd65b6b511c1e63c7fdd1692`  
		Last Modified: Fri, 22 Apr 2022 02:25:48 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34da960e123e0d72767a541ecf7347f03dfad9502e82a54cd713eb6c1e2d294b`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 2.2 MB (2183672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0ddf5cdd828e8ea2c4c69fedbb30d4aebf50bbc1c279fae4855faec077ae98`  
		Last Modified: Fri, 22 Apr 2022 02:25:47 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e906a7a4ca515f29ae2f9d042b9d50795a7722dff0e54711609032ab009449`  
		Last Modified: Fri, 22 Apr 2022 02:26:13 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8aa65ca376e03fed74f419a6a903362e83d6d4e1e1773ad67ad7183de7bbdf2`  
		Last Modified: Fri, 22 Apr 2022 02:26:26 GMT  
		Size: 89.8 MB (89815355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d48c43c28d400d613cd154b3e3182816a6e8b669d1fd7254e80bd5c51ae5f17`  
		Last Modified: Fri, 22 Apr 2022 02:26:13 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b5541b27b08286050b0bfd633e5710b2273e67032af256ca1137c955ccbd51`  
		Last Modified: Fri, 22 Apr 2022 02:26:13 GMT  
		Size: 6.8 KB (6775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.7.3`

```console
$ docker pull mariadb@sha256:3a557616cccfbe3fa9dbcd31086511b907498dbf2526888977c87c1c8a952694
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.7.3` - linux; amd64

```console
$ docker pull mariadb@sha256:c5cefb5639e0f9360734406cb0f8b7a119c29083705059a1c4509cf31b6f1dbe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128668138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a1ace59b072bf4850281c7a3262a76f762ef97d774a38f5a5cddda9514dd811`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:51:07 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 02:51:07 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 02:51:07 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 02:51:07 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 02:51:07 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:51:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:51:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:51:29 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:51:29 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:51:30 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:51:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:51:30 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:51:30 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8f6c64a8fa57732c8eb3db48d751c40e0795aa5ca42f05d27c2e9ab31075bc`  
		Last Modified: Fri, 22 Apr 2022 02:55:43 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9817bd990fc72a53340f7dfdda9343811b5a6f4cbc914369c092d3994a044a`  
		Last Modified: Fri, 22 Apr 2022 02:55:56 GMT  
		Size: 88.7 MB (88741666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14828b87067569c6589bb8a62987321b440e088af17c5e8a0163841f3bba2e26`  
		Last Modified: Fri, 22 Apr 2022 02:55:42 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233be9bdce04aeae1b3a83158f299fccc9e8ef3535617d5ea40ebe5b9dcac8c6`  
		Last Modified: Fri, 22 Apr 2022 02:55:42 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7.3` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:de0cb4b23ef923f913d2c4a2dc8164cd85c679fbc0b0f152188e7b0b59cc2805
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125721225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a812ba80dab1b9376c209ff5bfa06ee2d1fe4fd7382cff8b7dd05b2e02ab103`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:29:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 03:29:22 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:23 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 03:29:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 03:29:39 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 03:29:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:48 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 03:29:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 03:30:37 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 03:30:38 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 03:30:39 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 03:30:40 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 03:30:41 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 03:30:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 03:31:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 03:31:05 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 03:31:07 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 03:31:08 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 03:31:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 03:31:09 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 03:31:10 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7061769dfb44ec758f6d367a5d4ea0ae9e6f03ca107b7f4ee4b2419e2ae693b`  
		Last Modified: Fri, 22 Apr 2022 03:36:31 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc0a8ec71ebae8e12eafc6106df54088463cc344135ebd19dc41f331e0ed6f2`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 5.3 MB (5320310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87bc30abcdec1bcda27933f56dac195031b448391d01eb7ed27fe77b389117e7`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 3.4 MB (3370037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c05e5ca55fe31dfae11772d53c4dd507f38b7e27ba3b7b878954b5c1d9697f87`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617ab90f9424ca5c02f763590888d7804d6be962990b9f82717351743533c8f0`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 2.2 MB (2202477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bbb7ad258365e117ef11517dc6c0beadccf14acb57fba68848b61d4e0044111`  
		Last Modified: Fri, 22 Apr 2022 03:36:26 GMT  
		Size: 2.5 KB (2469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adee1bd260a8e20308d2463b97fdf304e75ff2a03259cb9b597295f8a899488d`  
		Last Modified: Fri, 22 Apr 2022 03:37:00 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600d1c5c23efadd0b4f5b2716ca3d427db04d06648bf9eeeffdca772ee584382`  
		Last Modified: Fri, 22 Apr 2022 03:37:13 GMT  
		Size: 87.6 MB (87644354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c9f5ecbe579c7837ce9f148319eb5dc065bedde53ae1ac35e0a124523c39ee`  
		Last Modified: Fri, 22 Apr 2022 03:37:00 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59eb437ecaf54263722ed5022a76bed608412ab4f94fc2aa7666d1653ddf23ce`  
		Last Modified: Fri, 22 Apr 2022 03:37:00 GMT  
		Size: 6.8 KB (6777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7.3` - linux; ppc64le

```console
$ docker pull mariadb@sha256:e66b201216b5bebbd358365e3b3c977f306720c2dcd66dad04da85aeeb1ac9ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.5 MB (139536731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ff5e20d4ebd7fe8753ba3d0e7907e1a21a78868e5672e580c4951ab3f27b484`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:34:08 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 10:34:09 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 10:34:11 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 10:34:12 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 10:34:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:34:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:36:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:36:14 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:36:15 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:36:16 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:36:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:36:19 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:36:21 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa16fdd8f2b7ed887c119c9ca942715f9f1d4e3d0704344fe671cb921c3df6e6`  
		Last Modified: Fri, 22 Apr 2022 10:52:43 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc7852c7cfc5a89e8ec199e80be577caf5cb6278d52334b86888dad8b9a5d19`  
		Last Modified: Fri, 22 Apr 2022 10:53:01 GMT  
		Size: 93.3 MB (93323480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90b1dfdfe9bb649c7f4ce895a13e16f1cefed0bd1dca47c742a8dbb7f7ecd33`  
		Last Modified: Fri, 22 Apr 2022 10:52:43 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf93f3686f15dba104bc6ae5f4303b33340d33a2d4244c00f76ef218d9ded2d`  
		Last Modified: Fri, 22 Apr 2022 10:52:43 GMT  
		Size: 6.8 KB (6778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7.3` - linux; s390x

```console
$ docker pull mariadb@sha256:b2805c726caa7af5fe4e44a3ade5afbbb7f7c780567c147cb36b5c7a363464b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127722709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a8b068ba5353d198e5fd7c34100da7ebc6771c257d75e23b80a211925de86aa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 00:39:34 GMT
ADD file:a5fe3b5fef5d5d99022e3a45894edf18c9e5f79c4be8020d61724cdc164256b3 in / 
# Fri, 22 Apr 2022 00:39:39 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:19:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:19:18 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:19:19 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:19:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:19:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:19:48 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:19:50 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:19:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:21:06 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 02:21:06 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 02:21:07 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 02:21:07 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 02:21:08 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:21:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:21:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:21:56 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:21:56 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:21:56 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:21:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:21:57 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:21:57 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:716ba34a9a0241d7bed3fa68865e745000f025af68d21dab7d692215c5074a58`  
		Last Modified: Tue, 19 Apr 2022 13:16:37 GMT  
		Size: 27.1 MB (27085718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bc8f5833a8cfe0537845df0a5d311b211ef889ed5d5e12ace1bd3eb30834c6`  
		Last Modified: Fri, 22 Apr 2022 02:25:50 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f4186175df1fdbe352452d13a8d94670ff3446432648e7b163e9a1c6a94d88`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 5.4 MB (5378760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea503bea58815ffe61d67ad911ffab94ad5a57e364db2126c3cb11e8f732d37`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 3.2 MB (3244218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76eb02e31628a4e2997c0f38de59eb7d09325086dd65b6b511c1e63c7fdd1692`  
		Last Modified: Fri, 22 Apr 2022 02:25:48 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34da960e123e0d72767a541ecf7347f03dfad9502e82a54cd713eb6c1e2d294b`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 2.2 MB (2183672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0ddf5cdd828e8ea2c4c69fedbb30d4aebf50bbc1c279fae4855faec077ae98`  
		Last Modified: Fri, 22 Apr 2022 02:25:47 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e906a7a4ca515f29ae2f9d042b9d50795a7722dff0e54711609032ab009449`  
		Last Modified: Fri, 22 Apr 2022 02:26:13 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8aa65ca376e03fed74f419a6a903362e83d6d4e1e1773ad67ad7183de7bbdf2`  
		Last Modified: Fri, 22 Apr 2022 02:26:26 GMT  
		Size: 89.8 MB (89815355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d48c43c28d400d613cd154b3e3182816a6e8b669d1fd7254e80bd5c51ae5f17`  
		Last Modified: Fri, 22 Apr 2022 02:26:13 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b5541b27b08286050b0bfd633e5710b2273e67032af256ca1137c955ccbd51`  
		Last Modified: Fri, 22 Apr 2022 02:26:13 GMT  
		Size: 6.8 KB (6775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.7.3-focal`

```console
$ docker pull mariadb@sha256:3a557616cccfbe3fa9dbcd31086511b907498dbf2526888977c87c1c8a952694
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.7.3-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:c5cefb5639e0f9360734406cb0f8b7a119c29083705059a1c4509cf31b6f1dbe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128668138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a1ace59b072bf4850281c7a3262a76f762ef97d774a38f5a5cddda9514dd811`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:51:07 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 02:51:07 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 02:51:07 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 02:51:07 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 02:51:07 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:51:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:51:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:51:29 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:51:29 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:51:30 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:51:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:51:30 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:51:30 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8f6c64a8fa57732c8eb3db48d751c40e0795aa5ca42f05d27c2e9ab31075bc`  
		Last Modified: Fri, 22 Apr 2022 02:55:43 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9817bd990fc72a53340f7dfdda9343811b5a6f4cbc914369c092d3994a044a`  
		Last Modified: Fri, 22 Apr 2022 02:55:56 GMT  
		Size: 88.7 MB (88741666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14828b87067569c6589bb8a62987321b440e088af17c5e8a0163841f3bba2e26`  
		Last Modified: Fri, 22 Apr 2022 02:55:42 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233be9bdce04aeae1b3a83158f299fccc9e8ef3535617d5ea40ebe5b9dcac8c6`  
		Last Modified: Fri, 22 Apr 2022 02:55:42 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7.3-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:de0cb4b23ef923f913d2c4a2dc8164cd85c679fbc0b0f152188e7b0b59cc2805
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125721225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a812ba80dab1b9376c209ff5bfa06ee2d1fe4fd7382cff8b7dd05b2e02ab103`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:29:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 03:29:22 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:23 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 03:29:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 03:29:39 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 03:29:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:48 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 03:29:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 03:30:37 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 03:30:38 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 03:30:39 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 03:30:40 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 03:30:41 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 03:30:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 03:31:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 03:31:05 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 03:31:07 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 03:31:08 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 03:31:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 03:31:09 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 03:31:10 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7061769dfb44ec758f6d367a5d4ea0ae9e6f03ca107b7f4ee4b2419e2ae693b`  
		Last Modified: Fri, 22 Apr 2022 03:36:31 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc0a8ec71ebae8e12eafc6106df54088463cc344135ebd19dc41f331e0ed6f2`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 5.3 MB (5320310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87bc30abcdec1bcda27933f56dac195031b448391d01eb7ed27fe77b389117e7`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 3.4 MB (3370037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c05e5ca55fe31dfae11772d53c4dd507f38b7e27ba3b7b878954b5c1d9697f87`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617ab90f9424ca5c02f763590888d7804d6be962990b9f82717351743533c8f0`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 2.2 MB (2202477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bbb7ad258365e117ef11517dc6c0beadccf14acb57fba68848b61d4e0044111`  
		Last Modified: Fri, 22 Apr 2022 03:36:26 GMT  
		Size: 2.5 KB (2469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adee1bd260a8e20308d2463b97fdf304e75ff2a03259cb9b597295f8a899488d`  
		Last Modified: Fri, 22 Apr 2022 03:37:00 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600d1c5c23efadd0b4f5b2716ca3d427db04d06648bf9eeeffdca772ee584382`  
		Last Modified: Fri, 22 Apr 2022 03:37:13 GMT  
		Size: 87.6 MB (87644354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c9f5ecbe579c7837ce9f148319eb5dc065bedde53ae1ac35e0a124523c39ee`  
		Last Modified: Fri, 22 Apr 2022 03:37:00 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59eb437ecaf54263722ed5022a76bed608412ab4f94fc2aa7666d1653ddf23ce`  
		Last Modified: Fri, 22 Apr 2022 03:37:00 GMT  
		Size: 6.8 KB (6777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7.3-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:e66b201216b5bebbd358365e3b3c977f306720c2dcd66dad04da85aeeb1ac9ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.5 MB (139536731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ff5e20d4ebd7fe8753ba3d0e7907e1a21a78868e5672e580c4951ab3f27b484`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:34:08 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 10:34:09 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 10:34:11 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 10:34:12 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 10:34:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:34:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:36:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:36:14 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:36:15 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:36:16 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:36:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:36:19 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:36:21 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa16fdd8f2b7ed887c119c9ca942715f9f1d4e3d0704344fe671cb921c3df6e6`  
		Last Modified: Fri, 22 Apr 2022 10:52:43 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc7852c7cfc5a89e8ec199e80be577caf5cb6278d52334b86888dad8b9a5d19`  
		Last Modified: Fri, 22 Apr 2022 10:53:01 GMT  
		Size: 93.3 MB (93323480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90b1dfdfe9bb649c7f4ce895a13e16f1cefed0bd1dca47c742a8dbb7f7ecd33`  
		Last Modified: Fri, 22 Apr 2022 10:52:43 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf93f3686f15dba104bc6ae5f4303b33340d33a2d4244c00f76ef218d9ded2d`  
		Last Modified: Fri, 22 Apr 2022 10:52:43 GMT  
		Size: 6.8 KB (6778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7.3-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:b2805c726caa7af5fe4e44a3ade5afbbb7f7c780567c147cb36b5c7a363464b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127722709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a8b068ba5353d198e5fd7c34100da7ebc6771c257d75e23b80a211925de86aa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 00:39:34 GMT
ADD file:a5fe3b5fef5d5d99022e3a45894edf18c9e5f79c4be8020d61724cdc164256b3 in / 
# Fri, 22 Apr 2022 00:39:39 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:19:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:19:18 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:19:19 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:19:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:19:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:19:48 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:19:50 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:19:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:21:06 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 02:21:06 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 02:21:07 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 02:21:07 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 02:21:08 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:21:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:21:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:21:56 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:21:56 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:21:56 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:21:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:21:57 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:21:57 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:716ba34a9a0241d7bed3fa68865e745000f025af68d21dab7d692215c5074a58`  
		Last Modified: Tue, 19 Apr 2022 13:16:37 GMT  
		Size: 27.1 MB (27085718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bc8f5833a8cfe0537845df0a5d311b211ef889ed5d5e12ace1bd3eb30834c6`  
		Last Modified: Fri, 22 Apr 2022 02:25:50 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f4186175df1fdbe352452d13a8d94670ff3446432648e7b163e9a1c6a94d88`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 5.4 MB (5378760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea503bea58815ffe61d67ad911ffab94ad5a57e364db2126c3cb11e8f732d37`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 3.2 MB (3244218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76eb02e31628a4e2997c0f38de59eb7d09325086dd65b6b511c1e63c7fdd1692`  
		Last Modified: Fri, 22 Apr 2022 02:25:48 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34da960e123e0d72767a541ecf7347f03dfad9502e82a54cd713eb6c1e2d294b`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 2.2 MB (2183672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0ddf5cdd828e8ea2c4c69fedbb30d4aebf50bbc1c279fae4855faec077ae98`  
		Last Modified: Fri, 22 Apr 2022 02:25:47 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e906a7a4ca515f29ae2f9d042b9d50795a7722dff0e54711609032ab009449`  
		Last Modified: Fri, 22 Apr 2022 02:26:13 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8aa65ca376e03fed74f419a6a903362e83d6d4e1e1773ad67ad7183de7bbdf2`  
		Last Modified: Fri, 22 Apr 2022 02:26:26 GMT  
		Size: 89.8 MB (89815355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d48c43c28d400d613cd154b3e3182816a6e8b669d1fd7254e80bd5c51ae5f17`  
		Last Modified: Fri, 22 Apr 2022 02:26:13 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b5541b27b08286050b0bfd633e5710b2273e67032af256ca1137c955ccbd51`  
		Last Modified: Fri, 22 Apr 2022 02:26:13 GMT  
		Size: 6.8 KB (6775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.8-rc`

```console
$ docker pull mariadb@sha256:c9238cf5c05cb7cdd175449a5864876624a4c6b5bbeb164ec43bee82ac111d6d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.8-rc` - linux; amd64

```console
$ docker pull mariadb@sha256:6207f31973a665b4d1c9ba7ea7ac726adad41a661a549561fc671b44148ce330
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.6 MB (128578395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab9732c0915d292a0e4f73669df378c84618d6492d687d02bd6217d4d3dff650`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:50:32 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 22 Apr 2022 02:50:32 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 22 Apr 2022 02:50:32 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 22 Apr 2022 02:50:32 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 22 Apr 2022 02:50:33 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:50:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:51:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:51:02 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:51:02 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:51:02 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:51:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:51:03 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:51:03 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14ba526ebec155d55cbb43daf63138efab1b47b098a037e64dd6acfcee49c6fd`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c3c04a1f7b4ecf07d5a5de05f17a2d0290974d190181a5f6a2533bde7931cf`  
		Last Modified: Fri, 22 Apr 2022 02:55:27 GMT  
		Size: 88.7 MB (88651923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8147174b3e651ed73d19ba9e151df9da5da3d253719e13ff39d98fb4f37b05b0`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e24d2b3f05313227b1155b461f451eac48ce5ae7c60d77d5cf22ed1c4bb2df9`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 6.8 KB (6773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8-rc` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:814212956f24bf7d485dddd622a602cf463d41cbe952946dea02f56c7829cda1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125650753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:169215082f9a7055ab78c69082660a7e8085644f7d7fbb937998b7dfafdcbced`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:29:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 03:29:22 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:23 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 03:29:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 03:29:39 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 03:29:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:48 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 03:29:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 03:29:51 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 22 Apr 2022 03:29:52 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 22 Apr 2022 03:29:53 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 22 Apr 2022 03:29:54 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 22 Apr 2022 03:29:55 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 03:29:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 03:30:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 03:30:18 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 03:30:19 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 03:30:20 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 03:30:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 03:30:21 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 03:30:22 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7061769dfb44ec758f6d367a5d4ea0ae9e6f03ca107b7f4ee4b2419e2ae693b`  
		Last Modified: Fri, 22 Apr 2022 03:36:31 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc0a8ec71ebae8e12eafc6106df54088463cc344135ebd19dc41f331e0ed6f2`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 5.3 MB (5320310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87bc30abcdec1bcda27933f56dac195031b448391d01eb7ed27fe77b389117e7`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 3.4 MB (3370037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c05e5ca55fe31dfae11772d53c4dd507f38b7e27ba3b7b878954b5c1d9697f87`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617ab90f9424ca5c02f763590888d7804d6be962990b9f82717351743533c8f0`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 2.2 MB (2202477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bbb7ad258365e117ef11517dc6c0beadccf14acb57fba68848b61d4e0044111`  
		Last Modified: Fri, 22 Apr 2022 03:36:26 GMT  
		Size: 2.5 KB (2469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85afb60cd7b1f7e09619805a5b846f641247be8dead53d80957df00b772ec440`  
		Last Modified: Fri, 22 Apr 2022 03:36:26 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e104cea62cdd730d4969322341072dd07a8ac60083bb447fa2c2a454947c1eb`  
		Last Modified: Fri, 22 Apr 2022 03:36:40 GMT  
		Size: 87.6 MB (87573880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bcbf803abc4baec10275b698c34a0ff66bc91754beb59f7ff3b04cb9ec689f5`  
		Last Modified: Fri, 22 Apr 2022 03:36:26 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b09524196818f5e26fdf3904ef6b8b2cbeeb750aea2569de784af07519dfda`  
		Last Modified: Fri, 22 Apr 2022 03:36:26 GMT  
		Size: 6.8 KB (6777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8-rc` - linux; ppc64le

```console
$ docker pull mariadb@sha256:89a7053031696f7d4e7553d8cab343f90e2a53df5e60091b29ae56fbe967e17a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.6 MB (139619033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c5e81f620d456e1b33bde7bf9cb5040219e3345e305dd9e8a0d53004c7cd5bb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:31:50 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 22 Apr 2022 10:31:51 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 22 Apr 2022 10:31:54 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 22 Apr 2022 10:31:55 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 22 Apr 2022 10:31:57 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:32:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:33:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:33:49 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:33:52 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:33:53 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:33:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:33:57 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:34:00 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ad9f52d7b4e854a5040fae3388098651787b071fe78342b69192cd1686a19ef`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b681bd97d5fa7c912ef840826913da6df694154fb9147f41dd223cb415316c`  
		Last Modified: Fri, 22 Apr 2022 10:52:21 GMT  
		Size: 93.4 MB (93405782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2baeda5a29e96eab044146b1ea14602da3bfcf2f2285cd12f4a43f2f6845c3d8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b269ad16de2005b90fdfbaa56368cb57a565049c8b9e4980dd91fc7d52543557`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 6.8 KB (6778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8-rc` - linux; s390x

```console
$ docker pull mariadb@sha256:c76ca29aedf81817f5b5c44c74fba2d9205af851850c6faca87445755dc4c46b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127687683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbeceb483cce646f28db321c4f1654cbcf4ed40d444f3b830997f6972e491759`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 00:39:34 GMT
ADD file:a5fe3b5fef5d5d99022e3a45894edf18c9e5f79c4be8020d61724cdc164256b3 in / 
# Fri, 22 Apr 2022 00:39:39 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:19:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:19:18 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:19:19 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:19:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:19:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:19:48 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:19:50 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:19:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:19:52 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 22 Apr 2022 02:19:52 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 22 Apr 2022 02:19:53 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 22 Apr 2022 02:19:53 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 22 Apr 2022 02:19:54 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:19:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:20:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:20:49 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:20:49 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:20:50 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:20:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:20:51 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:20:51 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:716ba34a9a0241d7bed3fa68865e745000f025af68d21dab7d692215c5074a58`  
		Last Modified: Tue, 19 Apr 2022 13:16:37 GMT  
		Size: 27.1 MB (27085718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bc8f5833a8cfe0537845df0a5d311b211ef889ed5d5e12ace1bd3eb30834c6`  
		Last Modified: Fri, 22 Apr 2022 02:25:50 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f4186175df1fdbe352452d13a8d94670ff3446432648e7b163e9a1c6a94d88`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 5.4 MB (5378760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea503bea58815ffe61d67ad911ffab94ad5a57e364db2126c3cb11e8f732d37`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 3.2 MB (3244218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76eb02e31628a4e2997c0f38de59eb7d09325086dd65b6b511c1e63c7fdd1692`  
		Last Modified: Fri, 22 Apr 2022 02:25:48 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34da960e123e0d72767a541ecf7347f03dfad9502e82a54cd713eb6c1e2d294b`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 2.2 MB (2183672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0ddf5cdd828e8ea2c4c69fedbb30d4aebf50bbc1c279fae4855faec077ae98`  
		Last Modified: Fri, 22 Apr 2022 02:25:47 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4ba62b910cb5597e9c0cd2021dfb695c794064eab1a7d836f0703ac7c9f4cd`  
		Last Modified: Fri, 22 Apr 2022 02:25:47 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bf8b985798f7ba131bf803d27319891e3ba63b1af55ec8b62db1774ba927065`  
		Last Modified: Fri, 22 Apr 2022 02:26:00 GMT  
		Size: 89.8 MB (89780333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fb9f4fbf77e6e3e22bf151c858b609c860735abe700df22f6df1e70d9442416`  
		Last Modified: Fri, 22 Apr 2022 02:25:47 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f5263367654b9b5be7517ca33c552026b40ea6536458d3bec38d908b4ded868`  
		Last Modified: Fri, 22 Apr 2022 02:25:47 GMT  
		Size: 6.8 KB (6772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.8-rc-focal`

```console
$ docker pull mariadb@sha256:c9238cf5c05cb7cdd175449a5864876624a4c6b5bbeb164ec43bee82ac111d6d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.8-rc-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:6207f31973a665b4d1c9ba7ea7ac726adad41a661a549561fc671b44148ce330
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.6 MB (128578395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab9732c0915d292a0e4f73669df378c84618d6492d687d02bd6217d4d3dff650`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:50:32 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 22 Apr 2022 02:50:32 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 22 Apr 2022 02:50:32 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 22 Apr 2022 02:50:32 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 22 Apr 2022 02:50:33 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:50:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:51:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:51:02 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:51:02 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:51:02 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:51:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:51:03 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:51:03 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14ba526ebec155d55cbb43daf63138efab1b47b098a037e64dd6acfcee49c6fd`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c3c04a1f7b4ecf07d5a5de05f17a2d0290974d190181a5f6a2533bde7931cf`  
		Last Modified: Fri, 22 Apr 2022 02:55:27 GMT  
		Size: 88.7 MB (88651923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8147174b3e651ed73d19ba9e151df9da5da3d253719e13ff39d98fb4f37b05b0`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e24d2b3f05313227b1155b461f451eac48ce5ae7c60d77d5cf22ed1c4bb2df9`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 6.8 KB (6773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8-rc-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:814212956f24bf7d485dddd622a602cf463d41cbe952946dea02f56c7829cda1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125650753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:169215082f9a7055ab78c69082660a7e8085644f7d7fbb937998b7dfafdcbced`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:29:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 03:29:22 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:23 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 03:29:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 03:29:39 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 03:29:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:48 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 03:29:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 03:29:51 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 22 Apr 2022 03:29:52 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 22 Apr 2022 03:29:53 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 22 Apr 2022 03:29:54 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 22 Apr 2022 03:29:55 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 03:29:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 03:30:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 03:30:18 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 03:30:19 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 03:30:20 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 03:30:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 03:30:21 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 03:30:22 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7061769dfb44ec758f6d367a5d4ea0ae9e6f03ca107b7f4ee4b2419e2ae693b`  
		Last Modified: Fri, 22 Apr 2022 03:36:31 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc0a8ec71ebae8e12eafc6106df54088463cc344135ebd19dc41f331e0ed6f2`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 5.3 MB (5320310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87bc30abcdec1bcda27933f56dac195031b448391d01eb7ed27fe77b389117e7`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 3.4 MB (3370037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c05e5ca55fe31dfae11772d53c4dd507f38b7e27ba3b7b878954b5c1d9697f87`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617ab90f9424ca5c02f763590888d7804d6be962990b9f82717351743533c8f0`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 2.2 MB (2202477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bbb7ad258365e117ef11517dc6c0beadccf14acb57fba68848b61d4e0044111`  
		Last Modified: Fri, 22 Apr 2022 03:36:26 GMT  
		Size: 2.5 KB (2469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85afb60cd7b1f7e09619805a5b846f641247be8dead53d80957df00b772ec440`  
		Last Modified: Fri, 22 Apr 2022 03:36:26 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e104cea62cdd730d4969322341072dd07a8ac60083bb447fa2c2a454947c1eb`  
		Last Modified: Fri, 22 Apr 2022 03:36:40 GMT  
		Size: 87.6 MB (87573880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bcbf803abc4baec10275b698c34a0ff66bc91754beb59f7ff3b04cb9ec689f5`  
		Last Modified: Fri, 22 Apr 2022 03:36:26 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b09524196818f5e26fdf3904ef6b8b2cbeeb750aea2569de784af07519dfda`  
		Last Modified: Fri, 22 Apr 2022 03:36:26 GMT  
		Size: 6.8 KB (6777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8-rc-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:89a7053031696f7d4e7553d8cab343f90e2a53df5e60091b29ae56fbe967e17a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.6 MB (139619033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c5e81f620d456e1b33bde7bf9cb5040219e3345e305dd9e8a0d53004c7cd5bb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:31:50 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 22 Apr 2022 10:31:51 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 22 Apr 2022 10:31:54 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 22 Apr 2022 10:31:55 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 22 Apr 2022 10:31:57 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:32:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:33:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:33:49 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:33:52 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:33:53 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:33:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:33:57 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:34:00 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ad9f52d7b4e854a5040fae3388098651787b071fe78342b69192cd1686a19ef`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b681bd97d5fa7c912ef840826913da6df694154fb9147f41dd223cb415316c`  
		Last Modified: Fri, 22 Apr 2022 10:52:21 GMT  
		Size: 93.4 MB (93405782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2baeda5a29e96eab044146b1ea14602da3bfcf2f2285cd12f4a43f2f6845c3d8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b269ad16de2005b90fdfbaa56368cb57a565049c8b9e4980dd91fc7d52543557`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 6.8 KB (6778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8-rc-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:c76ca29aedf81817f5b5c44c74fba2d9205af851850c6faca87445755dc4c46b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127687683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbeceb483cce646f28db321c4f1654cbcf4ed40d444f3b830997f6972e491759`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 00:39:34 GMT
ADD file:a5fe3b5fef5d5d99022e3a45894edf18c9e5f79c4be8020d61724cdc164256b3 in / 
# Fri, 22 Apr 2022 00:39:39 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:19:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:19:18 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:19:19 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:19:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:19:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:19:48 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:19:50 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:19:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:19:52 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 22 Apr 2022 02:19:52 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 22 Apr 2022 02:19:53 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 22 Apr 2022 02:19:53 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 22 Apr 2022 02:19:54 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:19:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:20:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:20:49 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:20:49 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:20:50 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:20:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:20:51 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:20:51 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:716ba34a9a0241d7bed3fa68865e745000f025af68d21dab7d692215c5074a58`  
		Last Modified: Tue, 19 Apr 2022 13:16:37 GMT  
		Size: 27.1 MB (27085718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bc8f5833a8cfe0537845df0a5d311b211ef889ed5d5e12ace1bd3eb30834c6`  
		Last Modified: Fri, 22 Apr 2022 02:25:50 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f4186175df1fdbe352452d13a8d94670ff3446432648e7b163e9a1c6a94d88`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 5.4 MB (5378760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea503bea58815ffe61d67ad911ffab94ad5a57e364db2126c3cb11e8f732d37`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 3.2 MB (3244218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76eb02e31628a4e2997c0f38de59eb7d09325086dd65b6b511c1e63c7fdd1692`  
		Last Modified: Fri, 22 Apr 2022 02:25:48 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34da960e123e0d72767a541ecf7347f03dfad9502e82a54cd713eb6c1e2d294b`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 2.2 MB (2183672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0ddf5cdd828e8ea2c4c69fedbb30d4aebf50bbc1c279fae4855faec077ae98`  
		Last Modified: Fri, 22 Apr 2022 02:25:47 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4ba62b910cb5597e9c0cd2021dfb695c794064eab1a7d836f0703ac7c9f4cd`  
		Last Modified: Fri, 22 Apr 2022 02:25:47 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bf8b985798f7ba131bf803d27319891e3ba63b1af55ec8b62db1774ba927065`  
		Last Modified: Fri, 22 Apr 2022 02:26:00 GMT  
		Size: 89.8 MB (89780333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fb9f4fbf77e6e3e22bf151c858b609c860735abe700df22f6df1e70d9442416`  
		Last Modified: Fri, 22 Apr 2022 02:25:47 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f5263367654b9b5be7517ca33c552026b40ea6536458d3bec38d908b4ded868`  
		Last Modified: Fri, 22 Apr 2022 02:25:47 GMT  
		Size: 6.8 KB (6772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.8.2-rc`

```console
$ docker pull mariadb@sha256:c9238cf5c05cb7cdd175449a5864876624a4c6b5bbeb164ec43bee82ac111d6d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.8.2-rc` - linux; amd64

```console
$ docker pull mariadb@sha256:6207f31973a665b4d1c9ba7ea7ac726adad41a661a549561fc671b44148ce330
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.6 MB (128578395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab9732c0915d292a0e4f73669df378c84618d6492d687d02bd6217d4d3dff650`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:50:32 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 22 Apr 2022 02:50:32 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 22 Apr 2022 02:50:32 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 22 Apr 2022 02:50:32 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 22 Apr 2022 02:50:33 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:50:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:51:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:51:02 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:51:02 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:51:02 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:51:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:51:03 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:51:03 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14ba526ebec155d55cbb43daf63138efab1b47b098a037e64dd6acfcee49c6fd`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c3c04a1f7b4ecf07d5a5de05f17a2d0290974d190181a5f6a2533bde7931cf`  
		Last Modified: Fri, 22 Apr 2022 02:55:27 GMT  
		Size: 88.7 MB (88651923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8147174b3e651ed73d19ba9e151df9da5da3d253719e13ff39d98fb4f37b05b0`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e24d2b3f05313227b1155b461f451eac48ce5ae7c60d77d5cf22ed1c4bb2df9`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 6.8 KB (6773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8.2-rc` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:814212956f24bf7d485dddd622a602cf463d41cbe952946dea02f56c7829cda1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125650753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:169215082f9a7055ab78c69082660a7e8085644f7d7fbb937998b7dfafdcbced`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:29:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 03:29:22 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:23 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 03:29:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 03:29:39 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 03:29:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:48 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 03:29:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 03:29:51 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 22 Apr 2022 03:29:52 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 22 Apr 2022 03:29:53 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 22 Apr 2022 03:29:54 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 22 Apr 2022 03:29:55 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 03:29:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 03:30:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 03:30:18 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 03:30:19 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 03:30:20 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 03:30:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 03:30:21 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 03:30:22 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7061769dfb44ec758f6d367a5d4ea0ae9e6f03ca107b7f4ee4b2419e2ae693b`  
		Last Modified: Fri, 22 Apr 2022 03:36:31 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc0a8ec71ebae8e12eafc6106df54088463cc344135ebd19dc41f331e0ed6f2`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 5.3 MB (5320310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87bc30abcdec1bcda27933f56dac195031b448391d01eb7ed27fe77b389117e7`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 3.4 MB (3370037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c05e5ca55fe31dfae11772d53c4dd507f38b7e27ba3b7b878954b5c1d9697f87`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617ab90f9424ca5c02f763590888d7804d6be962990b9f82717351743533c8f0`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 2.2 MB (2202477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bbb7ad258365e117ef11517dc6c0beadccf14acb57fba68848b61d4e0044111`  
		Last Modified: Fri, 22 Apr 2022 03:36:26 GMT  
		Size: 2.5 KB (2469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85afb60cd7b1f7e09619805a5b846f641247be8dead53d80957df00b772ec440`  
		Last Modified: Fri, 22 Apr 2022 03:36:26 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e104cea62cdd730d4969322341072dd07a8ac60083bb447fa2c2a454947c1eb`  
		Last Modified: Fri, 22 Apr 2022 03:36:40 GMT  
		Size: 87.6 MB (87573880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bcbf803abc4baec10275b698c34a0ff66bc91754beb59f7ff3b04cb9ec689f5`  
		Last Modified: Fri, 22 Apr 2022 03:36:26 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b09524196818f5e26fdf3904ef6b8b2cbeeb750aea2569de784af07519dfda`  
		Last Modified: Fri, 22 Apr 2022 03:36:26 GMT  
		Size: 6.8 KB (6777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8.2-rc` - linux; ppc64le

```console
$ docker pull mariadb@sha256:89a7053031696f7d4e7553d8cab343f90e2a53df5e60091b29ae56fbe967e17a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.6 MB (139619033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c5e81f620d456e1b33bde7bf9cb5040219e3345e305dd9e8a0d53004c7cd5bb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:31:50 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 22 Apr 2022 10:31:51 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 22 Apr 2022 10:31:54 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 22 Apr 2022 10:31:55 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 22 Apr 2022 10:31:57 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:32:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:33:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:33:49 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:33:52 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:33:53 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:33:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:33:57 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:34:00 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ad9f52d7b4e854a5040fae3388098651787b071fe78342b69192cd1686a19ef`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b681bd97d5fa7c912ef840826913da6df694154fb9147f41dd223cb415316c`  
		Last Modified: Fri, 22 Apr 2022 10:52:21 GMT  
		Size: 93.4 MB (93405782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2baeda5a29e96eab044146b1ea14602da3bfcf2f2285cd12f4a43f2f6845c3d8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b269ad16de2005b90fdfbaa56368cb57a565049c8b9e4980dd91fc7d52543557`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 6.8 KB (6778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8.2-rc` - linux; s390x

```console
$ docker pull mariadb@sha256:c76ca29aedf81817f5b5c44c74fba2d9205af851850c6faca87445755dc4c46b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127687683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbeceb483cce646f28db321c4f1654cbcf4ed40d444f3b830997f6972e491759`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 00:39:34 GMT
ADD file:a5fe3b5fef5d5d99022e3a45894edf18c9e5f79c4be8020d61724cdc164256b3 in / 
# Fri, 22 Apr 2022 00:39:39 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:19:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:19:18 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:19:19 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:19:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:19:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:19:48 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:19:50 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:19:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:19:52 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 22 Apr 2022 02:19:52 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 22 Apr 2022 02:19:53 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 22 Apr 2022 02:19:53 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 22 Apr 2022 02:19:54 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:19:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:20:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:20:49 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:20:49 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:20:50 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:20:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:20:51 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:20:51 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:716ba34a9a0241d7bed3fa68865e745000f025af68d21dab7d692215c5074a58`  
		Last Modified: Tue, 19 Apr 2022 13:16:37 GMT  
		Size: 27.1 MB (27085718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bc8f5833a8cfe0537845df0a5d311b211ef889ed5d5e12ace1bd3eb30834c6`  
		Last Modified: Fri, 22 Apr 2022 02:25:50 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f4186175df1fdbe352452d13a8d94670ff3446432648e7b163e9a1c6a94d88`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 5.4 MB (5378760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea503bea58815ffe61d67ad911ffab94ad5a57e364db2126c3cb11e8f732d37`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 3.2 MB (3244218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76eb02e31628a4e2997c0f38de59eb7d09325086dd65b6b511c1e63c7fdd1692`  
		Last Modified: Fri, 22 Apr 2022 02:25:48 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34da960e123e0d72767a541ecf7347f03dfad9502e82a54cd713eb6c1e2d294b`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 2.2 MB (2183672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0ddf5cdd828e8ea2c4c69fedbb30d4aebf50bbc1c279fae4855faec077ae98`  
		Last Modified: Fri, 22 Apr 2022 02:25:47 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4ba62b910cb5597e9c0cd2021dfb695c794064eab1a7d836f0703ac7c9f4cd`  
		Last Modified: Fri, 22 Apr 2022 02:25:47 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bf8b985798f7ba131bf803d27319891e3ba63b1af55ec8b62db1774ba927065`  
		Last Modified: Fri, 22 Apr 2022 02:26:00 GMT  
		Size: 89.8 MB (89780333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fb9f4fbf77e6e3e22bf151c858b609c860735abe700df22f6df1e70d9442416`  
		Last Modified: Fri, 22 Apr 2022 02:25:47 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f5263367654b9b5be7517ca33c552026b40ea6536458d3bec38d908b4ded868`  
		Last Modified: Fri, 22 Apr 2022 02:25:47 GMT  
		Size: 6.8 KB (6772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.8.2-rc-focal`

```console
$ docker pull mariadb@sha256:c9238cf5c05cb7cdd175449a5864876624a4c6b5bbeb164ec43bee82ac111d6d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.8.2-rc-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:6207f31973a665b4d1c9ba7ea7ac726adad41a661a549561fc671b44148ce330
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.6 MB (128578395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab9732c0915d292a0e4f73669df378c84618d6492d687d02bd6217d4d3dff650`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:50:32 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 22 Apr 2022 02:50:32 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 22 Apr 2022 02:50:32 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 22 Apr 2022 02:50:32 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 22 Apr 2022 02:50:33 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:50:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:51:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:51:02 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:51:02 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:51:02 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:51:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:51:03 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:51:03 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14ba526ebec155d55cbb43daf63138efab1b47b098a037e64dd6acfcee49c6fd`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c3c04a1f7b4ecf07d5a5de05f17a2d0290974d190181a5f6a2533bde7931cf`  
		Last Modified: Fri, 22 Apr 2022 02:55:27 GMT  
		Size: 88.7 MB (88651923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8147174b3e651ed73d19ba9e151df9da5da3d253719e13ff39d98fb4f37b05b0`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e24d2b3f05313227b1155b461f451eac48ce5ae7c60d77d5cf22ed1c4bb2df9`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 6.8 KB (6773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8.2-rc-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:814212956f24bf7d485dddd622a602cf463d41cbe952946dea02f56c7829cda1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125650753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:169215082f9a7055ab78c69082660a7e8085644f7d7fbb937998b7dfafdcbced`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:29:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 03:29:22 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:23 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 03:29:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 03:29:39 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 03:29:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:48 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 03:29:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 03:29:51 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 22 Apr 2022 03:29:52 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 22 Apr 2022 03:29:53 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 22 Apr 2022 03:29:54 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 22 Apr 2022 03:29:55 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 03:29:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 03:30:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 03:30:18 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 03:30:19 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 03:30:20 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 03:30:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 03:30:21 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 03:30:22 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7061769dfb44ec758f6d367a5d4ea0ae9e6f03ca107b7f4ee4b2419e2ae693b`  
		Last Modified: Fri, 22 Apr 2022 03:36:31 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc0a8ec71ebae8e12eafc6106df54088463cc344135ebd19dc41f331e0ed6f2`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 5.3 MB (5320310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87bc30abcdec1bcda27933f56dac195031b448391d01eb7ed27fe77b389117e7`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 3.4 MB (3370037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c05e5ca55fe31dfae11772d53c4dd507f38b7e27ba3b7b878954b5c1d9697f87`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617ab90f9424ca5c02f763590888d7804d6be962990b9f82717351743533c8f0`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 2.2 MB (2202477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bbb7ad258365e117ef11517dc6c0beadccf14acb57fba68848b61d4e0044111`  
		Last Modified: Fri, 22 Apr 2022 03:36:26 GMT  
		Size: 2.5 KB (2469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85afb60cd7b1f7e09619805a5b846f641247be8dead53d80957df00b772ec440`  
		Last Modified: Fri, 22 Apr 2022 03:36:26 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e104cea62cdd730d4969322341072dd07a8ac60083bb447fa2c2a454947c1eb`  
		Last Modified: Fri, 22 Apr 2022 03:36:40 GMT  
		Size: 87.6 MB (87573880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bcbf803abc4baec10275b698c34a0ff66bc91754beb59f7ff3b04cb9ec689f5`  
		Last Modified: Fri, 22 Apr 2022 03:36:26 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b09524196818f5e26fdf3904ef6b8b2cbeeb750aea2569de784af07519dfda`  
		Last Modified: Fri, 22 Apr 2022 03:36:26 GMT  
		Size: 6.8 KB (6777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8.2-rc-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:89a7053031696f7d4e7553d8cab343f90e2a53df5e60091b29ae56fbe967e17a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.6 MB (139619033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c5e81f620d456e1b33bde7bf9cb5040219e3345e305dd9e8a0d53004c7cd5bb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:31:50 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 22 Apr 2022 10:31:51 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 22 Apr 2022 10:31:54 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 22 Apr 2022 10:31:55 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 22 Apr 2022 10:31:57 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:32:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:33:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:33:49 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:33:52 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:33:53 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:33:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:33:57 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:34:00 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ad9f52d7b4e854a5040fae3388098651787b071fe78342b69192cd1686a19ef`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b681bd97d5fa7c912ef840826913da6df694154fb9147f41dd223cb415316c`  
		Last Modified: Fri, 22 Apr 2022 10:52:21 GMT  
		Size: 93.4 MB (93405782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2baeda5a29e96eab044146b1ea14602da3bfcf2f2285cd12f4a43f2f6845c3d8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b269ad16de2005b90fdfbaa56368cb57a565049c8b9e4980dd91fc7d52543557`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 6.8 KB (6778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8.2-rc-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:c76ca29aedf81817f5b5c44c74fba2d9205af851850c6faca87445755dc4c46b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127687683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbeceb483cce646f28db321c4f1654cbcf4ed40d444f3b830997f6972e491759`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 00:39:34 GMT
ADD file:a5fe3b5fef5d5d99022e3a45894edf18c9e5f79c4be8020d61724cdc164256b3 in / 
# Fri, 22 Apr 2022 00:39:39 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:19:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:19:18 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:19:19 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:19:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:19:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:19:48 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:19:50 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:19:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:19:52 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 22 Apr 2022 02:19:52 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 22 Apr 2022 02:19:53 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 22 Apr 2022 02:19:53 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 22 Apr 2022 02:19:54 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:19:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:20:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:20:49 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:20:49 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:20:50 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:20:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:20:51 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:20:51 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:716ba34a9a0241d7bed3fa68865e745000f025af68d21dab7d692215c5074a58`  
		Last Modified: Tue, 19 Apr 2022 13:16:37 GMT  
		Size: 27.1 MB (27085718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bc8f5833a8cfe0537845df0a5d311b211ef889ed5d5e12ace1bd3eb30834c6`  
		Last Modified: Fri, 22 Apr 2022 02:25:50 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f4186175df1fdbe352452d13a8d94670ff3446432648e7b163e9a1c6a94d88`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 5.4 MB (5378760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea503bea58815ffe61d67ad911ffab94ad5a57e364db2126c3cb11e8f732d37`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 3.2 MB (3244218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76eb02e31628a4e2997c0f38de59eb7d09325086dd65b6b511c1e63c7fdd1692`  
		Last Modified: Fri, 22 Apr 2022 02:25:48 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34da960e123e0d72767a541ecf7347f03dfad9502e82a54cd713eb6c1e2d294b`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 2.2 MB (2183672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0ddf5cdd828e8ea2c4c69fedbb30d4aebf50bbc1c279fae4855faec077ae98`  
		Last Modified: Fri, 22 Apr 2022 02:25:47 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4ba62b910cb5597e9c0cd2021dfb695c794064eab1a7d836f0703ac7c9f4cd`  
		Last Modified: Fri, 22 Apr 2022 02:25:47 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bf8b985798f7ba131bf803d27319891e3ba63b1af55ec8b62db1774ba927065`  
		Last Modified: Fri, 22 Apr 2022 02:26:00 GMT  
		Size: 89.8 MB (89780333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fb9f4fbf77e6e3e22bf151c858b609c860735abe700df22f6df1e70d9442416`  
		Last Modified: Fri, 22 Apr 2022 02:25:47 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f5263367654b9b5be7517ca33c552026b40ea6536458d3bec38d908b4ded868`  
		Last Modified: Fri, 22 Apr 2022 02:25:47 GMT  
		Size: 6.8 KB (6772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:focal`

```console
$ docker pull mariadb@sha256:3a557616cccfbe3fa9dbcd31086511b907498dbf2526888977c87c1c8a952694
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:focal` - linux; amd64

```console
$ docker pull mariadb@sha256:c5cefb5639e0f9360734406cb0f8b7a119c29083705059a1c4509cf31b6f1dbe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128668138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a1ace59b072bf4850281c7a3262a76f762ef97d774a38f5a5cddda9514dd811`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:51:07 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 02:51:07 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 02:51:07 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 02:51:07 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 02:51:07 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:51:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:51:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:51:29 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:51:29 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:51:30 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:51:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:51:30 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:51:30 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8f6c64a8fa57732c8eb3db48d751c40e0795aa5ca42f05d27c2e9ab31075bc`  
		Last Modified: Fri, 22 Apr 2022 02:55:43 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9817bd990fc72a53340f7dfdda9343811b5a6f4cbc914369c092d3994a044a`  
		Last Modified: Fri, 22 Apr 2022 02:55:56 GMT  
		Size: 88.7 MB (88741666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14828b87067569c6589bb8a62987321b440e088af17c5e8a0163841f3bba2e26`  
		Last Modified: Fri, 22 Apr 2022 02:55:42 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233be9bdce04aeae1b3a83158f299fccc9e8ef3535617d5ea40ebe5b9dcac8c6`  
		Last Modified: Fri, 22 Apr 2022 02:55:42 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:de0cb4b23ef923f913d2c4a2dc8164cd85c679fbc0b0f152188e7b0b59cc2805
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125721225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a812ba80dab1b9376c209ff5bfa06ee2d1fe4fd7382cff8b7dd05b2e02ab103`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:29:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 03:29:22 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:23 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 03:29:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 03:29:39 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 03:29:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:48 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 03:29:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 03:30:37 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 03:30:38 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 03:30:39 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 03:30:40 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 03:30:41 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 03:30:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 03:31:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 03:31:05 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 03:31:07 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 03:31:08 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 03:31:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 03:31:09 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 03:31:10 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7061769dfb44ec758f6d367a5d4ea0ae9e6f03ca107b7f4ee4b2419e2ae693b`  
		Last Modified: Fri, 22 Apr 2022 03:36:31 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc0a8ec71ebae8e12eafc6106df54088463cc344135ebd19dc41f331e0ed6f2`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 5.3 MB (5320310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87bc30abcdec1bcda27933f56dac195031b448391d01eb7ed27fe77b389117e7`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 3.4 MB (3370037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c05e5ca55fe31dfae11772d53c4dd507f38b7e27ba3b7b878954b5c1d9697f87`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617ab90f9424ca5c02f763590888d7804d6be962990b9f82717351743533c8f0`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 2.2 MB (2202477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bbb7ad258365e117ef11517dc6c0beadccf14acb57fba68848b61d4e0044111`  
		Last Modified: Fri, 22 Apr 2022 03:36:26 GMT  
		Size: 2.5 KB (2469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adee1bd260a8e20308d2463b97fdf304e75ff2a03259cb9b597295f8a899488d`  
		Last Modified: Fri, 22 Apr 2022 03:37:00 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600d1c5c23efadd0b4f5b2716ca3d427db04d06648bf9eeeffdca772ee584382`  
		Last Modified: Fri, 22 Apr 2022 03:37:13 GMT  
		Size: 87.6 MB (87644354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c9f5ecbe579c7837ce9f148319eb5dc065bedde53ae1ac35e0a124523c39ee`  
		Last Modified: Fri, 22 Apr 2022 03:37:00 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59eb437ecaf54263722ed5022a76bed608412ab4f94fc2aa7666d1653ddf23ce`  
		Last Modified: Fri, 22 Apr 2022 03:37:00 GMT  
		Size: 6.8 KB (6777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:e66b201216b5bebbd358365e3b3c977f306720c2dcd66dad04da85aeeb1ac9ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.5 MB (139536731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ff5e20d4ebd7fe8753ba3d0e7907e1a21a78868e5672e580c4951ab3f27b484`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:34:08 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 10:34:09 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 10:34:11 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 10:34:12 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 10:34:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:34:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:36:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:36:14 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:36:15 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:36:16 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:36:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:36:19 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:36:21 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa16fdd8f2b7ed887c119c9ca942715f9f1d4e3d0704344fe671cb921c3df6e6`  
		Last Modified: Fri, 22 Apr 2022 10:52:43 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc7852c7cfc5a89e8ec199e80be577caf5cb6278d52334b86888dad8b9a5d19`  
		Last Modified: Fri, 22 Apr 2022 10:53:01 GMT  
		Size: 93.3 MB (93323480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90b1dfdfe9bb649c7f4ce895a13e16f1cefed0bd1dca47c742a8dbb7f7ecd33`  
		Last Modified: Fri, 22 Apr 2022 10:52:43 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf93f3686f15dba104bc6ae5f4303b33340d33a2d4244c00f76ef218d9ded2d`  
		Last Modified: Fri, 22 Apr 2022 10:52:43 GMT  
		Size: 6.8 KB (6778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:focal` - linux; s390x

```console
$ docker pull mariadb@sha256:b2805c726caa7af5fe4e44a3ade5afbbb7f7c780567c147cb36b5c7a363464b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127722709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a8b068ba5353d198e5fd7c34100da7ebc6771c257d75e23b80a211925de86aa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 00:39:34 GMT
ADD file:a5fe3b5fef5d5d99022e3a45894edf18c9e5f79c4be8020d61724cdc164256b3 in / 
# Fri, 22 Apr 2022 00:39:39 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:19:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:19:18 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:19:19 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:19:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:19:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:19:48 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:19:50 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:19:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:21:06 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 02:21:06 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 02:21:07 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 02:21:07 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 02:21:08 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:21:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:21:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:21:56 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:21:56 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:21:56 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:21:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:21:57 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:21:57 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:716ba34a9a0241d7bed3fa68865e745000f025af68d21dab7d692215c5074a58`  
		Last Modified: Tue, 19 Apr 2022 13:16:37 GMT  
		Size: 27.1 MB (27085718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bc8f5833a8cfe0537845df0a5d311b211ef889ed5d5e12ace1bd3eb30834c6`  
		Last Modified: Fri, 22 Apr 2022 02:25:50 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f4186175df1fdbe352452d13a8d94670ff3446432648e7b163e9a1c6a94d88`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 5.4 MB (5378760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea503bea58815ffe61d67ad911ffab94ad5a57e364db2126c3cb11e8f732d37`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 3.2 MB (3244218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76eb02e31628a4e2997c0f38de59eb7d09325086dd65b6b511c1e63c7fdd1692`  
		Last Modified: Fri, 22 Apr 2022 02:25:48 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34da960e123e0d72767a541ecf7347f03dfad9502e82a54cd713eb6c1e2d294b`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 2.2 MB (2183672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0ddf5cdd828e8ea2c4c69fedbb30d4aebf50bbc1c279fae4855faec077ae98`  
		Last Modified: Fri, 22 Apr 2022 02:25:47 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e906a7a4ca515f29ae2f9d042b9d50795a7722dff0e54711609032ab009449`  
		Last Modified: Fri, 22 Apr 2022 02:26:13 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8aa65ca376e03fed74f419a6a903362e83d6d4e1e1773ad67ad7183de7bbdf2`  
		Last Modified: Fri, 22 Apr 2022 02:26:26 GMT  
		Size: 89.8 MB (89815355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d48c43c28d400d613cd154b3e3182816a6e8b669d1fd7254e80bd5c51ae5f17`  
		Last Modified: Fri, 22 Apr 2022 02:26:13 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b5541b27b08286050b0bfd633e5710b2273e67032af256ca1137c955ccbd51`  
		Last Modified: Fri, 22 Apr 2022 02:26:13 GMT  
		Size: 6.8 KB (6775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:latest`

```console
$ docker pull mariadb@sha256:3a557616cccfbe3fa9dbcd31086511b907498dbf2526888977c87c1c8a952694
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:latest` - linux; amd64

```console
$ docker pull mariadb@sha256:c5cefb5639e0f9360734406cb0f8b7a119c29083705059a1c4509cf31b6f1dbe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128668138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a1ace59b072bf4850281c7a3262a76f762ef97d774a38f5a5cddda9514dd811`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:51:07 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 02:51:07 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 02:51:07 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 02:51:07 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 02:51:07 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:51:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:51:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:51:29 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:51:29 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:51:30 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:51:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:51:30 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:51:30 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8f6c64a8fa57732c8eb3db48d751c40e0795aa5ca42f05d27c2e9ab31075bc`  
		Last Modified: Fri, 22 Apr 2022 02:55:43 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9817bd990fc72a53340f7dfdda9343811b5a6f4cbc914369c092d3994a044a`  
		Last Modified: Fri, 22 Apr 2022 02:55:56 GMT  
		Size: 88.7 MB (88741666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14828b87067569c6589bb8a62987321b440e088af17c5e8a0163841f3bba2e26`  
		Last Modified: Fri, 22 Apr 2022 02:55:42 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233be9bdce04aeae1b3a83158f299fccc9e8ef3535617d5ea40ebe5b9dcac8c6`  
		Last Modified: Fri, 22 Apr 2022 02:55:42 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:de0cb4b23ef923f913d2c4a2dc8164cd85c679fbc0b0f152188e7b0b59cc2805
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125721225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a812ba80dab1b9376c209ff5bfa06ee2d1fe4fd7382cff8b7dd05b2e02ab103`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:29:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 03:29:22 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:23 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 03:29:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 03:29:39 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 03:29:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:29:48 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 03:29:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 03:30:37 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 03:30:38 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 03:30:39 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 03:30:40 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 03:30:41 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 03:30:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 03:31:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 03:31:05 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 03:31:07 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 03:31:08 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 03:31:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 03:31:09 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 03:31:10 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7061769dfb44ec758f6d367a5d4ea0ae9e6f03ca107b7f4ee4b2419e2ae693b`  
		Last Modified: Fri, 22 Apr 2022 03:36:31 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc0a8ec71ebae8e12eafc6106df54088463cc344135ebd19dc41f331e0ed6f2`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 5.3 MB (5320310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87bc30abcdec1bcda27933f56dac195031b448391d01eb7ed27fe77b389117e7`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 3.4 MB (3370037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c05e5ca55fe31dfae11772d53c4dd507f38b7e27ba3b7b878954b5c1d9697f87`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617ab90f9424ca5c02f763590888d7804d6be962990b9f82717351743533c8f0`  
		Last Modified: Fri, 22 Apr 2022 03:36:29 GMT  
		Size: 2.2 MB (2202477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bbb7ad258365e117ef11517dc6c0beadccf14acb57fba68848b61d4e0044111`  
		Last Modified: Fri, 22 Apr 2022 03:36:26 GMT  
		Size: 2.5 KB (2469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adee1bd260a8e20308d2463b97fdf304e75ff2a03259cb9b597295f8a899488d`  
		Last Modified: Fri, 22 Apr 2022 03:37:00 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600d1c5c23efadd0b4f5b2716ca3d427db04d06648bf9eeeffdca772ee584382`  
		Last Modified: Fri, 22 Apr 2022 03:37:13 GMT  
		Size: 87.6 MB (87644354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c9f5ecbe579c7837ce9f148319eb5dc065bedde53ae1ac35e0a124523c39ee`  
		Last Modified: Fri, 22 Apr 2022 03:37:00 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59eb437ecaf54263722ed5022a76bed608412ab4f94fc2aa7666d1653ddf23ce`  
		Last Modified: Fri, 22 Apr 2022 03:37:00 GMT  
		Size: 6.8 KB (6777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; ppc64le

```console
$ docker pull mariadb@sha256:e66b201216b5bebbd358365e3b3c977f306720c2dcd66dad04da85aeeb1ac9ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.5 MB (139536731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ff5e20d4ebd7fe8753ba3d0e7907e1a21a78868e5672e580c4951ab3f27b484`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:34:08 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 10:34:09 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 10:34:11 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 10:34:12 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 10:34:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:34:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:36:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:36:14 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:36:15 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:36:16 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:36:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:36:19 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:36:21 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa16fdd8f2b7ed887c119c9ca942715f9f1d4e3d0704344fe671cb921c3df6e6`  
		Last Modified: Fri, 22 Apr 2022 10:52:43 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc7852c7cfc5a89e8ec199e80be577caf5cb6278d52334b86888dad8b9a5d19`  
		Last Modified: Fri, 22 Apr 2022 10:53:01 GMT  
		Size: 93.3 MB (93323480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90b1dfdfe9bb649c7f4ce895a13e16f1cefed0bd1dca47c742a8dbb7f7ecd33`  
		Last Modified: Fri, 22 Apr 2022 10:52:43 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf93f3686f15dba104bc6ae5f4303b33340d33a2d4244c00f76ef218d9ded2d`  
		Last Modified: Fri, 22 Apr 2022 10:52:43 GMT  
		Size: 6.8 KB (6778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; s390x

```console
$ docker pull mariadb@sha256:b2805c726caa7af5fe4e44a3ade5afbbb7f7c780567c147cb36b5c7a363464b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127722709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a8b068ba5353d198e5fd7c34100da7ebc6771c257d75e23b80a211925de86aa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 00:39:34 GMT
ADD file:a5fe3b5fef5d5d99022e3a45894edf18c9e5f79c4be8020d61724cdc164256b3 in / 
# Fri, 22 Apr 2022 00:39:39 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:19:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:19:18 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:19:19 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:19:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:19:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:19:48 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:19:50 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:19:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:21:06 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 02:21:06 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 02:21:07 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 02:21:07 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 02:21:08 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:21:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:21:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:21:56 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:21:56 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:21:56 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:21:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:21:57 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:21:57 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:716ba34a9a0241d7bed3fa68865e745000f025af68d21dab7d692215c5074a58`  
		Last Modified: Tue, 19 Apr 2022 13:16:37 GMT  
		Size: 27.1 MB (27085718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bc8f5833a8cfe0537845df0a5d311b211ef889ed5d5e12ace1bd3eb30834c6`  
		Last Modified: Fri, 22 Apr 2022 02:25:50 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f4186175df1fdbe352452d13a8d94670ff3446432648e7b163e9a1c6a94d88`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 5.4 MB (5378760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea503bea58815ffe61d67ad911ffab94ad5a57e364db2126c3cb11e8f732d37`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 3.2 MB (3244218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76eb02e31628a4e2997c0f38de59eb7d09325086dd65b6b511c1e63c7fdd1692`  
		Last Modified: Fri, 22 Apr 2022 02:25:48 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34da960e123e0d72767a541ecf7347f03dfad9502e82a54cd713eb6c1e2d294b`  
		Last Modified: Fri, 22 Apr 2022 02:25:49 GMT  
		Size: 2.2 MB (2183672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0ddf5cdd828e8ea2c4c69fedbb30d4aebf50bbc1c279fae4855faec077ae98`  
		Last Modified: Fri, 22 Apr 2022 02:25:47 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e906a7a4ca515f29ae2f9d042b9d50795a7722dff0e54711609032ab009449`  
		Last Modified: Fri, 22 Apr 2022 02:26:13 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8aa65ca376e03fed74f419a6a903362e83d6d4e1e1773ad67ad7183de7bbdf2`  
		Last Modified: Fri, 22 Apr 2022 02:26:26 GMT  
		Size: 89.8 MB (89815355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d48c43c28d400d613cd154b3e3182816a6e8b669d1fd7254e80bd5c51ae5f17`  
		Last Modified: Fri, 22 Apr 2022 02:26:13 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b5541b27b08286050b0bfd633e5710b2273e67032af256ca1137c955ccbd51`  
		Last Modified: Fri, 22 Apr 2022 02:26:13 GMT  
		Size: 6.8 KB (6775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
