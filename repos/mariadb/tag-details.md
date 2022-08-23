<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mariadb`

-	[`mariadb:10`](#mariadb10)
-	[`mariadb:10-jammy`](#mariadb10-jammy)
-	[`mariadb:10.10-rc`](#mariadb1010-rc)
-	[`mariadb:10.10-rc-jammy`](#mariadb1010-rc-jammy)
-	[`mariadb:10.10.1-rc`](#mariadb10101-rc)
-	[`mariadb:10.10.1-rc-jammy`](#mariadb10101-rc-jammy)
-	[`mariadb:10.3`](#mariadb103)
-	[`mariadb:10.3-focal`](#mariadb103-focal)
-	[`mariadb:10.3.36`](#mariadb10336)
-	[`mariadb:10.3.36-focal`](#mariadb10336-focal)
-	[`mariadb:10.4`](#mariadb104)
-	[`mariadb:10.4-focal`](#mariadb104-focal)
-	[`mariadb:10.4.26`](#mariadb10426)
-	[`mariadb:10.4.26-focal`](#mariadb10426-focal)
-	[`mariadb:10.5`](#mariadb105)
-	[`mariadb:10.5-focal`](#mariadb105-focal)
-	[`mariadb:10.5.17`](#mariadb10517)
-	[`mariadb:10.5.17-focal`](#mariadb10517-focal)
-	[`mariadb:10.6`](#mariadb106)
-	[`mariadb:10.6-focal`](#mariadb106-focal)
-	[`mariadb:10.6.9`](#mariadb1069)
-	[`mariadb:10.6.9-focal`](#mariadb1069-focal)
-	[`mariadb:10.7`](#mariadb107)
-	[`mariadb:10.7-focal`](#mariadb107-focal)
-	[`mariadb:10.7.5`](#mariadb1075)
-	[`mariadb:10.7.5-focal`](#mariadb1075-focal)
-	[`mariadb:10.8`](#mariadb108)
-	[`mariadb:10.8-jammy`](#mariadb108-jammy)
-	[`mariadb:10.8.4`](#mariadb1084)
-	[`mariadb:10.8.4-jammy`](#mariadb1084-jammy)
-	[`mariadb:10.9`](#mariadb109)
-	[`mariadb:10.9-jammy`](#mariadb109-jammy)
-	[`mariadb:10.9.2`](#mariadb1092)
-	[`mariadb:10.9.2-jammy`](#mariadb1092-jammy)
-	[`mariadb:jammy`](#mariadbjammy)
-	[`mariadb:latest`](#mariadblatest)

## `mariadb:10`

```console
$ docker pull mariadb@sha256:0abf60f81588662e716c27c7f1b54a72b3bf879e0ca88fc393e1741970ec7f3f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10` - linux; amd64

```console
$ docker pull mariadb@sha256:0a6ed934c1518abff64ed856b06f44006b4498b115941e19bbd910bd62a12232
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.9 MB (123908351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40b966d7252f541b41677fc35f8660fa90d14df0f33edc8085e6ca2dc0c5b247`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:55 GMT
ADD file:396eeb65c8d737180cc1219713cf59efb214027b79d8ea0b7e58a08e7c8d7a21 in / 
# Tue, 02 Aug 2022 01:30:56 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 20:19:21 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 02 Aug 2022 20:19:39 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 20:19:40 GMT
ENV GOSU_VERSION=1.14
# Tue, 02 Aug 2022 20:19:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 02 Aug 2022 20:19:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 02 Aug 2022 20:19:58 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 20:19:58 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 02 Aug 2022 20:19:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 02 Aug 2022 20:20:59 GMT
ARG MARIADB_MAJOR=10.8
# Tue, 02 Aug 2022 20:20:59 GMT
ENV MARIADB_MAJOR=10.8
# Tue, 02 Aug 2022 20:20:59 GMT
ARG MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 02 Aug 2022 20:20:59 GMT
ENV MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 02 Aug 2022 20:20:59 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
# Tue, 02 Aug 2022 20:21:00 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 02 Aug 2022 20:21:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 02 Aug 2022 20:21:19 GMT
VOLUME [/var/lib/mysql]
# Tue, 02 Aug 2022 20:21:19 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 02 Aug 2022 20:21:19 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 02 Aug 2022 20:21:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 20:21:20 GMT
EXPOSE 3306
# Tue, 02 Aug 2022 20:21:20 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d19f32bd9e4106d487f1a703fc2f09c8edadd92db4405d477978e8e466ab290d`  
		Last Modified: Tue, 02 Aug 2022 01:32:15 GMT  
		Size: 30.4 MB (30426136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f587559f9b58dcc08ed5b9fc08cc82b80ce995a37000098b1cdca2c199ae89f8`  
		Last Modified: Tue, 02 Aug 2022 20:26:32 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb060f92f2fef90ded1edd0a8c0609f95d414c40ff3684d1189beffa353f88b`  
		Last Modified: Tue, 02 Aug 2022 20:26:31 GMT  
		Size: 3.8 MB (3765797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27513e1f7a1e0c1c4f6197df108bf04d451bddf1da7bbdace8285098ba5dcf50`  
		Last Modified: Tue, 02 Aug 2022 20:26:31 GMT  
		Size: 2.0 MB (1992883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a84d3c510baac7a944c9669fc71e613930f5ca9c87cf616eeb06d2aa7c1917e`  
		Last Modified: Tue, 02 Aug 2022 20:26:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59731d2805a614a839795e79d61509494c939119e1dd7d76bf0f1b3a5f923c29`  
		Last Modified: Tue, 02 Aug 2022 20:26:31 GMT  
		Size: 2.3 MB (2298176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c008ca4420a867178be129dfe4311ce5ff0fcf8c2933d99ad49a3f0e3079cb3d`  
		Last Modified: Tue, 02 Aug 2022 20:26:28 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc47daf3f5d60b9b18f5ca3f556bc478eb967c997777a87459d43a9aea2fc6f`  
		Last Modified: Tue, 02 Aug 2022 20:26:58 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc547eec2be51eceb698e0766c93b76d55e7457043af4fe44ace5ca82927b1d4`  
		Last Modified: Tue, 02 Aug 2022 20:27:09 GMT  
		Size: 85.4 MB (85410459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bdaf629fe8214124455eb146db774a989c93271e8c3e264ece8ff4af772ea7b`  
		Last Modified: Tue, 02 Aug 2022 20:26:57 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddfbe3e290918fede8f6a3b0123b009178834c861a89c42c8b48075f8f8f420d`  
		Last Modified: Tue, 02 Aug 2022 20:26:58 GMT  
		Size: 6.7 KB (6696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:1f011a0b21919b39058355d972fea445857869ad1f867eb56bd1d274fd969e88
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.5 MB (102470825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3f8da7eeabb6549ac946f2b45ffe497556f6ad227d0bd4d41e09e73e6b34097`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:59 GMT
ADD file:3db67543ea64bf6723921d19cc5d0483db5c6658fc95834d8b2b5ed48a4cbacd in / 
# Tue, 02 Aug 2022 01:18:59 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 18:32:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 02 Aug 2022 18:32:16 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 18:32:17 GMT
ENV GOSU_VERSION=1.14
# Tue, 02 Aug 2022 18:32:33 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 02 Aug 2022 18:32:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 02 Aug 2022 18:32:42 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 18:32:42 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 02 Aug 2022 18:32:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 02 Aug 2022 18:33:28 GMT
ARG MARIADB_MAJOR=10.8
# Tue, 02 Aug 2022 18:33:29 GMT
ENV MARIADB_MAJOR=10.8
# Tue, 02 Aug 2022 18:33:30 GMT
ARG MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 02 Aug 2022 18:33:31 GMT
ENV MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 02 Aug 2022 18:33:32 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
# Tue, 02 Aug 2022 18:33:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 02 Aug 2022 18:33:52 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 02 Aug 2022 18:33:53 GMT
VOLUME [/var/lib/mysql]
# Tue, 02 Aug 2022 18:33:54 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 02 Aug 2022 18:33:55 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 02 Aug 2022 18:33:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 18:33:56 GMT
EXPOSE 3306
# Tue, 02 Aug 2022 18:33:57 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:4a3049d340b7d3651a954fd25a32c42feb1086889d6287e2f15468aef865c5c4`  
		Last Modified: Tue, 02 Aug 2022 01:20:49 GMT  
		Size: 28.4 MB (28381155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e5bedaed5f8e5343fee312eb2f21894d7b4026a0c692da89fe4f30a432e48b4`  
		Last Modified: Tue, 02 Aug 2022 18:41:32 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f07d81dfa02553c544d772dc3aa04ed6a2e6ad5b810ca742eee9a918786e5f`  
		Last Modified: Tue, 02 Aug 2022 18:41:30 GMT  
		Size: 3.6 MB (3594051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd6b8a20cb609d07274a17b8dd4ae810b6a98f76cf0ad513aa0c03eda46fcbce`  
		Last Modified: Tue, 02 Aug 2022 18:41:30 GMT  
		Size: 1.9 MB (1899200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3d39cfcf2768f9c1165cc0d3764c3649542f541a1ed3f18bec6283d58553e00`  
		Last Modified: Tue, 02 Aug 2022 18:41:30 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d230566e80222a9242f97419a6018684f4e324420ee89e4c0395f8107a124c91`  
		Last Modified: Tue, 02 Aug 2022 18:41:30 GMT  
		Size: 2.2 MB (2211614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c8c9abaef706c6185822ae21205ab5bc569494c4492a89eef44d8a855315c5`  
		Last Modified: Tue, 02 Aug 2022 18:41:27 GMT  
		Size: 2.5 KB (2465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9bff43ba5b5f6479659a8a7496d4156615c3cd9439c46779dd3feed3c4511ae`  
		Last Modified: Tue, 02 Aug 2022 18:41:57 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08cb73ef10f93c31f677c6818187b24c6bb65b4cb76ad5ed05e5b31853ef1b73`  
		Last Modified: Tue, 02 Aug 2022 18:42:08 GMT  
		Size: 66.4 MB (66369985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b16804fca7957e5cc3538c9a1a58af3e8e7a9eb0ee3318ffa413c7ebf4c76d4`  
		Last Modified: Tue, 02 Aug 2022 18:41:57 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fffad21dfd527f8685de9b3c864738e88bb8791db49ecdeb988d9d194a20d7cc`  
		Last Modified: Tue, 02 Aug 2022 18:41:57 GMT  
		Size: 6.7 KB (6699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10` - linux; ppc64le

```console
$ docker pull mariadb@sha256:017f8f45233c3bb9128302760d3c66df5253d31744a6e7401125b14233028d3a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.8 MB (116844233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf24d5b9794e7b70a566d82d3aa538d3b1657c23f08249227462a909b294c582`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 02 Aug 2022 01:31:12 GMT
ADD file:b6916c28c03568df4c2efc3da91ea6320f639cdbd2fa3f6741fcea7acad4fd5f in / 
# Tue, 02 Aug 2022 01:31:14 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 04:30:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 03 Aug 2022 04:30:30 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 04:30:31 GMT
ENV GOSU_VERSION=1.14
# Wed, 03 Aug 2022 04:30:49 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 03 Aug 2022 04:30:50 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 03 Aug 2022 04:31:03 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 04:31:03 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 03 Aug 2022 04:31:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 03 Aug 2022 04:32:26 GMT
ARG MARIADB_MAJOR=10.8
# Wed, 03 Aug 2022 04:32:26 GMT
ENV MARIADB_MAJOR=10.8
# Wed, 03 Aug 2022 04:32:26 GMT
ARG MARIADB_VERSION=1:10.8.3+maria~jammy
# Wed, 03 Aug 2022 04:32:27 GMT
ENV MARIADB_VERSION=1:10.8.3+maria~jammy
# Wed, 03 Aug 2022 04:32:27 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
# Wed, 03 Aug 2022 04:32:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 03 Aug 2022 04:33:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 03 Aug 2022 04:33:11 GMT
VOLUME [/var/lib/mysql]
# Wed, 03 Aug 2022 04:33:11 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Wed, 03 Aug 2022 04:33:12 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Wed, 03 Aug 2022 04:33:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 Aug 2022 04:33:12 GMT
EXPOSE 3306
# Wed, 03 Aug 2022 04:33:13 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:6f8c2fc0a4f976c1c0bd1c0e14022b3ed8b7c83cdb247c83016052c3678aaf28`  
		Last Modified: Tue, 02 Aug 2022 01:33:53 GMT  
		Size: 35.7 MB (35718004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da4a119144d25c65194f5210a2c0785d96c4b9d92c955f354d54e971b66cf0f`  
		Last Modified: Wed, 03 Aug 2022 04:43:49 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06895bfe56d4b1ebe076e361e483fe6fc6bfbaeb765ae25852c1993a6943452c`  
		Last Modified: Wed, 03 Aug 2022 04:43:47 GMT  
		Size: 4.5 MB (4503176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ee69296533cbe8c0bf533fa14d2f744068f58d5998026a4ba0c82bf9ea828ca`  
		Last Modified: Wed, 03 Aug 2022 04:43:47 GMT  
		Size: 1.9 MB (1921808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e76647cede58c06588416f8c141f66a1bf687145f5a0b0b2c530cdc63b14c805`  
		Last Modified: Wed, 03 Aug 2022 04:43:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b9befa094840721fea90813c85958f817ad561e93636ebd0730a9a395a0b46a`  
		Last Modified: Wed, 03 Aug 2022 04:43:47 GMT  
		Size: 2.4 MB (2404905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f92e1e86f56f2fadd73fdf7cc3428ca6687fbfa29af810bdb5c43b92ab77d02`  
		Last Modified: Wed, 03 Aug 2022 04:43:44 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b92a0e7592d7a0ad15eb1a53b8fcda1b2bb13d5dc516094d233fc4e8d23f53`  
		Last Modified: Wed, 03 Aug 2022 04:44:25 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c0e53f407a9d9f4fdfdb556976d3e976f93310c77b48124319cd55841b06ac`  
		Last Modified: Wed, 03 Aug 2022 04:44:43 GMT  
		Size: 72.3 MB (72281444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a525304ab204f12f8e1da79b296cd25e4eeda97bab0a3c0b8b21d27624c824c`  
		Last Modified: Wed, 03 Aug 2022 04:44:24 GMT  
		Size: 3.5 KB (3488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759170fa57f07b1b2ffc7f1dc434234f5446e9b18b7a5bb4bc1edbea87035db4`  
		Last Modified: Wed, 03 Aug 2022 04:44:24 GMT  
		Size: 6.7 KB (6694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10` - linux; s390x

```console
$ docker pull mariadb@sha256:12097ab474fe2ee789b394e1e8a6b489f2ca4ce5ebc8904a14cfddeedb17b8e5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (104979316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d95792c9ef5a984b01f32025b66c1495e316d034e94d5975da4069d260d40064`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 02 Aug 2022 01:02:17 GMT
ADD file:d5a5e56e0ca8287f27b257e3ddbc9675a1bdac1912afbbab6cddd891056cd144 in / 
# Tue, 02 Aug 2022 01:02:19 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 12:55:49 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 02 Aug 2022 12:56:06 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 12:56:07 GMT
ENV GOSU_VERSION=1.14
# Tue, 02 Aug 2022 12:56:16 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 02 Aug 2022 12:56:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 02 Aug 2022 12:56:22 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 12:56:22 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 02 Aug 2022 12:56:23 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 02 Aug 2022 12:57:08 GMT
ARG MARIADB_MAJOR=10.8
# Tue, 02 Aug 2022 12:57:08 GMT
ENV MARIADB_MAJOR=10.8
# Tue, 02 Aug 2022 12:57:08 GMT
ARG MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 02 Aug 2022 12:57:08 GMT
ENV MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 02 Aug 2022 12:57:09 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
# Tue, 02 Aug 2022 12:57:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 02 Aug 2022 12:57:31 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 02 Aug 2022 12:57:38 GMT
VOLUME [/var/lib/mysql]
# Tue, 02 Aug 2022 12:57:38 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 02 Aug 2022 12:57:38 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 02 Aug 2022 12:57:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 12:57:39 GMT
EXPOSE 3306
# Tue, 02 Aug 2022 12:57:39 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:f97967c51aac02138b615522a1bab9c75addd5896f43ade17ddaac44e0644283`  
		Last Modified: Tue, 02 Aug 2022 01:03:51 GMT  
		Size: 28.6 MB (28642785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:518030038f927b55f39a26dbee5d8d6e8c31cc0ddf7f23268b3dee3f001182c2`  
		Last Modified: Tue, 02 Aug 2022 13:01:03 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c5074a746c3e8a07e66d2d76ac4a7b9e0af6ffbf0cc8a87f601bb8b6913662`  
		Last Modified: Tue, 02 Aug 2022 13:01:02 GMT  
		Size: 3.7 MB (3675041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6140902b730422bc6cad80b27cf9005104adc5047e2e34955e4fbb5cf7d394`  
		Last Modified: Tue, 02 Aug 2022 13:01:02 GMT  
		Size: 2.0 MB (1955931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67105478e75b1563365dc4986a18198b1230a86bb142ade80fa52d1f71e2b6d7`  
		Last Modified: Tue, 02 Aug 2022 13:01:02 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af39a56c0cc78baeec34ac8d7b93879b9b0878bfcc89737ffecf164a865bd46b`  
		Last Modified: Tue, 02 Aug 2022 13:01:02 GMT  
		Size: 2.2 MB (2216654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c8957d63d730d9dbe5d508e565371ce9f1a318e16ad05c720373da4dbbe208`  
		Last Modified: Tue, 02 Aug 2022 13:01:00 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5461cdd4f49c09bdda524801b26ccc244a1f3b4daa635e39c8d982532b8646d7`  
		Last Modified: Tue, 02 Aug 2022 13:01:21 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c9a941eeee8bd3fcf6d0504466a69f3b30632b6d14fed1f53bc29439ded147`  
		Last Modified: Tue, 02 Aug 2022 13:01:30 GMT  
		Size: 68.5 MB (68473998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7458611c3efeaaf589463cdc0dff355cd54d57b45ece924dd1f1e136b26ef8dc`  
		Last Modified: Tue, 02 Aug 2022 13:01:21 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf3286637af3a581d1537b503e2b8404768d5a37566247553295844ea4b760d`  
		Last Modified: Tue, 02 Aug 2022 13:01:21 GMT  
		Size: 6.7 KB (6699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10-jammy`

```console
$ docker pull mariadb@sha256:0abf60f81588662e716c27c7f1b54a72b3bf879e0ca88fc393e1741970ec7f3f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10-jammy` - linux; amd64

```console
$ docker pull mariadb@sha256:0a6ed934c1518abff64ed856b06f44006b4498b115941e19bbd910bd62a12232
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.9 MB (123908351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40b966d7252f541b41677fc35f8660fa90d14df0f33edc8085e6ca2dc0c5b247`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:55 GMT
ADD file:396eeb65c8d737180cc1219713cf59efb214027b79d8ea0b7e58a08e7c8d7a21 in / 
# Tue, 02 Aug 2022 01:30:56 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 20:19:21 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 02 Aug 2022 20:19:39 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 20:19:40 GMT
ENV GOSU_VERSION=1.14
# Tue, 02 Aug 2022 20:19:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 02 Aug 2022 20:19:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 02 Aug 2022 20:19:58 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 20:19:58 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 02 Aug 2022 20:19:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 02 Aug 2022 20:20:59 GMT
ARG MARIADB_MAJOR=10.8
# Tue, 02 Aug 2022 20:20:59 GMT
ENV MARIADB_MAJOR=10.8
# Tue, 02 Aug 2022 20:20:59 GMT
ARG MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 02 Aug 2022 20:20:59 GMT
ENV MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 02 Aug 2022 20:20:59 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
# Tue, 02 Aug 2022 20:21:00 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 02 Aug 2022 20:21:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 02 Aug 2022 20:21:19 GMT
VOLUME [/var/lib/mysql]
# Tue, 02 Aug 2022 20:21:19 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 02 Aug 2022 20:21:19 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 02 Aug 2022 20:21:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 20:21:20 GMT
EXPOSE 3306
# Tue, 02 Aug 2022 20:21:20 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d19f32bd9e4106d487f1a703fc2f09c8edadd92db4405d477978e8e466ab290d`  
		Last Modified: Tue, 02 Aug 2022 01:32:15 GMT  
		Size: 30.4 MB (30426136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f587559f9b58dcc08ed5b9fc08cc82b80ce995a37000098b1cdca2c199ae89f8`  
		Last Modified: Tue, 02 Aug 2022 20:26:32 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb060f92f2fef90ded1edd0a8c0609f95d414c40ff3684d1189beffa353f88b`  
		Last Modified: Tue, 02 Aug 2022 20:26:31 GMT  
		Size: 3.8 MB (3765797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27513e1f7a1e0c1c4f6197df108bf04d451bddf1da7bbdace8285098ba5dcf50`  
		Last Modified: Tue, 02 Aug 2022 20:26:31 GMT  
		Size: 2.0 MB (1992883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a84d3c510baac7a944c9669fc71e613930f5ca9c87cf616eeb06d2aa7c1917e`  
		Last Modified: Tue, 02 Aug 2022 20:26:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59731d2805a614a839795e79d61509494c939119e1dd7d76bf0f1b3a5f923c29`  
		Last Modified: Tue, 02 Aug 2022 20:26:31 GMT  
		Size: 2.3 MB (2298176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c008ca4420a867178be129dfe4311ce5ff0fcf8c2933d99ad49a3f0e3079cb3d`  
		Last Modified: Tue, 02 Aug 2022 20:26:28 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc47daf3f5d60b9b18f5ca3f556bc478eb967c997777a87459d43a9aea2fc6f`  
		Last Modified: Tue, 02 Aug 2022 20:26:58 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc547eec2be51eceb698e0766c93b76d55e7457043af4fe44ace5ca82927b1d4`  
		Last Modified: Tue, 02 Aug 2022 20:27:09 GMT  
		Size: 85.4 MB (85410459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bdaf629fe8214124455eb146db774a989c93271e8c3e264ece8ff4af772ea7b`  
		Last Modified: Tue, 02 Aug 2022 20:26:57 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddfbe3e290918fede8f6a3b0123b009178834c861a89c42c8b48075f8f8f420d`  
		Last Modified: Tue, 02 Aug 2022 20:26:58 GMT  
		Size: 6.7 KB (6696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-jammy` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:1f011a0b21919b39058355d972fea445857869ad1f867eb56bd1d274fd969e88
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.5 MB (102470825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3f8da7eeabb6549ac946f2b45ffe497556f6ad227d0bd4d41e09e73e6b34097`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:59 GMT
ADD file:3db67543ea64bf6723921d19cc5d0483db5c6658fc95834d8b2b5ed48a4cbacd in / 
# Tue, 02 Aug 2022 01:18:59 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 18:32:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 02 Aug 2022 18:32:16 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 18:32:17 GMT
ENV GOSU_VERSION=1.14
# Tue, 02 Aug 2022 18:32:33 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 02 Aug 2022 18:32:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 02 Aug 2022 18:32:42 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 18:32:42 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 02 Aug 2022 18:32:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 02 Aug 2022 18:33:28 GMT
ARG MARIADB_MAJOR=10.8
# Tue, 02 Aug 2022 18:33:29 GMT
ENV MARIADB_MAJOR=10.8
# Tue, 02 Aug 2022 18:33:30 GMT
ARG MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 02 Aug 2022 18:33:31 GMT
ENV MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 02 Aug 2022 18:33:32 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
# Tue, 02 Aug 2022 18:33:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 02 Aug 2022 18:33:52 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 02 Aug 2022 18:33:53 GMT
VOLUME [/var/lib/mysql]
# Tue, 02 Aug 2022 18:33:54 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 02 Aug 2022 18:33:55 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 02 Aug 2022 18:33:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 18:33:56 GMT
EXPOSE 3306
# Tue, 02 Aug 2022 18:33:57 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:4a3049d340b7d3651a954fd25a32c42feb1086889d6287e2f15468aef865c5c4`  
		Last Modified: Tue, 02 Aug 2022 01:20:49 GMT  
		Size: 28.4 MB (28381155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e5bedaed5f8e5343fee312eb2f21894d7b4026a0c692da89fe4f30a432e48b4`  
		Last Modified: Tue, 02 Aug 2022 18:41:32 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f07d81dfa02553c544d772dc3aa04ed6a2e6ad5b810ca742eee9a918786e5f`  
		Last Modified: Tue, 02 Aug 2022 18:41:30 GMT  
		Size: 3.6 MB (3594051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd6b8a20cb609d07274a17b8dd4ae810b6a98f76cf0ad513aa0c03eda46fcbce`  
		Last Modified: Tue, 02 Aug 2022 18:41:30 GMT  
		Size: 1.9 MB (1899200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3d39cfcf2768f9c1165cc0d3764c3649542f541a1ed3f18bec6283d58553e00`  
		Last Modified: Tue, 02 Aug 2022 18:41:30 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d230566e80222a9242f97419a6018684f4e324420ee89e4c0395f8107a124c91`  
		Last Modified: Tue, 02 Aug 2022 18:41:30 GMT  
		Size: 2.2 MB (2211614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c8c9abaef706c6185822ae21205ab5bc569494c4492a89eef44d8a855315c5`  
		Last Modified: Tue, 02 Aug 2022 18:41:27 GMT  
		Size: 2.5 KB (2465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9bff43ba5b5f6479659a8a7496d4156615c3cd9439c46779dd3feed3c4511ae`  
		Last Modified: Tue, 02 Aug 2022 18:41:57 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08cb73ef10f93c31f677c6818187b24c6bb65b4cb76ad5ed05e5b31853ef1b73`  
		Last Modified: Tue, 02 Aug 2022 18:42:08 GMT  
		Size: 66.4 MB (66369985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b16804fca7957e5cc3538c9a1a58af3e8e7a9eb0ee3318ffa413c7ebf4c76d4`  
		Last Modified: Tue, 02 Aug 2022 18:41:57 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fffad21dfd527f8685de9b3c864738e88bb8791db49ecdeb988d9d194a20d7cc`  
		Last Modified: Tue, 02 Aug 2022 18:41:57 GMT  
		Size: 6.7 KB (6699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-jammy` - linux; ppc64le

```console
$ docker pull mariadb@sha256:017f8f45233c3bb9128302760d3c66df5253d31744a6e7401125b14233028d3a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.8 MB (116844233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf24d5b9794e7b70a566d82d3aa538d3b1657c23f08249227462a909b294c582`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 02 Aug 2022 01:31:12 GMT
ADD file:b6916c28c03568df4c2efc3da91ea6320f639cdbd2fa3f6741fcea7acad4fd5f in / 
# Tue, 02 Aug 2022 01:31:14 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 04:30:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 03 Aug 2022 04:30:30 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 04:30:31 GMT
ENV GOSU_VERSION=1.14
# Wed, 03 Aug 2022 04:30:49 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 03 Aug 2022 04:30:50 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 03 Aug 2022 04:31:03 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 04:31:03 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 03 Aug 2022 04:31:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 03 Aug 2022 04:32:26 GMT
ARG MARIADB_MAJOR=10.8
# Wed, 03 Aug 2022 04:32:26 GMT
ENV MARIADB_MAJOR=10.8
# Wed, 03 Aug 2022 04:32:26 GMT
ARG MARIADB_VERSION=1:10.8.3+maria~jammy
# Wed, 03 Aug 2022 04:32:27 GMT
ENV MARIADB_VERSION=1:10.8.3+maria~jammy
# Wed, 03 Aug 2022 04:32:27 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
# Wed, 03 Aug 2022 04:32:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 03 Aug 2022 04:33:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 03 Aug 2022 04:33:11 GMT
VOLUME [/var/lib/mysql]
# Wed, 03 Aug 2022 04:33:11 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Wed, 03 Aug 2022 04:33:12 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Wed, 03 Aug 2022 04:33:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 Aug 2022 04:33:12 GMT
EXPOSE 3306
# Wed, 03 Aug 2022 04:33:13 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:6f8c2fc0a4f976c1c0bd1c0e14022b3ed8b7c83cdb247c83016052c3678aaf28`  
		Last Modified: Tue, 02 Aug 2022 01:33:53 GMT  
		Size: 35.7 MB (35718004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da4a119144d25c65194f5210a2c0785d96c4b9d92c955f354d54e971b66cf0f`  
		Last Modified: Wed, 03 Aug 2022 04:43:49 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06895bfe56d4b1ebe076e361e483fe6fc6bfbaeb765ae25852c1993a6943452c`  
		Last Modified: Wed, 03 Aug 2022 04:43:47 GMT  
		Size: 4.5 MB (4503176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ee69296533cbe8c0bf533fa14d2f744068f58d5998026a4ba0c82bf9ea828ca`  
		Last Modified: Wed, 03 Aug 2022 04:43:47 GMT  
		Size: 1.9 MB (1921808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e76647cede58c06588416f8c141f66a1bf687145f5a0b0b2c530cdc63b14c805`  
		Last Modified: Wed, 03 Aug 2022 04:43:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b9befa094840721fea90813c85958f817ad561e93636ebd0730a9a395a0b46a`  
		Last Modified: Wed, 03 Aug 2022 04:43:47 GMT  
		Size: 2.4 MB (2404905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f92e1e86f56f2fadd73fdf7cc3428ca6687fbfa29af810bdb5c43b92ab77d02`  
		Last Modified: Wed, 03 Aug 2022 04:43:44 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b92a0e7592d7a0ad15eb1a53b8fcda1b2bb13d5dc516094d233fc4e8d23f53`  
		Last Modified: Wed, 03 Aug 2022 04:44:25 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c0e53f407a9d9f4fdfdb556976d3e976f93310c77b48124319cd55841b06ac`  
		Last Modified: Wed, 03 Aug 2022 04:44:43 GMT  
		Size: 72.3 MB (72281444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a525304ab204f12f8e1da79b296cd25e4eeda97bab0a3c0b8b21d27624c824c`  
		Last Modified: Wed, 03 Aug 2022 04:44:24 GMT  
		Size: 3.5 KB (3488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759170fa57f07b1b2ffc7f1dc434234f5446e9b18b7a5bb4bc1edbea87035db4`  
		Last Modified: Wed, 03 Aug 2022 04:44:24 GMT  
		Size: 6.7 KB (6694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-jammy` - linux; s390x

```console
$ docker pull mariadb@sha256:12097ab474fe2ee789b394e1e8a6b489f2ca4ce5ebc8904a14cfddeedb17b8e5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (104979316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d95792c9ef5a984b01f32025b66c1495e316d034e94d5975da4069d260d40064`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 02 Aug 2022 01:02:17 GMT
ADD file:d5a5e56e0ca8287f27b257e3ddbc9675a1bdac1912afbbab6cddd891056cd144 in / 
# Tue, 02 Aug 2022 01:02:19 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 12:55:49 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 02 Aug 2022 12:56:06 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 12:56:07 GMT
ENV GOSU_VERSION=1.14
# Tue, 02 Aug 2022 12:56:16 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 02 Aug 2022 12:56:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 02 Aug 2022 12:56:22 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 12:56:22 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 02 Aug 2022 12:56:23 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 02 Aug 2022 12:57:08 GMT
ARG MARIADB_MAJOR=10.8
# Tue, 02 Aug 2022 12:57:08 GMT
ENV MARIADB_MAJOR=10.8
# Tue, 02 Aug 2022 12:57:08 GMT
ARG MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 02 Aug 2022 12:57:08 GMT
ENV MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 02 Aug 2022 12:57:09 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
# Tue, 02 Aug 2022 12:57:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 02 Aug 2022 12:57:31 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 02 Aug 2022 12:57:38 GMT
VOLUME [/var/lib/mysql]
# Tue, 02 Aug 2022 12:57:38 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 02 Aug 2022 12:57:38 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 02 Aug 2022 12:57:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 12:57:39 GMT
EXPOSE 3306
# Tue, 02 Aug 2022 12:57:39 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:f97967c51aac02138b615522a1bab9c75addd5896f43ade17ddaac44e0644283`  
		Last Modified: Tue, 02 Aug 2022 01:03:51 GMT  
		Size: 28.6 MB (28642785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:518030038f927b55f39a26dbee5d8d6e8c31cc0ddf7f23268b3dee3f001182c2`  
		Last Modified: Tue, 02 Aug 2022 13:01:03 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c5074a746c3e8a07e66d2d76ac4a7b9e0af6ffbf0cc8a87f601bb8b6913662`  
		Last Modified: Tue, 02 Aug 2022 13:01:02 GMT  
		Size: 3.7 MB (3675041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6140902b730422bc6cad80b27cf9005104adc5047e2e34955e4fbb5cf7d394`  
		Last Modified: Tue, 02 Aug 2022 13:01:02 GMT  
		Size: 2.0 MB (1955931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67105478e75b1563365dc4986a18198b1230a86bb142ade80fa52d1f71e2b6d7`  
		Last Modified: Tue, 02 Aug 2022 13:01:02 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af39a56c0cc78baeec34ac8d7b93879b9b0878bfcc89737ffecf164a865bd46b`  
		Last Modified: Tue, 02 Aug 2022 13:01:02 GMT  
		Size: 2.2 MB (2216654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c8957d63d730d9dbe5d508e565371ce9f1a318e16ad05c720373da4dbbe208`  
		Last Modified: Tue, 02 Aug 2022 13:01:00 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5461cdd4f49c09bdda524801b26ccc244a1f3b4daa635e39c8d982532b8646d7`  
		Last Modified: Tue, 02 Aug 2022 13:01:21 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c9a941eeee8bd3fcf6d0504466a69f3b30632b6d14fed1f53bc29439ded147`  
		Last Modified: Tue, 02 Aug 2022 13:01:30 GMT  
		Size: 68.5 MB (68473998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7458611c3efeaaf589463cdc0dff355cd54d57b45ece924dd1f1e136b26ef8dc`  
		Last Modified: Tue, 02 Aug 2022 13:01:21 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf3286637af3a581d1537b503e2b8404768d5a37566247553295844ea4b760d`  
		Last Modified: Tue, 02 Aug 2022 13:01:21 GMT  
		Size: 6.7 KB (6699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.10-rc`

**does not exist** (yet?)

## `mariadb:10.10-rc-jammy`

**does not exist** (yet?)

## `mariadb:10.10.1-rc`

**does not exist** (yet?)

## `mariadb:10.10.1-rc-jammy`

**does not exist** (yet?)

## `mariadb:10.3`

```console
$ docker pull mariadb@sha256:3bfb0017ebd2136d385337cfdba6a2b32bf80a567b126797a602a763145b3a92
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3` - linux; amd64

```console
$ docker pull mariadb@sha256:adefacf8d1914afe10dbe2b6ffc2c568f4aa34d7d78ec55e99be48ca314f4358
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.2 MB (120198070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd091d34afbbadf43ff74f9182220d53c1a8f2fc15aa717336b0c64e902113bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:49 GMT
ADD file:af4cf77e6818016b697a1491101b40c71d06529ced65f36107749f099d6d4bdc in / 
# Tue, 02 Aug 2022 01:30:49 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 20:21:24 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 02 Aug 2022 20:21:32 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 20:21:32 GMT
ENV GOSU_VERSION=1.14
# Tue, 02 Aug 2022 20:21:42 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 02 Aug 2022 20:21:42 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 02 Aug 2022 20:21:49 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 20:21:49 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 02 Aug 2022 20:21:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 02 Aug 2022 20:23:57 GMT
ARG MARIADB_MAJOR=10.3
# Tue, 02 Aug 2022 20:23:57 GMT
ENV MARIADB_MAJOR=10.3
# Tue, 02 Aug 2022 20:23:57 GMT
ARG MARIADB_VERSION=1:10.3.35+maria~focal
# Tue, 02 Aug 2022 20:23:57 GMT
ENV MARIADB_VERSION=1:10.3.35+maria~focal
# Tue, 02 Aug 2022 20:23:57 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
# Tue, 02 Aug 2022 20:23:58 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 02 Aug 2022 20:24:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 02 Aug 2022 20:24:24 GMT
VOLUME [/var/lib/mysql]
# Tue, 02 Aug 2022 20:24:24 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Tue, 02 Aug 2022 20:24:25 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Tue, 02 Aug 2022 20:24:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 02 Aug 2022 20:24:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 20:24:25 GMT
EXPOSE 3306
# Tue, 02 Aug 2022 20:24:25 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3b65ec22a9e96affe680712973e88355927506aa3f792ff03330f3a3eb601a98`  
		Last Modified: Tue, 02 Aug 2022 01:31:59 GMT  
		Size: 28.6 MB (28572596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d19669910bc06b914ac5d4512b9aa15623df49e4ef03d20277f4a8fda0cf5631`  
		Last Modified: Tue, 02 Aug 2022 20:27:42 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c46f5717c584782c1a1498020ed1354006c97d58cb69a3607a17e1e0023da0e`  
		Last Modified: Tue, 02 Aug 2022 20:27:40 GMT  
		Size: 5.5 MB (5488983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea0278d54bb37ba2adf21e281d933e45b7c110f62e93e95b27c88940599003a1`  
		Last Modified: Tue, 02 Aug 2022 20:27:40 GMT  
		Size: 3.6 MB (3581823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80813ba5cb6ef218fb6cb3a25b964d31f0cd372ca1c2427c140d587a5a74a13`  
		Last Modified: Tue, 02 Aug 2022 20:27:39 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc4ac948168b66da6b55897167508489a2ab555945d5030db3362f06b232c51`  
		Last Modified: Tue, 02 Aug 2022 20:27:40 GMT  
		Size: 2.3 MB (2272442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d65facec905da8f0741a9561cf142ab88af72c392c88ab6d32c630704907f642`  
		Last Modified: Tue, 02 Aug 2022 20:27:37 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b34e52c4aa0391b348cdc25b8b4fc904c828c03c02f42e4e4992e2c6fd2aca`  
		Last Modified: Tue, 02 Aug 2022 20:29:38 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e25740d1c10a08792ab18933862e94cb87c4cd4297c539fa0dd6757d9de645`  
		Last Modified: Tue, 02 Aug 2022 20:29:50 GMT  
		Size: 80.3 MB (80267204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9987f81037aa04e4578292ac30b040606922f44354294aac3fe5679c5199cc96`  
		Last Modified: Tue, 02 Aug 2022 20:29:38 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58395125dec3691878ea124650c28bdae32e33d0653a63617e31e51ff9ae40be`  
		Last Modified: Tue, 02 Aug 2022 20:29:38 GMT  
		Size: 6.7 KB (6691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:220e50f6a55f29fd1f22eb7092b890f8688e90f175b2ff27f5e245ec0e3c1a4e`  
		Last Modified: Tue, 02 Aug 2022 20:29:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:18549782c1a9df3a37ab79f67e538a6863da0f70d9852e7b599845b7ad024d4a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117652395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25c5915a308fc62e110563674a326679102264146f728b6f4c10fc1ad56c78aa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:51 GMT
ADD file:151548d1bfac57d762f2c0b18b2378c363ffd1568da9fecd4be611db4832e8e2 in / 
# Tue, 02 Aug 2022 01:18:51 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 18:34:06 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 02 Aug 2022 18:34:17 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 18:34:18 GMT
ENV GOSU_VERSION=1.14
# Tue, 02 Aug 2022 18:34:33 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 02 Aug 2022 18:34:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 02 Aug 2022 18:34:42 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 18:34:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 02 Aug 2022 18:34:45 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 02 Aug 2022 18:37:31 GMT
ARG MARIADB_MAJOR=10.3
# Tue, 02 Aug 2022 18:37:32 GMT
ENV MARIADB_MAJOR=10.3
# Tue, 02 Aug 2022 18:37:33 GMT
ARG MARIADB_VERSION=1:10.3.35+maria~focal
# Tue, 02 Aug 2022 18:37:34 GMT
ENV MARIADB_VERSION=1:10.3.35+maria~focal
# Tue, 02 Aug 2022 18:37:35 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
# Tue, 02 Aug 2022 18:37:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 02 Aug 2022 18:38:07 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 02 Aug 2022 18:38:07 GMT
VOLUME [/var/lib/mysql]
# Tue, 02 Aug 2022 18:38:09 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Tue, 02 Aug 2022 18:38:10 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Tue, 02 Aug 2022 18:38:10 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 02 Aug 2022 18:38:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 18:38:12 GMT
EXPOSE 3306
# Tue, 02 Aug 2022 18:38:13 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a749a280e3e905de447c3d95a39e8aa1ede5835a6eadeb0c11596051592b675b`  
		Last Modified: Tue, 02 Aug 2022 01:20:32 GMT  
		Size: 27.2 MB (27191804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7d70702fc52aefacc8ccbff1968c3548d6400deb5e6c53d75f6dbc14905cb7`  
		Last Modified: Tue, 02 Aug 2022 18:42:44 GMT  
		Size: 1.7 KB (1722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9ffe290feb53a390aea694e16a663c4a420a71b1ebcd8053b07a44579782bbe`  
		Last Modified: Tue, 02 Aug 2022 18:42:44 GMT  
		Size: 5.3 MB (5321787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a430076265be6d7113b835ac1ab3e08dab46e41fff7e3ed070286125f1dbf6d`  
		Last Modified: Tue, 02 Aug 2022 18:42:43 GMT  
		Size: 3.4 MB (3367877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c880491c15580752404cccf2db4534a2d79f5b5cd1df18b3f6ea2754809020`  
		Last Modified: Tue, 02 Aug 2022 18:42:42 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ca8382cebf14e057456cd5ec8096f0053cdfe6029503875b74003df35d8c5e`  
		Last Modified: Tue, 02 Aug 2022 18:42:43 GMT  
		Size: 2.2 MB (2203204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88502488cc76b679835db628ad4d0f65e09a69018881918c6765cfb9e071feed`  
		Last Modified: Tue, 02 Aug 2022 18:42:40 GMT  
		Size: 2.5 KB (2466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4c6aca326cfd011967dc8cb41ffb93985998d801314ee6f71eae226c38b05f`  
		Last Modified: Tue, 02 Aug 2022 18:44:52 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d04251488d4f1aaccf2214e3ec64d06665fb736d5340f4eda42256e4763e0b6`  
		Last Modified: Tue, 02 Aug 2022 18:45:05 GMT  
		Size: 79.6 MB (79552791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b467d949890eaaa3738bc5f2fe0fa7b5a3f2cc0da3de58c4c67d172a5b4b18`  
		Last Modified: Tue, 02 Aug 2022 18:44:52 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9c894b5b7813a8c73743f44905b618b8a3676dcd6fe043766c67296088df78`  
		Last Modified: Tue, 02 Aug 2022 18:44:52 GMT  
		Size: 6.7 KB (6691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4b4305bbf6f97e7b626d11ee17c5a49af91e459e8efe2a43933e66b0d81ca0b`  
		Last Modified: Tue, 02 Aug 2022 18:44:52 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3` - linux; ppc64le

```console
$ docker pull mariadb@sha256:356580700f83c590b7573fb40ca823fc7caf68c00b0bb7a42364d58f35d1a577
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.1 MB (131089853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0993ff0dca76fb86695fa5e2daecb32eeb2783d0daca0f2114fff93ac6723183`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 02 Aug 2022 01:31:01 GMT
ADD file:75dd7889d4feb83b8504153b5ea6873e4ab0e616a4f4489ea81fd055b6ce9def in / 
# Tue, 02 Aug 2022 01:31:03 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 04:33:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 03 Aug 2022 04:34:01 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 04:34:01 GMT
ENV GOSU_VERSION=1.14
# Wed, 03 Aug 2022 04:34:21 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 03 Aug 2022 04:34:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 03 Aug 2022 04:34:35 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 04:34:36 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 03 Aug 2022 04:34:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 03 Aug 2022 04:38:52 GMT
ARG MARIADB_MAJOR=10.3
# Wed, 03 Aug 2022 04:38:52 GMT
ENV MARIADB_MAJOR=10.3
# Wed, 03 Aug 2022 04:38:53 GMT
ARG MARIADB_VERSION=1:10.3.35+maria~focal
# Wed, 03 Aug 2022 04:38:53 GMT
ENV MARIADB_VERSION=1:10.3.35+maria~focal
# Wed, 03 Aug 2022 04:38:54 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
# Wed, 03 Aug 2022 04:38:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 03 Aug 2022 04:39:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 03 Aug 2022 04:39:45 GMT
VOLUME [/var/lib/mysql]
# Wed, 03 Aug 2022 04:39:45 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Wed, 03 Aug 2022 04:39:46 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Wed, 03 Aug 2022 04:39:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 03 Aug 2022 04:39:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 Aug 2022 04:39:48 GMT
EXPOSE 3306
# Wed, 03 Aug 2022 04:39:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bf47d2be67f1a301865e78e8f78cc69c55dcc389921b4ba187dc0d333cbfd63b`  
		Last Modified: Tue, 02 Aug 2022 01:33:30 GMT  
		Size: 33.3 MB (33295352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b481bc43c771217829dcc78384d81402be7256c3fabe0fb95c0ad844e20eb486`  
		Last Modified: Wed, 03 Aug 2022 04:45:28 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f8f9934029ad30c4038aaa2505d3a55f09535b0f6cd3d115b622277ee43eec`  
		Last Modified: Wed, 03 Aug 2022 04:45:27 GMT  
		Size: 6.7 MB (6667750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ad8421e507f31703a57b5fcf441a19386060096de9f2d97716b6d1c03dd390`  
		Last Modified: Wed, 03 Aug 2022 04:45:27 GMT  
		Size: 3.7 MB (3669923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24953c586f1b7badf3268c6b00564095704918a0365c13b4d332008db8618e69`  
		Last Modified: Wed, 03 Aug 2022 04:45:25 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f4f22aaf2d7b83971e812c7422c924063814a37e635a032244e2b206911101b`  
		Last Modified: Wed, 03 Aug 2022 04:45:26 GMT  
		Size: 2.6 MB (2568638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57859f236e7f0146b0e787f561dafcb5fe2f724613fb2364c182a5ca2018030`  
		Last Modified: Wed, 03 Aug 2022 04:45:23 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f49b8240bf722469f85485d1c1342b9345cc26fda11b0bbde1dfb01252001c96`  
		Last Modified: Wed, 03 Aug 2022 04:48:29 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac1f38bfb906561435563ff3401a94bfea63d67fa6dba8bca155e688dddf52e9`  
		Last Modified: Wed, 03 Aug 2022 04:48:52 GMT  
		Size: 84.9 MB (84873162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a763f94bfde830ef49450ca5f3248bf11f1b555876cb6f1f69f362ee231ac6c9`  
		Last Modified: Wed, 03 Aug 2022 04:48:29 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e4f174f98983af302b564cb37b595c14ee815183e850bee8d4b3b7963bddac`  
		Last Modified: Wed, 03 Aug 2022 04:48:29 GMT  
		Size: 6.7 KB (6694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd0836943e8793a9dd84c800dd75611127dd26febb9b3b112454478d705e4db`  
		Last Modified: Wed, 03 Aug 2022 04:48:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3-focal`

```console
$ docker pull mariadb@sha256:3bfb0017ebd2136d385337cfdba6a2b32bf80a567b126797a602a763145b3a92
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:adefacf8d1914afe10dbe2b6ffc2c568f4aa34d7d78ec55e99be48ca314f4358
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.2 MB (120198070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd091d34afbbadf43ff74f9182220d53c1a8f2fc15aa717336b0c64e902113bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:49 GMT
ADD file:af4cf77e6818016b697a1491101b40c71d06529ced65f36107749f099d6d4bdc in / 
# Tue, 02 Aug 2022 01:30:49 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 20:21:24 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 02 Aug 2022 20:21:32 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 20:21:32 GMT
ENV GOSU_VERSION=1.14
# Tue, 02 Aug 2022 20:21:42 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 02 Aug 2022 20:21:42 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 02 Aug 2022 20:21:49 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 20:21:49 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 02 Aug 2022 20:21:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 02 Aug 2022 20:23:57 GMT
ARG MARIADB_MAJOR=10.3
# Tue, 02 Aug 2022 20:23:57 GMT
ENV MARIADB_MAJOR=10.3
# Tue, 02 Aug 2022 20:23:57 GMT
ARG MARIADB_VERSION=1:10.3.35+maria~focal
# Tue, 02 Aug 2022 20:23:57 GMT
ENV MARIADB_VERSION=1:10.3.35+maria~focal
# Tue, 02 Aug 2022 20:23:57 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
# Tue, 02 Aug 2022 20:23:58 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 02 Aug 2022 20:24:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 02 Aug 2022 20:24:24 GMT
VOLUME [/var/lib/mysql]
# Tue, 02 Aug 2022 20:24:24 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Tue, 02 Aug 2022 20:24:25 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Tue, 02 Aug 2022 20:24:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 02 Aug 2022 20:24:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 20:24:25 GMT
EXPOSE 3306
# Tue, 02 Aug 2022 20:24:25 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3b65ec22a9e96affe680712973e88355927506aa3f792ff03330f3a3eb601a98`  
		Last Modified: Tue, 02 Aug 2022 01:31:59 GMT  
		Size: 28.6 MB (28572596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d19669910bc06b914ac5d4512b9aa15623df49e4ef03d20277f4a8fda0cf5631`  
		Last Modified: Tue, 02 Aug 2022 20:27:42 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c46f5717c584782c1a1498020ed1354006c97d58cb69a3607a17e1e0023da0e`  
		Last Modified: Tue, 02 Aug 2022 20:27:40 GMT  
		Size: 5.5 MB (5488983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea0278d54bb37ba2adf21e281d933e45b7c110f62e93e95b27c88940599003a1`  
		Last Modified: Tue, 02 Aug 2022 20:27:40 GMT  
		Size: 3.6 MB (3581823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80813ba5cb6ef218fb6cb3a25b964d31f0cd372ca1c2427c140d587a5a74a13`  
		Last Modified: Tue, 02 Aug 2022 20:27:39 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc4ac948168b66da6b55897167508489a2ab555945d5030db3362f06b232c51`  
		Last Modified: Tue, 02 Aug 2022 20:27:40 GMT  
		Size: 2.3 MB (2272442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d65facec905da8f0741a9561cf142ab88af72c392c88ab6d32c630704907f642`  
		Last Modified: Tue, 02 Aug 2022 20:27:37 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b34e52c4aa0391b348cdc25b8b4fc904c828c03c02f42e4e4992e2c6fd2aca`  
		Last Modified: Tue, 02 Aug 2022 20:29:38 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e25740d1c10a08792ab18933862e94cb87c4cd4297c539fa0dd6757d9de645`  
		Last Modified: Tue, 02 Aug 2022 20:29:50 GMT  
		Size: 80.3 MB (80267204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9987f81037aa04e4578292ac30b040606922f44354294aac3fe5679c5199cc96`  
		Last Modified: Tue, 02 Aug 2022 20:29:38 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58395125dec3691878ea124650c28bdae32e33d0653a63617e31e51ff9ae40be`  
		Last Modified: Tue, 02 Aug 2022 20:29:38 GMT  
		Size: 6.7 KB (6691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:220e50f6a55f29fd1f22eb7092b890f8688e90f175b2ff27f5e245ec0e3c1a4e`  
		Last Modified: Tue, 02 Aug 2022 20:29:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:18549782c1a9df3a37ab79f67e538a6863da0f70d9852e7b599845b7ad024d4a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117652395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25c5915a308fc62e110563674a326679102264146f728b6f4c10fc1ad56c78aa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:51 GMT
ADD file:151548d1bfac57d762f2c0b18b2378c363ffd1568da9fecd4be611db4832e8e2 in / 
# Tue, 02 Aug 2022 01:18:51 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 18:34:06 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 02 Aug 2022 18:34:17 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 18:34:18 GMT
ENV GOSU_VERSION=1.14
# Tue, 02 Aug 2022 18:34:33 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 02 Aug 2022 18:34:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 02 Aug 2022 18:34:42 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 18:34:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 02 Aug 2022 18:34:45 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 02 Aug 2022 18:37:31 GMT
ARG MARIADB_MAJOR=10.3
# Tue, 02 Aug 2022 18:37:32 GMT
ENV MARIADB_MAJOR=10.3
# Tue, 02 Aug 2022 18:37:33 GMT
ARG MARIADB_VERSION=1:10.3.35+maria~focal
# Tue, 02 Aug 2022 18:37:34 GMT
ENV MARIADB_VERSION=1:10.3.35+maria~focal
# Tue, 02 Aug 2022 18:37:35 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
# Tue, 02 Aug 2022 18:37:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 02 Aug 2022 18:38:07 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 02 Aug 2022 18:38:07 GMT
VOLUME [/var/lib/mysql]
# Tue, 02 Aug 2022 18:38:09 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Tue, 02 Aug 2022 18:38:10 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Tue, 02 Aug 2022 18:38:10 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 02 Aug 2022 18:38:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 18:38:12 GMT
EXPOSE 3306
# Tue, 02 Aug 2022 18:38:13 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a749a280e3e905de447c3d95a39e8aa1ede5835a6eadeb0c11596051592b675b`  
		Last Modified: Tue, 02 Aug 2022 01:20:32 GMT  
		Size: 27.2 MB (27191804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7d70702fc52aefacc8ccbff1968c3548d6400deb5e6c53d75f6dbc14905cb7`  
		Last Modified: Tue, 02 Aug 2022 18:42:44 GMT  
		Size: 1.7 KB (1722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9ffe290feb53a390aea694e16a663c4a420a71b1ebcd8053b07a44579782bbe`  
		Last Modified: Tue, 02 Aug 2022 18:42:44 GMT  
		Size: 5.3 MB (5321787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a430076265be6d7113b835ac1ab3e08dab46e41fff7e3ed070286125f1dbf6d`  
		Last Modified: Tue, 02 Aug 2022 18:42:43 GMT  
		Size: 3.4 MB (3367877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c880491c15580752404cccf2db4534a2d79f5b5cd1df18b3f6ea2754809020`  
		Last Modified: Tue, 02 Aug 2022 18:42:42 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ca8382cebf14e057456cd5ec8096f0053cdfe6029503875b74003df35d8c5e`  
		Last Modified: Tue, 02 Aug 2022 18:42:43 GMT  
		Size: 2.2 MB (2203204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88502488cc76b679835db628ad4d0f65e09a69018881918c6765cfb9e071feed`  
		Last Modified: Tue, 02 Aug 2022 18:42:40 GMT  
		Size: 2.5 KB (2466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4c6aca326cfd011967dc8cb41ffb93985998d801314ee6f71eae226c38b05f`  
		Last Modified: Tue, 02 Aug 2022 18:44:52 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d04251488d4f1aaccf2214e3ec64d06665fb736d5340f4eda42256e4763e0b6`  
		Last Modified: Tue, 02 Aug 2022 18:45:05 GMT  
		Size: 79.6 MB (79552791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b467d949890eaaa3738bc5f2fe0fa7b5a3f2cc0da3de58c4c67d172a5b4b18`  
		Last Modified: Tue, 02 Aug 2022 18:44:52 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9c894b5b7813a8c73743f44905b618b8a3676dcd6fe043766c67296088df78`  
		Last Modified: Tue, 02 Aug 2022 18:44:52 GMT  
		Size: 6.7 KB (6691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4b4305bbf6f97e7b626d11ee17c5a49af91e459e8efe2a43933e66b0d81ca0b`  
		Last Modified: Tue, 02 Aug 2022 18:44:52 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:356580700f83c590b7573fb40ca823fc7caf68c00b0bb7a42364d58f35d1a577
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.1 MB (131089853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0993ff0dca76fb86695fa5e2daecb32eeb2783d0daca0f2114fff93ac6723183`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 02 Aug 2022 01:31:01 GMT
ADD file:75dd7889d4feb83b8504153b5ea6873e4ab0e616a4f4489ea81fd055b6ce9def in / 
# Tue, 02 Aug 2022 01:31:03 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 04:33:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 03 Aug 2022 04:34:01 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 04:34:01 GMT
ENV GOSU_VERSION=1.14
# Wed, 03 Aug 2022 04:34:21 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 03 Aug 2022 04:34:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 03 Aug 2022 04:34:35 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 04:34:36 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 03 Aug 2022 04:34:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 03 Aug 2022 04:38:52 GMT
ARG MARIADB_MAJOR=10.3
# Wed, 03 Aug 2022 04:38:52 GMT
ENV MARIADB_MAJOR=10.3
# Wed, 03 Aug 2022 04:38:53 GMT
ARG MARIADB_VERSION=1:10.3.35+maria~focal
# Wed, 03 Aug 2022 04:38:53 GMT
ENV MARIADB_VERSION=1:10.3.35+maria~focal
# Wed, 03 Aug 2022 04:38:54 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
# Wed, 03 Aug 2022 04:38:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 03 Aug 2022 04:39:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 03 Aug 2022 04:39:45 GMT
VOLUME [/var/lib/mysql]
# Wed, 03 Aug 2022 04:39:45 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Wed, 03 Aug 2022 04:39:46 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Wed, 03 Aug 2022 04:39:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 03 Aug 2022 04:39:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 Aug 2022 04:39:48 GMT
EXPOSE 3306
# Wed, 03 Aug 2022 04:39:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bf47d2be67f1a301865e78e8f78cc69c55dcc389921b4ba187dc0d333cbfd63b`  
		Last Modified: Tue, 02 Aug 2022 01:33:30 GMT  
		Size: 33.3 MB (33295352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b481bc43c771217829dcc78384d81402be7256c3fabe0fb95c0ad844e20eb486`  
		Last Modified: Wed, 03 Aug 2022 04:45:28 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f8f9934029ad30c4038aaa2505d3a55f09535b0f6cd3d115b622277ee43eec`  
		Last Modified: Wed, 03 Aug 2022 04:45:27 GMT  
		Size: 6.7 MB (6667750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ad8421e507f31703a57b5fcf441a19386060096de9f2d97716b6d1c03dd390`  
		Last Modified: Wed, 03 Aug 2022 04:45:27 GMT  
		Size: 3.7 MB (3669923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24953c586f1b7badf3268c6b00564095704918a0365c13b4d332008db8618e69`  
		Last Modified: Wed, 03 Aug 2022 04:45:25 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f4f22aaf2d7b83971e812c7422c924063814a37e635a032244e2b206911101b`  
		Last Modified: Wed, 03 Aug 2022 04:45:26 GMT  
		Size: 2.6 MB (2568638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57859f236e7f0146b0e787f561dafcb5fe2f724613fb2364c182a5ca2018030`  
		Last Modified: Wed, 03 Aug 2022 04:45:23 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f49b8240bf722469f85485d1c1342b9345cc26fda11b0bbde1dfb01252001c96`  
		Last Modified: Wed, 03 Aug 2022 04:48:29 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac1f38bfb906561435563ff3401a94bfea63d67fa6dba8bca155e688dddf52e9`  
		Last Modified: Wed, 03 Aug 2022 04:48:52 GMT  
		Size: 84.9 MB (84873162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a763f94bfde830ef49450ca5f3248bf11f1b555876cb6f1f69f362ee231ac6c9`  
		Last Modified: Wed, 03 Aug 2022 04:48:29 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e4f174f98983af302b564cb37b595c14ee815183e850bee8d4b3b7963bddac`  
		Last Modified: Wed, 03 Aug 2022 04:48:29 GMT  
		Size: 6.7 KB (6694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd0836943e8793a9dd84c800dd75611127dd26febb9b3b112454478d705e4db`  
		Last Modified: Wed, 03 Aug 2022 04:48:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3.36`

**does not exist** (yet?)

## `mariadb:10.3.36-focal`

**does not exist** (yet?)

## `mariadb:10.4`

```console
$ docker pull mariadb@sha256:fcfc5d2042bbfaae1200c96fb897f8b1c8d382a6e616055bc50a32bf5fa063cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4` - linux; amd64

```console
$ docker pull mariadb@sha256:d447716417416694a5bf0b1e732ab69239ed059563addaf3d6ab27ff02aeafd8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.8 MB (125823138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5322ff3cd8022a6113eebc1e8b17fd7162847610adf1018dec19693882abbdd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:49 GMT
ADD file:af4cf77e6818016b697a1491101b40c71d06529ced65f36107749f099d6d4bdc in / 
# Tue, 02 Aug 2022 01:30:49 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 20:21:24 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 02 Aug 2022 20:21:32 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 20:21:32 GMT
ENV GOSU_VERSION=1.14
# Tue, 02 Aug 2022 20:21:42 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 02 Aug 2022 20:21:42 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 02 Aug 2022 20:21:49 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 20:21:49 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 02 Aug 2022 20:21:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 02 Aug 2022 20:23:29 GMT
ARG MARIADB_MAJOR=10.4
# Tue, 02 Aug 2022 20:23:29 GMT
ENV MARIADB_MAJOR=10.4
# Tue, 02 Aug 2022 20:23:29 GMT
ARG MARIADB_VERSION=1:10.4.25+maria~focal
# Tue, 02 Aug 2022 20:23:29 GMT
ENV MARIADB_VERSION=1:10.4.25+maria~focal
# Tue, 02 Aug 2022 20:23:29 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
# Tue, 02 Aug 2022 20:23:30 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 02 Aug 2022 20:23:52 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 02 Aug 2022 20:23:53 GMT
VOLUME [/var/lib/mysql]
# Tue, 02 Aug 2022 20:23:53 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Tue, 02 Aug 2022 20:23:53 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Tue, 02 Aug 2022 20:23:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 02 Aug 2022 20:23:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 20:23:54 GMT
EXPOSE 3306
# Tue, 02 Aug 2022 20:23:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3b65ec22a9e96affe680712973e88355927506aa3f792ff03330f3a3eb601a98`  
		Last Modified: Tue, 02 Aug 2022 01:31:59 GMT  
		Size: 28.6 MB (28572596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d19669910bc06b914ac5d4512b9aa15623df49e4ef03d20277f4a8fda0cf5631`  
		Last Modified: Tue, 02 Aug 2022 20:27:42 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c46f5717c584782c1a1498020ed1354006c97d58cb69a3607a17e1e0023da0e`  
		Last Modified: Tue, 02 Aug 2022 20:27:40 GMT  
		Size: 5.5 MB (5488983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea0278d54bb37ba2adf21e281d933e45b7c110f62e93e95b27c88940599003a1`  
		Last Modified: Tue, 02 Aug 2022 20:27:40 GMT  
		Size: 3.6 MB (3581823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80813ba5cb6ef218fb6cb3a25b964d31f0cd372ca1c2427c140d587a5a74a13`  
		Last Modified: Tue, 02 Aug 2022 20:27:39 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc4ac948168b66da6b55897167508489a2ab555945d5030db3362f06b232c51`  
		Last Modified: Tue, 02 Aug 2022 20:27:40 GMT  
		Size: 2.3 MB (2272442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d65facec905da8f0741a9561cf142ab88af72c392c88ab6d32c630704907f642`  
		Last Modified: Tue, 02 Aug 2022 20:27:37 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751fcfc39d78647ab3325c196a4f447243fa20f7aac52b1deec8c75d9cfd4d7e`  
		Last Modified: Tue, 02 Aug 2022 20:29:08 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:367ee3fe9d819523d6c43776bf71b9882ed4be5d93e3321399dcd855aa48cf49`  
		Last Modified: Tue, 02 Aug 2022 20:29:22 GMT  
		Size: 85.9 MB (85892278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21f9e7c0c6ed2d639eebdfe9a657dc1a385d62a5e181cd4a38e48f1dae8765a8`  
		Last Modified: Tue, 02 Aug 2022 20:29:08 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c0300a16dfc5916acd814fdc454e6c151d7fc8b80455d63cccc3ac2d080aa6`  
		Last Modified: Tue, 02 Aug 2022 20:29:08 GMT  
		Size: 6.7 KB (6689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ccbf88baf43090ad5f31aaf3aa4676303c7122c10e80e7547e2eddee15e8a85`  
		Last Modified: Tue, 02 Aug 2022 20:29:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:97897537f890e470e3a7806246da3e8b691f6d09d27fcd11d1bd54c3bdba03b0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123180506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fe065923b0e402aa9415226696adc919ccf6b73dab5c241051009043354aa1c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:51 GMT
ADD file:151548d1bfac57d762f2c0b18b2378c363ffd1568da9fecd4be611db4832e8e2 in / 
# Tue, 02 Aug 2022 01:18:51 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 18:34:06 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 02 Aug 2022 18:34:17 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 18:34:18 GMT
ENV GOSU_VERSION=1.14
# Tue, 02 Aug 2022 18:34:33 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 02 Aug 2022 18:34:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 02 Aug 2022 18:34:42 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 18:34:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 02 Aug 2022 18:34:45 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 02 Aug 2022 18:36:47 GMT
ARG MARIADB_MAJOR=10.4
# Tue, 02 Aug 2022 18:36:48 GMT
ENV MARIADB_MAJOR=10.4
# Tue, 02 Aug 2022 18:36:49 GMT
ARG MARIADB_VERSION=1:10.4.25+maria~focal
# Tue, 02 Aug 2022 18:36:50 GMT
ENV MARIADB_VERSION=1:10.4.25+maria~focal
# Tue, 02 Aug 2022 18:36:51 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
# Tue, 02 Aug 2022 18:36:52 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 02 Aug 2022 18:37:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 02 Aug 2022 18:37:19 GMT
VOLUME [/var/lib/mysql]
# Tue, 02 Aug 2022 18:37:21 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Tue, 02 Aug 2022 18:37:22 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Tue, 02 Aug 2022 18:37:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 02 Aug 2022 18:37:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 18:37:24 GMT
EXPOSE 3306
# Tue, 02 Aug 2022 18:37:25 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a749a280e3e905de447c3d95a39e8aa1ede5835a6eadeb0c11596051592b675b`  
		Last Modified: Tue, 02 Aug 2022 01:20:32 GMT  
		Size: 27.2 MB (27191804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7d70702fc52aefacc8ccbff1968c3548d6400deb5e6c53d75f6dbc14905cb7`  
		Last Modified: Tue, 02 Aug 2022 18:42:44 GMT  
		Size: 1.7 KB (1722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9ffe290feb53a390aea694e16a663c4a420a71b1ebcd8053b07a44579782bbe`  
		Last Modified: Tue, 02 Aug 2022 18:42:44 GMT  
		Size: 5.3 MB (5321787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a430076265be6d7113b835ac1ab3e08dab46e41fff7e3ed070286125f1dbf6d`  
		Last Modified: Tue, 02 Aug 2022 18:42:43 GMT  
		Size: 3.4 MB (3367877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c880491c15580752404cccf2db4534a2d79f5b5cd1df18b3f6ea2754809020`  
		Last Modified: Tue, 02 Aug 2022 18:42:42 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ca8382cebf14e057456cd5ec8096f0053cdfe6029503875b74003df35d8c5e`  
		Last Modified: Tue, 02 Aug 2022 18:42:43 GMT  
		Size: 2.2 MB (2203204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88502488cc76b679835db628ad4d0f65e09a69018881918c6765cfb9e071feed`  
		Last Modified: Tue, 02 Aug 2022 18:42:40 GMT  
		Size: 2.5 KB (2466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f46350097da153c5f72fd94bcc96a40c6dffea0abdbcd8cd65797ed11dda312b`  
		Last Modified: Tue, 02 Aug 2022 18:44:20 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920d4559b118ac750a4b59f7b885180e7a59ecb12cc6cdbe60548297af15b90f`  
		Last Modified: Tue, 02 Aug 2022 18:44:33 GMT  
		Size: 85.1 MB (85080897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b324fa9127800969dc3e44a1af4b2bdd04bf1ea54c4040cae76ac608fff2ec6`  
		Last Modified: Tue, 02 Aug 2022 18:44:20 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e3c5507189d9fdc9e229de8b6283cad1935c0dd407d89d09bd6d7a58803cc39`  
		Last Modified: Tue, 02 Aug 2022 18:44:20 GMT  
		Size: 6.7 KB (6693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce51aa6efeb81f3e9cb4a09f171f97ca8f97f25c54f096905dc29ed804b4b555`  
		Last Modified: Tue, 02 Aug 2022 18:44:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4` - linux; ppc64le

```console
$ docker pull mariadb@sha256:d8eee7a3e4a346e80d17d78d978ded32c52d3b84a67ee5302b2dfc6bdea653bc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.7 MB (136722864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:650eccedf083bd7a9d4f659d7d8170d50e74a1e550fa3bd1f0ef1de0ee114fa6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 02 Aug 2022 01:31:01 GMT
ADD file:75dd7889d4feb83b8504153b5ea6873e4ab0e616a4f4489ea81fd055b6ce9def in / 
# Tue, 02 Aug 2022 01:31:03 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 04:33:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 03 Aug 2022 04:34:01 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 04:34:01 GMT
ENV GOSU_VERSION=1.14
# Wed, 03 Aug 2022 04:34:21 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 03 Aug 2022 04:34:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 03 Aug 2022 04:34:35 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 04:34:36 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 03 Aug 2022 04:34:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 03 Aug 2022 04:37:52 GMT
ARG MARIADB_MAJOR=10.4
# Wed, 03 Aug 2022 04:37:52 GMT
ENV MARIADB_MAJOR=10.4
# Wed, 03 Aug 2022 04:37:52 GMT
ARG MARIADB_VERSION=1:10.4.25+maria~focal
# Wed, 03 Aug 2022 04:37:53 GMT
ENV MARIADB_VERSION=1:10.4.25+maria~focal
# Wed, 03 Aug 2022 04:37:54 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
# Wed, 03 Aug 2022 04:37:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 03 Aug 2022 04:38:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 03 Aug 2022 04:38:43 GMT
VOLUME [/var/lib/mysql]
# Wed, 03 Aug 2022 04:38:44 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Wed, 03 Aug 2022 04:38:44 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Wed, 03 Aug 2022 04:38:45 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 03 Aug 2022 04:38:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 Aug 2022 04:38:45 GMT
EXPOSE 3306
# Wed, 03 Aug 2022 04:38:46 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bf47d2be67f1a301865e78e8f78cc69c55dcc389921b4ba187dc0d333cbfd63b`  
		Last Modified: Tue, 02 Aug 2022 01:33:30 GMT  
		Size: 33.3 MB (33295352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b481bc43c771217829dcc78384d81402be7256c3fabe0fb95c0ad844e20eb486`  
		Last Modified: Wed, 03 Aug 2022 04:45:28 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f8f9934029ad30c4038aaa2505d3a55f09535b0f6cd3d115b622277ee43eec`  
		Last Modified: Wed, 03 Aug 2022 04:45:27 GMT  
		Size: 6.7 MB (6667750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ad8421e507f31703a57b5fcf441a19386060096de9f2d97716b6d1c03dd390`  
		Last Modified: Wed, 03 Aug 2022 04:45:27 GMT  
		Size: 3.7 MB (3669923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24953c586f1b7badf3268c6b00564095704918a0365c13b4d332008db8618e69`  
		Last Modified: Wed, 03 Aug 2022 04:45:25 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f4f22aaf2d7b83971e812c7422c924063814a37e635a032244e2b206911101b`  
		Last Modified: Wed, 03 Aug 2022 04:45:26 GMT  
		Size: 2.6 MB (2568638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57859f236e7f0146b0e787f561dafcb5fe2f724613fb2364c182a5ca2018030`  
		Last Modified: Wed, 03 Aug 2022 04:45:23 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:239513439bb2f78c5a9489427540e6afbd071c4c6b350fc7ee167a2c38acb676`  
		Last Modified: Wed, 03 Aug 2022 04:47:43 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3bbd0b57ff8e4280982030a2ddb3cd287f7694a59f0a4fccbb4a4ecb651d51`  
		Last Modified: Wed, 03 Aug 2022 04:48:07 GMT  
		Size: 90.5 MB (90506174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:204e90eec981fdd89d2a881a311b3616d65c31dffef1d225d868e4d238eef384`  
		Last Modified: Wed, 03 Aug 2022 04:47:43 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d08a3c4fce7dd3eb927941d3f12380344c20e881994137c31c1ce8d58f17dc45`  
		Last Modified: Wed, 03 Aug 2022 04:47:43 GMT  
		Size: 6.7 KB (6694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95ff23c4c0b00ffa75e13114897cde91bcdb580d3af9fa8846aa13569196cc1`  
		Last Modified: Wed, 03 Aug 2022 04:47:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4-focal`

```console
$ docker pull mariadb@sha256:fcfc5d2042bbfaae1200c96fb897f8b1c8d382a6e616055bc50a32bf5fa063cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:d447716417416694a5bf0b1e732ab69239ed059563addaf3d6ab27ff02aeafd8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.8 MB (125823138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5322ff3cd8022a6113eebc1e8b17fd7162847610adf1018dec19693882abbdd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:49 GMT
ADD file:af4cf77e6818016b697a1491101b40c71d06529ced65f36107749f099d6d4bdc in / 
# Tue, 02 Aug 2022 01:30:49 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 20:21:24 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 02 Aug 2022 20:21:32 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 20:21:32 GMT
ENV GOSU_VERSION=1.14
# Tue, 02 Aug 2022 20:21:42 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 02 Aug 2022 20:21:42 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 02 Aug 2022 20:21:49 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 20:21:49 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 02 Aug 2022 20:21:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 02 Aug 2022 20:23:29 GMT
ARG MARIADB_MAJOR=10.4
# Tue, 02 Aug 2022 20:23:29 GMT
ENV MARIADB_MAJOR=10.4
# Tue, 02 Aug 2022 20:23:29 GMT
ARG MARIADB_VERSION=1:10.4.25+maria~focal
# Tue, 02 Aug 2022 20:23:29 GMT
ENV MARIADB_VERSION=1:10.4.25+maria~focal
# Tue, 02 Aug 2022 20:23:29 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
# Tue, 02 Aug 2022 20:23:30 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 02 Aug 2022 20:23:52 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 02 Aug 2022 20:23:53 GMT
VOLUME [/var/lib/mysql]
# Tue, 02 Aug 2022 20:23:53 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Tue, 02 Aug 2022 20:23:53 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Tue, 02 Aug 2022 20:23:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 02 Aug 2022 20:23:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 20:23:54 GMT
EXPOSE 3306
# Tue, 02 Aug 2022 20:23:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3b65ec22a9e96affe680712973e88355927506aa3f792ff03330f3a3eb601a98`  
		Last Modified: Tue, 02 Aug 2022 01:31:59 GMT  
		Size: 28.6 MB (28572596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d19669910bc06b914ac5d4512b9aa15623df49e4ef03d20277f4a8fda0cf5631`  
		Last Modified: Tue, 02 Aug 2022 20:27:42 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c46f5717c584782c1a1498020ed1354006c97d58cb69a3607a17e1e0023da0e`  
		Last Modified: Tue, 02 Aug 2022 20:27:40 GMT  
		Size: 5.5 MB (5488983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea0278d54bb37ba2adf21e281d933e45b7c110f62e93e95b27c88940599003a1`  
		Last Modified: Tue, 02 Aug 2022 20:27:40 GMT  
		Size: 3.6 MB (3581823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80813ba5cb6ef218fb6cb3a25b964d31f0cd372ca1c2427c140d587a5a74a13`  
		Last Modified: Tue, 02 Aug 2022 20:27:39 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc4ac948168b66da6b55897167508489a2ab555945d5030db3362f06b232c51`  
		Last Modified: Tue, 02 Aug 2022 20:27:40 GMT  
		Size: 2.3 MB (2272442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d65facec905da8f0741a9561cf142ab88af72c392c88ab6d32c630704907f642`  
		Last Modified: Tue, 02 Aug 2022 20:27:37 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751fcfc39d78647ab3325c196a4f447243fa20f7aac52b1deec8c75d9cfd4d7e`  
		Last Modified: Tue, 02 Aug 2022 20:29:08 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:367ee3fe9d819523d6c43776bf71b9882ed4be5d93e3321399dcd855aa48cf49`  
		Last Modified: Tue, 02 Aug 2022 20:29:22 GMT  
		Size: 85.9 MB (85892278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21f9e7c0c6ed2d639eebdfe9a657dc1a385d62a5e181cd4a38e48f1dae8765a8`  
		Last Modified: Tue, 02 Aug 2022 20:29:08 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c0300a16dfc5916acd814fdc454e6c151d7fc8b80455d63cccc3ac2d080aa6`  
		Last Modified: Tue, 02 Aug 2022 20:29:08 GMT  
		Size: 6.7 KB (6689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ccbf88baf43090ad5f31aaf3aa4676303c7122c10e80e7547e2eddee15e8a85`  
		Last Modified: Tue, 02 Aug 2022 20:29:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:97897537f890e470e3a7806246da3e8b691f6d09d27fcd11d1bd54c3bdba03b0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123180506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fe065923b0e402aa9415226696adc919ccf6b73dab5c241051009043354aa1c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:51 GMT
ADD file:151548d1bfac57d762f2c0b18b2378c363ffd1568da9fecd4be611db4832e8e2 in / 
# Tue, 02 Aug 2022 01:18:51 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 18:34:06 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 02 Aug 2022 18:34:17 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 18:34:18 GMT
ENV GOSU_VERSION=1.14
# Tue, 02 Aug 2022 18:34:33 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 02 Aug 2022 18:34:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 02 Aug 2022 18:34:42 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 18:34:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 02 Aug 2022 18:34:45 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 02 Aug 2022 18:36:47 GMT
ARG MARIADB_MAJOR=10.4
# Tue, 02 Aug 2022 18:36:48 GMT
ENV MARIADB_MAJOR=10.4
# Tue, 02 Aug 2022 18:36:49 GMT
ARG MARIADB_VERSION=1:10.4.25+maria~focal
# Tue, 02 Aug 2022 18:36:50 GMT
ENV MARIADB_VERSION=1:10.4.25+maria~focal
# Tue, 02 Aug 2022 18:36:51 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
# Tue, 02 Aug 2022 18:36:52 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 02 Aug 2022 18:37:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 02 Aug 2022 18:37:19 GMT
VOLUME [/var/lib/mysql]
# Tue, 02 Aug 2022 18:37:21 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Tue, 02 Aug 2022 18:37:22 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Tue, 02 Aug 2022 18:37:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 02 Aug 2022 18:37:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 18:37:24 GMT
EXPOSE 3306
# Tue, 02 Aug 2022 18:37:25 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a749a280e3e905de447c3d95a39e8aa1ede5835a6eadeb0c11596051592b675b`  
		Last Modified: Tue, 02 Aug 2022 01:20:32 GMT  
		Size: 27.2 MB (27191804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7d70702fc52aefacc8ccbff1968c3548d6400deb5e6c53d75f6dbc14905cb7`  
		Last Modified: Tue, 02 Aug 2022 18:42:44 GMT  
		Size: 1.7 KB (1722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9ffe290feb53a390aea694e16a663c4a420a71b1ebcd8053b07a44579782bbe`  
		Last Modified: Tue, 02 Aug 2022 18:42:44 GMT  
		Size: 5.3 MB (5321787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a430076265be6d7113b835ac1ab3e08dab46e41fff7e3ed070286125f1dbf6d`  
		Last Modified: Tue, 02 Aug 2022 18:42:43 GMT  
		Size: 3.4 MB (3367877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c880491c15580752404cccf2db4534a2d79f5b5cd1df18b3f6ea2754809020`  
		Last Modified: Tue, 02 Aug 2022 18:42:42 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ca8382cebf14e057456cd5ec8096f0053cdfe6029503875b74003df35d8c5e`  
		Last Modified: Tue, 02 Aug 2022 18:42:43 GMT  
		Size: 2.2 MB (2203204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88502488cc76b679835db628ad4d0f65e09a69018881918c6765cfb9e071feed`  
		Last Modified: Tue, 02 Aug 2022 18:42:40 GMT  
		Size: 2.5 KB (2466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f46350097da153c5f72fd94bcc96a40c6dffea0abdbcd8cd65797ed11dda312b`  
		Last Modified: Tue, 02 Aug 2022 18:44:20 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920d4559b118ac750a4b59f7b885180e7a59ecb12cc6cdbe60548297af15b90f`  
		Last Modified: Tue, 02 Aug 2022 18:44:33 GMT  
		Size: 85.1 MB (85080897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b324fa9127800969dc3e44a1af4b2bdd04bf1ea54c4040cae76ac608fff2ec6`  
		Last Modified: Tue, 02 Aug 2022 18:44:20 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e3c5507189d9fdc9e229de8b6283cad1935c0dd407d89d09bd6d7a58803cc39`  
		Last Modified: Tue, 02 Aug 2022 18:44:20 GMT  
		Size: 6.7 KB (6693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce51aa6efeb81f3e9cb4a09f171f97ca8f97f25c54f096905dc29ed804b4b555`  
		Last Modified: Tue, 02 Aug 2022 18:44:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:d8eee7a3e4a346e80d17d78d978ded32c52d3b84a67ee5302b2dfc6bdea653bc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.7 MB (136722864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:650eccedf083bd7a9d4f659d7d8170d50e74a1e550fa3bd1f0ef1de0ee114fa6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 02 Aug 2022 01:31:01 GMT
ADD file:75dd7889d4feb83b8504153b5ea6873e4ab0e616a4f4489ea81fd055b6ce9def in / 
# Tue, 02 Aug 2022 01:31:03 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 04:33:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 03 Aug 2022 04:34:01 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 04:34:01 GMT
ENV GOSU_VERSION=1.14
# Wed, 03 Aug 2022 04:34:21 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 03 Aug 2022 04:34:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 03 Aug 2022 04:34:35 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 04:34:36 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 03 Aug 2022 04:34:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 03 Aug 2022 04:37:52 GMT
ARG MARIADB_MAJOR=10.4
# Wed, 03 Aug 2022 04:37:52 GMT
ENV MARIADB_MAJOR=10.4
# Wed, 03 Aug 2022 04:37:52 GMT
ARG MARIADB_VERSION=1:10.4.25+maria~focal
# Wed, 03 Aug 2022 04:37:53 GMT
ENV MARIADB_VERSION=1:10.4.25+maria~focal
# Wed, 03 Aug 2022 04:37:54 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
# Wed, 03 Aug 2022 04:37:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 03 Aug 2022 04:38:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 03 Aug 2022 04:38:43 GMT
VOLUME [/var/lib/mysql]
# Wed, 03 Aug 2022 04:38:44 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Wed, 03 Aug 2022 04:38:44 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Wed, 03 Aug 2022 04:38:45 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 03 Aug 2022 04:38:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 Aug 2022 04:38:45 GMT
EXPOSE 3306
# Wed, 03 Aug 2022 04:38:46 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bf47d2be67f1a301865e78e8f78cc69c55dcc389921b4ba187dc0d333cbfd63b`  
		Last Modified: Tue, 02 Aug 2022 01:33:30 GMT  
		Size: 33.3 MB (33295352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b481bc43c771217829dcc78384d81402be7256c3fabe0fb95c0ad844e20eb486`  
		Last Modified: Wed, 03 Aug 2022 04:45:28 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f8f9934029ad30c4038aaa2505d3a55f09535b0f6cd3d115b622277ee43eec`  
		Last Modified: Wed, 03 Aug 2022 04:45:27 GMT  
		Size: 6.7 MB (6667750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ad8421e507f31703a57b5fcf441a19386060096de9f2d97716b6d1c03dd390`  
		Last Modified: Wed, 03 Aug 2022 04:45:27 GMT  
		Size: 3.7 MB (3669923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24953c586f1b7badf3268c6b00564095704918a0365c13b4d332008db8618e69`  
		Last Modified: Wed, 03 Aug 2022 04:45:25 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f4f22aaf2d7b83971e812c7422c924063814a37e635a032244e2b206911101b`  
		Last Modified: Wed, 03 Aug 2022 04:45:26 GMT  
		Size: 2.6 MB (2568638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57859f236e7f0146b0e787f561dafcb5fe2f724613fb2364c182a5ca2018030`  
		Last Modified: Wed, 03 Aug 2022 04:45:23 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:239513439bb2f78c5a9489427540e6afbd071c4c6b350fc7ee167a2c38acb676`  
		Last Modified: Wed, 03 Aug 2022 04:47:43 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3bbd0b57ff8e4280982030a2ddb3cd287f7694a59f0a4fccbb4a4ecb651d51`  
		Last Modified: Wed, 03 Aug 2022 04:48:07 GMT  
		Size: 90.5 MB (90506174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:204e90eec981fdd89d2a881a311b3616d65c31dffef1d225d868e4d238eef384`  
		Last Modified: Wed, 03 Aug 2022 04:47:43 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d08a3c4fce7dd3eb927941d3f12380344c20e881994137c31c1ce8d58f17dc45`  
		Last Modified: Wed, 03 Aug 2022 04:47:43 GMT  
		Size: 6.7 KB (6694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95ff23c4c0b00ffa75e13114897cde91bcdb580d3af9fa8846aa13569196cc1`  
		Last Modified: Wed, 03 Aug 2022 04:47:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4.26`

**does not exist** (yet?)

## `mariadb:10.4.26-focal`

**does not exist** (yet?)

## `mariadb:10.5`

```console
$ docker pull mariadb@sha256:473c1bd96f54846c857869f1774f180fc97075d096e82ce87ff0d00f64803bc5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.5` - linux; amd64

```console
$ docker pull mariadb@sha256:910c1742bad5346be709801726ffb14330f83b32afa82530b34719bf80a9c243
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.1 MB (128066304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83ea47900c5495b8a3627804273fbb724c1592d11cf11ce08d8d688bb3cd6f6c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:49 GMT
ADD file:af4cf77e6818016b697a1491101b40c71d06529ced65f36107749f099d6d4bdc in / 
# Tue, 02 Aug 2022 01:30:49 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 20:21:24 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 02 Aug 2022 20:21:32 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 20:21:32 GMT
ENV GOSU_VERSION=1.14
# Tue, 02 Aug 2022 20:21:42 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 02 Aug 2022 20:21:42 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 02 Aug 2022 20:21:49 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 20:21:49 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 02 Aug 2022 20:21:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 02 Aug 2022 20:23:01 GMT
ARG MARIADB_MAJOR=10.5
# Tue, 02 Aug 2022 20:23:01 GMT
ENV MARIADB_MAJOR=10.5
# Tue, 02 Aug 2022 20:23:01 GMT
ARG MARIADB_VERSION=1:10.5.16+maria~focal
# Tue, 02 Aug 2022 20:23:01 GMT
ENV MARIADB_VERSION=1:10.5.16+maria~focal
# Tue, 02 Aug 2022 20:23:01 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
# Tue, 02 Aug 2022 20:23:01 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 02 Aug 2022 20:23:23 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 02 Aug 2022 20:23:24 GMT
VOLUME [/var/lib/mysql]
# Tue, 02 Aug 2022 20:23:24 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Tue, 02 Aug 2022 20:23:24 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Tue, 02 Aug 2022 20:23:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 20:23:24 GMT
EXPOSE 3306
# Tue, 02 Aug 2022 20:23:24 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3b65ec22a9e96affe680712973e88355927506aa3f792ff03330f3a3eb601a98`  
		Last Modified: Tue, 02 Aug 2022 01:31:59 GMT  
		Size: 28.6 MB (28572596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d19669910bc06b914ac5d4512b9aa15623df49e4ef03d20277f4a8fda0cf5631`  
		Last Modified: Tue, 02 Aug 2022 20:27:42 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c46f5717c584782c1a1498020ed1354006c97d58cb69a3607a17e1e0023da0e`  
		Last Modified: Tue, 02 Aug 2022 20:27:40 GMT  
		Size: 5.5 MB (5488983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea0278d54bb37ba2adf21e281d933e45b7c110f62e93e95b27c88940599003a1`  
		Last Modified: Tue, 02 Aug 2022 20:27:40 GMT  
		Size: 3.6 MB (3581823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80813ba5cb6ef218fb6cb3a25b964d31f0cd372ca1c2427c140d587a5a74a13`  
		Last Modified: Tue, 02 Aug 2022 20:27:39 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc4ac948168b66da6b55897167508489a2ab555945d5030db3362f06b232c51`  
		Last Modified: Tue, 02 Aug 2022 20:27:40 GMT  
		Size: 2.3 MB (2272442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d65facec905da8f0741a9561cf142ab88af72c392c88ab6d32c630704907f642`  
		Last Modified: Tue, 02 Aug 2022 20:27:37 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68b10715d9bb4160d2ac31d5a7cfe51703b1c7addd4256d6e23910a2bca430a9`  
		Last Modified: Tue, 02 Aug 2022 20:28:39 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba6b1b231f2e46c2bb48f813248b8c338d247d21597d08bf54eeb4b2dc3456f`  
		Last Modified: Tue, 02 Aug 2022 20:28:52 GMT  
		Size: 88.1 MB (88135566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:058ed59cd119a24508bfe59d19260c5fb617115556679686ba8c4b5bcfcb9ac3`  
		Last Modified: Tue, 02 Aug 2022 20:28:39 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9e4955b52c41269e59331263ab1315cdc538209bdb6273eacd842c8fab721b`  
		Last Modified: Tue, 02 Aug 2022 20:28:39 GMT  
		Size: 6.7 KB (6689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:598ef479e99feea2749a234780c80def9b7ae5bc9b5f5a62400052f480b70ce3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.3 MB (125345920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22ff76a6fdcb615fc7a9e59ea1fb855f5844aafc946634f62d70a60f43ef6875`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:51 GMT
ADD file:151548d1bfac57d762f2c0b18b2378c363ffd1568da9fecd4be611db4832e8e2 in / 
# Tue, 02 Aug 2022 01:18:51 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 18:34:06 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 02 Aug 2022 18:34:17 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 18:34:18 GMT
ENV GOSU_VERSION=1.14
# Tue, 02 Aug 2022 18:34:33 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 02 Aug 2022 18:34:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 02 Aug 2022 18:34:42 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 18:34:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 02 Aug 2022 18:34:45 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 02 Aug 2022 18:36:10 GMT
ARG MARIADB_MAJOR=10.5
# Tue, 02 Aug 2022 18:36:10 GMT
ENV MARIADB_MAJOR=10.5
# Tue, 02 Aug 2022 18:36:11 GMT
ARG MARIADB_VERSION=1:10.5.16+maria~focal
# Tue, 02 Aug 2022 18:36:12 GMT
ENV MARIADB_VERSION=1:10.5.16+maria~focal
# Tue, 02 Aug 2022 18:36:13 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
# Tue, 02 Aug 2022 18:36:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 02 Aug 2022 18:36:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 02 Aug 2022 18:36:36 GMT
VOLUME [/var/lib/mysql]
# Tue, 02 Aug 2022 18:36:38 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Tue, 02 Aug 2022 18:36:39 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Tue, 02 Aug 2022 18:36:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 18:36:40 GMT
EXPOSE 3306
# Tue, 02 Aug 2022 18:36:41 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a749a280e3e905de447c3d95a39e8aa1ede5835a6eadeb0c11596051592b675b`  
		Last Modified: Tue, 02 Aug 2022 01:20:32 GMT  
		Size: 27.2 MB (27191804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7d70702fc52aefacc8ccbff1968c3548d6400deb5e6c53d75f6dbc14905cb7`  
		Last Modified: Tue, 02 Aug 2022 18:42:44 GMT  
		Size: 1.7 KB (1722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9ffe290feb53a390aea694e16a663c4a420a71b1ebcd8053b07a44579782bbe`  
		Last Modified: Tue, 02 Aug 2022 18:42:44 GMT  
		Size: 5.3 MB (5321787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a430076265be6d7113b835ac1ab3e08dab46e41fff7e3ed070286125f1dbf6d`  
		Last Modified: Tue, 02 Aug 2022 18:42:43 GMT  
		Size: 3.4 MB (3367877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c880491c15580752404cccf2db4534a2d79f5b5cd1df18b3f6ea2754809020`  
		Last Modified: Tue, 02 Aug 2022 18:42:42 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ca8382cebf14e057456cd5ec8096f0053cdfe6029503875b74003df35d8c5e`  
		Last Modified: Tue, 02 Aug 2022 18:42:43 GMT  
		Size: 2.2 MB (2203204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88502488cc76b679835db628ad4d0f65e09a69018881918c6765cfb9e071feed`  
		Last Modified: Tue, 02 Aug 2022 18:42:40 GMT  
		Size: 2.5 KB (2466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73aa7230fd929e56b7fcd0d101bdd8d8b73add7b2720289ed00e6674a544ab1e`  
		Last Modified: Tue, 02 Aug 2022 18:43:45 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea1eeff7908e7408838d82d32ed8cb66888856b2921cec73825eeaa4a69f4e2`  
		Last Modified: Tue, 02 Aug 2022 18:43:58 GMT  
		Size: 87.2 MB (87246433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6679315a9b306139817f609532ddfbd3b84d9b45e98992e4394e27c2aff6a432`  
		Last Modified: Tue, 02 Aug 2022 18:43:45 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d74c1d7b93dc0c7ec4f06651ead1e8661eb86245a1a2f321e2f24509aa29721b`  
		Last Modified: Tue, 02 Aug 2022 18:43:45 GMT  
		Size: 6.7 KB (6692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; ppc64le

```console
$ docker pull mariadb@sha256:8ecf5d02db487cd6a65193433145aedc853dfcaaee3eadab5dd6fbcf21825795
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.0 MB (138959202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46f42885e7344227f68e6636123fde4c4cc9b2a1767eb2dbb61451dce796fbf8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 02 Aug 2022 01:31:01 GMT
ADD file:75dd7889d4feb83b8504153b5ea6873e4ab0e616a4f4489ea81fd055b6ce9def in / 
# Tue, 02 Aug 2022 01:31:03 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 04:33:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 03 Aug 2022 04:34:01 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 04:34:01 GMT
ENV GOSU_VERSION=1.14
# Wed, 03 Aug 2022 04:34:21 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 03 Aug 2022 04:34:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 03 Aug 2022 04:34:35 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 04:34:36 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 03 Aug 2022 04:34:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 03 Aug 2022 04:36:52 GMT
ARG MARIADB_MAJOR=10.5
# Wed, 03 Aug 2022 04:36:52 GMT
ENV MARIADB_MAJOR=10.5
# Wed, 03 Aug 2022 04:36:53 GMT
ARG MARIADB_VERSION=1:10.5.16+maria~focal
# Wed, 03 Aug 2022 04:36:53 GMT
ENV MARIADB_VERSION=1:10.5.16+maria~focal
# Wed, 03 Aug 2022 04:36:54 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
# Wed, 03 Aug 2022 04:36:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 03 Aug 2022 04:37:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 03 Aug 2022 04:37:40 GMT
VOLUME [/var/lib/mysql]
# Wed, 03 Aug 2022 04:37:41 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Wed, 03 Aug 2022 04:37:41 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Wed, 03 Aug 2022 04:37:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 Aug 2022 04:37:42 GMT
EXPOSE 3306
# Wed, 03 Aug 2022 04:37:42 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bf47d2be67f1a301865e78e8f78cc69c55dcc389921b4ba187dc0d333cbfd63b`  
		Last Modified: Tue, 02 Aug 2022 01:33:30 GMT  
		Size: 33.3 MB (33295352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b481bc43c771217829dcc78384d81402be7256c3fabe0fb95c0ad844e20eb486`  
		Last Modified: Wed, 03 Aug 2022 04:45:28 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f8f9934029ad30c4038aaa2505d3a55f09535b0f6cd3d115b622277ee43eec`  
		Last Modified: Wed, 03 Aug 2022 04:45:27 GMT  
		Size: 6.7 MB (6667750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ad8421e507f31703a57b5fcf441a19386060096de9f2d97716b6d1c03dd390`  
		Last Modified: Wed, 03 Aug 2022 04:45:27 GMT  
		Size: 3.7 MB (3669923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24953c586f1b7badf3268c6b00564095704918a0365c13b4d332008db8618e69`  
		Last Modified: Wed, 03 Aug 2022 04:45:25 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f4f22aaf2d7b83971e812c7422c924063814a37e635a032244e2b206911101b`  
		Last Modified: Wed, 03 Aug 2022 04:45:26 GMT  
		Size: 2.6 MB (2568638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57859f236e7f0146b0e787f561dafcb5fe2f724613fb2364c182a5ca2018030`  
		Last Modified: Wed, 03 Aug 2022 04:45:23 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:146b40a4021735a682d5a05972875876ac0c1cc2a70a73acb4f30c6cc724b202`  
		Last Modified: Wed, 03 Aug 2022 04:46:57 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a92a4e7410fcdda957784d6c6177f0e226353c12bcb990b0d385e8c058254c9`  
		Last Modified: Wed, 03 Aug 2022 04:47:21 GMT  
		Size: 92.7 MB (92742635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b34ba869d573a89a056ca236ca9b943b6d402d68a5dcbdb5380fa6210a6d59`  
		Last Modified: Wed, 03 Aug 2022 04:46:57 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89512578d4589051968d276286a5c1395feb4a4775ae32c9f7ecf98c11e647c0`  
		Last Modified: Wed, 03 Aug 2022 04:46:57 GMT  
		Size: 6.7 KB (6694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; s390x

```console
$ docker pull mariadb@sha256:59382be91c195b87f350a69017cf00bcebd06fb303bea810018417b0f495743d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.3 MB (127285075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbc3525d94e8fe268838806e44807a1fe3116d843d147ec3de28a5c7372b2161`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 02 Aug 2022 01:02:06 GMT
ADD file:409a01624b482522ab1ba2da28ff57bceb3bf89ff2f3cae5c9ea6068f6993355 in / 
# Tue, 02 Aug 2022 01:02:08 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 12:57:51 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 02 Aug 2022 12:58:02 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 12:58:02 GMT
ENV GOSU_VERSION=1.14
# Tue, 02 Aug 2022 12:58:10 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 02 Aug 2022 12:58:11 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 02 Aug 2022 12:58:16 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 12:58:16 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 02 Aug 2022 12:58:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 02 Aug 2022 12:59:35 GMT
ARG MARIADB_MAJOR=10.5
# Tue, 02 Aug 2022 12:59:36 GMT
ENV MARIADB_MAJOR=10.5
# Tue, 02 Aug 2022 12:59:36 GMT
ARG MARIADB_VERSION=1:10.5.16+maria~focal
# Tue, 02 Aug 2022 12:59:36 GMT
ENV MARIADB_VERSION=1:10.5.16+maria~focal
# Tue, 02 Aug 2022 12:59:36 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
# Tue, 02 Aug 2022 12:59:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 02 Aug 2022 12:59:58 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 02 Aug 2022 13:00:04 GMT
VOLUME [/var/lib/mysql]
# Tue, 02 Aug 2022 13:00:04 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Tue, 02 Aug 2022 13:00:04 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Tue, 02 Aug 2022 13:00:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 13:00:05 GMT
EXPOSE 3306
# Tue, 02 Aug 2022 13:00:05 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d522b75fb69271e75617d2e7bbeede1210f48bffdc57121ee39534eea94e2815`  
		Last Modified: Tue, 02 Aug 2022 01:03:38 GMT  
		Size: 27.0 MB (27045363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b542230411fae56efa86753d30f5439f912d60eabb26102f6570d97473c7573`  
		Last Modified: Tue, 02 Aug 2022 13:01:52 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9116cff82c5514acc6d105cb940a79d66cc9ca17bc78527c303509b2dbc6f095`  
		Last Modified: Tue, 02 Aug 2022 13:01:51 GMT  
		Size: 5.4 MB (5372728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9de0756f9486981018019372396743263fc5ff93d3aefa2ad557cc5b3307689f`  
		Last Modified: Tue, 02 Aug 2022 13:01:51 GMT  
		Size: 3.2 MB (3240183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff661c0d7c1d54aca25ce7155b5446f9e7b2a43a4db6a70bd1876da78b06b98e`  
		Last Modified: Tue, 02 Aug 2022 13:01:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7962d6c3604efb9aeed7adbc9fa294d45741fc8843c76a1b0acda6b306208b6a`  
		Last Modified: Tue, 02 Aug 2022 13:01:51 GMT  
		Size: 2.2 MB (2183826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0834a13ee0d34f33d37fdf14c52e61904a4660c0154507ec87a01ddb58423a71`  
		Last Modified: Tue, 02 Aug 2022 13:01:49 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20d15d120b6848cb90865ad9c99d6951b9948934b2c6112a8f6d27e31ffa68dc`  
		Last Modified: Tue, 02 Aug 2022 13:02:39 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baafb3e5ae3fbfd2ffa2e890c9d8953db64ff74dde6d43b103cbb07430901dd9`  
		Last Modified: Tue, 02 Aug 2022 13:02:51 GMT  
		Size: 89.4 MB (89428074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58b713dfcd2d266e29596d726d7d12526ae3cb0edc5b64e60fbf64c7e30955ad`  
		Last Modified: Tue, 02 Aug 2022 13:02:39 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3d0b374d3180cc658751a5688a51f2aff52e93c9ecb9065f1ce957d536db21d`  
		Last Modified: Tue, 02 Aug 2022 13:02:39 GMT  
		Size: 6.7 KB (6694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5-focal`

```console
$ docker pull mariadb@sha256:473c1bd96f54846c857869f1774f180fc97075d096e82ce87ff0d00f64803bc5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.5-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:910c1742bad5346be709801726ffb14330f83b32afa82530b34719bf80a9c243
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.1 MB (128066304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83ea47900c5495b8a3627804273fbb724c1592d11cf11ce08d8d688bb3cd6f6c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:49 GMT
ADD file:af4cf77e6818016b697a1491101b40c71d06529ced65f36107749f099d6d4bdc in / 
# Tue, 02 Aug 2022 01:30:49 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 20:21:24 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 02 Aug 2022 20:21:32 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 20:21:32 GMT
ENV GOSU_VERSION=1.14
# Tue, 02 Aug 2022 20:21:42 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 02 Aug 2022 20:21:42 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 02 Aug 2022 20:21:49 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 20:21:49 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 02 Aug 2022 20:21:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 02 Aug 2022 20:23:01 GMT
ARG MARIADB_MAJOR=10.5
# Tue, 02 Aug 2022 20:23:01 GMT
ENV MARIADB_MAJOR=10.5
# Tue, 02 Aug 2022 20:23:01 GMT
ARG MARIADB_VERSION=1:10.5.16+maria~focal
# Tue, 02 Aug 2022 20:23:01 GMT
ENV MARIADB_VERSION=1:10.5.16+maria~focal
# Tue, 02 Aug 2022 20:23:01 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
# Tue, 02 Aug 2022 20:23:01 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 02 Aug 2022 20:23:23 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 02 Aug 2022 20:23:24 GMT
VOLUME [/var/lib/mysql]
# Tue, 02 Aug 2022 20:23:24 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Tue, 02 Aug 2022 20:23:24 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Tue, 02 Aug 2022 20:23:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 20:23:24 GMT
EXPOSE 3306
# Tue, 02 Aug 2022 20:23:24 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3b65ec22a9e96affe680712973e88355927506aa3f792ff03330f3a3eb601a98`  
		Last Modified: Tue, 02 Aug 2022 01:31:59 GMT  
		Size: 28.6 MB (28572596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d19669910bc06b914ac5d4512b9aa15623df49e4ef03d20277f4a8fda0cf5631`  
		Last Modified: Tue, 02 Aug 2022 20:27:42 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c46f5717c584782c1a1498020ed1354006c97d58cb69a3607a17e1e0023da0e`  
		Last Modified: Tue, 02 Aug 2022 20:27:40 GMT  
		Size: 5.5 MB (5488983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea0278d54bb37ba2adf21e281d933e45b7c110f62e93e95b27c88940599003a1`  
		Last Modified: Tue, 02 Aug 2022 20:27:40 GMT  
		Size: 3.6 MB (3581823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80813ba5cb6ef218fb6cb3a25b964d31f0cd372ca1c2427c140d587a5a74a13`  
		Last Modified: Tue, 02 Aug 2022 20:27:39 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc4ac948168b66da6b55897167508489a2ab555945d5030db3362f06b232c51`  
		Last Modified: Tue, 02 Aug 2022 20:27:40 GMT  
		Size: 2.3 MB (2272442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d65facec905da8f0741a9561cf142ab88af72c392c88ab6d32c630704907f642`  
		Last Modified: Tue, 02 Aug 2022 20:27:37 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68b10715d9bb4160d2ac31d5a7cfe51703b1c7addd4256d6e23910a2bca430a9`  
		Last Modified: Tue, 02 Aug 2022 20:28:39 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba6b1b231f2e46c2bb48f813248b8c338d247d21597d08bf54eeb4b2dc3456f`  
		Last Modified: Tue, 02 Aug 2022 20:28:52 GMT  
		Size: 88.1 MB (88135566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:058ed59cd119a24508bfe59d19260c5fb617115556679686ba8c4b5bcfcb9ac3`  
		Last Modified: Tue, 02 Aug 2022 20:28:39 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9e4955b52c41269e59331263ab1315cdc538209bdb6273eacd842c8fab721b`  
		Last Modified: Tue, 02 Aug 2022 20:28:39 GMT  
		Size: 6.7 KB (6689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:598ef479e99feea2749a234780c80def9b7ae5bc9b5f5a62400052f480b70ce3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.3 MB (125345920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22ff76a6fdcb615fc7a9e59ea1fb855f5844aafc946634f62d70a60f43ef6875`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:51 GMT
ADD file:151548d1bfac57d762f2c0b18b2378c363ffd1568da9fecd4be611db4832e8e2 in / 
# Tue, 02 Aug 2022 01:18:51 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 18:34:06 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 02 Aug 2022 18:34:17 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 18:34:18 GMT
ENV GOSU_VERSION=1.14
# Tue, 02 Aug 2022 18:34:33 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 02 Aug 2022 18:34:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 02 Aug 2022 18:34:42 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 18:34:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 02 Aug 2022 18:34:45 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 02 Aug 2022 18:36:10 GMT
ARG MARIADB_MAJOR=10.5
# Tue, 02 Aug 2022 18:36:10 GMT
ENV MARIADB_MAJOR=10.5
# Tue, 02 Aug 2022 18:36:11 GMT
ARG MARIADB_VERSION=1:10.5.16+maria~focal
# Tue, 02 Aug 2022 18:36:12 GMT
ENV MARIADB_VERSION=1:10.5.16+maria~focal
# Tue, 02 Aug 2022 18:36:13 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
# Tue, 02 Aug 2022 18:36:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 02 Aug 2022 18:36:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 02 Aug 2022 18:36:36 GMT
VOLUME [/var/lib/mysql]
# Tue, 02 Aug 2022 18:36:38 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Tue, 02 Aug 2022 18:36:39 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Tue, 02 Aug 2022 18:36:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 18:36:40 GMT
EXPOSE 3306
# Tue, 02 Aug 2022 18:36:41 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a749a280e3e905de447c3d95a39e8aa1ede5835a6eadeb0c11596051592b675b`  
		Last Modified: Tue, 02 Aug 2022 01:20:32 GMT  
		Size: 27.2 MB (27191804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7d70702fc52aefacc8ccbff1968c3548d6400deb5e6c53d75f6dbc14905cb7`  
		Last Modified: Tue, 02 Aug 2022 18:42:44 GMT  
		Size: 1.7 KB (1722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9ffe290feb53a390aea694e16a663c4a420a71b1ebcd8053b07a44579782bbe`  
		Last Modified: Tue, 02 Aug 2022 18:42:44 GMT  
		Size: 5.3 MB (5321787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a430076265be6d7113b835ac1ab3e08dab46e41fff7e3ed070286125f1dbf6d`  
		Last Modified: Tue, 02 Aug 2022 18:42:43 GMT  
		Size: 3.4 MB (3367877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c880491c15580752404cccf2db4534a2d79f5b5cd1df18b3f6ea2754809020`  
		Last Modified: Tue, 02 Aug 2022 18:42:42 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ca8382cebf14e057456cd5ec8096f0053cdfe6029503875b74003df35d8c5e`  
		Last Modified: Tue, 02 Aug 2022 18:42:43 GMT  
		Size: 2.2 MB (2203204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88502488cc76b679835db628ad4d0f65e09a69018881918c6765cfb9e071feed`  
		Last Modified: Tue, 02 Aug 2022 18:42:40 GMT  
		Size: 2.5 KB (2466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73aa7230fd929e56b7fcd0d101bdd8d8b73add7b2720289ed00e6674a544ab1e`  
		Last Modified: Tue, 02 Aug 2022 18:43:45 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea1eeff7908e7408838d82d32ed8cb66888856b2921cec73825eeaa4a69f4e2`  
		Last Modified: Tue, 02 Aug 2022 18:43:58 GMT  
		Size: 87.2 MB (87246433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6679315a9b306139817f609532ddfbd3b84d9b45e98992e4394e27c2aff6a432`  
		Last Modified: Tue, 02 Aug 2022 18:43:45 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d74c1d7b93dc0c7ec4f06651ead1e8661eb86245a1a2f321e2f24509aa29721b`  
		Last Modified: Tue, 02 Aug 2022 18:43:45 GMT  
		Size: 6.7 KB (6692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:8ecf5d02db487cd6a65193433145aedc853dfcaaee3eadab5dd6fbcf21825795
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.0 MB (138959202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46f42885e7344227f68e6636123fde4c4cc9b2a1767eb2dbb61451dce796fbf8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 02 Aug 2022 01:31:01 GMT
ADD file:75dd7889d4feb83b8504153b5ea6873e4ab0e616a4f4489ea81fd055b6ce9def in / 
# Tue, 02 Aug 2022 01:31:03 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 04:33:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 03 Aug 2022 04:34:01 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 04:34:01 GMT
ENV GOSU_VERSION=1.14
# Wed, 03 Aug 2022 04:34:21 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 03 Aug 2022 04:34:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 03 Aug 2022 04:34:35 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 04:34:36 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 03 Aug 2022 04:34:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 03 Aug 2022 04:36:52 GMT
ARG MARIADB_MAJOR=10.5
# Wed, 03 Aug 2022 04:36:52 GMT
ENV MARIADB_MAJOR=10.5
# Wed, 03 Aug 2022 04:36:53 GMT
ARG MARIADB_VERSION=1:10.5.16+maria~focal
# Wed, 03 Aug 2022 04:36:53 GMT
ENV MARIADB_VERSION=1:10.5.16+maria~focal
# Wed, 03 Aug 2022 04:36:54 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
# Wed, 03 Aug 2022 04:36:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 03 Aug 2022 04:37:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 03 Aug 2022 04:37:40 GMT
VOLUME [/var/lib/mysql]
# Wed, 03 Aug 2022 04:37:41 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Wed, 03 Aug 2022 04:37:41 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Wed, 03 Aug 2022 04:37:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 Aug 2022 04:37:42 GMT
EXPOSE 3306
# Wed, 03 Aug 2022 04:37:42 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bf47d2be67f1a301865e78e8f78cc69c55dcc389921b4ba187dc0d333cbfd63b`  
		Last Modified: Tue, 02 Aug 2022 01:33:30 GMT  
		Size: 33.3 MB (33295352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b481bc43c771217829dcc78384d81402be7256c3fabe0fb95c0ad844e20eb486`  
		Last Modified: Wed, 03 Aug 2022 04:45:28 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f8f9934029ad30c4038aaa2505d3a55f09535b0f6cd3d115b622277ee43eec`  
		Last Modified: Wed, 03 Aug 2022 04:45:27 GMT  
		Size: 6.7 MB (6667750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ad8421e507f31703a57b5fcf441a19386060096de9f2d97716b6d1c03dd390`  
		Last Modified: Wed, 03 Aug 2022 04:45:27 GMT  
		Size: 3.7 MB (3669923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24953c586f1b7badf3268c6b00564095704918a0365c13b4d332008db8618e69`  
		Last Modified: Wed, 03 Aug 2022 04:45:25 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f4f22aaf2d7b83971e812c7422c924063814a37e635a032244e2b206911101b`  
		Last Modified: Wed, 03 Aug 2022 04:45:26 GMT  
		Size: 2.6 MB (2568638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57859f236e7f0146b0e787f561dafcb5fe2f724613fb2364c182a5ca2018030`  
		Last Modified: Wed, 03 Aug 2022 04:45:23 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:146b40a4021735a682d5a05972875876ac0c1cc2a70a73acb4f30c6cc724b202`  
		Last Modified: Wed, 03 Aug 2022 04:46:57 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a92a4e7410fcdda957784d6c6177f0e226353c12bcb990b0d385e8c058254c9`  
		Last Modified: Wed, 03 Aug 2022 04:47:21 GMT  
		Size: 92.7 MB (92742635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b34ba869d573a89a056ca236ca9b943b6d402d68a5dcbdb5380fa6210a6d59`  
		Last Modified: Wed, 03 Aug 2022 04:46:57 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89512578d4589051968d276286a5c1395feb4a4775ae32c9f7ecf98c11e647c0`  
		Last Modified: Wed, 03 Aug 2022 04:46:57 GMT  
		Size: 6.7 KB (6694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:59382be91c195b87f350a69017cf00bcebd06fb303bea810018417b0f495743d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.3 MB (127285075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbc3525d94e8fe268838806e44807a1fe3116d843d147ec3de28a5c7372b2161`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 02 Aug 2022 01:02:06 GMT
ADD file:409a01624b482522ab1ba2da28ff57bceb3bf89ff2f3cae5c9ea6068f6993355 in / 
# Tue, 02 Aug 2022 01:02:08 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 12:57:51 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 02 Aug 2022 12:58:02 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 12:58:02 GMT
ENV GOSU_VERSION=1.14
# Tue, 02 Aug 2022 12:58:10 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 02 Aug 2022 12:58:11 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 02 Aug 2022 12:58:16 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 12:58:16 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 02 Aug 2022 12:58:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 02 Aug 2022 12:59:35 GMT
ARG MARIADB_MAJOR=10.5
# Tue, 02 Aug 2022 12:59:36 GMT
ENV MARIADB_MAJOR=10.5
# Tue, 02 Aug 2022 12:59:36 GMT
ARG MARIADB_VERSION=1:10.5.16+maria~focal
# Tue, 02 Aug 2022 12:59:36 GMT
ENV MARIADB_VERSION=1:10.5.16+maria~focal
# Tue, 02 Aug 2022 12:59:36 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
# Tue, 02 Aug 2022 12:59:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 02 Aug 2022 12:59:58 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 02 Aug 2022 13:00:04 GMT
VOLUME [/var/lib/mysql]
# Tue, 02 Aug 2022 13:00:04 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Tue, 02 Aug 2022 13:00:04 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Tue, 02 Aug 2022 13:00:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 13:00:05 GMT
EXPOSE 3306
# Tue, 02 Aug 2022 13:00:05 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d522b75fb69271e75617d2e7bbeede1210f48bffdc57121ee39534eea94e2815`  
		Last Modified: Tue, 02 Aug 2022 01:03:38 GMT  
		Size: 27.0 MB (27045363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b542230411fae56efa86753d30f5439f912d60eabb26102f6570d97473c7573`  
		Last Modified: Tue, 02 Aug 2022 13:01:52 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9116cff82c5514acc6d105cb940a79d66cc9ca17bc78527c303509b2dbc6f095`  
		Last Modified: Tue, 02 Aug 2022 13:01:51 GMT  
		Size: 5.4 MB (5372728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9de0756f9486981018019372396743263fc5ff93d3aefa2ad557cc5b3307689f`  
		Last Modified: Tue, 02 Aug 2022 13:01:51 GMT  
		Size: 3.2 MB (3240183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff661c0d7c1d54aca25ce7155b5446f9e7b2a43a4db6a70bd1876da78b06b98e`  
		Last Modified: Tue, 02 Aug 2022 13:01:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7962d6c3604efb9aeed7adbc9fa294d45741fc8843c76a1b0acda6b306208b6a`  
		Last Modified: Tue, 02 Aug 2022 13:01:51 GMT  
		Size: 2.2 MB (2183826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0834a13ee0d34f33d37fdf14c52e61904a4660c0154507ec87a01ddb58423a71`  
		Last Modified: Tue, 02 Aug 2022 13:01:49 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20d15d120b6848cb90865ad9c99d6951b9948934b2c6112a8f6d27e31ffa68dc`  
		Last Modified: Tue, 02 Aug 2022 13:02:39 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baafb3e5ae3fbfd2ffa2e890c9d8953db64ff74dde6d43b103cbb07430901dd9`  
		Last Modified: Tue, 02 Aug 2022 13:02:51 GMT  
		Size: 89.4 MB (89428074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58b713dfcd2d266e29596d726d7d12526ae3cb0edc5b64e60fbf64c7e30955ad`  
		Last Modified: Tue, 02 Aug 2022 13:02:39 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3d0b374d3180cc658751a5688a51f2aff52e93c9ecb9065f1ce957d536db21d`  
		Last Modified: Tue, 02 Aug 2022 13:02:39 GMT  
		Size: 6.7 KB (6694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5.17`

**does not exist** (yet?)

## `mariadb:10.5.17-focal`

**does not exist** (yet?)

## `mariadb:10.6`

```console
$ docker pull mariadb@sha256:e78a7000d93b2fabc0bfb6ff1504199f2f9bfb4a8b7350922c08dabf2b2bdbea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.6` - linux; amd64

```console
$ docker pull mariadb@sha256:18a9f72d33348c7a8cb505c02c347495311862db5f3b1494f2eb55fe2c0c774d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.4 MB (128350214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0c5b7b9981e7d661f6492d100bef118e068de7ff5d26302ae5cae028d716b97`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:49 GMT
ADD file:af4cf77e6818016b697a1491101b40c71d06529ced65f36107749f099d6d4bdc in / 
# Tue, 02 Aug 2022 01:30:49 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 20:21:24 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 02 Aug 2022 20:21:32 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 20:21:32 GMT
ENV GOSU_VERSION=1.14
# Tue, 02 Aug 2022 20:21:42 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 02 Aug 2022 20:21:42 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 02 Aug 2022 20:21:49 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 20:21:49 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 02 Aug 2022 20:21:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 02 Aug 2022 20:22:32 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 02 Aug 2022 20:22:32 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 02 Aug 2022 20:22:33 GMT
ARG MARIADB_VERSION=1:10.6.8+maria~focal
# Tue, 02 Aug 2022 20:22:33 GMT
ENV MARIADB_VERSION=1:10.6.8+maria~focal
# Tue, 02 Aug 2022 20:22:33 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
# Tue, 02 Aug 2022 20:22:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 02 Aug 2022 20:22:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 02 Aug 2022 20:22:56 GMT
VOLUME [/var/lib/mysql]
# Tue, 02 Aug 2022 20:22:56 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 02 Aug 2022 20:22:56 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 02 Aug 2022 20:22:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 20:22:56 GMT
EXPOSE 3306
# Tue, 02 Aug 2022 20:22:56 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:3b65ec22a9e96affe680712973e88355927506aa3f792ff03330f3a3eb601a98`  
		Last Modified: Tue, 02 Aug 2022 01:31:59 GMT  
		Size: 28.6 MB (28572596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d19669910bc06b914ac5d4512b9aa15623df49e4ef03d20277f4a8fda0cf5631`  
		Last Modified: Tue, 02 Aug 2022 20:27:42 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c46f5717c584782c1a1498020ed1354006c97d58cb69a3607a17e1e0023da0e`  
		Last Modified: Tue, 02 Aug 2022 20:27:40 GMT  
		Size: 5.5 MB (5488983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea0278d54bb37ba2adf21e281d933e45b7c110f62e93e95b27c88940599003a1`  
		Last Modified: Tue, 02 Aug 2022 20:27:40 GMT  
		Size: 3.6 MB (3581823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80813ba5cb6ef218fb6cb3a25b964d31f0cd372ca1c2427c140d587a5a74a13`  
		Last Modified: Tue, 02 Aug 2022 20:27:39 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc4ac948168b66da6b55897167508489a2ab555945d5030db3362f06b232c51`  
		Last Modified: Tue, 02 Aug 2022 20:27:40 GMT  
		Size: 2.3 MB (2272442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d65facec905da8f0741a9561cf142ab88af72c392c88ab6d32c630704907f642`  
		Last Modified: Tue, 02 Aug 2022 20:27:37 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5763bd0e9dcf8906ab3f6f03958389dd782eca9f1ad96f140f0e2d000b3086e`  
		Last Modified: Tue, 02 Aug 2022 20:28:09 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ce50f319e47bdd475c576ea13f7278e97a3175c12fb65ac3781bc620be3bd3a`  
		Last Modified: Tue, 02 Aug 2022 20:28:23 GMT  
		Size: 88.4 MB (88419472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf22e53975d3f8c02519c4b71feb436afce12bf0c8b92b4e30107a2be82cfce`  
		Last Modified: Tue, 02 Aug 2022 20:28:09 GMT  
		Size: 3.5 KB (3488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b47f74b397483f01fdfe8c4c1124d658861e8a5e7d8143fe1744bc99e21d90`  
		Last Modified: Tue, 02 Aug 2022 20:28:09 GMT  
		Size: 6.7 KB (6694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:1c8211242687771ba8775fd77e617f44d50de51af10ba1a60b6c1a12c3aa0a73
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.4 MB (125424161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76ca1eb53e914808b68c4be26966b4b26341224b78cdc44174451506c480b96b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:51 GMT
ADD file:151548d1bfac57d762f2c0b18b2378c363ffd1568da9fecd4be611db4832e8e2 in / 
# Tue, 02 Aug 2022 01:18:51 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 18:34:06 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 02 Aug 2022 18:34:17 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 18:34:18 GMT
ENV GOSU_VERSION=1.14
# Tue, 02 Aug 2022 18:34:33 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 02 Aug 2022 18:34:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 02 Aug 2022 18:34:42 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 18:34:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 02 Aug 2022 18:34:45 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 02 Aug 2022 18:35:32 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 02 Aug 2022 18:35:32 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 02 Aug 2022 18:35:33 GMT
ARG MARIADB_VERSION=1:10.6.8+maria~focal
# Tue, 02 Aug 2022 18:35:34 GMT
ENV MARIADB_VERSION=1:10.6.8+maria~focal
# Tue, 02 Aug 2022 18:35:35 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
# Tue, 02 Aug 2022 18:35:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 02 Aug 2022 18:35:58 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 02 Aug 2022 18:35:59 GMT
VOLUME [/var/lib/mysql]
# Tue, 02 Aug 2022 18:36:00 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 02 Aug 2022 18:36:01 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 02 Aug 2022 18:36:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 18:36:02 GMT
EXPOSE 3306
# Tue, 02 Aug 2022 18:36:03 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:a749a280e3e905de447c3d95a39e8aa1ede5835a6eadeb0c11596051592b675b`  
		Last Modified: Tue, 02 Aug 2022 01:20:32 GMT  
		Size: 27.2 MB (27191804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7d70702fc52aefacc8ccbff1968c3548d6400deb5e6c53d75f6dbc14905cb7`  
		Last Modified: Tue, 02 Aug 2022 18:42:44 GMT  
		Size: 1.7 KB (1722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9ffe290feb53a390aea694e16a663c4a420a71b1ebcd8053b07a44579782bbe`  
		Last Modified: Tue, 02 Aug 2022 18:42:44 GMT  
		Size: 5.3 MB (5321787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a430076265be6d7113b835ac1ab3e08dab46e41fff7e3ed070286125f1dbf6d`  
		Last Modified: Tue, 02 Aug 2022 18:42:43 GMT  
		Size: 3.4 MB (3367877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c880491c15580752404cccf2db4534a2d79f5b5cd1df18b3f6ea2754809020`  
		Last Modified: Tue, 02 Aug 2022 18:42:42 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ca8382cebf14e057456cd5ec8096f0053cdfe6029503875b74003df35d8c5e`  
		Last Modified: Tue, 02 Aug 2022 18:42:43 GMT  
		Size: 2.2 MB (2203204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88502488cc76b679835db628ad4d0f65e09a69018881918c6765cfb9e071feed`  
		Last Modified: Tue, 02 Aug 2022 18:42:40 GMT  
		Size: 2.5 KB (2466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae7307cb02fdd519b5d7db3c1f30d412779b83c0f83d4a7f158dc041a6b04a3`  
		Last Modified: Tue, 02 Aug 2022 18:43:13 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df60df6710cca87a5d1e1be55009d96bcfee6713469124932f98d485d5ab8199`  
		Last Modified: Tue, 02 Aug 2022 18:43:26 GMT  
		Size: 87.3 MB (87324673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb82d118ee8fca5b9a0db692402b5f23e230f67088b3b572096a838a27218041`  
		Last Modified: Tue, 02 Aug 2022 18:43:13 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce2f3952ce52f25a2e27142678fb9c50087932d4ae71476b13f8728b0a42ef9`  
		Last Modified: Tue, 02 Aug 2022 18:43:13 GMT  
		Size: 6.7 KB (6696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6` - linux; ppc64le

```console
$ docker pull mariadb@sha256:1b11d8c12a5364e8dc7e704047ff4e7577640062c67babd074eeeff198f0415b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.0 MB (139025283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b277eeb3a1cc241eefca94775f59fc06b461e3bce4060bd3f22ad0bad7c1f668`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 02 Aug 2022 01:31:01 GMT
ADD file:75dd7889d4feb83b8504153b5ea6873e4ab0e616a4f4489ea81fd055b6ce9def in / 
# Tue, 02 Aug 2022 01:31:03 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 04:33:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 03 Aug 2022 04:34:01 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 04:34:01 GMT
ENV GOSU_VERSION=1.14
# Wed, 03 Aug 2022 04:34:21 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 03 Aug 2022 04:34:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 03 Aug 2022 04:34:35 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 04:34:36 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 03 Aug 2022 04:34:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 03 Aug 2022 04:35:52 GMT
ARG MARIADB_MAJOR=10.6
# Wed, 03 Aug 2022 04:35:53 GMT
ENV MARIADB_MAJOR=10.6
# Wed, 03 Aug 2022 04:35:53 GMT
ARG MARIADB_VERSION=1:10.6.8+maria~focal
# Wed, 03 Aug 2022 04:35:53 GMT
ENV MARIADB_VERSION=1:10.6.8+maria~focal
# Wed, 03 Aug 2022 04:35:54 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
# Wed, 03 Aug 2022 04:35:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 03 Aug 2022 04:36:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 03 Aug 2022 04:36:40 GMT
VOLUME [/var/lib/mysql]
# Wed, 03 Aug 2022 04:36:41 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Wed, 03 Aug 2022 04:36:41 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Wed, 03 Aug 2022 04:36:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 Aug 2022 04:36:42 GMT
EXPOSE 3306
# Wed, 03 Aug 2022 04:36:42 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:bf47d2be67f1a301865e78e8f78cc69c55dcc389921b4ba187dc0d333cbfd63b`  
		Last Modified: Tue, 02 Aug 2022 01:33:30 GMT  
		Size: 33.3 MB (33295352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b481bc43c771217829dcc78384d81402be7256c3fabe0fb95c0ad844e20eb486`  
		Last Modified: Wed, 03 Aug 2022 04:45:28 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f8f9934029ad30c4038aaa2505d3a55f09535b0f6cd3d115b622277ee43eec`  
		Last Modified: Wed, 03 Aug 2022 04:45:27 GMT  
		Size: 6.7 MB (6667750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ad8421e507f31703a57b5fcf441a19386060096de9f2d97716b6d1c03dd390`  
		Last Modified: Wed, 03 Aug 2022 04:45:27 GMT  
		Size: 3.7 MB (3669923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24953c586f1b7badf3268c6b00564095704918a0365c13b4d332008db8618e69`  
		Last Modified: Wed, 03 Aug 2022 04:45:25 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f4f22aaf2d7b83971e812c7422c924063814a37e635a032244e2b206911101b`  
		Last Modified: Wed, 03 Aug 2022 04:45:26 GMT  
		Size: 2.6 MB (2568638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57859f236e7f0146b0e787f561dafcb5fe2f724613fb2364c182a5ca2018030`  
		Last Modified: Wed, 03 Aug 2022 04:45:23 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1abb7ca0778f18b6321d931ce6b922a2597450e921a7345216b6473947d61aa2`  
		Last Modified: Wed, 03 Aug 2022 04:46:10 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc412d1dc0bad051399c592960e71e3690338616e4b6837c9c4792c890b92f3`  
		Last Modified: Wed, 03 Aug 2022 04:46:34 GMT  
		Size: 92.8 MB (92808710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e762fc6deb17e2e3a2f41f857174cd04d2062dec645edd6efc8e0dd2e6d5bee9`  
		Last Modified: Wed, 03 Aug 2022 04:46:10 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:935e3244bde1b7941807c2a93114cf1aa5ed34459f44d8e683c92c0a0c6bc3c2`  
		Last Modified: Wed, 03 Aug 2022 04:46:10 GMT  
		Size: 6.7 KB (6699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6` - linux; s390x

```console
$ docker pull mariadb@sha256:094d648428e889a5d9c2ec1a3756d661d9ad52bd8031deda97d60a49bc4b426c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.4 MB (127357754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9c987c87b7d4a6f5b9ee4b7498186d1a6d5be62b3caa938ed66682c7a60c513`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 02 Aug 2022 01:02:06 GMT
ADD file:409a01624b482522ab1ba2da28ff57bceb3bf89ff2f3cae5c9ea6068f6993355 in / 
# Tue, 02 Aug 2022 01:02:08 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 12:57:51 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 02 Aug 2022 12:58:02 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 12:58:02 GMT
ENV GOSU_VERSION=1.14
# Tue, 02 Aug 2022 12:58:10 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 02 Aug 2022 12:58:11 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 02 Aug 2022 12:58:16 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 12:58:16 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 02 Aug 2022 12:58:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 02 Aug 2022 12:58:59 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 02 Aug 2022 12:58:59 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 02 Aug 2022 12:58:59 GMT
ARG MARIADB_VERSION=1:10.6.8+maria~focal
# Tue, 02 Aug 2022 12:59:00 GMT
ENV MARIADB_VERSION=1:10.6.8+maria~focal
# Tue, 02 Aug 2022 12:59:00 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
# Tue, 02 Aug 2022 12:59:01 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 02 Aug 2022 12:59:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 02 Aug 2022 12:59:25 GMT
VOLUME [/var/lib/mysql]
# Tue, 02 Aug 2022 12:59:25 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 02 Aug 2022 12:59:25 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 02 Aug 2022 12:59:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 12:59:26 GMT
EXPOSE 3306
# Tue, 02 Aug 2022 12:59:26 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d522b75fb69271e75617d2e7bbeede1210f48bffdc57121ee39534eea94e2815`  
		Last Modified: Tue, 02 Aug 2022 01:03:38 GMT  
		Size: 27.0 MB (27045363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b542230411fae56efa86753d30f5439f912d60eabb26102f6570d97473c7573`  
		Last Modified: Tue, 02 Aug 2022 13:01:52 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9116cff82c5514acc6d105cb940a79d66cc9ca17bc78527c303509b2dbc6f095`  
		Last Modified: Tue, 02 Aug 2022 13:01:51 GMT  
		Size: 5.4 MB (5372728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9de0756f9486981018019372396743263fc5ff93d3aefa2ad557cc5b3307689f`  
		Last Modified: Tue, 02 Aug 2022 13:01:51 GMT  
		Size: 3.2 MB (3240183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff661c0d7c1d54aca25ce7155b5446f9e7b2a43a4db6a70bd1876da78b06b98e`  
		Last Modified: Tue, 02 Aug 2022 13:01:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7962d6c3604efb9aeed7adbc9fa294d45741fc8843c76a1b0acda6b306208b6a`  
		Last Modified: Tue, 02 Aug 2022 13:01:51 GMT  
		Size: 2.2 MB (2183826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0834a13ee0d34f33d37fdf14c52e61904a4660c0154507ec87a01ddb58423a71`  
		Last Modified: Tue, 02 Aug 2022 13:01:49 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48fab4697854f490148d65832aecd4d5d470753f99ebd7dab895f806018820f`  
		Last Modified: Tue, 02 Aug 2022 13:02:16 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a73aff9544f2af693ce068da60e28265aeeb78562d2739d4aa7e00fe2173b3`  
		Last Modified: Tue, 02 Aug 2022 13:02:28 GMT  
		Size: 89.5 MB (89500752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e51ebb9416afd45bfdef43a83663ded70bee363c22a4ef0083374329fa41e975`  
		Last Modified: Tue, 02 Aug 2022 13:02:16 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f50ac00fe5226cde100ea6dfcf7a108cfc585c6d4518846593333e9cdbe6c46`  
		Last Modified: Tue, 02 Aug 2022 13:02:16 GMT  
		Size: 6.7 KB (6697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.6-focal`

```console
$ docker pull mariadb@sha256:e78a7000d93b2fabc0bfb6ff1504199f2f9bfb4a8b7350922c08dabf2b2bdbea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.6-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:18a9f72d33348c7a8cb505c02c347495311862db5f3b1494f2eb55fe2c0c774d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.4 MB (128350214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0c5b7b9981e7d661f6492d100bef118e068de7ff5d26302ae5cae028d716b97`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:49 GMT
ADD file:af4cf77e6818016b697a1491101b40c71d06529ced65f36107749f099d6d4bdc in / 
# Tue, 02 Aug 2022 01:30:49 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 20:21:24 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 02 Aug 2022 20:21:32 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 20:21:32 GMT
ENV GOSU_VERSION=1.14
# Tue, 02 Aug 2022 20:21:42 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 02 Aug 2022 20:21:42 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 02 Aug 2022 20:21:49 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 20:21:49 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 02 Aug 2022 20:21:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 02 Aug 2022 20:22:32 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 02 Aug 2022 20:22:32 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 02 Aug 2022 20:22:33 GMT
ARG MARIADB_VERSION=1:10.6.8+maria~focal
# Tue, 02 Aug 2022 20:22:33 GMT
ENV MARIADB_VERSION=1:10.6.8+maria~focal
# Tue, 02 Aug 2022 20:22:33 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
# Tue, 02 Aug 2022 20:22:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 02 Aug 2022 20:22:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 02 Aug 2022 20:22:56 GMT
VOLUME [/var/lib/mysql]
# Tue, 02 Aug 2022 20:22:56 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 02 Aug 2022 20:22:56 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 02 Aug 2022 20:22:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 20:22:56 GMT
EXPOSE 3306
# Tue, 02 Aug 2022 20:22:56 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:3b65ec22a9e96affe680712973e88355927506aa3f792ff03330f3a3eb601a98`  
		Last Modified: Tue, 02 Aug 2022 01:31:59 GMT  
		Size: 28.6 MB (28572596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d19669910bc06b914ac5d4512b9aa15623df49e4ef03d20277f4a8fda0cf5631`  
		Last Modified: Tue, 02 Aug 2022 20:27:42 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c46f5717c584782c1a1498020ed1354006c97d58cb69a3607a17e1e0023da0e`  
		Last Modified: Tue, 02 Aug 2022 20:27:40 GMT  
		Size: 5.5 MB (5488983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea0278d54bb37ba2adf21e281d933e45b7c110f62e93e95b27c88940599003a1`  
		Last Modified: Tue, 02 Aug 2022 20:27:40 GMT  
		Size: 3.6 MB (3581823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80813ba5cb6ef218fb6cb3a25b964d31f0cd372ca1c2427c140d587a5a74a13`  
		Last Modified: Tue, 02 Aug 2022 20:27:39 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc4ac948168b66da6b55897167508489a2ab555945d5030db3362f06b232c51`  
		Last Modified: Tue, 02 Aug 2022 20:27:40 GMT  
		Size: 2.3 MB (2272442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d65facec905da8f0741a9561cf142ab88af72c392c88ab6d32c630704907f642`  
		Last Modified: Tue, 02 Aug 2022 20:27:37 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5763bd0e9dcf8906ab3f6f03958389dd782eca9f1ad96f140f0e2d000b3086e`  
		Last Modified: Tue, 02 Aug 2022 20:28:09 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ce50f319e47bdd475c576ea13f7278e97a3175c12fb65ac3781bc620be3bd3a`  
		Last Modified: Tue, 02 Aug 2022 20:28:23 GMT  
		Size: 88.4 MB (88419472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf22e53975d3f8c02519c4b71feb436afce12bf0c8b92b4e30107a2be82cfce`  
		Last Modified: Tue, 02 Aug 2022 20:28:09 GMT  
		Size: 3.5 KB (3488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b47f74b397483f01fdfe8c4c1124d658861e8a5e7d8143fe1744bc99e21d90`  
		Last Modified: Tue, 02 Aug 2022 20:28:09 GMT  
		Size: 6.7 KB (6694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:1c8211242687771ba8775fd77e617f44d50de51af10ba1a60b6c1a12c3aa0a73
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.4 MB (125424161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76ca1eb53e914808b68c4be26966b4b26341224b78cdc44174451506c480b96b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:51 GMT
ADD file:151548d1bfac57d762f2c0b18b2378c363ffd1568da9fecd4be611db4832e8e2 in / 
# Tue, 02 Aug 2022 01:18:51 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 18:34:06 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 02 Aug 2022 18:34:17 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 18:34:18 GMT
ENV GOSU_VERSION=1.14
# Tue, 02 Aug 2022 18:34:33 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 02 Aug 2022 18:34:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 02 Aug 2022 18:34:42 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 18:34:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 02 Aug 2022 18:34:45 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 02 Aug 2022 18:35:32 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 02 Aug 2022 18:35:32 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 02 Aug 2022 18:35:33 GMT
ARG MARIADB_VERSION=1:10.6.8+maria~focal
# Tue, 02 Aug 2022 18:35:34 GMT
ENV MARIADB_VERSION=1:10.6.8+maria~focal
# Tue, 02 Aug 2022 18:35:35 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
# Tue, 02 Aug 2022 18:35:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 02 Aug 2022 18:35:58 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 02 Aug 2022 18:35:59 GMT
VOLUME [/var/lib/mysql]
# Tue, 02 Aug 2022 18:36:00 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 02 Aug 2022 18:36:01 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 02 Aug 2022 18:36:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 18:36:02 GMT
EXPOSE 3306
# Tue, 02 Aug 2022 18:36:03 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:a749a280e3e905de447c3d95a39e8aa1ede5835a6eadeb0c11596051592b675b`  
		Last Modified: Tue, 02 Aug 2022 01:20:32 GMT  
		Size: 27.2 MB (27191804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7d70702fc52aefacc8ccbff1968c3548d6400deb5e6c53d75f6dbc14905cb7`  
		Last Modified: Tue, 02 Aug 2022 18:42:44 GMT  
		Size: 1.7 KB (1722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9ffe290feb53a390aea694e16a663c4a420a71b1ebcd8053b07a44579782bbe`  
		Last Modified: Tue, 02 Aug 2022 18:42:44 GMT  
		Size: 5.3 MB (5321787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a430076265be6d7113b835ac1ab3e08dab46e41fff7e3ed070286125f1dbf6d`  
		Last Modified: Tue, 02 Aug 2022 18:42:43 GMT  
		Size: 3.4 MB (3367877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c880491c15580752404cccf2db4534a2d79f5b5cd1df18b3f6ea2754809020`  
		Last Modified: Tue, 02 Aug 2022 18:42:42 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ca8382cebf14e057456cd5ec8096f0053cdfe6029503875b74003df35d8c5e`  
		Last Modified: Tue, 02 Aug 2022 18:42:43 GMT  
		Size: 2.2 MB (2203204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88502488cc76b679835db628ad4d0f65e09a69018881918c6765cfb9e071feed`  
		Last Modified: Tue, 02 Aug 2022 18:42:40 GMT  
		Size: 2.5 KB (2466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae7307cb02fdd519b5d7db3c1f30d412779b83c0f83d4a7f158dc041a6b04a3`  
		Last Modified: Tue, 02 Aug 2022 18:43:13 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df60df6710cca87a5d1e1be55009d96bcfee6713469124932f98d485d5ab8199`  
		Last Modified: Tue, 02 Aug 2022 18:43:26 GMT  
		Size: 87.3 MB (87324673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb82d118ee8fca5b9a0db692402b5f23e230f67088b3b572096a838a27218041`  
		Last Modified: Tue, 02 Aug 2022 18:43:13 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce2f3952ce52f25a2e27142678fb9c50087932d4ae71476b13f8728b0a42ef9`  
		Last Modified: Tue, 02 Aug 2022 18:43:13 GMT  
		Size: 6.7 KB (6696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:1b11d8c12a5364e8dc7e704047ff4e7577640062c67babd074eeeff198f0415b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.0 MB (139025283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b277eeb3a1cc241eefca94775f59fc06b461e3bce4060bd3f22ad0bad7c1f668`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 02 Aug 2022 01:31:01 GMT
ADD file:75dd7889d4feb83b8504153b5ea6873e4ab0e616a4f4489ea81fd055b6ce9def in / 
# Tue, 02 Aug 2022 01:31:03 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 04:33:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 03 Aug 2022 04:34:01 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 04:34:01 GMT
ENV GOSU_VERSION=1.14
# Wed, 03 Aug 2022 04:34:21 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 03 Aug 2022 04:34:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 03 Aug 2022 04:34:35 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 04:34:36 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 03 Aug 2022 04:34:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 03 Aug 2022 04:35:52 GMT
ARG MARIADB_MAJOR=10.6
# Wed, 03 Aug 2022 04:35:53 GMT
ENV MARIADB_MAJOR=10.6
# Wed, 03 Aug 2022 04:35:53 GMT
ARG MARIADB_VERSION=1:10.6.8+maria~focal
# Wed, 03 Aug 2022 04:35:53 GMT
ENV MARIADB_VERSION=1:10.6.8+maria~focal
# Wed, 03 Aug 2022 04:35:54 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
# Wed, 03 Aug 2022 04:35:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 03 Aug 2022 04:36:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 03 Aug 2022 04:36:40 GMT
VOLUME [/var/lib/mysql]
# Wed, 03 Aug 2022 04:36:41 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Wed, 03 Aug 2022 04:36:41 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Wed, 03 Aug 2022 04:36:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 Aug 2022 04:36:42 GMT
EXPOSE 3306
# Wed, 03 Aug 2022 04:36:42 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:bf47d2be67f1a301865e78e8f78cc69c55dcc389921b4ba187dc0d333cbfd63b`  
		Last Modified: Tue, 02 Aug 2022 01:33:30 GMT  
		Size: 33.3 MB (33295352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b481bc43c771217829dcc78384d81402be7256c3fabe0fb95c0ad844e20eb486`  
		Last Modified: Wed, 03 Aug 2022 04:45:28 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f8f9934029ad30c4038aaa2505d3a55f09535b0f6cd3d115b622277ee43eec`  
		Last Modified: Wed, 03 Aug 2022 04:45:27 GMT  
		Size: 6.7 MB (6667750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ad8421e507f31703a57b5fcf441a19386060096de9f2d97716b6d1c03dd390`  
		Last Modified: Wed, 03 Aug 2022 04:45:27 GMT  
		Size: 3.7 MB (3669923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24953c586f1b7badf3268c6b00564095704918a0365c13b4d332008db8618e69`  
		Last Modified: Wed, 03 Aug 2022 04:45:25 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f4f22aaf2d7b83971e812c7422c924063814a37e635a032244e2b206911101b`  
		Last Modified: Wed, 03 Aug 2022 04:45:26 GMT  
		Size: 2.6 MB (2568638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57859f236e7f0146b0e787f561dafcb5fe2f724613fb2364c182a5ca2018030`  
		Last Modified: Wed, 03 Aug 2022 04:45:23 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1abb7ca0778f18b6321d931ce6b922a2597450e921a7345216b6473947d61aa2`  
		Last Modified: Wed, 03 Aug 2022 04:46:10 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc412d1dc0bad051399c592960e71e3690338616e4b6837c9c4792c890b92f3`  
		Last Modified: Wed, 03 Aug 2022 04:46:34 GMT  
		Size: 92.8 MB (92808710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e762fc6deb17e2e3a2f41f857174cd04d2062dec645edd6efc8e0dd2e6d5bee9`  
		Last Modified: Wed, 03 Aug 2022 04:46:10 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:935e3244bde1b7941807c2a93114cf1aa5ed34459f44d8e683c92c0a0c6bc3c2`  
		Last Modified: Wed, 03 Aug 2022 04:46:10 GMT  
		Size: 6.7 KB (6699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:094d648428e889a5d9c2ec1a3756d661d9ad52bd8031deda97d60a49bc4b426c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.4 MB (127357754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9c987c87b7d4a6f5b9ee4b7498186d1a6d5be62b3caa938ed66682c7a60c513`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 02 Aug 2022 01:02:06 GMT
ADD file:409a01624b482522ab1ba2da28ff57bceb3bf89ff2f3cae5c9ea6068f6993355 in / 
# Tue, 02 Aug 2022 01:02:08 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 12:57:51 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 02 Aug 2022 12:58:02 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 12:58:02 GMT
ENV GOSU_VERSION=1.14
# Tue, 02 Aug 2022 12:58:10 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 02 Aug 2022 12:58:11 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 02 Aug 2022 12:58:16 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 12:58:16 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 02 Aug 2022 12:58:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 02 Aug 2022 12:58:59 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 02 Aug 2022 12:58:59 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 02 Aug 2022 12:58:59 GMT
ARG MARIADB_VERSION=1:10.6.8+maria~focal
# Tue, 02 Aug 2022 12:59:00 GMT
ENV MARIADB_VERSION=1:10.6.8+maria~focal
# Tue, 02 Aug 2022 12:59:00 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
# Tue, 02 Aug 2022 12:59:01 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 02 Aug 2022 12:59:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 02 Aug 2022 12:59:25 GMT
VOLUME [/var/lib/mysql]
# Tue, 02 Aug 2022 12:59:25 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 02 Aug 2022 12:59:25 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 02 Aug 2022 12:59:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 12:59:26 GMT
EXPOSE 3306
# Tue, 02 Aug 2022 12:59:26 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d522b75fb69271e75617d2e7bbeede1210f48bffdc57121ee39534eea94e2815`  
		Last Modified: Tue, 02 Aug 2022 01:03:38 GMT  
		Size: 27.0 MB (27045363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b542230411fae56efa86753d30f5439f912d60eabb26102f6570d97473c7573`  
		Last Modified: Tue, 02 Aug 2022 13:01:52 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9116cff82c5514acc6d105cb940a79d66cc9ca17bc78527c303509b2dbc6f095`  
		Last Modified: Tue, 02 Aug 2022 13:01:51 GMT  
		Size: 5.4 MB (5372728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9de0756f9486981018019372396743263fc5ff93d3aefa2ad557cc5b3307689f`  
		Last Modified: Tue, 02 Aug 2022 13:01:51 GMT  
		Size: 3.2 MB (3240183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff661c0d7c1d54aca25ce7155b5446f9e7b2a43a4db6a70bd1876da78b06b98e`  
		Last Modified: Tue, 02 Aug 2022 13:01:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7962d6c3604efb9aeed7adbc9fa294d45741fc8843c76a1b0acda6b306208b6a`  
		Last Modified: Tue, 02 Aug 2022 13:01:51 GMT  
		Size: 2.2 MB (2183826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0834a13ee0d34f33d37fdf14c52e61904a4660c0154507ec87a01ddb58423a71`  
		Last Modified: Tue, 02 Aug 2022 13:01:49 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48fab4697854f490148d65832aecd4d5d470753f99ebd7dab895f806018820f`  
		Last Modified: Tue, 02 Aug 2022 13:02:16 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a73aff9544f2af693ce068da60e28265aeeb78562d2739d4aa7e00fe2173b3`  
		Last Modified: Tue, 02 Aug 2022 13:02:28 GMT  
		Size: 89.5 MB (89500752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e51ebb9416afd45bfdef43a83663ded70bee363c22a4ef0083374329fa41e975`  
		Last Modified: Tue, 02 Aug 2022 13:02:16 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f50ac00fe5226cde100ea6dfcf7a108cfc585c6d4518846593333e9cdbe6c46`  
		Last Modified: Tue, 02 Aug 2022 13:02:16 GMT  
		Size: 6.7 KB (6697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.6.9`

**does not exist** (yet?)

## `mariadb:10.6.9-focal`

**does not exist** (yet?)

## `mariadb:10.7`

```console
$ docker pull mariadb@sha256:370a54b7c77d7bc9660782c5cba4c629e704558d9eb3a5fc364d60942e470039
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.7` - linux; amd64

```console
$ docker pull mariadb@sha256:c26e88939772f09fa0f6a504937edd13a039ff90d35f9a88111cbb4ca6bc2fbf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.8 MB (128818595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2981a583f839d7c2fbc47fe026ee6474fc18235cc32013a4f90b1449d32fd6d2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:49 GMT
ADD file:af4cf77e6818016b697a1491101b40c71d06529ced65f36107749f099d6d4bdc in / 
# Tue, 02 Aug 2022 01:30:49 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 20:21:24 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 02 Aug 2022 20:21:32 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 20:21:32 GMT
ENV GOSU_VERSION=1.14
# Tue, 02 Aug 2022 20:21:42 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 02 Aug 2022 20:21:42 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 02 Aug 2022 20:21:49 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 20:21:49 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 02 Aug 2022 20:21:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 02 Aug 2022 20:21:51 GMT
ARG MARIADB_MAJOR=10.7
# Tue, 02 Aug 2022 20:21:51 GMT
ENV MARIADB_MAJOR=10.7
# Tue, 02 Aug 2022 20:21:51 GMT
ARG MARIADB_VERSION=1:10.7.4+maria~focal
# Tue, 02 Aug 2022 20:21:51 GMT
ENV MARIADB_VERSION=1:10.7.4+maria~focal
# Tue, 02 Aug 2022 20:21:51 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
# Tue, 02 Aug 2022 20:21:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 02 Aug 2022 20:22:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 02 Aug 2022 20:22:25 GMT
VOLUME [/var/lib/mysql]
# Tue, 02 Aug 2022 20:22:25 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 02 Aug 2022 20:22:25 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 02 Aug 2022 20:22:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 20:22:25 GMT
EXPOSE 3306
# Tue, 02 Aug 2022 20:22:25 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:3b65ec22a9e96affe680712973e88355927506aa3f792ff03330f3a3eb601a98`  
		Last Modified: Tue, 02 Aug 2022 01:31:59 GMT  
		Size: 28.6 MB (28572596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d19669910bc06b914ac5d4512b9aa15623df49e4ef03d20277f4a8fda0cf5631`  
		Last Modified: Tue, 02 Aug 2022 20:27:42 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c46f5717c584782c1a1498020ed1354006c97d58cb69a3607a17e1e0023da0e`  
		Last Modified: Tue, 02 Aug 2022 20:27:40 GMT  
		Size: 5.5 MB (5488983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea0278d54bb37ba2adf21e281d933e45b7c110f62e93e95b27c88940599003a1`  
		Last Modified: Tue, 02 Aug 2022 20:27:40 GMT  
		Size: 3.6 MB (3581823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80813ba5cb6ef218fb6cb3a25b964d31f0cd372ca1c2427c140d587a5a74a13`  
		Last Modified: Tue, 02 Aug 2022 20:27:39 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc4ac948168b66da6b55897167508489a2ab555945d5030db3362f06b232c51`  
		Last Modified: Tue, 02 Aug 2022 20:27:40 GMT  
		Size: 2.3 MB (2272442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d65facec905da8f0741a9561cf142ab88af72c392c88ab6d32c630704907f642`  
		Last Modified: Tue, 02 Aug 2022 20:27:37 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358251aad8e5836a9ee090af455dc61f72ecf817cfcf45e95e8cb0996dec80fe`  
		Last Modified: Tue, 02 Aug 2022 20:27:37 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554f622363d579cadd3d18cd0ec71a57856a84f51155b503098e17e4f908e191`  
		Last Modified: Tue, 02 Aug 2022 20:27:52 GMT  
		Size: 88.9 MB (88887851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88ee10923f3d04fbb7ea23436666c985b73ada0ef38aee7d4f307fd921d4f31`  
		Last Modified: Tue, 02 Aug 2022 20:27:37 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:067d457acefca730ab83a23a44203996aa51407e601f01141b662619d7a14bf2`  
		Last Modified: Tue, 02 Aug 2022 20:27:37 GMT  
		Size: 6.7 KB (6696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:4f5af175bc868d273bf03b138dd75c7299b5f33cd5789b5c4fc2798fab2ff753
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.9 MB (125907158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f873d0c6cf12bfd2b3f5d8e9d839d07115a3ba465664129691aceb82895ae343`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:51 GMT
ADD file:151548d1bfac57d762f2c0b18b2378c363ffd1568da9fecd4be611db4832e8e2 in / 
# Tue, 02 Aug 2022 01:18:51 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 18:34:06 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 02 Aug 2022 18:34:17 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 18:34:18 GMT
ENV GOSU_VERSION=1.14
# Tue, 02 Aug 2022 18:34:33 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 02 Aug 2022 18:34:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 02 Aug 2022 18:34:42 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 18:34:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 02 Aug 2022 18:34:45 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 02 Aug 2022 18:34:46 GMT
ARG MARIADB_MAJOR=10.7
# Tue, 02 Aug 2022 18:34:47 GMT
ENV MARIADB_MAJOR=10.7
# Tue, 02 Aug 2022 18:34:48 GMT
ARG MARIADB_VERSION=1:10.7.4+maria~focal
# Tue, 02 Aug 2022 18:34:49 GMT
ENV MARIADB_VERSION=1:10.7.4+maria~focal
# Tue, 02 Aug 2022 18:34:50 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
# Tue, 02 Aug 2022 18:34:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 02 Aug 2022 18:35:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 02 Aug 2022 18:35:14 GMT
VOLUME [/var/lib/mysql]
# Tue, 02 Aug 2022 18:35:16 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 02 Aug 2022 18:35:17 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 02 Aug 2022 18:35:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 18:35:18 GMT
EXPOSE 3306
# Tue, 02 Aug 2022 18:35:19 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:a749a280e3e905de447c3d95a39e8aa1ede5835a6eadeb0c11596051592b675b`  
		Last Modified: Tue, 02 Aug 2022 01:20:32 GMT  
		Size: 27.2 MB (27191804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7d70702fc52aefacc8ccbff1968c3548d6400deb5e6c53d75f6dbc14905cb7`  
		Last Modified: Tue, 02 Aug 2022 18:42:44 GMT  
		Size: 1.7 KB (1722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9ffe290feb53a390aea694e16a663c4a420a71b1ebcd8053b07a44579782bbe`  
		Last Modified: Tue, 02 Aug 2022 18:42:44 GMT  
		Size: 5.3 MB (5321787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a430076265be6d7113b835ac1ab3e08dab46e41fff7e3ed070286125f1dbf6d`  
		Last Modified: Tue, 02 Aug 2022 18:42:43 GMT  
		Size: 3.4 MB (3367877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c880491c15580752404cccf2db4534a2d79f5b5cd1df18b3f6ea2754809020`  
		Last Modified: Tue, 02 Aug 2022 18:42:42 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ca8382cebf14e057456cd5ec8096f0053cdfe6029503875b74003df35d8c5e`  
		Last Modified: Tue, 02 Aug 2022 18:42:43 GMT  
		Size: 2.2 MB (2203204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88502488cc76b679835db628ad4d0f65e09a69018881918c6765cfb9e071feed`  
		Last Modified: Tue, 02 Aug 2022 18:42:40 GMT  
		Size: 2.5 KB (2466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9de3bd4d6fac28344afff3704daa788ce9fb41f278768ad4628667013073f385`  
		Last Modified: Tue, 02 Aug 2022 18:42:40 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a757a0c4be796915a937cf877cfd9b2c286ec749d6069fd498ad56d6c1fc6f`  
		Last Modified: Tue, 02 Aug 2022 18:42:54 GMT  
		Size: 87.8 MB (87807667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faef2ca41942f4d6ff9406a58ca9a1109a04ce810b4081eb3da6f765b1241da7`  
		Last Modified: Tue, 02 Aug 2022 18:42:40 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3da936e34985dde60992a2acbf865e29dee94677edd25978ca769aa6a25a367`  
		Last Modified: Tue, 02 Aug 2022 18:42:40 GMT  
		Size: 6.7 KB (6698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7` - linux; ppc64le

```console
$ docker pull mariadb@sha256:4a664560afa32d0b3a1fed826eb28b69888019c26695a43b94683da7dbc73308
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.7 MB (139736107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0dc97925b9f1616d888aae7c2a9ba53e01c9a356b7c76fc5fde5a88f23deb77a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 02 Aug 2022 01:31:01 GMT
ADD file:75dd7889d4feb83b8504153b5ea6873e4ab0e616a4f4489ea81fd055b6ce9def in / 
# Tue, 02 Aug 2022 01:31:03 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 04:33:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 03 Aug 2022 04:34:01 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 04:34:01 GMT
ENV GOSU_VERSION=1.14
# Wed, 03 Aug 2022 04:34:21 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 03 Aug 2022 04:34:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 03 Aug 2022 04:34:35 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 04:34:36 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 03 Aug 2022 04:34:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 03 Aug 2022 04:34:38 GMT
ARG MARIADB_MAJOR=10.7
# Wed, 03 Aug 2022 04:34:38 GMT
ENV MARIADB_MAJOR=10.7
# Wed, 03 Aug 2022 04:34:39 GMT
ARG MARIADB_VERSION=1:10.7.4+maria~focal
# Wed, 03 Aug 2022 04:34:39 GMT
ENV MARIADB_VERSION=1:10.7.4+maria~focal
# Wed, 03 Aug 2022 04:34:39 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
# Wed, 03 Aug 2022 04:34:40 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 03 Aug 2022 04:35:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 03 Aug 2022 04:35:44 GMT
VOLUME [/var/lib/mysql]
# Wed, 03 Aug 2022 04:35:45 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Wed, 03 Aug 2022 04:35:45 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Wed, 03 Aug 2022 04:35:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 Aug 2022 04:35:46 GMT
EXPOSE 3306
# Wed, 03 Aug 2022 04:35:46 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:bf47d2be67f1a301865e78e8f78cc69c55dcc389921b4ba187dc0d333cbfd63b`  
		Last Modified: Tue, 02 Aug 2022 01:33:30 GMT  
		Size: 33.3 MB (33295352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b481bc43c771217829dcc78384d81402be7256c3fabe0fb95c0ad844e20eb486`  
		Last Modified: Wed, 03 Aug 2022 04:45:28 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f8f9934029ad30c4038aaa2505d3a55f09535b0f6cd3d115b622277ee43eec`  
		Last Modified: Wed, 03 Aug 2022 04:45:27 GMT  
		Size: 6.7 MB (6667750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ad8421e507f31703a57b5fcf441a19386060096de9f2d97716b6d1c03dd390`  
		Last Modified: Wed, 03 Aug 2022 04:45:27 GMT  
		Size: 3.7 MB (3669923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24953c586f1b7badf3268c6b00564095704918a0365c13b4d332008db8618e69`  
		Last Modified: Wed, 03 Aug 2022 04:45:25 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f4f22aaf2d7b83971e812c7422c924063814a37e635a032244e2b206911101b`  
		Last Modified: Wed, 03 Aug 2022 04:45:26 GMT  
		Size: 2.6 MB (2568638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57859f236e7f0146b0e787f561dafcb5fe2f724613fb2364c182a5ca2018030`  
		Last Modified: Wed, 03 Aug 2022 04:45:23 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:061b00b4877a36fd987606f01d61263f942d14c09d8bdc2010c5aa7c91d79a00`  
		Last Modified: Wed, 03 Aug 2022 04:45:23 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd31762f95f0d2de05ec7925929fd82a98b77a3190cdc441ebb893970cb28603`  
		Last Modified: Wed, 03 Aug 2022 04:45:48 GMT  
		Size: 93.5 MB (93519533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f45f4d591d09f24e8b784ff4c4fc28a88bd658250abbfc3bb018bdf3cc04a24`  
		Last Modified: Wed, 03 Aug 2022 04:45:23 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11fd53028c82cb7c837514ec51d1b120696ca3c29745085d00dfab071ac60256`  
		Last Modified: Wed, 03 Aug 2022 04:45:23 GMT  
		Size: 6.7 KB (6699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7` - linux; s390x

```console
$ docker pull mariadb@sha256:983d4d449de4574b810c778737dce0de76ce4e0b60f65739e31270e76274975c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.9 MB (127858317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7e6065ff0eb69aa1b47d1cf813ee537fad7a2668f6ff282bff8564a41d38e17`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 02 Aug 2022 01:02:06 GMT
ADD file:409a01624b482522ab1ba2da28ff57bceb3bf89ff2f3cae5c9ea6068f6993355 in / 
# Tue, 02 Aug 2022 01:02:08 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 12:57:51 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 02 Aug 2022 12:58:02 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 12:58:02 GMT
ENV GOSU_VERSION=1.14
# Tue, 02 Aug 2022 12:58:10 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 02 Aug 2022 12:58:11 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 02 Aug 2022 12:58:16 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 12:58:16 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 02 Aug 2022 12:58:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 02 Aug 2022 12:58:17 GMT
ARG MARIADB_MAJOR=10.7
# Tue, 02 Aug 2022 12:58:17 GMT
ENV MARIADB_MAJOR=10.7
# Tue, 02 Aug 2022 12:58:17 GMT
ARG MARIADB_VERSION=1:10.7.4+maria~focal
# Tue, 02 Aug 2022 12:58:17 GMT
ENV MARIADB_VERSION=1:10.7.4+maria~focal
# Tue, 02 Aug 2022 12:58:18 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
# Tue, 02 Aug 2022 12:58:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 02 Aug 2022 12:58:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 02 Aug 2022 12:58:51 GMT
VOLUME [/var/lib/mysql]
# Tue, 02 Aug 2022 12:58:51 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 02 Aug 2022 12:58:51 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 02 Aug 2022 12:58:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 12:58:51 GMT
EXPOSE 3306
# Tue, 02 Aug 2022 12:58:51 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d522b75fb69271e75617d2e7bbeede1210f48bffdc57121ee39534eea94e2815`  
		Last Modified: Tue, 02 Aug 2022 01:03:38 GMT  
		Size: 27.0 MB (27045363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b542230411fae56efa86753d30f5439f912d60eabb26102f6570d97473c7573`  
		Last Modified: Tue, 02 Aug 2022 13:01:52 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9116cff82c5514acc6d105cb940a79d66cc9ca17bc78527c303509b2dbc6f095`  
		Last Modified: Tue, 02 Aug 2022 13:01:51 GMT  
		Size: 5.4 MB (5372728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9de0756f9486981018019372396743263fc5ff93d3aefa2ad557cc5b3307689f`  
		Last Modified: Tue, 02 Aug 2022 13:01:51 GMT  
		Size: 3.2 MB (3240183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff661c0d7c1d54aca25ce7155b5446f9e7b2a43a4db6a70bd1876da78b06b98e`  
		Last Modified: Tue, 02 Aug 2022 13:01:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7962d6c3604efb9aeed7adbc9fa294d45741fc8843c76a1b0acda6b306208b6a`  
		Last Modified: Tue, 02 Aug 2022 13:01:51 GMT  
		Size: 2.2 MB (2183826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0834a13ee0d34f33d37fdf14c52e61904a4660c0154507ec87a01ddb58423a71`  
		Last Modified: Tue, 02 Aug 2022 13:01:49 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f66369d5a4c009ebe9246d8a133104f8420008a6bd6316b490347cac7a3d7d`  
		Last Modified: Tue, 02 Aug 2022 13:01:50 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131afc7827c69d5c869c428b98c50114e61ea0bf33fd5b0a7c18dacdd8b69b41`  
		Last Modified: Tue, 02 Aug 2022 13:02:05 GMT  
		Size: 90.0 MB (90001314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e38955428ecef9bb56078bbd9c2ce76420b37f4255ceb8ed9f251442cf6f3397`  
		Last Modified: Tue, 02 Aug 2022 13:01:49 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6748802bc4fb1e547708f66b1ca51b3e56149e9a9afe01a5e11d6e4fd9186fd8`  
		Last Modified: Tue, 02 Aug 2022 13:01:49 GMT  
		Size: 6.7 KB (6698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.7-focal`

```console
$ docker pull mariadb@sha256:370a54b7c77d7bc9660782c5cba4c629e704558d9eb3a5fc364d60942e470039
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.7-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:c26e88939772f09fa0f6a504937edd13a039ff90d35f9a88111cbb4ca6bc2fbf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.8 MB (128818595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2981a583f839d7c2fbc47fe026ee6474fc18235cc32013a4f90b1449d32fd6d2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:49 GMT
ADD file:af4cf77e6818016b697a1491101b40c71d06529ced65f36107749f099d6d4bdc in / 
# Tue, 02 Aug 2022 01:30:49 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 20:21:24 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 02 Aug 2022 20:21:32 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 20:21:32 GMT
ENV GOSU_VERSION=1.14
# Tue, 02 Aug 2022 20:21:42 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 02 Aug 2022 20:21:42 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 02 Aug 2022 20:21:49 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 20:21:49 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 02 Aug 2022 20:21:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 02 Aug 2022 20:21:51 GMT
ARG MARIADB_MAJOR=10.7
# Tue, 02 Aug 2022 20:21:51 GMT
ENV MARIADB_MAJOR=10.7
# Tue, 02 Aug 2022 20:21:51 GMT
ARG MARIADB_VERSION=1:10.7.4+maria~focal
# Tue, 02 Aug 2022 20:21:51 GMT
ENV MARIADB_VERSION=1:10.7.4+maria~focal
# Tue, 02 Aug 2022 20:21:51 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
# Tue, 02 Aug 2022 20:21:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 02 Aug 2022 20:22:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 02 Aug 2022 20:22:25 GMT
VOLUME [/var/lib/mysql]
# Tue, 02 Aug 2022 20:22:25 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 02 Aug 2022 20:22:25 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 02 Aug 2022 20:22:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 20:22:25 GMT
EXPOSE 3306
# Tue, 02 Aug 2022 20:22:25 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:3b65ec22a9e96affe680712973e88355927506aa3f792ff03330f3a3eb601a98`  
		Last Modified: Tue, 02 Aug 2022 01:31:59 GMT  
		Size: 28.6 MB (28572596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d19669910bc06b914ac5d4512b9aa15623df49e4ef03d20277f4a8fda0cf5631`  
		Last Modified: Tue, 02 Aug 2022 20:27:42 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c46f5717c584782c1a1498020ed1354006c97d58cb69a3607a17e1e0023da0e`  
		Last Modified: Tue, 02 Aug 2022 20:27:40 GMT  
		Size: 5.5 MB (5488983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea0278d54bb37ba2adf21e281d933e45b7c110f62e93e95b27c88940599003a1`  
		Last Modified: Tue, 02 Aug 2022 20:27:40 GMT  
		Size: 3.6 MB (3581823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80813ba5cb6ef218fb6cb3a25b964d31f0cd372ca1c2427c140d587a5a74a13`  
		Last Modified: Tue, 02 Aug 2022 20:27:39 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc4ac948168b66da6b55897167508489a2ab555945d5030db3362f06b232c51`  
		Last Modified: Tue, 02 Aug 2022 20:27:40 GMT  
		Size: 2.3 MB (2272442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d65facec905da8f0741a9561cf142ab88af72c392c88ab6d32c630704907f642`  
		Last Modified: Tue, 02 Aug 2022 20:27:37 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358251aad8e5836a9ee090af455dc61f72ecf817cfcf45e95e8cb0996dec80fe`  
		Last Modified: Tue, 02 Aug 2022 20:27:37 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554f622363d579cadd3d18cd0ec71a57856a84f51155b503098e17e4f908e191`  
		Last Modified: Tue, 02 Aug 2022 20:27:52 GMT  
		Size: 88.9 MB (88887851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88ee10923f3d04fbb7ea23436666c985b73ada0ef38aee7d4f307fd921d4f31`  
		Last Modified: Tue, 02 Aug 2022 20:27:37 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:067d457acefca730ab83a23a44203996aa51407e601f01141b662619d7a14bf2`  
		Last Modified: Tue, 02 Aug 2022 20:27:37 GMT  
		Size: 6.7 KB (6696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:4f5af175bc868d273bf03b138dd75c7299b5f33cd5789b5c4fc2798fab2ff753
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.9 MB (125907158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f873d0c6cf12bfd2b3f5d8e9d839d07115a3ba465664129691aceb82895ae343`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:51 GMT
ADD file:151548d1bfac57d762f2c0b18b2378c363ffd1568da9fecd4be611db4832e8e2 in / 
# Tue, 02 Aug 2022 01:18:51 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 18:34:06 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 02 Aug 2022 18:34:17 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 18:34:18 GMT
ENV GOSU_VERSION=1.14
# Tue, 02 Aug 2022 18:34:33 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 02 Aug 2022 18:34:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 02 Aug 2022 18:34:42 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 18:34:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 02 Aug 2022 18:34:45 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 02 Aug 2022 18:34:46 GMT
ARG MARIADB_MAJOR=10.7
# Tue, 02 Aug 2022 18:34:47 GMT
ENV MARIADB_MAJOR=10.7
# Tue, 02 Aug 2022 18:34:48 GMT
ARG MARIADB_VERSION=1:10.7.4+maria~focal
# Tue, 02 Aug 2022 18:34:49 GMT
ENV MARIADB_VERSION=1:10.7.4+maria~focal
# Tue, 02 Aug 2022 18:34:50 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
# Tue, 02 Aug 2022 18:34:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 02 Aug 2022 18:35:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 02 Aug 2022 18:35:14 GMT
VOLUME [/var/lib/mysql]
# Tue, 02 Aug 2022 18:35:16 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 02 Aug 2022 18:35:17 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 02 Aug 2022 18:35:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 18:35:18 GMT
EXPOSE 3306
# Tue, 02 Aug 2022 18:35:19 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:a749a280e3e905de447c3d95a39e8aa1ede5835a6eadeb0c11596051592b675b`  
		Last Modified: Tue, 02 Aug 2022 01:20:32 GMT  
		Size: 27.2 MB (27191804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7d70702fc52aefacc8ccbff1968c3548d6400deb5e6c53d75f6dbc14905cb7`  
		Last Modified: Tue, 02 Aug 2022 18:42:44 GMT  
		Size: 1.7 KB (1722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9ffe290feb53a390aea694e16a663c4a420a71b1ebcd8053b07a44579782bbe`  
		Last Modified: Tue, 02 Aug 2022 18:42:44 GMT  
		Size: 5.3 MB (5321787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a430076265be6d7113b835ac1ab3e08dab46e41fff7e3ed070286125f1dbf6d`  
		Last Modified: Tue, 02 Aug 2022 18:42:43 GMT  
		Size: 3.4 MB (3367877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c880491c15580752404cccf2db4534a2d79f5b5cd1df18b3f6ea2754809020`  
		Last Modified: Tue, 02 Aug 2022 18:42:42 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ca8382cebf14e057456cd5ec8096f0053cdfe6029503875b74003df35d8c5e`  
		Last Modified: Tue, 02 Aug 2022 18:42:43 GMT  
		Size: 2.2 MB (2203204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88502488cc76b679835db628ad4d0f65e09a69018881918c6765cfb9e071feed`  
		Last Modified: Tue, 02 Aug 2022 18:42:40 GMT  
		Size: 2.5 KB (2466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9de3bd4d6fac28344afff3704daa788ce9fb41f278768ad4628667013073f385`  
		Last Modified: Tue, 02 Aug 2022 18:42:40 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a757a0c4be796915a937cf877cfd9b2c286ec749d6069fd498ad56d6c1fc6f`  
		Last Modified: Tue, 02 Aug 2022 18:42:54 GMT  
		Size: 87.8 MB (87807667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faef2ca41942f4d6ff9406a58ca9a1109a04ce810b4081eb3da6f765b1241da7`  
		Last Modified: Tue, 02 Aug 2022 18:42:40 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3da936e34985dde60992a2acbf865e29dee94677edd25978ca769aa6a25a367`  
		Last Modified: Tue, 02 Aug 2022 18:42:40 GMT  
		Size: 6.7 KB (6698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:4a664560afa32d0b3a1fed826eb28b69888019c26695a43b94683da7dbc73308
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.7 MB (139736107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0dc97925b9f1616d888aae7c2a9ba53e01c9a356b7c76fc5fde5a88f23deb77a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 02 Aug 2022 01:31:01 GMT
ADD file:75dd7889d4feb83b8504153b5ea6873e4ab0e616a4f4489ea81fd055b6ce9def in / 
# Tue, 02 Aug 2022 01:31:03 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 04:33:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 03 Aug 2022 04:34:01 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 04:34:01 GMT
ENV GOSU_VERSION=1.14
# Wed, 03 Aug 2022 04:34:21 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 03 Aug 2022 04:34:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 03 Aug 2022 04:34:35 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 04:34:36 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 03 Aug 2022 04:34:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 03 Aug 2022 04:34:38 GMT
ARG MARIADB_MAJOR=10.7
# Wed, 03 Aug 2022 04:34:38 GMT
ENV MARIADB_MAJOR=10.7
# Wed, 03 Aug 2022 04:34:39 GMT
ARG MARIADB_VERSION=1:10.7.4+maria~focal
# Wed, 03 Aug 2022 04:34:39 GMT
ENV MARIADB_VERSION=1:10.7.4+maria~focal
# Wed, 03 Aug 2022 04:34:39 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
# Wed, 03 Aug 2022 04:34:40 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 03 Aug 2022 04:35:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 03 Aug 2022 04:35:44 GMT
VOLUME [/var/lib/mysql]
# Wed, 03 Aug 2022 04:35:45 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Wed, 03 Aug 2022 04:35:45 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Wed, 03 Aug 2022 04:35:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 Aug 2022 04:35:46 GMT
EXPOSE 3306
# Wed, 03 Aug 2022 04:35:46 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:bf47d2be67f1a301865e78e8f78cc69c55dcc389921b4ba187dc0d333cbfd63b`  
		Last Modified: Tue, 02 Aug 2022 01:33:30 GMT  
		Size: 33.3 MB (33295352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b481bc43c771217829dcc78384d81402be7256c3fabe0fb95c0ad844e20eb486`  
		Last Modified: Wed, 03 Aug 2022 04:45:28 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f8f9934029ad30c4038aaa2505d3a55f09535b0f6cd3d115b622277ee43eec`  
		Last Modified: Wed, 03 Aug 2022 04:45:27 GMT  
		Size: 6.7 MB (6667750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ad8421e507f31703a57b5fcf441a19386060096de9f2d97716b6d1c03dd390`  
		Last Modified: Wed, 03 Aug 2022 04:45:27 GMT  
		Size: 3.7 MB (3669923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24953c586f1b7badf3268c6b00564095704918a0365c13b4d332008db8618e69`  
		Last Modified: Wed, 03 Aug 2022 04:45:25 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f4f22aaf2d7b83971e812c7422c924063814a37e635a032244e2b206911101b`  
		Last Modified: Wed, 03 Aug 2022 04:45:26 GMT  
		Size: 2.6 MB (2568638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57859f236e7f0146b0e787f561dafcb5fe2f724613fb2364c182a5ca2018030`  
		Last Modified: Wed, 03 Aug 2022 04:45:23 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:061b00b4877a36fd987606f01d61263f942d14c09d8bdc2010c5aa7c91d79a00`  
		Last Modified: Wed, 03 Aug 2022 04:45:23 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd31762f95f0d2de05ec7925929fd82a98b77a3190cdc441ebb893970cb28603`  
		Last Modified: Wed, 03 Aug 2022 04:45:48 GMT  
		Size: 93.5 MB (93519533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f45f4d591d09f24e8b784ff4c4fc28a88bd658250abbfc3bb018bdf3cc04a24`  
		Last Modified: Wed, 03 Aug 2022 04:45:23 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11fd53028c82cb7c837514ec51d1b120696ca3c29745085d00dfab071ac60256`  
		Last Modified: Wed, 03 Aug 2022 04:45:23 GMT  
		Size: 6.7 KB (6699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:983d4d449de4574b810c778737dce0de76ce4e0b60f65739e31270e76274975c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.9 MB (127858317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7e6065ff0eb69aa1b47d1cf813ee537fad7a2668f6ff282bff8564a41d38e17`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 02 Aug 2022 01:02:06 GMT
ADD file:409a01624b482522ab1ba2da28ff57bceb3bf89ff2f3cae5c9ea6068f6993355 in / 
# Tue, 02 Aug 2022 01:02:08 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 12:57:51 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 02 Aug 2022 12:58:02 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 12:58:02 GMT
ENV GOSU_VERSION=1.14
# Tue, 02 Aug 2022 12:58:10 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 02 Aug 2022 12:58:11 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 02 Aug 2022 12:58:16 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 12:58:16 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 02 Aug 2022 12:58:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 02 Aug 2022 12:58:17 GMT
ARG MARIADB_MAJOR=10.7
# Tue, 02 Aug 2022 12:58:17 GMT
ENV MARIADB_MAJOR=10.7
# Tue, 02 Aug 2022 12:58:17 GMT
ARG MARIADB_VERSION=1:10.7.4+maria~focal
# Tue, 02 Aug 2022 12:58:17 GMT
ENV MARIADB_VERSION=1:10.7.4+maria~focal
# Tue, 02 Aug 2022 12:58:18 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
# Tue, 02 Aug 2022 12:58:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 02 Aug 2022 12:58:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 02 Aug 2022 12:58:51 GMT
VOLUME [/var/lib/mysql]
# Tue, 02 Aug 2022 12:58:51 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 02 Aug 2022 12:58:51 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 02 Aug 2022 12:58:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 12:58:51 GMT
EXPOSE 3306
# Tue, 02 Aug 2022 12:58:51 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d522b75fb69271e75617d2e7bbeede1210f48bffdc57121ee39534eea94e2815`  
		Last Modified: Tue, 02 Aug 2022 01:03:38 GMT  
		Size: 27.0 MB (27045363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b542230411fae56efa86753d30f5439f912d60eabb26102f6570d97473c7573`  
		Last Modified: Tue, 02 Aug 2022 13:01:52 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9116cff82c5514acc6d105cb940a79d66cc9ca17bc78527c303509b2dbc6f095`  
		Last Modified: Tue, 02 Aug 2022 13:01:51 GMT  
		Size: 5.4 MB (5372728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9de0756f9486981018019372396743263fc5ff93d3aefa2ad557cc5b3307689f`  
		Last Modified: Tue, 02 Aug 2022 13:01:51 GMT  
		Size: 3.2 MB (3240183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff661c0d7c1d54aca25ce7155b5446f9e7b2a43a4db6a70bd1876da78b06b98e`  
		Last Modified: Tue, 02 Aug 2022 13:01:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7962d6c3604efb9aeed7adbc9fa294d45741fc8843c76a1b0acda6b306208b6a`  
		Last Modified: Tue, 02 Aug 2022 13:01:51 GMT  
		Size: 2.2 MB (2183826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0834a13ee0d34f33d37fdf14c52e61904a4660c0154507ec87a01ddb58423a71`  
		Last Modified: Tue, 02 Aug 2022 13:01:49 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f66369d5a4c009ebe9246d8a133104f8420008a6bd6316b490347cac7a3d7d`  
		Last Modified: Tue, 02 Aug 2022 13:01:50 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131afc7827c69d5c869c428b98c50114e61ea0bf33fd5b0a7c18dacdd8b69b41`  
		Last Modified: Tue, 02 Aug 2022 13:02:05 GMT  
		Size: 90.0 MB (90001314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e38955428ecef9bb56078bbd9c2ce76420b37f4255ceb8ed9f251442cf6f3397`  
		Last Modified: Tue, 02 Aug 2022 13:01:49 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6748802bc4fb1e547708f66b1ca51b3e56149e9a9afe01a5e11d6e4fd9186fd8`  
		Last Modified: Tue, 02 Aug 2022 13:01:49 GMT  
		Size: 6.7 KB (6698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.7.5`

**does not exist** (yet?)

## `mariadb:10.7.5-focal`

**does not exist** (yet?)

## `mariadb:10.8`

```console
$ docker pull mariadb@sha256:0abf60f81588662e716c27c7f1b54a72b3bf879e0ca88fc393e1741970ec7f3f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.8` - linux; amd64

```console
$ docker pull mariadb@sha256:0a6ed934c1518abff64ed856b06f44006b4498b115941e19bbd910bd62a12232
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.9 MB (123908351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40b966d7252f541b41677fc35f8660fa90d14df0f33edc8085e6ca2dc0c5b247`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:55 GMT
ADD file:396eeb65c8d737180cc1219713cf59efb214027b79d8ea0b7e58a08e7c8d7a21 in / 
# Tue, 02 Aug 2022 01:30:56 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 20:19:21 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 02 Aug 2022 20:19:39 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 20:19:40 GMT
ENV GOSU_VERSION=1.14
# Tue, 02 Aug 2022 20:19:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 02 Aug 2022 20:19:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 02 Aug 2022 20:19:58 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 20:19:58 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 02 Aug 2022 20:19:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 02 Aug 2022 20:20:59 GMT
ARG MARIADB_MAJOR=10.8
# Tue, 02 Aug 2022 20:20:59 GMT
ENV MARIADB_MAJOR=10.8
# Tue, 02 Aug 2022 20:20:59 GMT
ARG MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 02 Aug 2022 20:20:59 GMT
ENV MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 02 Aug 2022 20:20:59 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
# Tue, 02 Aug 2022 20:21:00 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 02 Aug 2022 20:21:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 02 Aug 2022 20:21:19 GMT
VOLUME [/var/lib/mysql]
# Tue, 02 Aug 2022 20:21:19 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 02 Aug 2022 20:21:19 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 02 Aug 2022 20:21:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 20:21:20 GMT
EXPOSE 3306
# Tue, 02 Aug 2022 20:21:20 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d19f32bd9e4106d487f1a703fc2f09c8edadd92db4405d477978e8e466ab290d`  
		Last Modified: Tue, 02 Aug 2022 01:32:15 GMT  
		Size: 30.4 MB (30426136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f587559f9b58dcc08ed5b9fc08cc82b80ce995a37000098b1cdca2c199ae89f8`  
		Last Modified: Tue, 02 Aug 2022 20:26:32 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb060f92f2fef90ded1edd0a8c0609f95d414c40ff3684d1189beffa353f88b`  
		Last Modified: Tue, 02 Aug 2022 20:26:31 GMT  
		Size: 3.8 MB (3765797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27513e1f7a1e0c1c4f6197df108bf04d451bddf1da7bbdace8285098ba5dcf50`  
		Last Modified: Tue, 02 Aug 2022 20:26:31 GMT  
		Size: 2.0 MB (1992883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a84d3c510baac7a944c9669fc71e613930f5ca9c87cf616eeb06d2aa7c1917e`  
		Last Modified: Tue, 02 Aug 2022 20:26:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59731d2805a614a839795e79d61509494c939119e1dd7d76bf0f1b3a5f923c29`  
		Last Modified: Tue, 02 Aug 2022 20:26:31 GMT  
		Size: 2.3 MB (2298176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c008ca4420a867178be129dfe4311ce5ff0fcf8c2933d99ad49a3f0e3079cb3d`  
		Last Modified: Tue, 02 Aug 2022 20:26:28 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc47daf3f5d60b9b18f5ca3f556bc478eb967c997777a87459d43a9aea2fc6f`  
		Last Modified: Tue, 02 Aug 2022 20:26:58 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc547eec2be51eceb698e0766c93b76d55e7457043af4fe44ace5ca82927b1d4`  
		Last Modified: Tue, 02 Aug 2022 20:27:09 GMT  
		Size: 85.4 MB (85410459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bdaf629fe8214124455eb146db774a989c93271e8c3e264ece8ff4af772ea7b`  
		Last Modified: Tue, 02 Aug 2022 20:26:57 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddfbe3e290918fede8f6a3b0123b009178834c861a89c42c8b48075f8f8f420d`  
		Last Modified: Tue, 02 Aug 2022 20:26:58 GMT  
		Size: 6.7 KB (6696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:1f011a0b21919b39058355d972fea445857869ad1f867eb56bd1d274fd969e88
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.5 MB (102470825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3f8da7eeabb6549ac946f2b45ffe497556f6ad227d0bd4d41e09e73e6b34097`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:59 GMT
ADD file:3db67543ea64bf6723921d19cc5d0483db5c6658fc95834d8b2b5ed48a4cbacd in / 
# Tue, 02 Aug 2022 01:18:59 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 18:32:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 02 Aug 2022 18:32:16 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 18:32:17 GMT
ENV GOSU_VERSION=1.14
# Tue, 02 Aug 2022 18:32:33 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 02 Aug 2022 18:32:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 02 Aug 2022 18:32:42 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 18:32:42 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 02 Aug 2022 18:32:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 02 Aug 2022 18:33:28 GMT
ARG MARIADB_MAJOR=10.8
# Tue, 02 Aug 2022 18:33:29 GMT
ENV MARIADB_MAJOR=10.8
# Tue, 02 Aug 2022 18:33:30 GMT
ARG MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 02 Aug 2022 18:33:31 GMT
ENV MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 02 Aug 2022 18:33:32 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
# Tue, 02 Aug 2022 18:33:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 02 Aug 2022 18:33:52 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 02 Aug 2022 18:33:53 GMT
VOLUME [/var/lib/mysql]
# Tue, 02 Aug 2022 18:33:54 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 02 Aug 2022 18:33:55 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 02 Aug 2022 18:33:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 18:33:56 GMT
EXPOSE 3306
# Tue, 02 Aug 2022 18:33:57 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:4a3049d340b7d3651a954fd25a32c42feb1086889d6287e2f15468aef865c5c4`  
		Last Modified: Tue, 02 Aug 2022 01:20:49 GMT  
		Size: 28.4 MB (28381155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e5bedaed5f8e5343fee312eb2f21894d7b4026a0c692da89fe4f30a432e48b4`  
		Last Modified: Tue, 02 Aug 2022 18:41:32 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f07d81dfa02553c544d772dc3aa04ed6a2e6ad5b810ca742eee9a918786e5f`  
		Last Modified: Tue, 02 Aug 2022 18:41:30 GMT  
		Size: 3.6 MB (3594051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd6b8a20cb609d07274a17b8dd4ae810b6a98f76cf0ad513aa0c03eda46fcbce`  
		Last Modified: Tue, 02 Aug 2022 18:41:30 GMT  
		Size: 1.9 MB (1899200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3d39cfcf2768f9c1165cc0d3764c3649542f541a1ed3f18bec6283d58553e00`  
		Last Modified: Tue, 02 Aug 2022 18:41:30 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d230566e80222a9242f97419a6018684f4e324420ee89e4c0395f8107a124c91`  
		Last Modified: Tue, 02 Aug 2022 18:41:30 GMT  
		Size: 2.2 MB (2211614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c8c9abaef706c6185822ae21205ab5bc569494c4492a89eef44d8a855315c5`  
		Last Modified: Tue, 02 Aug 2022 18:41:27 GMT  
		Size: 2.5 KB (2465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9bff43ba5b5f6479659a8a7496d4156615c3cd9439c46779dd3feed3c4511ae`  
		Last Modified: Tue, 02 Aug 2022 18:41:57 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08cb73ef10f93c31f677c6818187b24c6bb65b4cb76ad5ed05e5b31853ef1b73`  
		Last Modified: Tue, 02 Aug 2022 18:42:08 GMT  
		Size: 66.4 MB (66369985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b16804fca7957e5cc3538c9a1a58af3e8e7a9eb0ee3318ffa413c7ebf4c76d4`  
		Last Modified: Tue, 02 Aug 2022 18:41:57 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fffad21dfd527f8685de9b3c864738e88bb8791db49ecdeb988d9d194a20d7cc`  
		Last Modified: Tue, 02 Aug 2022 18:41:57 GMT  
		Size: 6.7 KB (6699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8` - linux; ppc64le

```console
$ docker pull mariadb@sha256:017f8f45233c3bb9128302760d3c66df5253d31744a6e7401125b14233028d3a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.8 MB (116844233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf24d5b9794e7b70a566d82d3aa538d3b1657c23f08249227462a909b294c582`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 02 Aug 2022 01:31:12 GMT
ADD file:b6916c28c03568df4c2efc3da91ea6320f639cdbd2fa3f6741fcea7acad4fd5f in / 
# Tue, 02 Aug 2022 01:31:14 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 04:30:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 03 Aug 2022 04:30:30 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 04:30:31 GMT
ENV GOSU_VERSION=1.14
# Wed, 03 Aug 2022 04:30:49 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 03 Aug 2022 04:30:50 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 03 Aug 2022 04:31:03 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 04:31:03 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 03 Aug 2022 04:31:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 03 Aug 2022 04:32:26 GMT
ARG MARIADB_MAJOR=10.8
# Wed, 03 Aug 2022 04:32:26 GMT
ENV MARIADB_MAJOR=10.8
# Wed, 03 Aug 2022 04:32:26 GMT
ARG MARIADB_VERSION=1:10.8.3+maria~jammy
# Wed, 03 Aug 2022 04:32:27 GMT
ENV MARIADB_VERSION=1:10.8.3+maria~jammy
# Wed, 03 Aug 2022 04:32:27 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
# Wed, 03 Aug 2022 04:32:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 03 Aug 2022 04:33:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 03 Aug 2022 04:33:11 GMT
VOLUME [/var/lib/mysql]
# Wed, 03 Aug 2022 04:33:11 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Wed, 03 Aug 2022 04:33:12 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Wed, 03 Aug 2022 04:33:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 Aug 2022 04:33:12 GMT
EXPOSE 3306
# Wed, 03 Aug 2022 04:33:13 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:6f8c2fc0a4f976c1c0bd1c0e14022b3ed8b7c83cdb247c83016052c3678aaf28`  
		Last Modified: Tue, 02 Aug 2022 01:33:53 GMT  
		Size: 35.7 MB (35718004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da4a119144d25c65194f5210a2c0785d96c4b9d92c955f354d54e971b66cf0f`  
		Last Modified: Wed, 03 Aug 2022 04:43:49 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06895bfe56d4b1ebe076e361e483fe6fc6bfbaeb765ae25852c1993a6943452c`  
		Last Modified: Wed, 03 Aug 2022 04:43:47 GMT  
		Size: 4.5 MB (4503176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ee69296533cbe8c0bf533fa14d2f744068f58d5998026a4ba0c82bf9ea828ca`  
		Last Modified: Wed, 03 Aug 2022 04:43:47 GMT  
		Size: 1.9 MB (1921808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e76647cede58c06588416f8c141f66a1bf687145f5a0b0b2c530cdc63b14c805`  
		Last Modified: Wed, 03 Aug 2022 04:43:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b9befa094840721fea90813c85958f817ad561e93636ebd0730a9a395a0b46a`  
		Last Modified: Wed, 03 Aug 2022 04:43:47 GMT  
		Size: 2.4 MB (2404905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f92e1e86f56f2fadd73fdf7cc3428ca6687fbfa29af810bdb5c43b92ab77d02`  
		Last Modified: Wed, 03 Aug 2022 04:43:44 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b92a0e7592d7a0ad15eb1a53b8fcda1b2bb13d5dc516094d233fc4e8d23f53`  
		Last Modified: Wed, 03 Aug 2022 04:44:25 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c0e53f407a9d9f4fdfdb556976d3e976f93310c77b48124319cd55841b06ac`  
		Last Modified: Wed, 03 Aug 2022 04:44:43 GMT  
		Size: 72.3 MB (72281444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a525304ab204f12f8e1da79b296cd25e4eeda97bab0a3c0b8b21d27624c824c`  
		Last Modified: Wed, 03 Aug 2022 04:44:24 GMT  
		Size: 3.5 KB (3488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759170fa57f07b1b2ffc7f1dc434234f5446e9b18b7a5bb4bc1edbea87035db4`  
		Last Modified: Wed, 03 Aug 2022 04:44:24 GMT  
		Size: 6.7 KB (6694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8` - linux; s390x

```console
$ docker pull mariadb@sha256:12097ab474fe2ee789b394e1e8a6b489f2ca4ce5ebc8904a14cfddeedb17b8e5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (104979316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d95792c9ef5a984b01f32025b66c1495e316d034e94d5975da4069d260d40064`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 02 Aug 2022 01:02:17 GMT
ADD file:d5a5e56e0ca8287f27b257e3ddbc9675a1bdac1912afbbab6cddd891056cd144 in / 
# Tue, 02 Aug 2022 01:02:19 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 12:55:49 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 02 Aug 2022 12:56:06 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 12:56:07 GMT
ENV GOSU_VERSION=1.14
# Tue, 02 Aug 2022 12:56:16 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 02 Aug 2022 12:56:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 02 Aug 2022 12:56:22 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 12:56:22 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 02 Aug 2022 12:56:23 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 02 Aug 2022 12:57:08 GMT
ARG MARIADB_MAJOR=10.8
# Tue, 02 Aug 2022 12:57:08 GMT
ENV MARIADB_MAJOR=10.8
# Tue, 02 Aug 2022 12:57:08 GMT
ARG MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 02 Aug 2022 12:57:08 GMT
ENV MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 02 Aug 2022 12:57:09 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
# Tue, 02 Aug 2022 12:57:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 02 Aug 2022 12:57:31 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 02 Aug 2022 12:57:38 GMT
VOLUME [/var/lib/mysql]
# Tue, 02 Aug 2022 12:57:38 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 02 Aug 2022 12:57:38 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 02 Aug 2022 12:57:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 12:57:39 GMT
EXPOSE 3306
# Tue, 02 Aug 2022 12:57:39 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:f97967c51aac02138b615522a1bab9c75addd5896f43ade17ddaac44e0644283`  
		Last Modified: Tue, 02 Aug 2022 01:03:51 GMT  
		Size: 28.6 MB (28642785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:518030038f927b55f39a26dbee5d8d6e8c31cc0ddf7f23268b3dee3f001182c2`  
		Last Modified: Tue, 02 Aug 2022 13:01:03 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c5074a746c3e8a07e66d2d76ac4a7b9e0af6ffbf0cc8a87f601bb8b6913662`  
		Last Modified: Tue, 02 Aug 2022 13:01:02 GMT  
		Size: 3.7 MB (3675041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6140902b730422bc6cad80b27cf9005104adc5047e2e34955e4fbb5cf7d394`  
		Last Modified: Tue, 02 Aug 2022 13:01:02 GMT  
		Size: 2.0 MB (1955931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67105478e75b1563365dc4986a18198b1230a86bb142ade80fa52d1f71e2b6d7`  
		Last Modified: Tue, 02 Aug 2022 13:01:02 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af39a56c0cc78baeec34ac8d7b93879b9b0878bfcc89737ffecf164a865bd46b`  
		Last Modified: Tue, 02 Aug 2022 13:01:02 GMT  
		Size: 2.2 MB (2216654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c8957d63d730d9dbe5d508e565371ce9f1a318e16ad05c720373da4dbbe208`  
		Last Modified: Tue, 02 Aug 2022 13:01:00 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5461cdd4f49c09bdda524801b26ccc244a1f3b4daa635e39c8d982532b8646d7`  
		Last Modified: Tue, 02 Aug 2022 13:01:21 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c9a941eeee8bd3fcf6d0504466a69f3b30632b6d14fed1f53bc29439ded147`  
		Last Modified: Tue, 02 Aug 2022 13:01:30 GMT  
		Size: 68.5 MB (68473998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7458611c3efeaaf589463cdc0dff355cd54d57b45ece924dd1f1e136b26ef8dc`  
		Last Modified: Tue, 02 Aug 2022 13:01:21 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf3286637af3a581d1537b503e2b8404768d5a37566247553295844ea4b760d`  
		Last Modified: Tue, 02 Aug 2022 13:01:21 GMT  
		Size: 6.7 KB (6699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.8-jammy`

```console
$ docker pull mariadb@sha256:0abf60f81588662e716c27c7f1b54a72b3bf879e0ca88fc393e1741970ec7f3f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.8-jammy` - linux; amd64

```console
$ docker pull mariadb@sha256:0a6ed934c1518abff64ed856b06f44006b4498b115941e19bbd910bd62a12232
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.9 MB (123908351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40b966d7252f541b41677fc35f8660fa90d14df0f33edc8085e6ca2dc0c5b247`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:55 GMT
ADD file:396eeb65c8d737180cc1219713cf59efb214027b79d8ea0b7e58a08e7c8d7a21 in / 
# Tue, 02 Aug 2022 01:30:56 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 20:19:21 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 02 Aug 2022 20:19:39 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 20:19:40 GMT
ENV GOSU_VERSION=1.14
# Tue, 02 Aug 2022 20:19:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 02 Aug 2022 20:19:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 02 Aug 2022 20:19:58 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 20:19:58 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 02 Aug 2022 20:19:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 02 Aug 2022 20:20:59 GMT
ARG MARIADB_MAJOR=10.8
# Tue, 02 Aug 2022 20:20:59 GMT
ENV MARIADB_MAJOR=10.8
# Tue, 02 Aug 2022 20:20:59 GMT
ARG MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 02 Aug 2022 20:20:59 GMT
ENV MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 02 Aug 2022 20:20:59 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
# Tue, 02 Aug 2022 20:21:00 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 02 Aug 2022 20:21:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 02 Aug 2022 20:21:19 GMT
VOLUME [/var/lib/mysql]
# Tue, 02 Aug 2022 20:21:19 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 02 Aug 2022 20:21:19 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 02 Aug 2022 20:21:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 20:21:20 GMT
EXPOSE 3306
# Tue, 02 Aug 2022 20:21:20 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d19f32bd9e4106d487f1a703fc2f09c8edadd92db4405d477978e8e466ab290d`  
		Last Modified: Tue, 02 Aug 2022 01:32:15 GMT  
		Size: 30.4 MB (30426136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f587559f9b58dcc08ed5b9fc08cc82b80ce995a37000098b1cdca2c199ae89f8`  
		Last Modified: Tue, 02 Aug 2022 20:26:32 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb060f92f2fef90ded1edd0a8c0609f95d414c40ff3684d1189beffa353f88b`  
		Last Modified: Tue, 02 Aug 2022 20:26:31 GMT  
		Size: 3.8 MB (3765797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27513e1f7a1e0c1c4f6197df108bf04d451bddf1da7bbdace8285098ba5dcf50`  
		Last Modified: Tue, 02 Aug 2022 20:26:31 GMT  
		Size: 2.0 MB (1992883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a84d3c510baac7a944c9669fc71e613930f5ca9c87cf616eeb06d2aa7c1917e`  
		Last Modified: Tue, 02 Aug 2022 20:26:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59731d2805a614a839795e79d61509494c939119e1dd7d76bf0f1b3a5f923c29`  
		Last Modified: Tue, 02 Aug 2022 20:26:31 GMT  
		Size: 2.3 MB (2298176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c008ca4420a867178be129dfe4311ce5ff0fcf8c2933d99ad49a3f0e3079cb3d`  
		Last Modified: Tue, 02 Aug 2022 20:26:28 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc47daf3f5d60b9b18f5ca3f556bc478eb967c997777a87459d43a9aea2fc6f`  
		Last Modified: Tue, 02 Aug 2022 20:26:58 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc547eec2be51eceb698e0766c93b76d55e7457043af4fe44ace5ca82927b1d4`  
		Last Modified: Tue, 02 Aug 2022 20:27:09 GMT  
		Size: 85.4 MB (85410459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bdaf629fe8214124455eb146db774a989c93271e8c3e264ece8ff4af772ea7b`  
		Last Modified: Tue, 02 Aug 2022 20:26:57 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddfbe3e290918fede8f6a3b0123b009178834c861a89c42c8b48075f8f8f420d`  
		Last Modified: Tue, 02 Aug 2022 20:26:58 GMT  
		Size: 6.7 KB (6696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8-jammy` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:1f011a0b21919b39058355d972fea445857869ad1f867eb56bd1d274fd969e88
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.5 MB (102470825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3f8da7eeabb6549ac946f2b45ffe497556f6ad227d0bd4d41e09e73e6b34097`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:59 GMT
ADD file:3db67543ea64bf6723921d19cc5d0483db5c6658fc95834d8b2b5ed48a4cbacd in / 
# Tue, 02 Aug 2022 01:18:59 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 18:32:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 02 Aug 2022 18:32:16 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 18:32:17 GMT
ENV GOSU_VERSION=1.14
# Tue, 02 Aug 2022 18:32:33 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 02 Aug 2022 18:32:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 02 Aug 2022 18:32:42 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 18:32:42 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 02 Aug 2022 18:32:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 02 Aug 2022 18:33:28 GMT
ARG MARIADB_MAJOR=10.8
# Tue, 02 Aug 2022 18:33:29 GMT
ENV MARIADB_MAJOR=10.8
# Tue, 02 Aug 2022 18:33:30 GMT
ARG MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 02 Aug 2022 18:33:31 GMT
ENV MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 02 Aug 2022 18:33:32 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
# Tue, 02 Aug 2022 18:33:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 02 Aug 2022 18:33:52 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 02 Aug 2022 18:33:53 GMT
VOLUME [/var/lib/mysql]
# Tue, 02 Aug 2022 18:33:54 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 02 Aug 2022 18:33:55 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 02 Aug 2022 18:33:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 18:33:56 GMT
EXPOSE 3306
# Tue, 02 Aug 2022 18:33:57 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:4a3049d340b7d3651a954fd25a32c42feb1086889d6287e2f15468aef865c5c4`  
		Last Modified: Tue, 02 Aug 2022 01:20:49 GMT  
		Size: 28.4 MB (28381155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e5bedaed5f8e5343fee312eb2f21894d7b4026a0c692da89fe4f30a432e48b4`  
		Last Modified: Tue, 02 Aug 2022 18:41:32 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f07d81dfa02553c544d772dc3aa04ed6a2e6ad5b810ca742eee9a918786e5f`  
		Last Modified: Tue, 02 Aug 2022 18:41:30 GMT  
		Size: 3.6 MB (3594051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd6b8a20cb609d07274a17b8dd4ae810b6a98f76cf0ad513aa0c03eda46fcbce`  
		Last Modified: Tue, 02 Aug 2022 18:41:30 GMT  
		Size: 1.9 MB (1899200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3d39cfcf2768f9c1165cc0d3764c3649542f541a1ed3f18bec6283d58553e00`  
		Last Modified: Tue, 02 Aug 2022 18:41:30 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d230566e80222a9242f97419a6018684f4e324420ee89e4c0395f8107a124c91`  
		Last Modified: Tue, 02 Aug 2022 18:41:30 GMT  
		Size: 2.2 MB (2211614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c8c9abaef706c6185822ae21205ab5bc569494c4492a89eef44d8a855315c5`  
		Last Modified: Tue, 02 Aug 2022 18:41:27 GMT  
		Size: 2.5 KB (2465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9bff43ba5b5f6479659a8a7496d4156615c3cd9439c46779dd3feed3c4511ae`  
		Last Modified: Tue, 02 Aug 2022 18:41:57 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08cb73ef10f93c31f677c6818187b24c6bb65b4cb76ad5ed05e5b31853ef1b73`  
		Last Modified: Tue, 02 Aug 2022 18:42:08 GMT  
		Size: 66.4 MB (66369985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b16804fca7957e5cc3538c9a1a58af3e8e7a9eb0ee3318ffa413c7ebf4c76d4`  
		Last Modified: Tue, 02 Aug 2022 18:41:57 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fffad21dfd527f8685de9b3c864738e88bb8791db49ecdeb988d9d194a20d7cc`  
		Last Modified: Tue, 02 Aug 2022 18:41:57 GMT  
		Size: 6.7 KB (6699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8-jammy` - linux; ppc64le

```console
$ docker pull mariadb@sha256:017f8f45233c3bb9128302760d3c66df5253d31744a6e7401125b14233028d3a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.8 MB (116844233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf24d5b9794e7b70a566d82d3aa538d3b1657c23f08249227462a909b294c582`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 02 Aug 2022 01:31:12 GMT
ADD file:b6916c28c03568df4c2efc3da91ea6320f639cdbd2fa3f6741fcea7acad4fd5f in / 
# Tue, 02 Aug 2022 01:31:14 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 04:30:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 03 Aug 2022 04:30:30 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 04:30:31 GMT
ENV GOSU_VERSION=1.14
# Wed, 03 Aug 2022 04:30:49 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 03 Aug 2022 04:30:50 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 03 Aug 2022 04:31:03 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 04:31:03 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 03 Aug 2022 04:31:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 03 Aug 2022 04:32:26 GMT
ARG MARIADB_MAJOR=10.8
# Wed, 03 Aug 2022 04:32:26 GMT
ENV MARIADB_MAJOR=10.8
# Wed, 03 Aug 2022 04:32:26 GMT
ARG MARIADB_VERSION=1:10.8.3+maria~jammy
# Wed, 03 Aug 2022 04:32:27 GMT
ENV MARIADB_VERSION=1:10.8.3+maria~jammy
# Wed, 03 Aug 2022 04:32:27 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
# Wed, 03 Aug 2022 04:32:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 03 Aug 2022 04:33:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 03 Aug 2022 04:33:11 GMT
VOLUME [/var/lib/mysql]
# Wed, 03 Aug 2022 04:33:11 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Wed, 03 Aug 2022 04:33:12 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Wed, 03 Aug 2022 04:33:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 Aug 2022 04:33:12 GMT
EXPOSE 3306
# Wed, 03 Aug 2022 04:33:13 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:6f8c2fc0a4f976c1c0bd1c0e14022b3ed8b7c83cdb247c83016052c3678aaf28`  
		Last Modified: Tue, 02 Aug 2022 01:33:53 GMT  
		Size: 35.7 MB (35718004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da4a119144d25c65194f5210a2c0785d96c4b9d92c955f354d54e971b66cf0f`  
		Last Modified: Wed, 03 Aug 2022 04:43:49 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06895bfe56d4b1ebe076e361e483fe6fc6bfbaeb765ae25852c1993a6943452c`  
		Last Modified: Wed, 03 Aug 2022 04:43:47 GMT  
		Size: 4.5 MB (4503176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ee69296533cbe8c0bf533fa14d2f744068f58d5998026a4ba0c82bf9ea828ca`  
		Last Modified: Wed, 03 Aug 2022 04:43:47 GMT  
		Size: 1.9 MB (1921808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e76647cede58c06588416f8c141f66a1bf687145f5a0b0b2c530cdc63b14c805`  
		Last Modified: Wed, 03 Aug 2022 04:43:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b9befa094840721fea90813c85958f817ad561e93636ebd0730a9a395a0b46a`  
		Last Modified: Wed, 03 Aug 2022 04:43:47 GMT  
		Size: 2.4 MB (2404905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f92e1e86f56f2fadd73fdf7cc3428ca6687fbfa29af810bdb5c43b92ab77d02`  
		Last Modified: Wed, 03 Aug 2022 04:43:44 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b92a0e7592d7a0ad15eb1a53b8fcda1b2bb13d5dc516094d233fc4e8d23f53`  
		Last Modified: Wed, 03 Aug 2022 04:44:25 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c0e53f407a9d9f4fdfdb556976d3e976f93310c77b48124319cd55841b06ac`  
		Last Modified: Wed, 03 Aug 2022 04:44:43 GMT  
		Size: 72.3 MB (72281444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a525304ab204f12f8e1da79b296cd25e4eeda97bab0a3c0b8b21d27624c824c`  
		Last Modified: Wed, 03 Aug 2022 04:44:24 GMT  
		Size: 3.5 KB (3488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759170fa57f07b1b2ffc7f1dc434234f5446e9b18b7a5bb4bc1edbea87035db4`  
		Last Modified: Wed, 03 Aug 2022 04:44:24 GMT  
		Size: 6.7 KB (6694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8-jammy` - linux; s390x

```console
$ docker pull mariadb@sha256:12097ab474fe2ee789b394e1e8a6b489f2ca4ce5ebc8904a14cfddeedb17b8e5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (104979316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d95792c9ef5a984b01f32025b66c1495e316d034e94d5975da4069d260d40064`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 02 Aug 2022 01:02:17 GMT
ADD file:d5a5e56e0ca8287f27b257e3ddbc9675a1bdac1912afbbab6cddd891056cd144 in / 
# Tue, 02 Aug 2022 01:02:19 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 12:55:49 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 02 Aug 2022 12:56:06 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 12:56:07 GMT
ENV GOSU_VERSION=1.14
# Tue, 02 Aug 2022 12:56:16 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 02 Aug 2022 12:56:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 02 Aug 2022 12:56:22 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 12:56:22 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 02 Aug 2022 12:56:23 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 02 Aug 2022 12:57:08 GMT
ARG MARIADB_MAJOR=10.8
# Tue, 02 Aug 2022 12:57:08 GMT
ENV MARIADB_MAJOR=10.8
# Tue, 02 Aug 2022 12:57:08 GMT
ARG MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 02 Aug 2022 12:57:08 GMT
ENV MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 02 Aug 2022 12:57:09 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
# Tue, 02 Aug 2022 12:57:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 02 Aug 2022 12:57:31 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 02 Aug 2022 12:57:38 GMT
VOLUME [/var/lib/mysql]
# Tue, 02 Aug 2022 12:57:38 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 02 Aug 2022 12:57:38 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 02 Aug 2022 12:57:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 12:57:39 GMT
EXPOSE 3306
# Tue, 02 Aug 2022 12:57:39 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:f97967c51aac02138b615522a1bab9c75addd5896f43ade17ddaac44e0644283`  
		Last Modified: Tue, 02 Aug 2022 01:03:51 GMT  
		Size: 28.6 MB (28642785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:518030038f927b55f39a26dbee5d8d6e8c31cc0ddf7f23268b3dee3f001182c2`  
		Last Modified: Tue, 02 Aug 2022 13:01:03 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c5074a746c3e8a07e66d2d76ac4a7b9e0af6ffbf0cc8a87f601bb8b6913662`  
		Last Modified: Tue, 02 Aug 2022 13:01:02 GMT  
		Size: 3.7 MB (3675041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6140902b730422bc6cad80b27cf9005104adc5047e2e34955e4fbb5cf7d394`  
		Last Modified: Tue, 02 Aug 2022 13:01:02 GMT  
		Size: 2.0 MB (1955931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67105478e75b1563365dc4986a18198b1230a86bb142ade80fa52d1f71e2b6d7`  
		Last Modified: Tue, 02 Aug 2022 13:01:02 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af39a56c0cc78baeec34ac8d7b93879b9b0878bfcc89737ffecf164a865bd46b`  
		Last Modified: Tue, 02 Aug 2022 13:01:02 GMT  
		Size: 2.2 MB (2216654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c8957d63d730d9dbe5d508e565371ce9f1a318e16ad05c720373da4dbbe208`  
		Last Modified: Tue, 02 Aug 2022 13:01:00 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5461cdd4f49c09bdda524801b26ccc244a1f3b4daa635e39c8d982532b8646d7`  
		Last Modified: Tue, 02 Aug 2022 13:01:21 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c9a941eeee8bd3fcf6d0504466a69f3b30632b6d14fed1f53bc29439ded147`  
		Last Modified: Tue, 02 Aug 2022 13:01:30 GMT  
		Size: 68.5 MB (68473998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7458611c3efeaaf589463cdc0dff355cd54d57b45ece924dd1f1e136b26ef8dc`  
		Last Modified: Tue, 02 Aug 2022 13:01:21 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf3286637af3a581d1537b503e2b8404768d5a37566247553295844ea4b760d`  
		Last Modified: Tue, 02 Aug 2022 13:01:21 GMT  
		Size: 6.7 KB (6699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.8.4`

**does not exist** (yet?)

## `mariadb:10.8.4-jammy`

**does not exist** (yet?)

## `mariadb:10.9`

**does not exist** (yet?)

## `mariadb:10.9-jammy`

**does not exist** (yet?)

## `mariadb:10.9.2`

**does not exist** (yet?)

## `mariadb:10.9.2-jammy`

**does not exist** (yet?)

## `mariadb:jammy`

```console
$ docker pull mariadb@sha256:0abf60f81588662e716c27c7f1b54a72b3bf879e0ca88fc393e1741970ec7f3f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:jammy` - linux; amd64

```console
$ docker pull mariadb@sha256:0a6ed934c1518abff64ed856b06f44006b4498b115941e19bbd910bd62a12232
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.9 MB (123908351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40b966d7252f541b41677fc35f8660fa90d14df0f33edc8085e6ca2dc0c5b247`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:55 GMT
ADD file:396eeb65c8d737180cc1219713cf59efb214027b79d8ea0b7e58a08e7c8d7a21 in / 
# Tue, 02 Aug 2022 01:30:56 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 20:19:21 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 02 Aug 2022 20:19:39 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 20:19:40 GMT
ENV GOSU_VERSION=1.14
# Tue, 02 Aug 2022 20:19:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 02 Aug 2022 20:19:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 02 Aug 2022 20:19:58 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 20:19:58 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 02 Aug 2022 20:19:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 02 Aug 2022 20:20:59 GMT
ARG MARIADB_MAJOR=10.8
# Tue, 02 Aug 2022 20:20:59 GMT
ENV MARIADB_MAJOR=10.8
# Tue, 02 Aug 2022 20:20:59 GMT
ARG MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 02 Aug 2022 20:20:59 GMT
ENV MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 02 Aug 2022 20:20:59 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
# Tue, 02 Aug 2022 20:21:00 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 02 Aug 2022 20:21:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 02 Aug 2022 20:21:19 GMT
VOLUME [/var/lib/mysql]
# Tue, 02 Aug 2022 20:21:19 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 02 Aug 2022 20:21:19 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 02 Aug 2022 20:21:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 20:21:20 GMT
EXPOSE 3306
# Tue, 02 Aug 2022 20:21:20 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d19f32bd9e4106d487f1a703fc2f09c8edadd92db4405d477978e8e466ab290d`  
		Last Modified: Tue, 02 Aug 2022 01:32:15 GMT  
		Size: 30.4 MB (30426136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f587559f9b58dcc08ed5b9fc08cc82b80ce995a37000098b1cdca2c199ae89f8`  
		Last Modified: Tue, 02 Aug 2022 20:26:32 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb060f92f2fef90ded1edd0a8c0609f95d414c40ff3684d1189beffa353f88b`  
		Last Modified: Tue, 02 Aug 2022 20:26:31 GMT  
		Size: 3.8 MB (3765797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27513e1f7a1e0c1c4f6197df108bf04d451bddf1da7bbdace8285098ba5dcf50`  
		Last Modified: Tue, 02 Aug 2022 20:26:31 GMT  
		Size: 2.0 MB (1992883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a84d3c510baac7a944c9669fc71e613930f5ca9c87cf616eeb06d2aa7c1917e`  
		Last Modified: Tue, 02 Aug 2022 20:26:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59731d2805a614a839795e79d61509494c939119e1dd7d76bf0f1b3a5f923c29`  
		Last Modified: Tue, 02 Aug 2022 20:26:31 GMT  
		Size: 2.3 MB (2298176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c008ca4420a867178be129dfe4311ce5ff0fcf8c2933d99ad49a3f0e3079cb3d`  
		Last Modified: Tue, 02 Aug 2022 20:26:28 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc47daf3f5d60b9b18f5ca3f556bc478eb967c997777a87459d43a9aea2fc6f`  
		Last Modified: Tue, 02 Aug 2022 20:26:58 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc547eec2be51eceb698e0766c93b76d55e7457043af4fe44ace5ca82927b1d4`  
		Last Modified: Tue, 02 Aug 2022 20:27:09 GMT  
		Size: 85.4 MB (85410459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bdaf629fe8214124455eb146db774a989c93271e8c3e264ece8ff4af772ea7b`  
		Last Modified: Tue, 02 Aug 2022 20:26:57 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddfbe3e290918fede8f6a3b0123b009178834c861a89c42c8b48075f8f8f420d`  
		Last Modified: Tue, 02 Aug 2022 20:26:58 GMT  
		Size: 6.7 KB (6696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:jammy` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:1f011a0b21919b39058355d972fea445857869ad1f867eb56bd1d274fd969e88
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.5 MB (102470825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3f8da7eeabb6549ac946f2b45ffe497556f6ad227d0bd4d41e09e73e6b34097`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:59 GMT
ADD file:3db67543ea64bf6723921d19cc5d0483db5c6658fc95834d8b2b5ed48a4cbacd in / 
# Tue, 02 Aug 2022 01:18:59 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 18:32:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 02 Aug 2022 18:32:16 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 18:32:17 GMT
ENV GOSU_VERSION=1.14
# Tue, 02 Aug 2022 18:32:33 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 02 Aug 2022 18:32:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 02 Aug 2022 18:32:42 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 18:32:42 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 02 Aug 2022 18:32:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 02 Aug 2022 18:33:28 GMT
ARG MARIADB_MAJOR=10.8
# Tue, 02 Aug 2022 18:33:29 GMT
ENV MARIADB_MAJOR=10.8
# Tue, 02 Aug 2022 18:33:30 GMT
ARG MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 02 Aug 2022 18:33:31 GMT
ENV MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 02 Aug 2022 18:33:32 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
# Tue, 02 Aug 2022 18:33:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 02 Aug 2022 18:33:52 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 02 Aug 2022 18:33:53 GMT
VOLUME [/var/lib/mysql]
# Tue, 02 Aug 2022 18:33:54 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 02 Aug 2022 18:33:55 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 02 Aug 2022 18:33:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 18:33:56 GMT
EXPOSE 3306
# Tue, 02 Aug 2022 18:33:57 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:4a3049d340b7d3651a954fd25a32c42feb1086889d6287e2f15468aef865c5c4`  
		Last Modified: Tue, 02 Aug 2022 01:20:49 GMT  
		Size: 28.4 MB (28381155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e5bedaed5f8e5343fee312eb2f21894d7b4026a0c692da89fe4f30a432e48b4`  
		Last Modified: Tue, 02 Aug 2022 18:41:32 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f07d81dfa02553c544d772dc3aa04ed6a2e6ad5b810ca742eee9a918786e5f`  
		Last Modified: Tue, 02 Aug 2022 18:41:30 GMT  
		Size: 3.6 MB (3594051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd6b8a20cb609d07274a17b8dd4ae810b6a98f76cf0ad513aa0c03eda46fcbce`  
		Last Modified: Tue, 02 Aug 2022 18:41:30 GMT  
		Size: 1.9 MB (1899200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3d39cfcf2768f9c1165cc0d3764c3649542f541a1ed3f18bec6283d58553e00`  
		Last Modified: Tue, 02 Aug 2022 18:41:30 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d230566e80222a9242f97419a6018684f4e324420ee89e4c0395f8107a124c91`  
		Last Modified: Tue, 02 Aug 2022 18:41:30 GMT  
		Size: 2.2 MB (2211614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c8c9abaef706c6185822ae21205ab5bc569494c4492a89eef44d8a855315c5`  
		Last Modified: Tue, 02 Aug 2022 18:41:27 GMT  
		Size: 2.5 KB (2465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9bff43ba5b5f6479659a8a7496d4156615c3cd9439c46779dd3feed3c4511ae`  
		Last Modified: Tue, 02 Aug 2022 18:41:57 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08cb73ef10f93c31f677c6818187b24c6bb65b4cb76ad5ed05e5b31853ef1b73`  
		Last Modified: Tue, 02 Aug 2022 18:42:08 GMT  
		Size: 66.4 MB (66369985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b16804fca7957e5cc3538c9a1a58af3e8e7a9eb0ee3318ffa413c7ebf4c76d4`  
		Last Modified: Tue, 02 Aug 2022 18:41:57 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fffad21dfd527f8685de9b3c864738e88bb8791db49ecdeb988d9d194a20d7cc`  
		Last Modified: Tue, 02 Aug 2022 18:41:57 GMT  
		Size: 6.7 KB (6699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:jammy` - linux; ppc64le

```console
$ docker pull mariadb@sha256:017f8f45233c3bb9128302760d3c66df5253d31744a6e7401125b14233028d3a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.8 MB (116844233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf24d5b9794e7b70a566d82d3aa538d3b1657c23f08249227462a909b294c582`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 02 Aug 2022 01:31:12 GMT
ADD file:b6916c28c03568df4c2efc3da91ea6320f639cdbd2fa3f6741fcea7acad4fd5f in / 
# Tue, 02 Aug 2022 01:31:14 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 04:30:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 03 Aug 2022 04:30:30 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 04:30:31 GMT
ENV GOSU_VERSION=1.14
# Wed, 03 Aug 2022 04:30:49 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 03 Aug 2022 04:30:50 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 03 Aug 2022 04:31:03 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 04:31:03 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 03 Aug 2022 04:31:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 03 Aug 2022 04:32:26 GMT
ARG MARIADB_MAJOR=10.8
# Wed, 03 Aug 2022 04:32:26 GMT
ENV MARIADB_MAJOR=10.8
# Wed, 03 Aug 2022 04:32:26 GMT
ARG MARIADB_VERSION=1:10.8.3+maria~jammy
# Wed, 03 Aug 2022 04:32:27 GMT
ENV MARIADB_VERSION=1:10.8.3+maria~jammy
# Wed, 03 Aug 2022 04:32:27 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
# Wed, 03 Aug 2022 04:32:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 03 Aug 2022 04:33:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 03 Aug 2022 04:33:11 GMT
VOLUME [/var/lib/mysql]
# Wed, 03 Aug 2022 04:33:11 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Wed, 03 Aug 2022 04:33:12 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Wed, 03 Aug 2022 04:33:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 Aug 2022 04:33:12 GMT
EXPOSE 3306
# Wed, 03 Aug 2022 04:33:13 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:6f8c2fc0a4f976c1c0bd1c0e14022b3ed8b7c83cdb247c83016052c3678aaf28`  
		Last Modified: Tue, 02 Aug 2022 01:33:53 GMT  
		Size: 35.7 MB (35718004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da4a119144d25c65194f5210a2c0785d96c4b9d92c955f354d54e971b66cf0f`  
		Last Modified: Wed, 03 Aug 2022 04:43:49 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06895bfe56d4b1ebe076e361e483fe6fc6bfbaeb765ae25852c1993a6943452c`  
		Last Modified: Wed, 03 Aug 2022 04:43:47 GMT  
		Size: 4.5 MB (4503176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ee69296533cbe8c0bf533fa14d2f744068f58d5998026a4ba0c82bf9ea828ca`  
		Last Modified: Wed, 03 Aug 2022 04:43:47 GMT  
		Size: 1.9 MB (1921808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e76647cede58c06588416f8c141f66a1bf687145f5a0b0b2c530cdc63b14c805`  
		Last Modified: Wed, 03 Aug 2022 04:43:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b9befa094840721fea90813c85958f817ad561e93636ebd0730a9a395a0b46a`  
		Last Modified: Wed, 03 Aug 2022 04:43:47 GMT  
		Size: 2.4 MB (2404905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f92e1e86f56f2fadd73fdf7cc3428ca6687fbfa29af810bdb5c43b92ab77d02`  
		Last Modified: Wed, 03 Aug 2022 04:43:44 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b92a0e7592d7a0ad15eb1a53b8fcda1b2bb13d5dc516094d233fc4e8d23f53`  
		Last Modified: Wed, 03 Aug 2022 04:44:25 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c0e53f407a9d9f4fdfdb556976d3e976f93310c77b48124319cd55841b06ac`  
		Last Modified: Wed, 03 Aug 2022 04:44:43 GMT  
		Size: 72.3 MB (72281444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a525304ab204f12f8e1da79b296cd25e4eeda97bab0a3c0b8b21d27624c824c`  
		Last Modified: Wed, 03 Aug 2022 04:44:24 GMT  
		Size: 3.5 KB (3488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759170fa57f07b1b2ffc7f1dc434234f5446e9b18b7a5bb4bc1edbea87035db4`  
		Last Modified: Wed, 03 Aug 2022 04:44:24 GMT  
		Size: 6.7 KB (6694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:jammy` - linux; s390x

```console
$ docker pull mariadb@sha256:12097ab474fe2ee789b394e1e8a6b489f2ca4ce5ebc8904a14cfddeedb17b8e5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (104979316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d95792c9ef5a984b01f32025b66c1495e316d034e94d5975da4069d260d40064`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 02 Aug 2022 01:02:17 GMT
ADD file:d5a5e56e0ca8287f27b257e3ddbc9675a1bdac1912afbbab6cddd891056cd144 in / 
# Tue, 02 Aug 2022 01:02:19 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 12:55:49 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 02 Aug 2022 12:56:06 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 12:56:07 GMT
ENV GOSU_VERSION=1.14
# Tue, 02 Aug 2022 12:56:16 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 02 Aug 2022 12:56:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 02 Aug 2022 12:56:22 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 12:56:22 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 02 Aug 2022 12:56:23 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 02 Aug 2022 12:57:08 GMT
ARG MARIADB_MAJOR=10.8
# Tue, 02 Aug 2022 12:57:08 GMT
ENV MARIADB_MAJOR=10.8
# Tue, 02 Aug 2022 12:57:08 GMT
ARG MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 02 Aug 2022 12:57:08 GMT
ENV MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 02 Aug 2022 12:57:09 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
# Tue, 02 Aug 2022 12:57:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 02 Aug 2022 12:57:31 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 02 Aug 2022 12:57:38 GMT
VOLUME [/var/lib/mysql]
# Tue, 02 Aug 2022 12:57:38 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 02 Aug 2022 12:57:38 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 02 Aug 2022 12:57:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 12:57:39 GMT
EXPOSE 3306
# Tue, 02 Aug 2022 12:57:39 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:f97967c51aac02138b615522a1bab9c75addd5896f43ade17ddaac44e0644283`  
		Last Modified: Tue, 02 Aug 2022 01:03:51 GMT  
		Size: 28.6 MB (28642785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:518030038f927b55f39a26dbee5d8d6e8c31cc0ddf7f23268b3dee3f001182c2`  
		Last Modified: Tue, 02 Aug 2022 13:01:03 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c5074a746c3e8a07e66d2d76ac4a7b9e0af6ffbf0cc8a87f601bb8b6913662`  
		Last Modified: Tue, 02 Aug 2022 13:01:02 GMT  
		Size: 3.7 MB (3675041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6140902b730422bc6cad80b27cf9005104adc5047e2e34955e4fbb5cf7d394`  
		Last Modified: Tue, 02 Aug 2022 13:01:02 GMT  
		Size: 2.0 MB (1955931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67105478e75b1563365dc4986a18198b1230a86bb142ade80fa52d1f71e2b6d7`  
		Last Modified: Tue, 02 Aug 2022 13:01:02 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af39a56c0cc78baeec34ac8d7b93879b9b0878bfcc89737ffecf164a865bd46b`  
		Last Modified: Tue, 02 Aug 2022 13:01:02 GMT  
		Size: 2.2 MB (2216654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c8957d63d730d9dbe5d508e565371ce9f1a318e16ad05c720373da4dbbe208`  
		Last Modified: Tue, 02 Aug 2022 13:01:00 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5461cdd4f49c09bdda524801b26ccc244a1f3b4daa635e39c8d982532b8646d7`  
		Last Modified: Tue, 02 Aug 2022 13:01:21 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c9a941eeee8bd3fcf6d0504466a69f3b30632b6d14fed1f53bc29439ded147`  
		Last Modified: Tue, 02 Aug 2022 13:01:30 GMT  
		Size: 68.5 MB (68473998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7458611c3efeaaf589463cdc0dff355cd54d57b45ece924dd1f1e136b26ef8dc`  
		Last Modified: Tue, 02 Aug 2022 13:01:21 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf3286637af3a581d1537b503e2b8404768d5a37566247553295844ea4b760d`  
		Last Modified: Tue, 02 Aug 2022 13:01:21 GMT  
		Size: 6.7 KB (6699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:latest`

```console
$ docker pull mariadb@sha256:0abf60f81588662e716c27c7f1b54a72b3bf879e0ca88fc393e1741970ec7f3f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:latest` - linux; amd64

```console
$ docker pull mariadb@sha256:0a6ed934c1518abff64ed856b06f44006b4498b115941e19bbd910bd62a12232
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.9 MB (123908351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40b966d7252f541b41677fc35f8660fa90d14df0f33edc8085e6ca2dc0c5b247`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:55 GMT
ADD file:396eeb65c8d737180cc1219713cf59efb214027b79d8ea0b7e58a08e7c8d7a21 in / 
# Tue, 02 Aug 2022 01:30:56 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 20:19:21 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 02 Aug 2022 20:19:39 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 20:19:40 GMT
ENV GOSU_VERSION=1.14
# Tue, 02 Aug 2022 20:19:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 02 Aug 2022 20:19:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 02 Aug 2022 20:19:58 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 20:19:58 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 02 Aug 2022 20:19:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 02 Aug 2022 20:20:59 GMT
ARG MARIADB_MAJOR=10.8
# Tue, 02 Aug 2022 20:20:59 GMT
ENV MARIADB_MAJOR=10.8
# Tue, 02 Aug 2022 20:20:59 GMT
ARG MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 02 Aug 2022 20:20:59 GMT
ENV MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 02 Aug 2022 20:20:59 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
# Tue, 02 Aug 2022 20:21:00 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 02 Aug 2022 20:21:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 02 Aug 2022 20:21:19 GMT
VOLUME [/var/lib/mysql]
# Tue, 02 Aug 2022 20:21:19 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 02 Aug 2022 20:21:19 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 02 Aug 2022 20:21:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 20:21:20 GMT
EXPOSE 3306
# Tue, 02 Aug 2022 20:21:20 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d19f32bd9e4106d487f1a703fc2f09c8edadd92db4405d477978e8e466ab290d`  
		Last Modified: Tue, 02 Aug 2022 01:32:15 GMT  
		Size: 30.4 MB (30426136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f587559f9b58dcc08ed5b9fc08cc82b80ce995a37000098b1cdca2c199ae89f8`  
		Last Modified: Tue, 02 Aug 2022 20:26:32 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb060f92f2fef90ded1edd0a8c0609f95d414c40ff3684d1189beffa353f88b`  
		Last Modified: Tue, 02 Aug 2022 20:26:31 GMT  
		Size: 3.8 MB (3765797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27513e1f7a1e0c1c4f6197df108bf04d451bddf1da7bbdace8285098ba5dcf50`  
		Last Modified: Tue, 02 Aug 2022 20:26:31 GMT  
		Size: 2.0 MB (1992883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a84d3c510baac7a944c9669fc71e613930f5ca9c87cf616eeb06d2aa7c1917e`  
		Last Modified: Tue, 02 Aug 2022 20:26:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59731d2805a614a839795e79d61509494c939119e1dd7d76bf0f1b3a5f923c29`  
		Last Modified: Tue, 02 Aug 2022 20:26:31 GMT  
		Size: 2.3 MB (2298176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c008ca4420a867178be129dfe4311ce5ff0fcf8c2933d99ad49a3f0e3079cb3d`  
		Last Modified: Tue, 02 Aug 2022 20:26:28 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc47daf3f5d60b9b18f5ca3f556bc478eb967c997777a87459d43a9aea2fc6f`  
		Last Modified: Tue, 02 Aug 2022 20:26:58 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc547eec2be51eceb698e0766c93b76d55e7457043af4fe44ace5ca82927b1d4`  
		Last Modified: Tue, 02 Aug 2022 20:27:09 GMT  
		Size: 85.4 MB (85410459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bdaf629fe8214124455eb146db774a989c93271e8c3e264ece8ff4af772ea7b`  
		Last Modified: Tue, 02 Aug 2022 20:26:57 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddfbe3e290918fede8f6a3b0123b009178834c861a89c42c8b48075f8f8f420d`  
		Last Modified: Tue, 02 Aug 2022 20:26:58 GMT  
		Size: 6.7 KB (6696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:1f011a0b21919b39058355d972fea445857869ad1f867eb56bd1d274fd969e88
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.5 MB (102470825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3f8da7eeabb6549ac946f2b45ffe497556f6ad227d0bd4d41e09e73e6b34097`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:59 GMT
ADD file:3db67543ea64bf6723921d19cc5d0483db5c6658fc95834d8b2b5ed48a4cbacd in / 
# Tue, 02 Aug 2022 01:18:59 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 18:32:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 02 Aug 2022 18:32:16 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 18:32:17 GMT
ENV GOSU_VERSION=1.14
# Tue, 02 Aug 2022 18:32:33 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 02 Aug 2022 18:32:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 02 Aug 2022 18:32:42 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 18:32:42 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 02 Aug 2022 18:32:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 02 Aug 2022 18:33:28 GMT
ARG MARIADB_MAJOR=10.8
# Tue, 02 Aug 2022 18:33:29 GMT
ENV MARIADB_MAJOR=10.8
# Tue, 02 Aug 2022 18:33:30 GMT
ARG MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 02 Aug 2022 18:33:31 GMT
ENV MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 02 Aug 2022 18:33:32 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
# Tue, 02 Aug 2022 18:33:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 02 Aug 2022 18:33:52 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 02 Aug 2022 18:33:53 GMT
VOLUME [/var/lib/mysql]
# Tue, 02 Aug 2022 18:33:54 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 02 Aug 2022 18:33:55 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 02 Aug 2022 18:33:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 18:33:56 GMT
EXPOSE 3306
# Tue, 02 Aug 2022 18:33:57 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:4a3049d340b7d3651a954fd25a32c42feb1086889d6287e2f15468aef865c5c4`  
		Last Modified: Tue, 02 Aug 2022 01:20:49 GMT  
		Size: 28.4 MB (28381155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e5bedaed5f8e5343fee312eb2f21894d7b4026a0c692da89fe4f30a432e48b4`  
		Last Modified: Tue, 02 Aug 2022 18:41:32 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f07d81dfa02553c544d772dc3aa04ed6a2e6ad5b810ca742eee9a918786e5f`  
		Last Modified: Tue, 02 Aug 2022 18:41:30 GMT  
		Size: 3.6 MB (3594051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd6b8a20cb609d07274a17b8dd4ae810b6a98f76cf0ad513aa0c03eda46fcbce`  
		Last Modified: Tue, 02 Aug 2022 18:41:30 GMT  
		Size: 1.9 MB (1899200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3d39cfcf2768f9c1165cc0d3764c3649542f541a1ed3f18bec6283d58553e00`  
		Last Modified: Tue, 02 Aug 2022 18:41:30 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d230566e80222a9242f97419a6018684f4e324420ee89e4c0395f8107a124c91`  
		Last Modified: Tue, 02 Aug 2022 18:41:30 GMT  
		Size: 2.2 MB (2211614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c8c9abaef706c6185822ae21205ab5bc569494c4492a89eef44d8a855315c5`  
		Last Modified: Tue, 02 Aug 2022 18:41:27 GMT  
		Size: 2.5 KB (2465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9bff43ba5b5f6479659a8a7496d4156615c3cd9439c46779dd3feed3c4511ae`  
		Last Modified: Tue, 02 Aug 2022 18:41:57 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08cb73ef10f93c31f677c6818187b24c6bb65b4cb76ad5ed05e5b31853ef1b73`  
		Last Modified: Tue, 02 Aug 2022 18:42:08 GMT  
		Size: 66.4 MB (66369985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b16804fca7957e5cc3538c9a1a58af3e8e7a9eb0ee3318ffa413c7ebf4c76d4`  
		Last Modified: Tue, 02 Aug 2022 18:41:57 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fffad21dfd527f8685de9b3c864738e88bb8791db49ecdeb988d9d194a20d7cc`  
		Last Modified: Tue, 02 Aug 2022 18:41:57 GMT  
		Size: 6.7 KB (6699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; ppc64le

```console
$ docker pull mariadb@sha256:017f8f45233c3bb9128302760d3c66df5253d31744a6e7401125b14233028d3a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.8 MB (116844233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf24d5b9794e7b70a566d82d3aa538d3b1657c23f08249227462a909b294c582`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 02 Aug 2022 01:31:12 GMT
ADD file:b6916c28c03568df4c2efc3da91ea6320f639cdbd2fa3f6741fcea7acad4fd5f in / 
# Tue, 02 Aug 2022 01:31:14 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 04:30:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 03 Aug 2022 04:30:30 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 04:30:31 GMT
ENV GOSU_VERSION=1.14
# Wed, 03 Aug 2022 04:30:49 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 03 Aug 2022 04:30:50 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 03 Aug 2022 04:31:03 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 04:31:03 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 03 Aug 2022 04:31:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 03 Aug 2022 04:32:26 GMT
ARG MARIADB_MAJOR=10.8
# Wed, 03 Aug 2022 04:32:26 GMT
ENV MARIADB_MAJOR=10.8
# Wed, 03 Aug 2022 04:32:26 GMT
ARG MARIADB_VERSION=1:10.8.3+maria~jammy
# Wed, 03 Aug 2022 04:32:27 GMT
ENV MARIADB_VERSION=1:10.8.3+maria~jammy
# Wed, 03 Aug 2022 04:32:27 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
# Wed, 03 Aug 2022 04:32:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 03 Aug 2022 04:33:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 03 Aug 2022 04:33:11 GMT
VOLUME [/var/lib/mysql]
# Wed, 03 Aug 2022 04:33:11 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Wed, 03 Aug 2022 04:33:12 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Wed, 03 Aug 2022 04:33:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 Aug 2022 04:33:12 GMT
EXPOSE 3306
# Wed, 03 Aug 2022 04:33:13 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:6f8c2fc0a4f976c1c0bd1c0e14022b3ed8b7c83cdb247c83016052c3678aaf28`  
		Last Modified: Tue, 02 Aug 2022 01:33:53 GMT  
		Size: 35.7 MB (35718004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da4a119144d25c65194f5210a2c0785d96c4b9d92c955f354d54e971b66cf0f`  
		Last Modified: Wed, 03 Aug 2022 04:43:49 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06895bfe56d4b1ebe076e361e483fe6fc6bfbaeb765ae25852c1993a6943452c`  
		Last Modified: Wed, 03 Aug 2022 04:43:47 GMT  
		Size: 4.5 MB (4503176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ee69296533cbe8c0bf533fa14d2f744068f58d5998026a4ba0c82bf9ea828ca`  
		Last Modified: Wed, 03 Aug 2022 04:43:47 GMT  
		Size: 1.9 MB (1921808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e76647cede58c06588416f8c141f66a1bf687145f5a0b0b2c530cdc63b14c805`  
		Last Modified: Wed, 03 Aug 2022 04:43:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b9befa094840721fea90813c85958f817ad561e93636ebd0730a9a395a0b46a`  
		Last Modified: Wed, 03 Aug 2022 04:43:47 GMT  
		Size: 2.4 MB (2404905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f92e1e86f56f2fadd73fdf7cc3428ca6687fbfa29af810bdb5c43b92ab77d02`  
		Last Modified: Wed, 03 Aug 2022 04:43:44 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b92a0e7592d7a0ad15eb1a53b8fcda1b2bb13d5dc516094d233fc4e8d23f53`  
		Last Modified: Wed, 03 Aug 2022 04:44:25 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c0e53f407a9d9f4fdfdb556976d3e976f93310c77b48124319cd55841b06ac`  
		Last Modified: Wed, 03 Aug 2022 04:44:43 GMT  
		Size: 72.3 MB (72281444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a525304ab204f12f8e1da79b296cd25e4eeda97bab0a3c0b8b21d27624c824c`  
		Last Modified: Wed, 03 Aug 2022 04:44:24 GMT  
		Size: 3.5 KB (3488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759170fa57f07b1b2ffc7f1dc434234f5446e9b18b7a5bb4bc1edbea87035db4`  
		Last Modified: Wed, 03 Aug 2022 04:44:24 GMT  
		Size: 6.7 KB (6694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; s390x

```console
$ docker pull mariadb@sha256:12097ab474fe2ee789b394e1e8a6b489f2ca4ce5ebc8904a14cfddeedb17b8e5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (104979316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d95792c9ef5a984b01f32025b66c1495e316d034e94d5975da4069d260d40064`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 02 Aug 2022 01:02:17 GMT
ADD file:d5a5e56e0ca8287f27b257e3ddbc9675a1bdac1912afbbab6cddd891056cd144 in / 
# Tue, 02 Aug 2022 01:02:19 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 12:55:49 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 02 Aug 2022 12:56:06 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 12:56:07 GMT
ENV GOSU_VERSION=1.14
# Tue, 02 Aug 2022 12:56:16 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 02 Aug 2022 12:56:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 02 Aug 2022 12:56:22 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 12:56:22 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 02 Aug 2022 12:56:23 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 02 Aug 2022 12:57:08 GMT
ARG MARIADB_MAJOR=10.8
# Tue, 02 Aug 2022 12:57:08 GMT
ENV MARIADB_MAJOR=10.8
# Tue, 02 Aug 2022 12:57:08 GMT
ARG MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 02 Aug 2022 12:57:08 GMT
ENV MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 02 Aug 2022 12:57:09 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
# Tue, 02 Aug 2022 12:57:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 02 Aug 2022 12:57:31 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 02 Aug 2022 12:57:38 GMT
VOLUME [/var/lib/mysql]
# Tue, 02 Aug 2022 12:57:38 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 02 Aug 2022 12:57:38 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 02 Aug 2022 12:57:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 12:57:39 GMT
EXPOSE 3306
# Tue, 02 Aug 2022 12:57:39 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:f97967c51aac02138b615522a1bab9c75addd5896f43ade17ddaac44e0644283`  
		Last Modified: Tue, 02 Aug 2022 01:03:51 GMT  
		Size: 28.6 MB (28642785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:518030038f927b55f39a26dbee5d8d6e8c31cc0ddf7f23268b3dee3f001182c2`  
		Last Modified: Tue, 02 Aug 2022 13:01:03 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c5074a746c3e8a07e66d2d76ac4a7b9e0af6ffbf0cc8a87f601bb8b6913662`  
		Last Modified: Tue, 02 Aug 2022 13:01:02 GMT  
		Size: 3.7 MB (3675041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6140902b730422bc6cad80b27cf9005104adc5047e2e34955e4fbb5cf7d394`  
		Last Modified: Tue, 02 Aug 2022 13:01:02 GMT  
		Size: 2.0 MB (1955931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67105478e75b1563365dc4986a18198b1230a86bb142ade80fa52d1f71e2b6d7`  
		Last Modified: Tue, 02 Aug 2022 13:01:02 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af39a56c0cc78baeec34ac8d7b93879b9b0878bfcc89737ffecf164a865bd46b`  
		Last Modified: Tue, 02 Aug 2022 13:01:02 GMT  
		Size: 2.2 MB (2216654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c8957d63d730d9dbe5d508e565371ce9f1a318e16ad05c720373da4dbbe208`  
		Last Modified: Tue, 02 Aug 2022 13:01:00 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5461cdd4f49c09bdda524801b26ccc244a1f3b4daa635e39c8d982532b8646d7`  
		Last Modified: Tue, 02 Aug 2022 13:01:21 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c9a941eeee8bd3fcf6d0504466a69f3b30632b6d14fed1f53bc29439ded147`  
		Last Modified: Tue, 02 Aug 2022 13:01:30 GMT  
		Size: 68.5 MB (68473998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7458611c3efeaaf589463cdc0dff355cd54d57b45ece924dd1f1e136b26ef8dc`  
		Last Modified: Tue, 02 Aug 2022 13:01:21 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf3286637af3a581d1537b503e2b8404768d5a37566247553295844ea4b760d`  
		Last Modified: Tue, 02 Aug 2022 13:01:21 GMT  
		Size: 6.7 KB (6699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
