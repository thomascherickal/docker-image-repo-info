<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mariadb`

-	[`mariadb:10`](#mariadb10)
-	[`mariadb:10-jammy`](#mariadb10-jammy)
-	[`mariadb:10.2`](#mariadb102)
-	[`mariadb:10.2-bionic`](#mariadb102-bionic)
-	[`mariadb:10.2.44`](#mariadb10244)
-	[`mariadb:10.2.44-bionic`](#mariadb10244-bionic)
-	[`mariadb:10.3`](#mariadb103)
-	[`mariadb:10.3-focal`](#mariadb103-focal)
-	[`mariadb:10.3.35`](#mariadb10335)
-	[`mariadb:10.3.35-focal`](#mariadb10335-focal)
-	[`mariadb:10.4`](#mariadb104)
-	[`mariadb:10.4-focal`](#mariadb104-focal)
-	[`mariadb:10.4.25`](#mariadb10425)
-	[`mariadb:10.4.25-focal`](#mariadb10425-focal)
-	[`mariadb:10.5`](#mariadb105)
-	[`mariadb:10.5-focal`](#mariadb105-focal)
-	[`mariadb:10.5.16`](#mariadb10516)
-	[`mariadb:10.5.16-focal`](#mariadb10516-focal)
-	[`mariadb:10.6`](#mariadb106)
-	[`mariadb:10.6-focal`](#mariadb106-focal)
-	[`mariadb:10.6.8`](#mariadb1068)
-	[`mariadb:10.6.8-focal`](#mariadb1068-focal)
-	[`mariadb:10.7`](#mariadb107)
-	[`mariadb:10.7-focal`](#mariadb107-focal)
-	[`mariadb:10.7.4`](#mariadb1074)
-	[`mariadb:10.7.4-focal`](#mariadb1074-focal)
-	[`mariadb:10.8`](#mariadb108)
-	[`mariadb:10.8-jammy`](#mariadb108-jammy)
-	[`mariadb:10.8.3`](#mariadb1083)
-	[`mariadb:10.8.3-jammy`](#mariadb1083-jammy)
-	[`mariadb:10.9-rc`](#mariadb109-rc)
-	[`mariadb:10.9-rc-jammy`](#mariadb109-rc-jammy)
-	[`mariadb:10.9.1-rc`](#mariadb1091-rc)
-	[`mariadb:10.9.1-rc-jammy`](#mariadb1091-rc-jammy)
-	[`mariadb:jammy`](#mariadbjammy)
-	[`mariadb:latest`](#mariadblatest)

## `mariadb:10`

```console
$ docker pull mariadb@sha256:88fcb7d92c7f61cd885c4d309c98461f3607aa6dbd57a2474be86e1956b36d13
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10` - linux; amd64

```console
$ docker pull mariadb@sha256:483a080b5bcdf0a898ef4574209080f7a42896c7134c60c55b4d4cb5ab3a8d6f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.9 MB (123859860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea81af801379dae14e596b55612f355a63cfca2ed53cf27d047340f4890cf25c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:25 GMT
ADD file:11157b07dde10107f3f6f2b892c869ea83868475d5825167b5f466a7e410eb05 in / 
# Mon, 06 Jun 2022 22:21:26 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:40:40 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 00:40:56 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:40:56 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 00:41:06 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 00:41:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 00:41:13 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:41:13 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 00:41:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 00:42:02 GMT
ARG MARIADB_MAJOR=10.8
# Tue, 07 Jun 2022 00:42:03 GMT
ENV MARIADB_MAJOR=10.8
# Tue, 07 Jun 2022 00:42:03 GMT
ARG MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 07 Jun 2022 00:42:03 GMT
ENV MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 07 Jun 2022 00:42:03 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
# Tue, 07 Jun 2022 00:42:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 00:42:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 00:42:23 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 00:42:23 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 00:42:23 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 07 Jun 2022 00:42:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 00:42:23 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 00:42:23 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:405f018f9d1d0f351c196b841a7c7f226fb8ea448acd6339a9ed8741600275a2`  
		Last Modified: Wed, 01 Jun 2022 03:03:39 GMT  
		Size: 30.4 MB (30423715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a85079b8234f1744aeed618170b84c2f6b970a320e10616ff031d3be24b5cd4`  
		Last Modified: Tue, 07 Jun 2022 00:47:43 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:579c7ff691b1abc2640eb61104ca92a223103daf11214a248cc580163536e70d`  
		Last Modified: Tue, 07 Jun 2022 00:47:42 GMT  
		Size: 3.8 MB (3765124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4976663b5d6daa78634cc56c60cb837f47e79832759e9bdb8f1c592b194411bf`  
		Last Modified: Tue, 07 Jun 2022 00:47:42 GMT  
		Size: 2.0 MB (1991845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:169024b1fb136785c2ed5f758e9707ce456f38d8007d568f863be47b0873afd7`  
		Last Modified: Tue, 07 Jun 2022 00:47:41 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ffe8ce897f6bfdab5ac2fa06b95c2a6187161ced620b3b00e71b31e7b75e47`  
		Last Modified: Tue, 07 Jun 2022 00:47:42 GMT  
		Size: 2.3 MB (2297483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b583c09d23c314a64c34258bda89aaefc6c4b3a488297892863af1dd61bb4113`  
		Last Modified: Tue, 07 Jun 2022 00:47:39 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b9f0c08d08f4ae53297606d8c0aea35c96566d2e544a8a32efb72eebc3749b6`  
		Last Modified: Tue, 07 Jun 2022 00:48:08 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cd51f98458654de3ea7c535ee562e9f9251fd6a0818629346bcadaaa768b71a`  
		Last Modified: Tue, 07 Jun 2022 00:48:20 GMT  
		Size: 85.4 MB (85366786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f506bb8acafbb672f41df13b1d99173b9217140c8137ecc9daec14c4e00f70`  
		Last Modified: Tue, 07 Jun 2022 00:48:08 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d689f79ba4ea066cd24d5c7f7ae294a524fc166bb7f9e8b60d48472f35277a`  
		Last Modified: Tue, 07 Jun 2022 00:48:08 GMT  
		Size: 6.7 KB (6699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:b6764b02b5eb8d6274207dbb827317cafc8694c1505185aa092d5551f8a793f2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.5 MB (104543896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecc004eed0c26ad5c4e0d75baff2cb4e7fdc144f713d053c256f6455b608d280`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:52 GMT
ADD file:1e18e22e32f06a7e93275cf3a2eb2a1d3892be27628bdae2de4b2aadb992bd50 in / 
# Fri, 29 Apr 2022 22:49:53 GMT
CMD ["bash"]
# Mon, 23 May 2022 18:40:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Mon, 23 May 2022 18:40:25 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 23 May 2022 18:40:26 GMT
ENV GOSU_VERSION=1.14
# Mon, 23 May 2022 18:40:43 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 23 May 2022 18:40:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 23 May 2022 18:40:53 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 23 May 2022 18:40:53 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Mon, 23 May 2022 18:40:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Mon, 23 May 2022 18:41:40 GMT
ARG MARIADB_MAJOR=10.8
# Mon, 23 May 2022 18:41:41 GMT
ENV MARIADB_MAJOR=10.8
# Mon, 23 May 2022 18:41:42 GMT
ARG MARIADB_VERSION=1:10.8.3+maria~jammy
# Mon, 23 May 2022 18:41:43 GMT
ENV MARIADB_VERSION=1:10.8.3+maria~jammy
# Mon, 23 May 2022 18:41:44 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
# Mon, 23 May 2022 18:41:45 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 23 May 2022 18:42:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 23 May 2022 18:42:04 GMT
VOLUME [/var/lib/mysql]
# Mon, 23 May 2022 18:42:06 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Mon, 23 May 2022 18:42:07 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Mon, 23 May 2022 18:42:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 18:42:08 GMT
EXPOSE 3306
# Mon, 23 May 2022 18:42:09 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:b84950154c181a602d2e93b68e84660f96dc78f94ae36f3df2db8d5701abb6a5`  
		Last Modified: Fri, 29 Apr 2022 22:52:07 GMT  
		Size: 28.4 MB (28376457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ae07faadba444656d4d080edc85dcaba97c3ac8f3ac415b136c2add7ff5393`  
		Last Modified: Mon, 23 May 2022 18:47:26 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46428e702eff2922592a3c96fbe5e3764cbca14a5a770718e36a51ad4c9dc906`  
		Last Modified: Mon, 23 May 2022 18:47:25 GMT  
		Size: 3.6 MB (3592731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e775e0ed5a0037f1c4cce3ef74f7025c80ec7e27e1e60a27c1f39d53e944c75`  
		Last Modified: Mon, 23 May 2022 18:47:25 GMT  
		Size: 4.0 MB (4014468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:031c54d0d9d9d4a999c13ba6733390868914e2c9c66b3ee2feb98e2a93de5d99`  
		Last Modified: Mon, 23 May 2022 18:47:24 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602265dc68e116e160f1e4da3863e9ff8313798a78e0d68554915d7cb1d970b9`  
		Last Modified: Mon, 23 May 2022 18:47:25 GMT  
		Size: 2.2 MB (2210433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d1d131fb6cb45f460fd0eb002edad2f1273dd1d769fff5ad071a2356a239edc`  
		Last Modified: Mon, 23 May 2022 18:47:22 GMT  
		Size: 2.5 KB (2470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a33ea1b30434b058f9b0ea3af9c9638014b6e11714eaa4888fceb806344fe49`  
		Last Modified: Mon, 23 May 2022 18:47:50 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9539c6148f07eaa2bb03fae3339771575a22824c8b4d9a6ab5cc10210d114a0c`  
		Last Modified: Mon, 23 May 2022 18:48:01 GMT  
		Size: 66.3 MB (66334981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38aa29868643c4f4f19f60129f5a981a1b09518e1621b1ffdcdf6f06c8261231`  
		Last Modified: Mon, 23 May 2022 18:47:50 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3702214dffba8174c27ba1d8d97eebb416c8b984871b3a18b8c497c26b227a77`  
		Last Modified: Mon, 23 May 2022 18:47:50 GMT  
		Size: 6.7 KB (6700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10` - linux; ppc64le

```console
$ docker pull mariadb@sha256:9f0a93c25897df9a9b2ca3becf35fccdfd9531009c57b1481d8d027f8722dc49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.5 MB (139538393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b9fdde589bdb89bddd62d2076c08de8ca866b15932b15f44b9809efd0a2c54d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:28 GMT
ADD file:55691ac7d76af0fcfafc39ebd1e5a4f2d7018147d6db6f89812db33fbaffc2f9 in / 
# Fri, 29 Apr 2022 23:22:33 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:50:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:52:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:52:19 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:53:06 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:53:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:53:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:53:51 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:54:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:59:29 GMT
ARG MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 00:59:47 GMT
ENV MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 00:59:55 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Sat, 30 Apr 2022 01:00:09 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Sat, 30 Apr 2022 01:00:25 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 01:00:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:03:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:03:59 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:04:00 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:04:02 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:04:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:04:08 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:04:10 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:e9c0a77cb9f0f7330e3fc62254e4c8ae89ed4bba21209fdc1088195250f950b9`  
		Last Modified: Fri, 29 Apr 2022 23:25:23 GMT  
		Size: 33.3 MB (33290661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933fb2862e2716afd28ee38ed71eb9097a647fd38b4378b802ba4928e819c444`  
		Last Modified: Sat, 30 Apr 2022 01:20:57 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6899bc35ca339b1fbd966c280b0f1a2c3acd469ad358d3b3f48b1e6a1b7bd5`  
		Last Modified: Sat, 30 Apr 2022 01:20:56 GMT  
		Size: 6.7 MB (6667588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185278c53367843a392ed443f9de142076add930e26c0765cd604902e7e0026f`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 3.7 MB (3672592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356d5cab0b98f71595c34fffd4c19a0d48f05279ac84eb9068b1090bafb87d6f`  
		Last Modified: Sat, 30 Apr 2022 01:20:54 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd37e664a57394de1d81b89e36f57a4318e77c9dcbd17a16966cc7924f323fa`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 2.6 MB (2568397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bc301781015b0c1df07f994700ffdfde0f31a2be7b1063ae698b5280f77aa5`  
		Last Modified: Sat, 30 Apr 2022 01:20:51 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c38d1aea9df71e0e7b7a07ebbf73d3df047d6925b8517612731ce14b29d81e6f`  
		Last Modified: Sat, 30 Apr 2022 01:21:32 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219c8b280b85bfcb106c1c23cb4f820d20c27c361c26bc4b7b20b972ae0e550d`  
		Last Modified: Sat, 30 Apr 2022 01:21:50 GMT  
		Size: 93.3 MB (93324167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7ca5c34dd9a2fb0cbcf95168f69c6aa33df79bce1e843d573af62fc0ca0bf60`  
		Last Modified: Sat, 30 Apr 2022 01:21:32 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86ec7c5c6f4af575453b8a299723e99a51c614cf4d411dc507c8c4970ecaf71`  
		Last Modified: Sat, 30 Apr 2022 01:21:32 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10` - linux; s390x

```console
$ docker pull mariadb@sha256:a9c536d0da138dacf56fd611cd76171a5e7f21b2c254495939f45200a2d2ec7e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (104950766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fad948eb6c3a1c6724e95ac01927251304a6d53ddb9014a73f6964b6092b994`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 07 Jun 2022 04:05:41 GMT
ADD file:5412b0d16961079a78b96411ca23f1838ac09c2fae839829476380b5389e49f8 in / 
# Tue, 07 Jun 2022 04:05:45 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:46:42 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 06:46:54 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:46:55 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 06:47:15 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 06:47:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 06:47:27 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:47:27 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 06:47:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 06:48:14 GMT
ARG MARIADB_MAJOR=10.8
# Tue, 07 Jun 2022 06:48:15 GMT
ENV MARIADB_MAJOR=10.8
# Tue, 07 Jun 2022 06:48:15 GMT
ARG MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 07 Jun 2022 06:48:15 GMT
ENV MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 07 Jun 2022 06:48:15 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
# Tue, 07 Jun 2022 06:48:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 06:48:49 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 06:48:56 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 06:48:56 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 06:48:56 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 07 Jun 2022 06:48:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 06:48:57 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 06:48:57 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:6fa1296f44090f6150dfb96d6ae217a58b9d66c56d7a986c35657df6bd1a89f0`  
		Last Modified: Tue, 07 Jun 2022 04:08:13 GMT  
		Size: 28.6 MB (28638482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e980d0c8e278a504f0f8cb00cbb715bc7239eb7e9e13f635db0c77b7e9625c`  
		Last Modified: Tue, 07 Jun 2022 06:53:30 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec96ea557bfa670cf2072437f6b01b817a185da1ef3e1b694d61b29c5da1561e`  
		Last Modified: Tue, 07 Jun 2022 06:53:29 GMT  
		Size: 3.7 MB (3674855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:726015530ec97a71af69b3bda1ced0b4bbdb013fc074478728335d1c714e1ed0`  
		Last Modified: Tue, 07 Jun 2022 06:53:29 GMT  
		Size: 2.0 MB (1954988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b4bef35a73fc4bcfe6311f2e5045128a3861bcd38b075463b870d13c0967b9`  
		Last Modified: Tue, 07 Jun 2022 06:53:29 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe29a6e8adabddd30630efcb94fa1700cbd3c96aa623c45d34e889d00358fc07`  
		Last Modified: Tue, 07 Jun 2022 06:53:29 GMT  
		Size: 2.2 MB (2215965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3784b0c624b488911de05f153cfb7a59247ee32628f054fc1672d59c993907b8`  
		Last Modified: Tue, 07 Jun 2022 06:53:28 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1811da06c80a8ea4d1138022303a2aee104a2e92377d041edeeea75286fc8df9`  
		Last Modified: Tue, 07 Jun 2022 06:53:50 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b002fb05e958857048b5e3de1eaf8add56ee8be42579108a53beda62649599c`  
		Last Modified: Tue, 07 Jun 2022 06:53:59 GMT  
		Size: 68.5 MB (68451571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12dfba249abcff12b977205f137dffac3b7456bee31377d44e3c935b68ae5e7`  
		Last Modified: Tue, 07 Jun 2022 06:53:50 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fecfeca76a356593a14b01d27c7d0301e7f5b59b14fe638cc7c1b2c0e3dfdeb8`  
		Last Modified: Tue, 07 Jun 2022 06:53:50 GMT  
		Size: 6.7 KB (6694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10-jammy`

```console
$ docker pull mariadb@sha256:8be45db6728d9f755064b1553a20475120a962e49db52dff30f77c487c2da60d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mariadb:10-jammy` - linux; amd64

```console
$ docker pull mariadb@sha256:483a080b5bcdf0a898ef4574209080f7a42896c7134c60c55b4d4cb5ab3a8d6f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.9 MB (123859860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea81af801379dae14e596b55612f355a63cfca2ed53cf27d047340f4890cf25c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:25 GMT
ADD file:11157b07dde10107f3f6f2b892c869ea83868475d5825167b5f466a7e410eb05 in / 
# Mon, 06 Jun 2022 22:21:26 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:40:40 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 00:40:56 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:40:56 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 00:41:06 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 00:41:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 00:41:13 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:41:13 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 00:41:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 00:42:02 GMT
ARG MARIADB_MAJOR=10.8
# Tue, 07 Jun 2022 00:42:03 GMT
ENV MARIADB_MAJOR=10.8
# Tue, 07 Jun 2022 00:42:03 GMT
ARG MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 07 Jun 2022 00:42:03 GMT
ENV MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 07 Jun 2022 00:42:03 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
# Tue, 07 Jun 2022 00:42:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 00:42:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 00:42:23 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 00:42:23 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 00:42:23 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 07 Jun 2022 00:42:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 00:42:23 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 00:42:23 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:405f018f9d1d0f351c196b841a7c7f226fb8ea448acd6339a9ed8741600275a2`  
		Last Modified: Wed, 01 Jun 2022 03:03:39 GMT  
		Size: 30.4 MB (30423715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a85079b8234f1744aeed618170b84c2f6b970a320e10616ff031d3be24b5cd4`  
		Last Modified: Tue, 07 Jun 2022 00:47:43 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:579c7ff691b1abc2640eb61104ca92a223103daf11214a248cc580163536e70d`  
		Last Modified: Tue, 07 Jun 2022 00:47:42 GMT  
		Size: 3.8 MB (3765124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4976663b5d6daa78634cc56c60cb837f47e79832759e9bdb8f1c592b194411bf`  
		Last Modified: Tue, 07 Jun 2022 00:47:42 GMT  
		Size: 2.0 MB (1991845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:169024b1fb136785c2ed5f758e9707ce456f38d8007d568f863be47b0873afd7`  
		Last Modified: Tue, 07 Jun 2022 00:47:41 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ffe8ce897f6bfdab5ac2fa06b95c2a6187161ced620b3b00e71b31e7b75e47`  
		Last Modified: Tue, 07 Jun 2022 00:47:42 GMT  
		Size: 2.3 MB (2297483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b583c09d23c314a64c34258bda89aaefc6c4b3a488297892863af1dd61bb4113`  
		Last Modified: Tue, 07 Jun 2022 00:47:39 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b9f0c08d08f4ae53297606d8c0aea35c96566d2e544a8a32efb72eebc3749b6`  
		Last Modified: Tue, 07 Jun 2022 00:48:08 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cd51f98458654de3ea7c535ee562e9f9251fd6a0818629346bcadaaa768b71a`  
		Last Modified: Tue, 07 Jun 2022 00:48:20 GMT  
		Size: 85.4 MB (85366786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f506bb8acafbb672f41df13b1d99173b9217140c8137ecc9daec14c4e00f70`  
		Last Modified: Tue, 07 Jun 2022 00:48:08 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d689f79ba4ea066cd24d5c7f7ae294a524fc166bb7f9e8b60d48472f35277a`  
		Last Modified: Tue, 07 Jun 2022 00:48:08 GMT  
		Size: 6.7 KB (6699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-jammy` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:b6764b02b5eb8d6274207dbb827317cafc8694c1505185aa092d5551f8a793f2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.5 MB (104543896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecc004eed0c26ad5c4e0d75baff2cb4e7fdc144f713d053c256f6455b608d280`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:52 GMT
ADD file:1e18e22e32f06a7e93275cf3a2eb2a1d3892be27628bdae2de4b2aadb992bd50 in / 
# Fri, 29 Apr 2022 22:49:53 GMT
CMD ["bash"]
# Mon, 23 May 2022 18:40:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Mon, 23 May 2022 18:40:25 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 23 May 2022 18:40:26 GMT
ENV GOSU_VERSION=1.14
# Mon, 23 May 2022 18:40:43 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 23 May 2022 18:40:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 23 May 2022 18:40:53 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 23 May 2022 18:40:53 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Mon, 23 May 2022 18:40:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Mon, 23 May 2022 18:41:40 GMT
ARG MARIADB_MAJOR=10.8
# Mon, 23 May 2022 18:41:41 GMT
ENV MARIADB_MAJOR=10.8
# Mon, 23 May 2022 18:41:42 GMT
ARG MARIADB_VERSION=1:10.8.3+maria~jammy
# Mon, 23 May 2022 18:41:43 GMT
ENV MARIADB_VERSION=1:10.8.3+maria~jammy
# Mon, 23 May 2022 18:41:44 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
# Mon, 23 May 2022 18:41:45 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 23 May 2022 18:42:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 23 May 2022 18:42:04 GMT
VOLUME [/var/lib/mysql]
# Mon, 23 May 2022 18:42:06 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Mon, 23 May 2022 18:42:07 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Mon, 23 May 2022 18:42:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 18:42:08 GMT
EXPOSE 3306
# Mon, 23 May 2022 18:42:09 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:b84950154c181a602d2e93b68e84660f96dc78f94ae36f3df2db8d5701abb6a5`  
		Last Modified: Fri, 29 Apr 2022 22:52:07 GMT  
		Size: 28.4 MB (28376457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ae07faadba444656d4d080edc85dcaba97c3ac8f3ac415b136c2add7ff5393`  
		Last Modified: Mon, 23 May 2022 18:47:26 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46428e702eff2922592a3c96fbe5e3764cbca14a5a770718e36a51ad4c9dc906`  
		Last Modified: Mon, 23 May 2022 18:47:25 GMT  
		Size: 3.6 MB (3592731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e775e0ed5a0037f1c4cce3ef74f7025c80ec7e27e1e60a27c1f39d53e944c75`  
		Last Modified: Mon, 23 May 2022 18:47:25 GMT  
		Size: 4.0 MB (4014468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:031c54d0d9d9d4a999c13ba6733390868914e2c9c66b3ee2feb98e2a93de5d99`  
		Last Modified: Mon, 23 May 2022 18:47:24 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602265dc68e116e160f1e4da3863e9ff8313798a78e0d68554915d7cb1d970b9`  
		Last Modified: Mon, 23 May 2022 18:47:25 GMT  
		Size: 2.2 MB (2210433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d1d131fb6cb45f460fd0eb002edad2f1273dd1d769fff5ad071a2356a239edc`  
		Last Modified: Mon, 23 May 2022 18:47:22 GMT  
		Size: 2.5 KB (2470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a33ea1b30434b058f9b0ea3af9c9638014b6e11714eaa4888fceb806344fe49`  
		Last Modified: Mon, 23 May 2022 18:47:50 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9539c6148f07eaa2bb03fae3339771575a22824c8b4d9a6ab5cc10210d114a0c`  
		Last Modified: Mon, 23 May 2022 18:48:01 GMT  
		Size: 66.3 MB (66334981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38aa29868643c4f4f19f60129f5a981a1b09518e1621b1ffdcdf6f06c8261231`  
		Last Modified: Mon, 23 May 2022 18:47:50 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3702214dffba8174c27ba1d8d97eebb416c8b984871b3a18b8c497c26b227a77`  
		Last Modified: Mon, 23 May 2022 18:47:50 GMT  
		Size: 6.7 KB (6700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-jammy` - linux; s390x

```console
$ docker pull mariadb@sha256:a9c536d0da138dacf56fd611cd76171a5e7f21b2c254495939f45200a2d2ec7e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (104950766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fad948eb6c3a1c6724e95ac01927251304a6d53ddb9014a73f6964b6092b994`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 07 Jun 2022 04:05:41 GMT
ADD file:5412b0d16961079a78b96411ca23f1838ac09c2fae839829476380b5389e49f8 in / 
# Tue, 07 Jun 2022 04:05:45 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:46:42 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 06:46:54 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:46:55 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 06:47:15 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 06:47:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 06:47:27 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:47:27 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 06:47:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 06:48:14 GMT
ARG MARIADB_MAJOR=10.8
# Tue, 07 Jun 2022 06:48:15 GMT
ENV MARIADB_MAJOR=10.8
# Tue, 07 Jun 2022 06:48:15 GMT
ARG MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 07 Jun 2022 06:48:15 GMT
ENV MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 07 Jun 2022 06:48:15 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
# Tue, 07 Jun 2022 06:48:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 06:48:49 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 06:48:56 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 06:48:56 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 06:48:56 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 07 Jun 2022 06:48:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 06:48:57 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 06:48:57 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:6fa1296f44090f6150dfb96d6ae217a58b9d66c56d7a986c35657df6bd1a89f0`  
		Last Modified: Tue, 07 Jun 2022 04:08:13 GMT  
		Size: 28.6 MB (28638482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e980d0c8e278a504f0f8cb00cbb715bc7239eb7e9e13f635db0c77b7e9625c`  
		Last Modified: Tue, 07 Jun 2022 06:53:30 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec96ea557bfa670cf2072437f6b01b817a185da1ef3e1b694d61b29c5da1561e`  
		Last Modified: Tue, 07 Jun 2022 06:53:29 GMT  
		Size: 3.7 MB (3674855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:726015530ec97a71af69b3bda1ced0b4bbdb013fc074478728335d1c714e1ed0`  
		Last Modified: Tue, 07 Jun 2022 06:53:29 GMT  
		Size: 2.0 MB (1954988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b4bef35a73fc4bcfe6311f2e5045128a3861bcd38b075463b870d13c0967b9`  
		Last Modified: Tue, 07 Jun 2022 06:53:29 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe29a6e8adabddd30630efcb94fa1700cbd3c96aa623c45d34e889d00358fc07`  
		Last Modified: Tue, 07 Jun 2022 06:53:29 GMT  
		Size: 2.2 MB (2215965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3784b0c624b488911de05f153cfb7a59247ee32628f054fc1672d59c993907b8`  
		Last Modified: Tue, 07 Jun 2022 06:53:28 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1811da06c80a8ea4d1138022303a2aee104a2e92377d041edeeea75286fc8df9`  
		Last Modified: Tue, 07 Jun 2022 06:53:50 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b002fb05e958857048b5e3de1eaf8add56ee8be42579108a53beda62649599c`  
		Last Modified: Tue, 07 Jun 2022 06:53:59 GMT  
		Size: 68.5 MB (68451571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12dfba249abcff12b977205f137dffac3b7456bee31377d44e3c935b68ae5e7`  
		Last Modified: Tue, 07 Jun 2022 06:53:50 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fecfeca76a356593a14b01d27c7d0301e7f5b59b14fe638cc7c1b2c0e3dfdeb8`  
		Last Modified: Tue, 07 Jun 2022 06:53:50 GMT  
		Size: 6.7 KB (6694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2`

```console
$ docker pull mariadb@sha256:b7c94079802d8c85d67d77305de520cfa8a6eee9d7fd735845345c18a67dc805
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2` - linux; amd64

```console
$ docker pull mariadb@sha256:4838b9eb45b62843192d19e4204d05ccef90ee4ae2216c8ee06d220070f233ec
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.3 MB (109334465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6851bb0ecffe34347de2e4bbbaa0fe9ae243b19760674d35c03aacc70a319f4d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:04 GMT
ADD file:40290d9a94ae76c35ab1f57178130ce1c5b976e34a91e77472ecf7e945ab64f9 in / 
# Mon, 06 Jun 2022 22:21:05 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:45:42 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 00:45:51 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:45:51 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 00:46:04 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 00:46:04 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 00:46:12 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:46:12 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 00:46:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 00:46:13 GMT
ARG MARIADB_MAJOR=10.2
# Tue, 07 Jun 2022 00:46:13 GMT
ENV MARIADB_MAJOR=10.2
# Tue, 07 Jun 2022 00:46:13 GMT
ARG MARIADB_VERSION=1:10.2.44+maria~bionic
# Tue, 07 Jun 2022 00:46:13 GMT
ENV MARIADB_VERSION=1:10.2.44+maria~bionic
# Tue, 07 Jun 2022 00:46:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.44/repo/ubuntu/ bionic main
# Tue, 07 Jun 2022 00:46:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.44/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 00:46:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.44/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 00:46:52 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 00:46:52 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 00:46:52 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Tue, 07 Jun 2022 00:46:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.44/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 07 Jun 2022 00:46:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 00:46:53 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 00:46:53 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:09db6f815738b9c8f25420c47e093f89abaabaa653f9678587b57e8f4400b5ff`  
		Last Modified: Wed, 01 Jun 2022 21:51:21 GMT  
		Size: 26.7 MB (26711626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4807eae0721dbd9932b407dc5d98dc58f2e06513813b4fca2712a92a15b86689`  
		Last Modified: Tue, 07 Jun 2022 00:51:21 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac4d47b6011a1f00d7b234da4777bd0e83179924772c19ccf284bf6af12c4b58`  
		Last Modified: Tue, 07 Jun 2022 00:51:22 GMT  
		Size: 4.8 MB (4817768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e00b950b062eb928bdd8038c2a4500a0b383888e13d5b44c80daca4b4e2f7726`  
		Last Modified: Tue, 07 Jun 2022 00:51:19 GMT  
		Size: 3.6 MB (3553828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f97dc9289c3d74b5fe3e1e62414caa678ed61ad1b33e1b4a1f11ca0167564ac`  
		Last Modified: Tue, 07 Jun 2022 00:51:18 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97255914ba4732e73cf80e7db7e9dc3a4bc2d527bbcfd51eae1f3e65f907a2e6`  
		Last Modified: Tue, 07 Jun 2022 00:51:19 GMT  
		Size: 1.6 MB (1583760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6840b0cb638bc582977a5a9af0b429474bbfa6934e87215358ebb262955d5e2`  
		Last Modified: Tue, 07 Jun 2022 00:51:19 GMT  
		Size: 2.5 KB (2488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f37547518f9f02a2e2aaf92dc69f9e7d4d5ab2027ed99192c36b6562ebd48b8`  
		Last Modified: Tue, 07 Jun 2022 00:51:16 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2971e73bb99cc4318b313d0ec9e62d37eac52fad19bdb075544b8ee089224b36`  
		Last Modified: Tue, 07 Jun 2022 00:51:27 GMT  
		Size: 72.7 MB (72652336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c48b57f36a4248042242ac1dfa4345c9cce6f515155bb7a95a94099f05e1062e`  
		Last Modified: Tue, 07 Jun 2022 00:51:16 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bec65571c7e23e3216197998a553bfe6781ed026bccaae95a7e674d163b4360`  
		Last Modified: Tue, 07 Jun 2022 00:51:16 GMT  
		Size: 6.7 KB (6694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2918faba8f77eb2e5367c5b34d8caf9756c4798e7561dd00a5e57d426d60baa7`  
		Last Modified: Tue, 07 Jun 2022 00:51:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:e9720f678d59c5a35fdec63dd9db8de5925355d47c7f6329f0ad8692918ec0f5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.3 MB (104282083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:add1daf576ef2aa23b79c70e43fab60541b1ad409ae9dd9c48f61f04680e6d1b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:26 GMT
ADD file:78300bda9e889eaa778190cac0e569ff379d5e533e86b086248476e6ba9b4b2d in / 
# Fri, 29 Apr 2022 22:49:26 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:08:34 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:08:46 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:08:46 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:09:03 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:09:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:09:12 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:09:13 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:09:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:09:16 GMT
ARG MARIADB_MAJOR=10.2
# Sat, 30 Apr 2022 00:09:17 GMT
ENV MARIADB_MAJOR=10.2
# Mon, 23 May 2022 18:45:29 GMT
ARG MARIADB_VERSION=1:10.2.44+maria~bionic
# Mon, 23 May 2022 18:45:30 GMT
ENV MARIADB_VERSION=1:10.2.44+maria~bionic
# Mon, 23 May 2022 18:45:31 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.44/repo/ubuntu/ bionic main
# Mon, 23 May 2022 18:45:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.44/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 23 May 2022 18:46:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.44/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 23 May 2022 18:46:03 GMT
VOLUME [/var/lib/mysql]
# Mon, 23 May 2022 18:46:04 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Mon, 23 May 2022 18:46:05 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Mon, 23 May 2022 18:46:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.44/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 23 May 2022 18:46:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 18:46:07 GMT
EXPOSE 3306
# Mon, 23 May 2022 18:46:08 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e196da37f904f62d236ea302bf13ba07711cc62b35774f86ecda18bcc9ed57c6`  
		Last Modified: Fri, 29 Apr 2022 22:51:14 GMT  
		Size: 23.7 MB (23735089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ddffcde8b39b72c10cbcd5d96f2307b6d6857369d4a57beb67277bd9f18aedc`  
		Last Modified: Sat, 30 Apr 2022 00:14:32 GMT  
		Size: 1.9 KB (1854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed99cb2e83bbae3472b1b2ab68249e1c7dec481cc489c7d69b2627706d3058e7`  
		Last Modified: Sat, 30 Apr 2022 00:14:32 GMT  
		Size: 4.3 MB (4261792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:745c5d6a542769b03497a41228d4f31506c746d9f5ec5bf393f426c2a27c815b`  
		Last Modified: Sat, 30 Apr 2022 00:14:30 GMT  
		Size: 3.2 MB (3207565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8e8f86c5634b4f012cd1f27e537c696a24e4c684810681da4d92d4f232d43a`  
		Last Modified: Sat, 30 Apr 2022 00:14:29 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2279bacf1382c4ea4fafacc8f579b65d5e2c3949c934e3d1c3efe6fab90ec2cf`  
		Last Modified: Sat, 30 Apr 2022 00:14:30 GMT  
		Size: 1.5 MB (1530621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e032a6d669d1fd06479b50389ac1237c010ebdc2fe3008e47c9c210355e610`  
		Last Modified: Sat, 30 Apr 2022 00:14:29 GMT  
		Size: 5.1 KB (5145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8642d3e9a0c45bbba9e78ed2a84f158e9eb4c7be818dfe7963fa5bdfbb9a5b27`  
		Last Modified: Mon, 23 May 2022 18:51:14 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c4271ff6b8dceba8be6c8563d23152c01bdbe9101ebbe661d61aee10662970`  
		Last Modified: Mon, 23 May 2022 18:51:25 GMT  
		Size: 71.5 MB (71529264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5549de856ddfae43ac8ca443c50d292801362822c16c3fcec716472a6a2d40b1`  
		Last Modified: Mon, 23 May 2022 18:51:14 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d5ea630f979a85ef2066038f1b9a1e77b12ba3235f495a8b5be1983dda3f5e`  
		Last Modified: Mon, 23 May 2022 18:51:14 GMT  
		Size: 6.7 KB (6694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffab573772b47c39377a3828310a236d0297612867a74e7a36b9e1db30fa0370`  
		Last Modified: Mon, 23 May 2022 18:51:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2` - linux; ppc64le

```console
$ docker pull mariadb@sha256:df96ea3a0e5f539059056499b3d5bd9b1a58ac1dc516575432502ede74330534
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117736745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c8b59d225add3e463a7a63174b1268a09b842b8d97f131118683047b89bfbbb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 07 Jun 2022 05:45:31 GMT
ADD file:00feca269255d07b1ddb816beb48357c556d80ab79aa81bc448abc4271d845a5 in / 
# Tue, 07 Jun 2022 05:45:36 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 09:11:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 09:12:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 09:12:28 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 09:13:09 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 09:13:16 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 09:13:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 09:13:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 09:13:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 09:13:52 GMT
ARG MARIADB_MAJOR=10.2
# Tue, 07 Jun 2022 09:13:55 GMT
ENV MARIADB_MAJOR=10.2
# Tue, 07 Jun 2022 09:13:57 GMT
ARG MARIADB_VERSION=1:10.2.44+maria~bionic
# Tue, 07 Jun 2022 09:13:58 GMT
ENV MARIADB_VERSION=1:10.2.44+maria~bionic
# Tue, 07 Jun 2022 09:14:00 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.44/repo/ubuntu/ bionic main
# Tue, 07 Jun 2022 09:14:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.44/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 09:15:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.44/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 09:15:45 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 09:15:46 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 09:15:46 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Tue, 07 Jun 2022 09:15:52 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.44/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 07 Jun 2022 09:15:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 09:16:01 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 09:16:04 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:868ede65862ecf99802bf8944efd378ff1e0751772424cea9084f390deb9f9b2`  
		Last Modified: Tue, 07 Jun 2022 05:48:49 GMT  
		Size: 30.4 MB (30442859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:983cdbbe432683ab8ba3c017f72ff80175ca4f2cdff7d89fb09211b290fa1644`  
		Last Modified: Tue, 07 Jun 2022 09:20:48 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:747b92057fb659c561654f06015a8e02c6b1952f9825371a829861344798ed2e`  
		Last Modified: Tue, 07 Jun 2022 09:20:49 GMT  
		Size: 5.6 MB (5634399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f19dea4ef2503888b21d5a804fb82b4d1b34d7532fe310b079c2acc4d4a23b`  
		Last Modified: Tue, 07 Jun 2022 09:20:47 GMT  
		Size: 3.5 MB (3533925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913fdf09fb6c1d2ee1c333be0f85426ef3a9d46646c1f9077c326672e1f1ca1d`  
		Last Modified: Tue, 07 Jun 2022 09:20:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7707c5204fd4cc2e12dae7367c954e54da990936847175a7cddd179225f8dd14`  
		Last Modified: Tue, 07 Jun 2022 09:20:46 GMT  
		Size: 1.9 MB (1940554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27faa63dfc3a0a16f955fa69f467c27a9f64a189f03cac2e3d4596ebb1e4f2da`  
		Last Modified: Tue, 07 Jun 2022 09:20:45 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2612d482d53133c57a5cb5a320876d66ff2746a205ad91d3777bf8d3c8efe941`  
		Last Modified: Tue, 07 Jun 2022 09:20:43 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba91e76f328f469e4eba02d49d3a226939f79dd8e115f349dfae63940f34e61`  
		Last Modified: Tue, 07 Jun 2022 09:20:57 GMT  
		Size: 76.2 MB (76169848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a19167a72c78a271da8871c24014e551d80f0d3f27968e18fe6011eddde4fb8f`  
		Last Modified: Tue, 07 Jun 2022 09:20:43 GMT  
		Size: 3.5 KB (3497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f4d3f847824a7e49d036dbd317d814da41c552ea5850e87be21d62a556b47a`  
		Last Modified: Tue, 07 Jun 2022 09:20:43 GMT  
		Size: 6.7 KB (6690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073327f70bbdba5db3ec604ad76695579dcb47ded06553a053f63fb7d4f59a1b`  
		Last Modified: Tue, 07 Jun 2022 09:20:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2-bionic`

```console
$ docker pull mariadb@sha256:b7c94079802d8c85d67d77305de520cfa8a6eee9d7fd735845345c18a67dc805
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2-bionic` - linux; amd64

```console
$ docker pull mariadb@sha256:4838b9eb45b62843192d19e4204d05ccef90ee4ae2216c8ee06d220070f233ec
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.3 MB (109334465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6851bb0ecffe34347de2e4bbbaa0fe9ae243b19760674d35c03aacc70a319f4d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:04 GMT
ADD file:40290d9a94ae76c35ab1f57178130ce1c5b976e34a91e77472ecf7e945ab64f9 in / 
# Mon, 06 Jun 2022 22:21:05 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:45:42 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 00:45:51 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:45:51 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 00:46:04 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 00:46:04 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 00:46:12 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:46:12 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 00:46:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 00:46:13 GMT
ARG MARIADB_MAJOR=10.2
# Tue, 07 Jun 2022 00:46:13 GMT
ENV MARIADB_MAJOR=10.2
# Tue, 07 Jun 2022 00:46:13 GMT
ARG MARIADB_VERSION=1:10.2.44+maria~bionic
# Tue, 07 Jun 2022 00:46:13 GMT
ENV MARIADB_VERSION=1:10.2.44+maria~bionic
# Tue, 07 Jun 2022 00:46:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.44/repo/ubuntu/ bionic main
# Tue, 07 Jun 2022 00:46:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.44/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 00:46:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.44/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 00:46:52 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 00:46:52 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 00:46:52 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Tue, 07 Jun 2022 00:46:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.44/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 07 Jun 2022 00:46:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 00:46:53 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 00:46:53 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:09db6f815738b9c8f25420c47e093f89abaabaa653f9678587b57e8f4400b5ff`  
		Last Modified: Wed, 01 Jun 2022 21:51:21 GMT  
		Size: 26.7 MB (26711626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4807eae0721dbd9932b407dc5d98dc58f2e06513813b4fca2712a92a15b86689`  
		Last Modified: Tue, 07 Jun 2022 00:51:21 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac4d47b6011a1f00d7b234da4777bd0e83179924772c19ccf284bf6af12c4b58`  
		Last Modified: Tue, 07 Jun 2022 00:51:22 GMT  
		Size: 4.8 MB (4817768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e00b950b062eb928bdd8038c2a4500a0b383888e13d5b44c80daca4b4e2f7726`  
		Last Modified: Tue, 07 Jun 2022 00:51:19 GMT  
		Size: 3.6 MB (3553828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f97dc9289c3d74b5fe3e1e62414caa678ed61ad1b33e1b4a1f11ca0167564ac`  
		Last Modified: Tue, 07 Jun 2022 00:51:18 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97255914ba4732e73cf80e7db7e9dc3a4bc2d527bbcfd51eae1f3e65f907a2e6`  
		Last Modified: Tue, 07 Jun 2022 00:51:19 GMT  
		Size: 1.6 MB (1583760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6840b0cb638bc582977a5a9af0b429474bbfa6934e87215358ebb262955d5e2`  
		Last Modified: Tue, 07 Jun 2022 00:51:19 GMT  
		Size: 2.5 KB (2488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f37547518f9f02a2e2aaf92dc69f9e7d4d5ab2027ed99192c36b6562ebd48b8`  
		Last Modified: Tue, 07 Jun 2022 00:51:16 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2971e73bb99cc4318b313d0ec9e62d37eac52fad19bdb075544b8ee089224b36`  
		Last Modified: Tue, 07 Jun 2022 00:51:27 GMT  
		Size: 72.7 MB (72652336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c48b57f36a4248042242ac1dfa4345c9cce6f515155bb7a95a94099f05e1062e`  
		Last Modified: Tue, 07 Jun 2022 00:51:16 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bec65571c7e23e3216197998a553bfe6781ed026bccaae95a7e674d163b4360`  
		Last Modified: Tue, 07 Jun 2022 00:51:16 GMT  
		Size: 6.7 KB (6694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2918faba8f77eb2e5367c5b34d8caf9756c4798e7561dd00a5e57d426d60baa7`  
		Last Modified: Tue, 07 Jun 2022 00:51:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2-bionic` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:e9720f678d59c5a35fdec63dd9db8de5925355d47c7f6329f0ad8692918ec0f5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.3 MB (104282083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:add1daf576ef2aa23b79c70e43fab60541b1ad409ae9dd9c48f61f04680e6d1b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:26 GMT
ADD file:78300bda9e889eaa778190cac0e569ff379d5e533e86b086248476e6ba9b4b2d in / 
# Fri, 29 Apr 2022 22:49:26 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:08:34 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:08:46 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:08:46 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:09:03 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:09:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:09:12 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:09:13 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:09:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:09:16 GMT
ARG MARIADB_MAJOR=10.2
# Sat, 30 Apr 2022 00:09:17 GMT
ENV MARIADB_MAJOR=10.2
# Mon, 23 May 2022 18:45:29 GMT
ARG MARIADB_VERSION=1:10.2.44+maria~bionic
# Mon, 23 May 2022 18:45:30 GMT
ENV MARIADB_VERSION=1:10.2.44+maria~bionic
# Mon, 23 May 2022 18:45:31 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.44/repo/ubuntu/ bionic main
# Mon, 23 May 2022 18:45:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.44/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 23 May 2022 18:46:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.44/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 23 May 2022 18:46:03 GMT
VOLUME [/var/lib/mysql]
# Mon, 23 May 2022 18:46:04 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Mon, 23 May 2022 18:46:05 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Mon, 23 May 2022 18:46:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.44/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 23 May 2022 18:46:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 18:46:07 GMT
EXPOSE 3306
# Mon, 23 May 2022 18:46:08 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e196da37f904f62d236ea302bf13ba07711cc62b35774f86ecda18bcc9ed57c6`  
		Last Modified: Fri, 29 Apr 2022 22:51:14 GMT  
		Size: 23.7 MB (23735089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ddffcde8b39b72c10cbcd5d96f2307b6d6857369d4a57beb67277bd9f18aedc`  
		Last Modified: Sat, 30 Apr 2022 00:14:32 GMT  
		Size: 1.9 KB (1854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed99cb2e83bbae3472b1b2ab68249e1c7dec481cc489c7d69b2627706d3058e7`  
		Last Modified: Sat, 30 Apr 2022 00:14:32 GMT  
		Size: 4.3 MB (4261792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:745c5d6a542769b03497a41228d4f31506c746d9f5ec5bf393f426c2a27c815b`  
		Last Modified: Sat, 30 Apr 2022 00:14:30 GMT  
		Size: 3.2 MB (3207565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8e8f86c5634b4f012cd1f27e537c696a24e4c684810681da4d92d4f232d43a`  
		Last Modified: Sat, 30 Apr 2022 00:14:29 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2279bacf1382c4ea4fafacc8f579b65d5e2c3949c934e3d1c3efe6fab90ec2cf`  
		Last Modified: Sat, 30 Apr 2022 00:14:30 GMT  
		Size: 1.5 MB (1530621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e032a6d669d1fd06479b50389ac1237c010ebdc2fe3008e47c9c210355e610`  
		Last Modified: Sat, 30 Apr 2022 00:14:29 GMT  
		Size: 5.1 KB (5145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8642d3e9a0c45bbba9e78ed2a84f158e9eb4c7be818dfe7963fa5bdfbb9a5b27`  
		Last Modified: Mon, 23 May 2022 18:51:14 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c4271ff6b8dceba8be6c8563d23152c01bdbe9101ebbe661d61aee10662970`  
		Last Modified: Mon, 23 May 2022 18:51:25 GMT  
		Size: 71.5 MB (71529264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5549de856ddfae43ac8ca443c50d292801362822c16c3fcec716472a6a2d40b1`  
		Last Modified: Mon, 23 May 2022 18:51:14 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d5ea630f979a85ef2066038f1b9a1e77b12ba3235f495a8b5be1983dda3f5e`  
		Last Modified: Mon, 23 May 2022 18:51:14 GMT  
		Size: 6.7 KB (6694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffab573772b47c39377a3828310a236d0297612867a74e7a36b9e1db30fa0370`  
		Last Modified: Mon, 23 May 2022 18:51:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2-bionic` - linux; ppc64le

```console
$ docker pull mariadb@sha256:df96ea3a0e5f539059056499b3d5bd9b1a58ac1dc516575432502ede74330534
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117736745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c8b59d225add3e463a7a63174b1268a09b842b8d97f131118683047b89bfbbb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 07 Jun 2022 05:45:31 GMT
ADD file:00feca269255d07b1ddb816beb48357c556d80ab79aa81bc448abc4271d845a5 in / 
# Tue, 07 Jun 2022 05:45:36 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 09:11:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 09:12:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 09:12:28 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 09:13:09 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 09:13:16 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 09:13:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 09:13:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 09:13:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 09:13:52 GMT
ARG MARIADB_MAJOR=10.2
# Tue, 07 Jun 2022 09:13:55 GMT
ENV MARIADB_MAJOR=10.2
# Tue, 07 Jun 2022 09:13:57 GMT
ARG MARIADB_VERSION=1:10.2.44+maria~bionic
# Tue, 07 Jun 2022 09:13:58 GMT
ENV MARIADB_VERSION=1:10.2.44+maria~bionic
# Tue, 07 Jun 2022 09:14:00 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.44/repo/ubuntu/ bionic main
# Tue, 07 Jun 2022 09:14:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.44/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 09:15:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.44/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 09:15:45 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 09:15:46 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 09:15:46 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Tue, 07 Jun 2022 09:15:52 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.44/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 07 Jun 2022 09:15:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 09:16:01 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 09:16:04 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:868ede65862ecf99802bf8944efd378ff1e0751772424cea9084f390deb9f9b2`  
		Last Modified: Tue, 07 Jun 2022 05:48:49 GMT  
		Size: 30.4 MB (30442859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:983cdbbe432683ab8ba3c017f72ff80175ca4f2cdff7d89fb09211b290fa1644`  
		Last Modified: Tue, 07 Jun 2022 09:20:48 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:747b92057fb659c561654f06015a8e02c6b1952f9825371a829861344798ed2e`  
		Last Modified: Tue, 07 Jun 2022 09:20:49 GMT  
		Size: 5.6 MB (5634399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f19dea4ef2503888b21d5a804fb82b4d1b34d7532fe310b079c2acc4d4a23b`  
		Last Modified: Tue, 07 Jun 2022 09:20:47 GMT  
		Size: 3.5 MB (3533925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913fdf09fb6c1d2ee1c333be0f85426ef3a9d46646c1f9077c326672e1f1ca1d`  
		Last Modified: Tue, 07 Jun 2022 09:20:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7707c5204fd4cc2e12dae7367c954e54da990936847175a7cddd179225f8dd14`  
		Last Modified: Tue, 07 Jun 2022 09:20:46 GMT  
		Size: 1.9 MB (1940554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27faa63dfc3a0a16f955fa69f467c27a9f64a189f03cac2e3d4596ebb1e4f2da`  
		Last Modified: Tue, 07 Jun 2022 09:20:45 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2612d482d53133c57a5cb5a320876d66ff2746a205ad91d3777bf8d3c8efe941`  
		Last Modified: Tue, 07 Jun 2022 09:20:43 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba91e76f328f469e4eba02d49d3a226939f79dd8e115f349dfae63940f34e61`  
		Last Modified: Tue, 07 Jun 2022 09:20:57 GMT  
		Size: 76.2 MB (76169848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a19167a72c78a271da8871c24014e551d80f0d3f27968e18fe6011eddde4fb8f`  
		Last Modified: Tue, 07 Jun 2022 09:20:43 GMT  
		Size: 3.5 KB (3497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f4d3f847824a7e49d036dbd317d814da41c552ea5850e87be21d62a556b47a`  
		Last Modified: Tue, 07 Jun 2022 09:20:43 GMT  
		Size: 6.7 KB (6690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073327f70bbdba5db3ec604ad76695579dcb47ded06553a053f63fb7d4f59a1b`  
		Last Modified: Tue, 07 Jun 2022 09:20:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2.44`

```console
$ docker pull mariadb@sha256:b7c94079802d8c85d67d77305de520cfa8a6eee9d7fd735845345c18a67dc805
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2.44` - linux; amd64

```console
$ docker pull mariadb@sha256:4838b9eb45b62843192d19e4204d05ccef90ee4ae2216c8ee06d220070f233ec
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.3 MB (109334465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6851bb0ecffe34347de2e4bbbaa0fe9ae243b19760674d35c03aacc70a319f4d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:04 GMT
ADD file:40290d9a94ae76c35ab1f57178130ce1c5b976e34a91e77472ecf7e945ab64f9 in / 
# Mon, 06 Jun 2022 22:21:05 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:45:42 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 00:45:51 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:45:51 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 00:46:04 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 00:46:04 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 00:46:12 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:46:12 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 00:46:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 00:46:13 GMT
ARG MARIADB_MAJOR=10.2
# Tue, 07 Jun 2022 00:46:13 GMT
ENV MARIADB_MAJOR=10.2
# Tue, 07 Jun 2022 00:46:13 GMT
ARG MARIADB_VERSION=1:10.2.44+maria~bionic
# Tue, 07 Jun 2022 00:46:13 GMT
ENV MARIADB_VERSION=1:10.2.44+maria~bionic
# Tue, 07 Jun 2022 00:46:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.44/repo/ubuntu/ bionic main
# Tue, 07 Jun 2022 00:46:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.44/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 00:46:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.44/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 00:46:52 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 00:46:52 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 00:46:52 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Tue, 07 Jun 2022 00:46:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.44/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 07 Jun 2022 00:46:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 00:46:53 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 00:46:53 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:09db6f815738b9c8f25420c47e093f89abaabaa653f9678587b57e8f4400b5ff`  
		Last Modified: Wed, 01 Jun 2022 21:51:21 GMT  
		Size: 26.7 MB (26711626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4807eae0721dbd9932b407dc5d98dc58f2e06513813b4fca2712a92a15b86689`  
		Last Modified: Tue, 07 Jun 2022 00:51:21 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac4d47b6011a1f00d7b234da4777bd0e83179924772c19ccf284bf6af12c4b58`  
		Last Modified: Tue, 07 Jun 2022 00:51:22 GMT  
		Size: 4.8 MB (4817768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e00b950b062eb928bdd8038c2a4500a0b383888e13d5b44c80daca4b4e2f7726`  
		Last Modified: Tue, 07 Jun 2022 00:51:19 GMT  
		Size: 3.6 MB (3553828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f97dc9289c3d74b5fe3e1e62414caa678ed61ad1b33e1b4a1f11ca0167564ac`  
		Last Modified: Tue, 07 Jun 2022 00:51:18 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97255914ba4732e73cf80e7db7e9dc3a4bc2d527bbcfd51eae1f3e65f907a2e6`  
		Last Modified: Tue, 07 Jun 2022 00:51:19 GMT  
		Size: 1.6 MB (1583760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6840b0cb638bc582977a5a9af0b429474bbfa6934e87215358ebb262955d5e2`  
		Last Modified: Tue, 07 Jun 2022 00:51:19 GMT  
		Size: 2.5 KB (2488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f37547518f9f02a2e2aaf92dc69f9e7d4d5ab2027ed99192c36b6562ebd48b8`  
		Last Modified: Tue, 07 Jun 2022 00:51:16 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2971e73bb99cc4318b313d0ec9e62d37eac52fad19bdb075544b8ee089224b36`  
		Last Modified: Tue, 07 Jun 2022 00:51:27 GMT  
		Size: 72.7 MB (72652336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c48b57f36a4248042242ac1dfa4345c9cce6f515155bb7a95a94099f05e1062e`  
		Last Modified: Tue, 07 Jun 2022 00:51:16 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bec65571c7e23e3216197998a553bfe6781ed026bccaae95a7e674d163b4360`  
		Last Modified: Tue, 07 Jun 2022 00:51:16 GMT  
		Size: 6.7 KB (6694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2918faba8f77eb2e5367c5b34d8caf9756c4798e7561dd00a5e57d426d60baa7`  
		Last Modified: Tue, 07 Jun 2022 00:51:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2.44` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:e9720f678d59c5a35fdec63dd9db8de5925355d47c7f6329f0ad8692918ec0f5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.3 MB (104282083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:add1daf576ef2aa23b79c70e43fab60541b1ad409ae9dd9c48f61f04680e6d1b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:26 GMT
ADD file:78300bda9e889eaa778190cac0e569ff379d5e533e86b086248476e6ba9b4b2d in / 
# Fri, 29 Apr 2022 22:49:26 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:08:34 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:08:46 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:08:46 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:09:03 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:09:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:09:12 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:09:13 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:09:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:09:16 GMT
ARG MARIADB_MAJOR=10.2
# Sat, 30 Apr 2022 00:09:17 GMT
ENV MARIADB_MAJOR=10.2
# Mon, 23 May 2022 18:45:29 GMT
ARG MARIADB_VERSION=1:10.2.44+maria~bionic
# Mon, 23 May 2022 18:45:30 GMT
ENV MARIADB_VERSION=1:10.2.44+maria~bionic
# Mon, 23 May 2022 18:45:31 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.44/repo/ubuntu/ bionic main
# Mon, 23 May 2022 18:45:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.44/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 23 May 2022 18:46:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.44/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 23 May 2022 18:46:03 GMT
VOLUME [/var/lib/mysql]
# Mon, 23 May 2022 18:46:04 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Mon, 23 May 2022 18:46:05 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Mon, 23 May 2022 18:46:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.44/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 23 May 2022 18:46:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 18:46:07 GMT
EXPOSE 3306
# Mon, 23 May 2022 18:46:08 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e196da37f904f62d236ea302bf13ba07711cc62b35774f86ecda18bcc9ed57c6`  
		Last Modified: Fri, 29 Apr 2022 22:51:14 GMT  
		Size: 23.7 MB (23735089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ddffcde8b39b72c10cbcd5d96f2307b6d6857369d4a57beb67277bd9f18aedc`  
		Last Modified: Sat, 30 Apr 2022 00:14:32 GMT  
		Size: 1.9 KB (1854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed99cb2e83bbae3472b1b2ab68249e1c7dec481cc489c7d69b2627706d3058e7`  
		Last Modified: Sat, 30 Apr 2022 00:14:32 GMT  
		Size: 4.3 MB (4261792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:745c5d6a542769b03497a41228d4f31506c746d9f5ec5bf393f426c2a27c815b`  
		Last Modified: Sat, 30 Apr 2022 00:14:30 GMT  
		Size: 3.2 MB (3207565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8e8f86c5634b4f012cd1f27e537c696a24e4c684810681da4d92d4f232d43a`  
		Last Modified: Sat, 30 Apr 2022 00:14:29 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2279bacf1382c4ea4fafacc8f579b65d5e2c3949c934e3d1c3efe6fab90ec2cf`  
		Last Modified: Sat, 30 Apr 2022 00:14:30 GMT  
		Size: 1.5 MB (1530621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e032a6d669d1fd06479b50389ac1237c010ebdc2fe3008e47c9c210355e610`  
		Last Modified: Sat, 30 Apr 2022 00:14:29 GMT  
		Size: 5.1 KB (5145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8642d3e9a0c45bbba9e78ed2a84f158e9eb4c7be818dfe7963fa5bdfbb9a5b27`  
		Last Modified: Mon, 23 May 2022 18:51:14 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c4271ff6b8dceba8be6c8563d23152c01bdbe9101ebbe661d61aee10662970`  
		Last Modified: Mon, 23 May 2022 18:51:25 GMT  
		Size: 71.5 MB (71529264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5549de856ddfae43ac8ca443c50d292801362822c16c3fcec716472a6a2d40b1`  
		Last Modified: Mon, 23 May 2022 18:51:14 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d5ea630f979a85ef2066038f1b9a1e77b12ba3235f495a8b5be1983dda3f5e`  
		Last Modified: Mon, 23 May 2022 18:51:14 GMT  
		Size: 6.7 KB (6694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffab573772b47c39377a3828310a236d0297612867a74e7a36b9e1db30fa0370`  
		Last Modified: Mon, 23 May 2022 18:51:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2.44` - linux; ppc64le

```console
$ docker pull mariadb@sha256:df96ea3a0e5f539059056499b3d5bd9b1a58ac1dc516575432502ede74330534
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117736745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c8b59d225add3e463a7a63174b1268a09b842b8d97f131118683047b89bfbbb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 07 Jun 2022 05:45:31 GMT
ADD file:00feca269255d07b1ddb816beb48357c556d80ab79aa81bc448abc4271d845a5 in / 
# Tue, 07 Jun 2022 05:45:36 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 09:11:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 09:12:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 09:12:28 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 09:13:09 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 09:13:16 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 09:13:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 09:13:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 09:13:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 09:13:52 GMT
ARG MARIADB_MAJOR=10.2
# Tue, 07 Jun 2022 09:13:55 GMT
ENV MARIADB_MAJOR=10.2
# Tue, 07 Jun 2022 09:13:57 GMT
ARG MARIADB_VERSION=1:10.2.44+maria~bionic
# Tue, 07 Jun 2022 09:13:58 GMT
ENV MARIADB_VERSION=1:10.2.44+maria~bionic
# Tue, 07 Jun 2022 09:14:00 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.44/repo/ubuntu/ bionic main
# Tue, 07 Jun 2022 09:14:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.44/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 09:15:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.44/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 09:15:45 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 09:15:46 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 09:15:46 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Tue, 07 Jun 2022 09:15:52 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.44/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 07 Jun 2022 09:15:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 09:16:01 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 09:16:04 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:868ede65862ecf99802bf8944efd378ff1e0751772424cea9084f390deb9f9b2`  
		Last Modified: Tue, 07 Jun 2022 05:48:49 GMT  
		Size: 30.4 MB (30442859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:983cdbbe432683ab8ba3c017f72ff80175ca4f2cdff7d89fb09211b290fa1644`  
		Last Modified: Tue, 07 Jun 2022 09:20:48 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:747b92057fb659c561654f06015a8e02c6b1952f9825371a829861344798ed2e`  
		Last Modified: Tue, 07 Jun 2022 09:20:49 GMT  
		Size: 5.6 MB (5634399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f19dea4ef2503888b21d5a804fb82b4d1b34d7532fe310b079c2acc4d4a23b`  
		Last Modified: Tue, 07 Jun 2022 09:20:47 GMT  
		Size: 3.5 MB (3533925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913fdf09fb6c1d2ee1c333be0f85426ef3a9d46646c1f9077c326672e1f1ca1d`  
		Last Modified: Tue, 07 Jun 2022 09:20:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7707c5204fd4cc2e12dae7367c954e54da990936847175a7cddd179225f8dd14`  
		Last Modified: Tue, 07 Jun 2022 09:20:46 GMT  
		Size: 1.9 MB (1940554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27faa63dfc3a0a16f955fa69f467c27a9f64a189f03cac2e3d4596ebb1e4f2da`  
		Last Modified: Tue, 07 Jun 2022 09:20:45 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2612d482d53133c57a5cb5a320876d66ff2746a205ad91d3777bf8d3c8efe941`  
		Last Modified: Tue, 07 Jun 2022 09:20:43 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba91e76f328f469e4eba02d49d3a226939f79dd8e115f349dfae63940f34e61`  
		Last Modified: Tue, 07 Jun 2022 09:20:57 GMT  
		Size: 76.2 MB (76169848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a19167a72c78a271da8871c24014e551d80f0d3f27968e18fe6011eddde4fb8f`  
		Last Modified: Tue, 07 Jun 2022 09:20:43 GMT  
		Size: 3.5 KB (3497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f4d3f847824a7e49d036dbd317d814da41c552ea5850e87be21d62a556b47a`  
		Last Modified: Tue, 07 Jun 2022 09:20:43 GMT  
		Size: 6.7 KB (6690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073327f70bbdba5db3ec604ad76695579dcb47ded06553a053f63fb7d4f59a1b`  
		Last Modified: Tue, 07 Jun 2022 09:20:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2.44-bionic`

```console
$ docker pull mariadb@sha256:b7c94079802d8c85d67d77305de520cfa8a6eee9d7fd735845345c18a67dc805
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2.44-bionic` - linux; amd64

```console
$ docker pull mariadb@sha256:4838b9eb45b62843192d19e4204d05ccef90ee4ae2216c8ee06d220070f233ec
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.3 MB (109334465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6851bb0ecffe34347de2e4bbbaa0fe9ae243b19760674d35c03aacc70a319f4d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:04 GMT
ADD file:40290d9a94ae76c35ab1f57178130ce1c5b976e34a91e77472ecf7e945ab64f9 in / 
# Mon, 06 Jun 2022 22:21:05 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:45:42 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 00:45:51 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:45:51 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 00:46:04 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 00:46:04 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 00:46:12 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:46:12 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 00:46:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 00:46:13 GMT
ARG MARIADB_MAJOR=10.2
# Tue, 07 Jun 2022 00:46:13 GMT
ENV MARIADB_MAJOR=10.2
# Tue, 07 Jun 2022 00:46:13 GMT
ARG MARIADB_VERSION=1:10.2.44+maria~bionic
# Tue, 07 Jun 2022 00:46:13 GMT
ENV MARIADB_VERSION=1:10.2.44+maria~bionic
# Tue, 07 Jun 2022 00:46:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.44/repo/ubuntu/ bionic main
# Tue, 07 Jun 2022 00:46:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.44/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 00:46:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.44/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 00:46:52 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 00:46:52 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 00:46:52 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Tue, 07 Jun 2022 00:46:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.44/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 07 Jun 2022 00:46:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 00:46:53 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 00:46:53 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:09db6f815738b9c8f25420c47e093f89abaabaa653f9678587b57e8f4400b5ff`  
		Last Modified: Wed, 01 Jun 2022 21:51:21 GMT  
		Size: 26.7 MB (26711626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4807eae0721dbd9932b407dc5d98dc58f2e06513813b4fca2712a92a15b86689`  
		Last Modified: Tue, 07 Jun 2022 00:51:21 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac4d47b6011a1f00d7b234da4777bd0e83179924772c19ccf284bf6af12c4b58`  
		Last Modified: Tue, 07 Jun 2022 00:51:22 GMT  
		Size: 4.8 MB (4817768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e00b950b062eb928bdd8038c2a4500a0b383888e13d5b44c80daca4b4e2f7726`  
		Last Modified: Tue, 07 Jun 2022 00:51:19 GMT  
		Size: 3.6 MB (3553828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f97dc9289c3d74b5fe3e1e62414caa678ed61ad1b33e1b4a1f11ca0167564ac`  
		Last Modified: Tue, 07 Jun 2022 00:51:18 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97255914ba4732e73cf80e7db7e9dc3a4bc2d527bbcfd51eae1f3e65f907a2e6`  
		Last Modified: Tue, 07 Jun 2022 00:51:19 GMT  
		Size: 1.6 MB (1583760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6840b0cb638bc582977a5a9af0b429474bbfa6934e87215358ebb262955d5e2`  
		Last Modified: Tue, 07 Jun 2022 00:51:19 GMT  
		Size: 2.5 KB (2488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f37547518f9f02a2e2aaf92dc69f9e7d4d5ab2027ed99192c36b6562ebd48b8`  
		Last Modified: Tue, 07 Jun 2022 00:51:16 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2971e73bb99cc4318b313d0ec9e62d37eac52fad19bdb075544b8ee089224b36`  
		Last Modified: Tue, 07 Jun 2022 00:51:27 GMT  
		Size: 72.7 MB (72652336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c48b57f36a4248042242ac1dfa4345c9cce6f515155bb7a95a94099f05e1062e`  
		Last Modified: Tue, 07 Jun 2022 00:51:16 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bec65571c7e23e3216197998a553bfe6781ed026bccaae95a7e674d163b4360`  
		Last Modified: Tue, 07 Jun 2022 00:51:16 GMT  
		Size: 6.7 KB (6694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2918faba8f77eb2e5367c5b34d8caf9756c4798e7561dd00a5e57d426d60baa7`  
		Last Modified: Tue, 07 Jun 2022 00:51:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2.44-bionic` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:e9720f678d59c5a35fdec63dd9db8de5925355d47c7f6329f0ad8692918ec0f5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.3 MB (104282083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:add1daf576ef2aa23b79c70e43fab60541b1ad409ae9dd9c48f61f04680e6d1b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:26 GMT
ADD file:78300bda9e889eaa778190cac0e569ff379d5e533e86b086248476e6ba9b4b2d in / 
# Fri, 29 Apr 2022 22:49:26 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:08:34 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:08:46 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:08:46 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:09:03 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:09:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:09:12 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:09:13 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:09:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:09:16 GMT
ARG MARIADB_MAJOR=10.2
# Sat, 30 Apr 2022 00:09:17 GMT
ENV MARIADB_MAJOR=10.2
# Mon, 23 May 2022 18:45:29 GMT
ARG MARIADB_VERSION=1:10.2.44+maria~bionic
# Mon, 23 May 2022 18:45:30 GMT
ENV MARIADB_VERSION=1:10.2.44+maria~bionic
# Mon, 23 May 2022 18:45:31 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.44/repo/ubuntu/ bionic main
# Mon, 23 May 2022 18:45:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.44/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 23 May 2022 18:46:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.44/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 23 May 2022 18:46:03 GMT
VOLUME [/var/lib/mysql]
# Mon, 23 May 2022 18:46:04 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Mon, 23 May 2022 18:46:05 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Mon, 23 May 2022 18:46:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.44/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 23 May 2022 18:46:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 18:46:07 GMT
EXPOSE 3306
# Mon, 23 May 2022 18:46:08 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e196da37f904f62d236ea302bf13ba07711cc62b35774f86ecda18bcc9ed57c6`  
		Last Modified: Fri, 29 Apr 2022 22:51:14 GMT  
		Size: 23.7 MB (23735089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ddffcde8b39b72c10cbcd5d96f2307b6d6857369d4a57beb67277bd9f18aedc`  
		Last Modified: Sat, 30 Apr 2022 00:14:32 GMT  
		Size: 1.9 KB (1854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed99cb2e83bbae3472b1b2ab68249e1c7dec481cc489c7d69b2627706d3058e7`  
		Last Modified: Sat, 30 Apr 2022 00:14:32 GMT  
		Size: 4.3 MB (4261792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:745c5d6a542769b03497a41228d4f31506c746d9f5ec5bf393f426c2a27c815b`  
		Last Modified: Sat, 30 Apr 2022 00:14:30 GMT  
		Size: 3.2 MB (3207565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8e8f86c5634b4f012cd1f27e537c696a24e4c684810681da4d92d4f232d43a`  
		Last Modified: Sat, 30 Apr 2022 00:14:29 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2279bacf1382c4ea4fafacc8f579b65d5e2c3949c934e3d1c3efe6fab90ec2cf`  
		Last Modified: Sat, 30 Apr 2022 00:14:30 GMT  
		Size: 1.5 MB (1530621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e032a6d669d1fd06479b50389ac1237c010ebdc2fe3008e47c9c210355e610`  
		Last Modified: Sat, 30 Apr 2022 00:14:29 GMT  
		Size: 5.1 KB (5145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8642d3e9a0c45bbba9e78ed2a84f158e9eb4c7be818dfe7963fa5bdfbb9a5b27`  
		Last Modified: Mon, 23 May 2022 18:51:14 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c4271ff6b8dceba8be6c8563d23152c01bdbe9101ebbe661d61aee10662970`  
		Last Modified: Mon, 23 May 2022 18:51:25 GMT  
		Size: 71.5 MB (71529264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5549de856ddfae43ac8ca443c50d292801362822c16c3fcec716472a6a2d40b1`  
		Last Modified: Mon, 23 May 2022 18:51:14 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d5ea630f979a85ef2066038f1b9a1e77b12ba3235f495a8b5be1983dda3f5e`  
		Last Modified: Mon, 23 May 2022 18:51:14 GMT  
		Size: 6.7 KB (6694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffab573772b47c39377a3828310a236d0297612867a74e7a36b9e1db30fa0370`  
		Last Modified: Mon, 23 May 2022 18:51:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2.44-bionic` - linux; ppc64le

```console
$ docker pull mariadb@sha256:df96ea3a0e5f539059056499b3d5bd9b1a58ac1dc516575432502ede74330534
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117736745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c8b59d225add3e463a7a63174b1268a09b842b8d97f131118683047b89bfbbb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 07 Jun 2022 05:45:31 GMT
ADD file:00feca269255d07b1ddb816beb48357c556d80ab79aa81bc448abc4271d845a5 in / 
# Tue, 07 Jun 2022 05:45:36 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 09:11:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 09:12:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 09:12:28 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 09:13:09 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 09:13:16 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 09:13:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 09:13:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 09:13:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 09:13:52 GMT
ARG MARIADB_MAJOR=10.2
# Tue, 07 Jun 2022 09:13:55 GMT
ENV MARIADB_MAJOR=10.2
# Tue, 07 Jun 2022 09:13:57 GMT
ARG MARIADB_VERSION=1:10.2.44+maria~bionic
# Tue, 07 Jun 2022 09:13:58 GMT
ENV MARIADB_VERSION=1:10.2.44+maria~bionic
# Tue, 07 Jun 2022 09:14:00 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.44/repo/ubuntu/ bionic main
# Tue, 07 Jun 2022 09:14:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.44/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 09:15:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.44/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 09:15:45 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 09:15:46 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 09:15:46 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Tue, 07 Jun 2022 09:15:52 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.44/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 07 Jun 2022 09:15:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 09:16:01 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 09:16:04 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:868ede65862ecf99802bf8944efd378ff1e0751772424cea9084f390deb9f9b2`  
		Last Modified: Tue, 07 Jun 2022 05:48:49 GMT  
		Size: 30.4 MB (30442859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:983cdbbe432683ab8ba3c017f72ff80175ca4f2cdff7d89fb09211b290fa1644`  
		Last Modified: Tue, 07 Jun 2022 09:20:48 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:747b92057fb659c561654f06015a8e02c6b1952f9825371a829861344798ed2e`  
		Last Modified: Tue, 07 Jun 2022 09:20:49 GMT  
		Size: 5.6 MB (5634399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f19dea4ef2503888b21d5a804fb82b4d1b34d7532fe310b079c2acc4d4a23b`  
		Last Modified: Tue, 07 Jun 2022 09:20:47 GMT  
		Size: 3.5 MB (3533925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913fdf09fb6c1d2ee1c333be0f85426ef3a9d46646c1f9077c326672e1f1ca1d`  
		Last Modified: Tue, 07 Jun 2022 09:20:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7707c5204fd4cc2e12dae7367c954e54da990936847175a7cddd179225f8dd14`  
		Last Modified: Tue, 07 Jun 2022 09:20:46 GMT  
		Size: 1.9 MB (1940554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27faa63dfc3a0a16f955fa69f467c27a9f64a189f03cac2e3d4596ebb1e4f2da`  
		Last Modified: Tue, 07 Jun 2022 09:20:45 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2612d482d53133c57a5cb5a320876d66ff2746a205ad91d3777bf8d3c8efe941`  
		Last Modified: Tue, 07 Jun 2022 09:20:43 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba91e76f328f469e4eba02d49d3a226939f79dd8e115f349dfae63940f34e61`  
		Last Modified: Tue, 07 Jun 2022 09:20:57 GMT  
		Size: 76.2 MB (76169848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a19167a72c78a271da8871c24014e551d80f0d3f27968e18fe6011eddde4fb8f`  
		Last Modified: Tue, 07 Jun 2022 09:20:43 GMT  
		Size: 3.5 KB (3497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f4d3f847824a7e49d036dbd317d814da41c552ea5850e87be21d62a556b47a`  
		Last Modified: Tue, 07 Jun 2022 09:20:43 GMT  
		Size: 6.7 KB (6690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073327f70bbdba5db3ec604ad76695579dcb47ded06553a053f63fb7d4f59a1b`  
		Last Modified: Tue, 07 Jun 2022 09:20:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3`

```console
$ docker pull mariadb@sha256:46ed12b7c2b89b8ea9690861ada81f50f2ba3eccfb7a820d5fcb295c83431e6a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3` - linux; amd64

```console
$ docker pull mariadb@sha256:8185282e1c12d51e3b1b7043e7c541196b33fa7d71f5df4d26c0f6cb5b1a023b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.2 MB (120166559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7211b4227b56738c0dc31ba1b2c15c322134f707ac0a2ee0accd2e8d6838913`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:42:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 00:42:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:42:35 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 00:42:46 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 00:42:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 00:42:53 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:42:53 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 00:42:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 00:45:01 GMT
ARG MARIADB_MAJOR=10.3
# Tue, 07 Jun 2022 00:45:01 GMT
ENV MARIADB_MAJOR=10.3
# Tue, 07 Jun 2022 00:45:01 GMT
ARG MARIADB_VERSION=1:10.3.35+maria~focal
# Tue, 07 Jun 2022 00:45:01 GMT
ENV MARIADB_VERSION=1:10.3.35+maria~focal
# Tue, 07 Jun 2022 00:45:01 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
# Tue, 07 Jun 2022 00:45:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 00:45:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 00:45:33 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 00:45:33 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 00:45:33 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Tue, 07 Jun 2022 00:45:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 07 Jun 2022 00:45:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 00:45:34 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 00:45:34 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59dcb80bbedb867b19c4eb004e84c86ae3475041d5bd11672bae9ba6be45084f`  
		Last Modified: Tue, 07 Jun 2022 00:48:53 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6c41888e0f25dece871c7e65daad879fc39d7da0a84f6b67ae0d4e1f4a6f8a`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 5.5 MB (5488991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de82bf1cd45986845f81bc71a119bf5ceaec50c145064ea58e5729f4bd6d0d22`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 3.6 MB (3585352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316c0826d235e46a7a9adcfcc3068c004818dc2611a41b69e6e7bea02316b70f`  
		Last Modified: Tue, 07 Jun 2022 00:48:51 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b82e623f5d9ed1cc04e5adc22adc6805abdba4aecc5b427aec6c31223a64dca6`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 2.3 MB (2272315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3daba1f86bc0fd099576f61e5eea0961cdefed1dc443ffb96b6a50c8f054b0b0`  
		Last Modified: Tue, 07 Jun 2022 00:48:49 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae5f5297e44fa8576d8cba5edeb0f6bcbba2d13d78504733a435edfaf675f4c`  
		Last Modified: Tue, 07 Jun 2022 00:50:47 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a399420e15d3f88656c1aa23156f8f0ffbe901be2cbdb04da21287497777194b`  
		Last Modified: Tue, 07 Jun 2022 00:50:59 GMT  
		Size: 80.2 MB (80232253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1179237169a7302cbd05986d859802c88f4c40b14685a714887740fdbe64f391`  
		Last Modified: Tue, 07 Jun 2022 00:50:47 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b09ecefdf18e9d3e4120a212b98d8a8f1be59b53626af7376d2448dfcf5e30ec`  
		Last Modified: Tue, 07 Jun 2022 00:50:47 GMT  
		Size: 6.7 KB (6690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ebffa6e7f3bd3d44b65a9ede071f8fda7929387c29dc8efbe18ecd5fe68c69a`  
		Last Modified: Tue, 07 Jun 2022 00:50:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:29eba27ea2398b359c15ad9cd8382727f7a95651a86914393df1d2ba6fdedb7d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117592246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a73a6b4bc2fe0d9e9d6515aee85b0e64beb35afde8718eb65c170d010f1209b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:03:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:03:44 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:03:45 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:04:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:04:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:04:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:04:10 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:04:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:07:50 GMT
ARG MARIADB_MAJOR=10.3
# Sat, 30 Apr 2022 00:07:51 GMT
ENV MARIADB_MAJOR=10.3
# Mon, 23 May 2022 18:44:45 GMT
ARG MARIADB_VERSION=1:10.3.35+maria~focal
# Mon, 23 May 2022 18:44:46 GMT
ENV MARIADB_VERSION=1:10.3.35+maria~focal
# Mon, 23 May 2022 18:44:47 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
# Mon, 23 May 2022 18:44:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 23 May 2022 18:45:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 23 May 2022 18:45:14 GMT
VOLUME [/var/lib/mysql]
# Mon, 23 May 2022 18:45:16 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Mon, 23 May 2022 18:45:17 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Mon, 23 May 2022 18:45:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 23 May 2022 18:45:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 18:45:19 GMT
EXPOSE 3306
# Mon, 23 May 2022 18:45:20 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932d0da437931580c9d7f118c259624e1c3ec8e81acb2acf5740d945e511ba78`  
		Last Modified: Sat, 30 Apr 2022 00:11:03 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc35c765a7328bd99273ee471b6b108980755023d4bcb1927fa7717942a9d318`  
		Last Modified: Sat, 30 Apr 2022 00:11:02 GMT  
		Size: 5.3 MB (5320183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88bae007bd9c42610e465ab436d60b2457b10b735a1bc8e5daba38f548c026`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 3.4 MB (3369899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7734d2f7be989dfe94fb891565830b8101d8e9bdbcbce8e5a7e1b1932eb3ac3c`  
		Last Modified: Sat, 30 Apr 2022 00:11:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24600bac48ce2157027e68df9e26a81754edc6f7e099c33c0a89de879dba5d9`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 2.2 MB (2202385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da05700210f681c47e021b8f3ce45f244f696854cfd656f0cd46e59cb8ca9b7d`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11d91c81167b97fd688c89c8661dd2090b118a00c9e4d5cf447c1f9b984d7ad7`  
		Last Modified: Mon, 23 May 2022 18:50:43 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0abb8afdaeab72a91b2d5af7dc150780f17d2c6f56646fa6ecfc137865aa2dd`  
		Last Modified: Mon, 23 May 2022 18:50:55 GMT  
		Size: 79.5 MB (79515444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a15518853e77b139d69972807cdd43a0752ed028475006e3ff0c1f9e261848d`  
		Last Modified: Mon, 23 May 2022 18:50:43 GMT  
		Size: 3.5 KB (3497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5f0665fe7d2108d19241b1f7d30186abc06e9c55d24aa366a550fa988e8ca9`  
		Last Modified: Mon, 23 May 2022 18:50:43 GMT  
		Size: 6.7 KB (6693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9b8a787243bcd17a20fac81c7addc504f111a3c06c859ae0c4c8ac3c7f0507`  
		Last Modified: Mon, 23 May 2022 18:50:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3` - linux; ppc64le

```console
$ docker pull mariadb@sha256:d512ce2edbb705fc8f741a1b2df00212e6a7d615cc427c8253915a772129c062
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.0 MB (131036649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78c940a2c84aa82092c4fc95fc1363b732f86115130732a5d7da52820599ee8b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 07 Jun 2022 05:46:02 GMT
ADD file:86506a94b834ba2b6f10dc0d1955bee539be1cf565e4ccc2c4bc074e0375f115 in / 
# Tue, 07 Jun 2022 05:46:06 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 08:57:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 08:57:48 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 08:57:54 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 08:58:44 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 08:58:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 08:59:09 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 08:59:14 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 08:59:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 09:09:30 GMT
ARG MARIADB_MAJOR=10.3
# Tue, 07 Jun 2022 09:09:32 GMT
ENV MARIADB_MAJOR=10.3
# Tue, 07 Jun 2022 09:09:35 GMT
ARG MARIADB_VERSION=1:10.3.35+maria~focal
# Tue, 07 Jun 2022 09:09:37 GMT
ENV MARIADB_VERSION=1:10.3.35+maria~focal
# Tue, 07 Jun 2022 09:09:39 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
# Tue, 07 Jun 2022 09:09:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 09:11:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 09:11:20 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 09:11:22 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 09:11:23 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Tue, 07 Jun 2022 09:11:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 07 Jun 2022 09:11:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 09:11:32 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 09:11:34 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3f52d061d2d3fdde0d3a099bbeae64080476c9650e9f3ba05de898d5bb5f03e8`  
		Last Modified: Tue, 07 Jun 2022 05:49:10 GMT  
		Size: 33.3 MB (33294345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b33a69d2ff59c89a297c597798ade8ea874f546d95513bd628c17fd7afda14`  
		Last Modified: Tue, 07 Jun 2022 09:17:18 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56a2c22a499e4928a88ae9201c66f507be8b9f10804ea7d0934710a6f91e5ec5`  
		Last Modified: Tue, 07 Jun 2022 09:17:18 GMT  
		Size: 6.7 MB (6667490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892b2ffb492b6d36ce25b68cf708d3c9bc9e0210e0cbbe7f575d3424c35d6b96`  
		Last Modified: Tue, 07 Jun 2022 09:17:17 GMT  
		Size: 3.7 MB (3672362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f80e77ec2bb0d7d685ca6e56f718adc6d253a98e069ebd5439f0c973194758`  
		Last Modified: Tue, 07 Jun 2022 09:17:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b0b3a9b79c49528e8e9da2d5d4954fc4e5392ee848c19c52a4d3369feb63d9`  
		Last Modified: Tue, 07 Jun 2022 09:17:16 GMT  
		Size: 2.6 MB (2568258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617e76c5eb45b560720c75ad4c60429a026cbbcb8467360cc70a7dace9ec4e5a`  
		Last Modified: Tue, 07 Jun 2022 09:17:13 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c76afa2f9b8c0de0c04d0255b8646667dee277f515efd76c4b8d25abc36d573b`  
		Last Modified: Tue, 07 Jun 2022 09:19:59 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a5c6e4389d875da6bb41a51b291b7b41e131ab216972ac29700f2c5136e124e`  
		Last Modified: Tue, 07 Jun 2022 09:20:16 GMT  
		Size: 84.8 MB (84819169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ee4158a6f6c038083a106a52ac8dbfcd5cc6b3d0e0b2ff91dd1d0673a892ecf`  
		Last Modified: Tue, 07 Jun 2022 09:19:59 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6738a30bf3051aecf38054c4526a741830fc7f9972b0c4184480dcde66a275b5`  
		Last Modified: Tue, 07 Jun 2022 09:19:59 GMT  
		Size: 6.7 KB (6691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df92c20d5b09a08ff94318bd4d3f6f6ace8697ccf0463d4800fd4e310c6e891d`  
		Last Modified: Tue, 07 Jun 2022 09:19:59 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3-focal`

```console
$ docker pull mariadb@sha256:46ed12b7c2b89b8ea9690861ada81f50f2ba3eccfb7a820d5fcb295c83431e6a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:8185282e1c12d51e3b1b7043e7c541196b33fa7d71f5df4d26c0f6cb5b1a023b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.2 MB (120166559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7211b4227b56738c0dc31ba1b2c15c322134f707ac0a2ee0accd2e8d6838913`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:42:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 00:42:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:42:35 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 00:42:46 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 00:42:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 00:42:53 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:42:53 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 00:42:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 00:45:01 GMT
ARG MARIADB_MAJOR=10.3
# Tue, 07 Jun 2022 00:45:01 GMT
ENV MARIADB_MAJOR=10.3
# Tue, 07 Jun 2022 00:45:01 GMT
ARG MARIADB_VERSION=1:10.3.35+maria~focal
# Tue, 07 Jun 2022 00:45:01 GMT
ENV MARIADB_VERSION=1:10.3.35+maria~focal
# Tue, 07 Jun 2022 00:45:01 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
# Tue, 07 Jun 2022 00:45:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 00:45:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 00:45:33 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 00:45:33 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 00:45:33 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Tue, 07 Jun 2022 00:45:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 07 Jun 2022 00:45:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 00:45:34 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 00:45:34 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59dcb80bbedb867b19c4eb004e84c86ae3475041d5bd11672bae9ba6be45084f`  
		Last Modified: Tue, 07 Jun 2022 00:48:53 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6c41888e0f25dece871c7e65daad879fc39d7da0a84f6b67ae0d4e1f4a6f8a`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 5.5 MB (5488991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de82bf1cd45986845f81bc71a119bf5ceaec50c145064ea58e5729f4bd6d0d22`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 3.6 MB (3585352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316c0826d235e46a7a9adcfcc3068c004818dc2611a41b69e6e7bea02316b70f`  
		Last Modified: Tue, 07 Jun 2022 00:48:51 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b82e623f5d9ed1cc04e5adc22adc6805abdba4aecc5b427aec6c31223a64dca6`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 2.3 MB (2272315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3daba1f86bc0fd099576f61e5eea0961cdefed1dc443ffb96b6a50c8f054b0b0`  
		Last Modified: Tue, 07 Jun 2022 00:48:49 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae5f5297e44fa8576d8cba5edeb0f6bcbba2d13d78504733a435edfaf675f4c`  
		Last Modified: Tue, 07 Jun 2022 00:50:47 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a399420e15d3f88656c1aa23156f8f0ffbe901be2cbdb04da21287497777194b`  
		Last Modified: Tue, 07 Jun 2022 00:50:59 GMT  
		Size: 80.2 MB (80232253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1179237169a7302cbd05986d859802c88f4c40b14685a714887740fdbe64f391`  
		Last Modified: Tue, 07 Jun 2022 00:50:47 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b09ecefdf18e9d3e4120a212b98d8a8f1be59b53626af7376d2448dfcf5e30ec`  
		Last Modified: Tue, 07 Jun 2022 00:50:47 GMT  
		Size: 6.7 KB (6690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ebffa6e7f3bd3d44b65a9ede071f8fda7929387c29dc8efbe18ecd5fe68c69a`  
		Last Modified: Tue, 07 Jun 2022 00:50:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:29eba27ea2398b359c15ad9cd8382727f7a95651a86914393df1d2ba6fdedb7d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117592246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a73a6b4bc2fe0d9e9d6515aee85b0e64beb35afde8718eb65c170d010f1209b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:03:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:03:44 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:03:45 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:04:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:04:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:04:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:04:10 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:04:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:07:50 GMT
ARG MARIADB_MAJOR=10.3
# Sat, 30 Apr 2022 00:07:51 GMT
ENV MARIADB_MAJOR=10.3
# Mon, 23 May 2022 18:44:45 GMT
ARG MARIADB_VERSION=1:10.3.35+maria~focal
# Mon, 23 May 2022 18:44:46 GMT
ENV MARIADB_VERSION=1:10.3.35+maria~focal
# Mon, 23 May 2022 18:44:47 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
# Mon, 23 May 2022 18:44:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 23 May 2022 18:45:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 23 May 2022 18:45:14 GMT
VOLUME [/var/lib/mysql]
# Mon, 23 May 2022 18:45:16 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Mon, 23 May 2022 18:45:17 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Mon, 23 May 2022 18:45:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 23 May 2022 18:45:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 18:45:19 GMT
EXPOSE 3306
# Mon, 23 May 2022 18:45:20 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932d0da437931580c9d7f118c259624e1c3ec8e81acb2acf5740d945e511ba78`  
		Last Modified: Sat, 30 Apr 2022 00:11:03 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc35c765a7328bd99273ee471b6b108980755023d4bcb1927fa7717942a9d318`  
		Last Modified: Sat, 30 Apr 2022 00:11:02 GMT  
		Size: 5.3 MB (5320183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88bae007bd9c42610e465ab436d60b2457b10b735a1bc8e5daba38f548c026`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 3.4 MB (3369899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7734d2f7be989dfe94fb891565830b8101d8e9bdbcbce8e5a7e1b1932eb3ac3c`  
		Last Modified: Sat, 30 Apr 2022 00:11:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24600bac48ce2157027e68df9e26a81754edc6f7e099c33c0a89de879dba5d9`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 2.2 MB (2202385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da05700210f681c47e021b8f3ce45f244f696854cfd656f0cd46e59cb8ca9b7d`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11d91c81167b97fd688c89c8661dd2090b118a00c9e4d5cf447c1f9b984d7ad7`  
		Last Modified: Mon, 23 May 2022 18:50:43 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0abb8afdaeab72a91b2d5af7dc150780f17d2c6f56646fa6ecfc137865aa2dd`  
		Last Modified: Mon, 23 May 2022 18:50:55 GMT  
		Size: 79.5 MB (79515444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a15518853e77b139d69972807cdd43a0752ed028475006e3ff0c1f9e261848d`  
		Last Modified: Mon, 23 May 2022 18:50:43 GMT  
		Size: 3.5 KB (3497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5f0665fe7d2108d19241b1f7d30186abc06e9c55d24aa366a550fa988e8ca9`  
		Last Modified: Mon, 23 May 2022 18:50:43 GMT  
		Size: 6.7 KB (6693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9b8a787243bcd17a20fac81c7addc504f111a3c06c859ae0c4c8ac3c7f0507`  
		Last Modified: Mon, 23 May 2022 18:50:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:d512ce2edbb705fc8f741a1b2df00212e6a7d615cc427c8253915a772129c062
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.0 MB (131036649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78c940a2c84aa82092c4fc95fc1363b732f86115130732a5d7da52820599ee8b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 07 Jun 2022 05:46:02 GMT
ADD file:86506a94b834ba2b6f10dc0d1955bee539be1cf565e4ccc2c4bc074e0375f115 in / 
# Tue, 07 Jun 2022 05:46:06 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 08:57:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 08:57:48 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 08:57:54 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 08:58:44 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 08:58:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 08:59:09 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 08:59:14 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 08:59:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 09:09:30 GMT
ARG MARIADB_MAJOR=10.3
# Tue, 07 Jun 2022 09:09:32 GMT
ENV MARIADB_MAJOR=10.3
# Tue, 07 Jun 2022 09:09:35 GMT
ARG MARIADB_VERSION=1:10.3.35+maria~focal
# Tue, 07 Jun 2022 09:09:37 GMT
ENV MARIADB_VERSION=1:10.3.35+maria~focal
# Tue, 07 Jun 2022 09:09:39 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
# Tue, 07 Jun 2022 09:09:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 09:11:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 09:11:20 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 09:11:22 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 09:11:23 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Tue, 07 Jun 2022 09:11:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 07 Jun 2022 09:11:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 09:11:32 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 09:11:34 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3f52d061d2d3fdde0d3a099bbeae64080476c9650e9f3ba05de898d5bb5f03e8`  
		Last Modified: Tue, 07 Jun 2022 05:49:10 GMT  
		Size: 33.3 MB (33294345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b33a69d2ff59c89a297c597798ade8ea874f546d95513bd628c17fd7afda14`  
		Last Modified: Tue, 07 Jun 2022 09:17:18 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56a2c22a499e4928a88ae9201c66f507be8b9f10804ea7d0934710a6f91e5ec5`  
		Last Modified: Tue, 07 Jun 2022 09:17:18 GMT  
		Size: 6.7 MB (6667490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892b2ffb492b6d36ce25b68cf708d3c9bc9e0210e0cbbe7f575d3424c35d6b96`  
		Last Modified: Tue, 07 Jun 2022 09:17:17 GMT  
		Size: 3.7 MB (3672362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f80e77ec2bb0d7d685ca6e56f718adc6d253a98e069ebd5439f0c973194758`  
		Last Modified: Tue, 07 Jun 2022 09:17:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b0b3a9b79c49528e8e9da2d5d4954fc4e5392ee848c19c52a4d3369feb63d9`  
		Last Modified: Tue, 07 Jun 2022 09:17:16 GMT  
		Size: 2.6 MB (2568258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617e76c5eb45b560720c75ad4c60429a026cbbcb8467360cc70a7dace9ec4e5a`  
		Last Modified: Tue, 07 Jun 2022 09:17:13 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c76afa2f9b8c0de0c04d0255b8646667dee277f515efd76c4b8d25abc36d573b`  
		Last Modified: Tue, 07 Jun 2022 09:19:59 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a5c6e4389d875da6bb41a51b291b7b41e131ab216972ac29700f2c5136e124e`  
		Last Modified: Tue, 07 Jun 2022 09:20:16 GMT  
		Size: 84.8 MB (84819169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ee4158a6f6c038083a106a52ac8dbfcd5cc6b3d0e0b2ff91dd1d0673a892ecf`  
		Last Modified: Tue, 07 Jun 2022 09:19:59 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6738a30bf3051aecf38054c4526a741830fc7f9972b0c4184480dcde66a275b5`  
		Last Modified: Tue, 07 Jun 2022 09:19:59 GMT  
		Size: 6.7 KB (6691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df92c20d5b09a08ff94318bd4d3f6f6ace8697ccf0463d4800fd4e310c6e891d`  
		Last Modified: Tue, 07 Jun 2022 09:19:59 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3.35`

```console
$ docker pull mariadb@sha256:46ed12b7c2b89b8ea9690861ada81f50f2ba3eccfb7a820d5fcb295c83431e6a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3.35` - linux; amd64

```console
$ docker pull mariadb@sha256:8185282e1c12d51e3b1b7043e7c541196b33fa7d71f5df4d26c0f6cb5b1a023b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.2 MB (120166559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7211b4227b56738c0dc31ba1b2c15c322134f707ac0a2ee0accd2e8d6838913`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:42:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 00:42:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:42:35 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 00:42:46 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 00:42:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 00:42:53 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:42:53 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 00:42:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 00:45:01 GMT
ARG MARIADB_MAJOR=10.3
# Tue, 07 Jun 2022 00:45:01 GMT
ENV MARIADB_MAJOR=10.3
# Tue, 07 Jun 2022 00:45:01 GMT
ARG MARIADB_VERSION=1:10.3.35+maria~focal
# Tue, 07 Jun 2022 00:45:01 GMT
ENV MARIADB_VERSION=1:10.3.35+maria~focal
# Tue, 07 Jun 2022 00:45:01 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
# Tue, 07 Jun 2022 00:45:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 00:45:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 00:45:33 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 00:45:33 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 00:45:33 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Tue, 07 Jun 2022 00:45:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 07 Jun 2022 00:45:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 00:45:34 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 00:45:34 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59dcb80bbedb867b19c4eb004e84c86ae3475041d5bd11672bae9ba6be45084f`  
		Last Modified: Tue, 07 Jun 2022 00:48:53 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6c41888e0f25dece871c7e65daad879fc39d7da0a84f6b67ae0d4e1f4a6f8a`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 5.5 MB (5488991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de82bf1cd45986845f81bc71a119bf5ceaec50c145064ea58e5729f4bd6d0d22`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 3.6 MB (3585352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316c0826d235e46a7a9adcfcc3068c004818dc2611a41b69e6e7bea02316b70f`  
		Last Modified: Tue, 07 Jun 2022 00:48:51 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b82e623f5d9ed1cc04e5adc22adc6805abdba4aecc5b427aec6c31223a64dca6`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 2.3 MB (2272315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3daba1f86bc0fd099576f61e5eea0961cdefed1dc443ffb96b6a50c8f054b0b0`  
		Last Modified: Tue, 07 Jun 2022 00:48:49 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae5f5297e44fa8576d8cba5edeb0f6bcbba2d13d78504733a435edfaf675f4c`  
		Last Modified: Tue, 07 Jun 2022 00:50:47 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a399420e15d3f88656c1aa23156f8f0ffbe901be2cbdb04da21287497777194b`  
		Last Modified: Tue, 07 Jun 2022 00:50:59 GMT  
		Size: 80.2 MB (80232253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1179237169a7302cbd05986d859802c88f4c40b14685a714887740fdbe64f391`  
		Last Modified: Tue, 07 Jun 2022 00:50:47 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b09ecefdf18e9d3e4120a212b98d8a8f1be59b53626af7376d2448dfcf5e30ec`  
		Last Modified: Tue, 07 Jun 2022 00:50:47 GMT  
		Size: 6.7 KB (6690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ebffa6e7f3bd3d44b65a9ede071f8fda7929387c29dc8efbe18ecd5fe68c69a`  
		Last Modified: Tue, 07 Jun 2022 00:50:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.35` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:29eba27ea2398b359c15ad9cd8382727f7a95651a86914393df1d2ba6fdedb7d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117592246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a73a6b4bc2fe0d9e9d6515aee85b0e64beb35afde8718eb65c170d010f1209b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:03:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:03:44 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:03:45 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:04:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:04:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:04:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:04:10 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:04:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:07:50 GMT
ARG MARIADB_MAJOR=10.3
# Sat, 30 Apr 2022 00:07:51 GMT
ENV MARIADB_MAJOR=10.3
# Mon, 23 May 2022 18:44:45 GMT
ARG MARIADB_VERSION=1:10.3.35+maria~focal
# Mon, 23 May 2022 18:44:46 GMT
ENV MARIADB_VERSION=1:10.3.35+maria~focal
# Mon, 23 May 2022 18:44:47 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
# Mon, 23 May 2022 18:44:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 23 May 2022 18:45:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 23 May 2022 18:45:14 GMT
VOLUME [/var/lib/mysql]
# Mon, 23 May 2022 18:45:16 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Mon, 23 May 2022 18:45:17 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Mon, 23 May 2022 18:45:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 23 May 2022 18:45:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 18:45:19 GMT
EXPOSE 3306
# Mon, 23 May 2022 18:45:20 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932d0da437931580c9d7f118c259624e1c3ec8e81acb2acf5740d945e511ba78`  
		Last Modified: Sat, 30 Apr 2022 00:11:03 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc35c765a7328bd99273ee471b6b108980755023d4bcb1927fa7717942a9d318`  
		Last Modified: Sat, 30 Apr 2022 00:11:02 GMT  
		Size: 5.3 MB (5320183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88bae007bd9c42610e465ab436d60b2457b10b735a1bc8e5daba38f548c026`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 3.4 MB (3369899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7734d2f7be989dfe94fb891565830b8101d8e9bdbcbce8e5a7e1b1932eb3ac3c`  
		Last Modified: Sat, 30 Apr 2022 00:11:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24600bac48ce2157027e68df9e26a81754edc6f7e099c33c0a89de879dba5d9`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 2.2 MB (2202385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da05700210f681c47e021b8f3ce45f244f696854cfd656f0cd46e59cb8ca9b7d`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11d91c81167b97fd688c89c8661dd2090b118a00c9e4d5cf447c1f9b984d7ad7`  
		Last Modified: Mon, 23 May 2022 18:50:43 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0abb8afdaeab72a91b2d5af7dc150780f17d2c6f56646fa6ecfc137865aa2dd`  
		Last Modified: Mon, 23 May 2022 18:50:55 GMT  
		Size: 79.5 MB (79515444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a15518853e77b139d69972807cdd43a0752ed028475006e3ff0c1f9e261848d`  
		Last Modified: Mon, 23 May 2022 18:50:43 GMT  
		Size: 3.5 KB (3497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5f0665fe7d2108d19241b1f7d30186abc06e9c55d24aa366a550fa988e8ca9`  
		Last Modified: Mon, 23 May 2022 18:50:43 GMT  
		Size: 6.7 KB (6693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9b8a787243bcd17a20fac81c7addc504f111a3c06c859ae0c4c8ac3c7f0507`  
		Last Modified: Mon, 23 May 2022 18:50:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.35` - linux; ppc64le

```console
$ docker pull mariadb@sha256:d512ce2edbb705fc8f741a1b2df00212e6a7d615cc427c8253915a772129c062
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.0 MB (131036649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78c940a2c84aa82092c4fc95fc1363b732f86115130732a5d7da52820599ee8b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 07 Jun 2022 05:46:02 GMT
ADD file:86506a94b834ba2b6f10dc0d1955bee539be1cf565e4ccc2c4bc074e0375f115 in / 
# Tue, 07 Jun 2022 05:46:06 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 08:57:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 08:57:48 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 08:57:54 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 08:58:44 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 08:58:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 08:59:09 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 08:59:14 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 08:59:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 09:09:30 GMT
ARG MARIADB_MAJOR=10.3
# Tue, 07 Jun 2022 09:09:32 GMT
ENV MARIADB_MAJOR=10.3
# Tue, 07 Jun 2022 09:09:35 GMT
ARG MARIADB_VERSION=1:10.3.35+maria~focal
# Tue, 07 Jun 2022 09:09:37 GMT
ENV MARIADB_VERSION=1:10.3.35+maria~focal
# Tue, 07 Jun 2022 09:09:39 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
# Tue, 07 Jun 2022 09:09:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 09:11:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 09:11:20 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 09:11:22 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 09:11:23 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Tue, 07 Jun 2022 09:11:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 07 Jun 2022 09:11:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 09:11:32 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 09:11:34 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3f52d061d2d3fdde0d3a099bbeae64080476c9650e9f3ba05de898d5bb5f03e8`  
		Last Modified: Tue, 07 Jun 2022 05:49:10 GMT  
		Size: 33.3 MB (33294345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b33a69d2ff59c89a297c597798ade8ea874f546d95513bd628c17fd7afda14`  
		Last Modified: Tue, 07 Jun 2022 09:17:18 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56a2c22a499e4928a88ae9201c66f507be8b9f10804ea7d0934710a6f91e5ec5`  
		Last Modified: Tue, 07 Jun 2022 09:17:18 GMT  
		Size: 6.7 MB (6667490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892b2ffb492b6d36ce25b68cf708d3c9bc9e0210e0cbbe7f575d3424c35d6b96`  
		Last Modified: Tue, 07 Jun 2022 09:17:17 GMT  
		Size: 3.7 MB (3672362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f80e77ec2bb0d7d685ca6e56f718adc6d253a98e069ebd5439f0c973194758`  
		Last Modified: Tue, 07 Jun 2022 09:17:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b0b3a9b79c49528e8e9da2d5d4954fc4e5392ee848c19c52a4d3369feb63d9`  
		Last Modified: Tue, 07 Jun 2022 09:17:16 GMT  
		Size: 2.6 MB (2568258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617e76c5eb45b560720c75ad4c60429a026cbbcb8467360cc70a7dace9ec4e5a`  
		Last Modified: Tue, 07 Jun 2022 09:17:13 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c76afa2f9b8c0de0c04d0255b8646667dee277f515efd76c4b8d25abc36d573b`  
		Last Modified: Tue, 07 Jun 2022 09:19:59 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a5c6e4389d875da6bb41a51b291b7b41e131ab216972ac29700f2c5136e124e`  
		Last Modified: Tue, 07 Jun 2022 09:20:16 GMT  
		Size: 84.8 MB (84819169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ee4158a6f6c038083a106a52ac8dbfcd5cc6b3d0e0b2ff91dd1d0673a892ecf`  
		Last Modified: Tue, 07 Jun 2022 09:19:59 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6738a30bf3051aecf38054c4526a741830fc7f9972b0c4184480dcde66a275b5`  
		Last Modified: Tue, 07 Jun 2022 09:19:59 GMT  
		Size: 6.7 KB (6691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df92c20d5b09a08ff94318bd4d3f6f6ace8697ccf0463d4800fd4e310c6e891d`  
		Last Modified: Tue, 07 Jun 2022 09:19:59 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3.35-focal`

```console
$ docker pull mariadb@sha256:46ed12b7c2b89b8ea9690861ada81f50f2ba3eccfb7a820d5fcb295c83431e6a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3.35-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:8185282e1c12d51e3b1b7043e7c541196b33fa7d71f5df4d26c0f6cb5b1a023b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.2 MB (120166559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7211b4227b56738c0dc31ba1b2c15c322134f707ac0a2ee0accd2e8d6838913`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:42:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 00:42:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:42:35 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 00:42:46 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 00:42:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 00:42:53 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:42:53 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 00:42:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 00:45:01 GMT
ARG MARIADB_MAJOR=10.3
# Tue, 07 Jun 2022 00:45:01 GMT
ENV MARIADB_MAJOR=10.3
# Tue, 07 Jun 2022 00:45:01 GMT
ARG MARIADB_VERSION=1:10.3.35+maria~focal
# Tue, 07 Jun 2022 00:45:01 GMT
ENV MARIADB_VERSION=1:10.3.35+maria~focal
# Tue, 07 Jun 2022 00:45:01 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
# Tue, 07 Jun 2022 00:45:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 00:45:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 00:45:33 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 00:45:33 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 00:45:33 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Tue, 07 Jun 2022 00:45:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 07 Jun 2022 00:45:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 00:45:34 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 00:45:34 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59dcb80bbedb867b19c4eb004e84c86ae3475041d5bd11672bae9ba6be45084f`  
		Last Modified: Tue, 07 Jun 2022 00:48:53 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6c41888e0f25dece871c7e65daad879fc39d7da0a84f6b67ae0d4e1f4a6f8a`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 5.5 MB (5488991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de82bf1cd45986845f81bc71a119bf5ceaec50c145064ea58e5729f4bd6d0d22`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 3.6 MB (3585352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316c0826d235e46a7a9adcfcc3068c004818dc2611a41b69e6e7bea02316b70f`  
		Last Modified: Tue, 07 Jun 2022 00:48:51 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b82e623f5d9ed1cc04e5adc22adc6805abdba4aecc5b427aec6c31223a64dca6`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 2.3 MB (2272315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3daba1f86bc0fd099576f61e5eea0961cdefed1dc443ffb96b6a50c8f054b0b0`  
		Last Modified: Tue, 07 Jun 2022 00:48:49 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae5f5297e44fa8576d8cba5edeb0f6bcbba2d13d78504733a435edfaf675f4c`  
		Last Modified: Tue, 07 Jun 2022 00:50:47 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a399420e15d3f88656c1aa23156f8f0ffbe901be2cbdb04da21287497777194b`  
		Last Modified: Tue, 07 Jun 2022 00:50:59 GMT  
		Size: 80.2 MB (80232253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1179237169a7302cbd05986d859802c88f4c40b14685a714887740fdbe64f391`  
		Last Modified: Tue, 07 Jun 2022 00:50:47 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b09ecefdf18e9d3e4120a212b98d8a8f1be59b53626af7376d2448dfcf5e30ec`  
		Last Modified: Tue, 07 Jun 2022 00:50:47 GMT  
		Size: 6.7 KB (6690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ebffa6e7f3bd3d44b65a9ede071f8fda7929387c29dc8efbe18ecd5fe68c69a`  
		Last Modified: Tue, 07 Jun 2022 00:50:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.35-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:29eba27ea2398b359c15ad9cd8382727f7a95651a86914393df1d2ba6fdedb7d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117592246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a73a6b4bc2fe0d9e9d6515aee85b0e64beb35afde8718eb65c170d010f1209b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:03:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:03:44 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:03:45 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:04:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:04:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:04:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:04:10 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:04:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:07:50 GMT
ARG MARIADB_MAJOR=10.3
# Sat, 30 Apr 2022 00:07:51 GMT
ENV MARIADB_MAJOR=10.3
# Mon, 23 May 2022 18:44:45 GMT
ARG MARIADB_VERSION=1:10.3.35+maria~focal
# Mon, 23 May 2022 18:44:46 GMT
ENV MARIADB_VERSION=1:10.3.35+maria~focal
# Mon, 23 May 2022 18:44:47 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
# Mon, 23 May 2022 18:44:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 23 May 2022 18:45:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 23 May 2022 18:45:14 GMT
VOLUME [/var/lib/mysql]
# Mon, 23 May 2022 18:45:16 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Mon, 23 May 2022 18:45:17 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Mon, 23 May 2022 18:45:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 23 May 2022 18:45:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 18:45:19 GMT
EXPOSE 3306
# Mon, 23 May 2022 18:45:20 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932d0da437931580c9d7f118c259624e1c3ec8e81acb2acf5740d945e511ba78`  
		Last Modified: Sat, 30 Apr 2022 00:11:03 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc35c765a7328bd99273ee471b6b108980755023d4bcb1927fa7717942a9d318`  
		Last Modified: Sat, 30 Apr 2022 00:11:02 GMT  
		Size: 5.3 MB (5320183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88bae007bd9c42610e465ab436d60b2457b10b735a1bc8e5daba38f548c026`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 3.4 MB (3369899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7734d2f7be989dfe94fb891565830b8101d8e9bdbcbce8e5a7e1b1932eb3ac3c`  
		Last Modified: Sat, 30 Apr 2022 00:11:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24600bac48ce2157027e68df9e26a81754edc6f7e099c33c0a89de879dba5d9`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 2.2 MB (2202385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da05700210f681c47e021b8f3ce45f244f696854cfd656f0cd46e59cb8ca9b7d`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11d91c81167b97fd688c89c8661dd2090b118a00c9e4d5cf447c1f9b984d7ad7`  
		Last Modified: Mon, 23 May 2022 18:50:43 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0abb8afdaeab72a91b2d5af7dc150780f17d2c6f56646fa6ecfc137865aa2dd`  
		Last Modified: Mon, 23 May 2022 18:50:55 GMT  
		Size: 79.5 MB (79515444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a15518853e77b139d69972807cdd43a0752ed028475006e3ff0c1f9e261848d`  
		Last Modified: Mon, 23 May 2022 18:50:43 GMT  
		Size: 3.5 KB (3497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5f0665fe7d2108d19241b1f7d30186abc06e9c55d24aa366a550fa988e8ca9`  
		Last Modified: Mon, 23 May 2022 18:50:43 GMT  
		Size: 6.7 KB (6693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9b8a787243bcd17a20fac81c7addc504f111a3c06c859ae0c4c8ac3c7f0507`  
		Last Modified: Mon, 23 May 2022 18:50:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.35-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:d512ce2edbb705fc8f741a1b2df00212e6a7d615cc427c8253915a772129c062
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.0 MB (131036649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78c940a2c84aa82092c4fc95fc1363b732f86115130732a5d7da52820599ee8b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 07 Jun 2022 05:46:02 GMT
ADD file:86506a94b834ba2b6f10dc0d1955bee539be1cf565e4ccc2c4bc074e0375f115 in / 
# Tue, 07 Jun 2022 05:46:06 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 08:57:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 08:57:48 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 08:57:54 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 08:58:44 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 08:58:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 08:59:09 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 08:59:14 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 08:59:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 09:09:30 GMT
ARG MARIADB_MAJOR=10.3
# Tue, 07 Jun 2022 09:09:32 GMT
ENV MARIADB_MAJOR=10.3
# Tue, 07 Jun 2022 09:09:35 GMT
ARG MARIADB_VERSION=1:10.3.35+maria~focal
# Tue, 07 Jun 2022 09:09:37 GMT
ENV MARIADB_VERSION=1:10.3.35+maria~focal
# Tue, 07 Jun 2022 09:09:39 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
# Tue, 07 Jun 2022 09:09:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 09:11:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 09:11:20 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 09:11:22 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 09:11:23 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Tue, 07 Jun 2022 09:11:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.35/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 07 Jun 2022 09:11:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 09:11:32 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 09:11:34 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3f52d061d2d3fdde0d3a099bbeae64080476c9650e9f3ba05de898d5bb5f03e8`  
		Last Modified: Tue, 07 Jun 2022 05:49:10 GMT  
		Size: 33.3 MB (33294345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b33a69d2ff59c89a297c597798ade8ea874f546d95513bd628c17fd7afda14`  
		Last Modified: Tue, 07 Jun 2022 09:17:18 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56a2c22a499e4928a88ae9201c66f507be8b9f10804ea7d0934710a6f91e5ec5`  
		Last Modified: Tue, 07 Jun 2022 09:17:18 GMT  
		Size: 6.7 MB (6667490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892b2ffb492b6d36ce25b68cf708d3c9bc9e0210e0cbbe7f575d3424c35d6b96`  
		Last Modified: Tue, 07 Jun 2022 09:17:17 GMT  
		Size: 3.7 MB (3672362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f80e77ec2bb0d7d685ca6e56f718adc6d253a98e069ebd5439f0c973194758`  
		Last Modified: Tue, 07 Jun 2022 09:17:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b0b3a9b79c49528e8e9da2d5d4954fc4e5392ee848c19c52a4d3369feb63d9`  
		Last Modified: Tue, 07 Jun 2022 09:17:16 GMT  
		Size: 2.6 MB (2568258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617e76c5eb45b560720c75ad4c60429a026cbbcb8467360cc70a7dace9ec4e5a`  
		Last Modified: Tue, 07 Jun 2022 09:17:13 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c76afa2f9b8c0de0c04d0255b8646667dee277f515efd76c4b8d25abc36d573b`  
		Last Modified: Tue, 07 Jun 2022 09:19:59 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a5c6e4389d875da6bb41a51b291b7b41e131ab216972ac29700f2c5136e124e`  
		Last Modified: Tue, 07 Jun 2022 09:20:16 GMT  
		Size: 84.8 MB (84819169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ee4158a6f6c038083a106a52ac8dbfcd5cc6b3d0e0b2ff91dd1d0673a892ecf`  
		Last Modified: Tue, 07 Jun 2022 09:19:59 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6738a30bf3051aecf38054c4526a741830fc7f9972b0c4184480dcde66a275b5`  
		Last Modified: Tue, 07 Jun 2022 09:19:59 GMT  
		Size: 6.7 KB (6691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df92c20d5b09a08ff94318bd4d3f6f6ace8697ccf0463d4800fd4e310c6e891d`  
		Last Modified: Tue, 07 Jun 2022 09:19:59 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4`

```console
$ docker pull mariadb@sha256:d1bd4c46e650e414b54c1667dcaca6ff3e6c044c2682600e477fcbfa4129b1f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4` - linux; amd64

```console
$ docker pull mariadb@sha256:9e962ec1649ede39337396d097572a561dd718cfb8acb99b657facf25ee25cab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.8 MB (125780636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8981e672fce893dc60d226f2969193dbd8139e589df7620eed2c4ff1505d309`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:42:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 00:42:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:42:35 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 00:42:46 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 00:42:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 00:42:53 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:42:53 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 00:42:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 00:44:32 GMT
ARG MARIADB_MAJOR=10.4
# Tue, 07 Jun 2022 00:44:32 GMT
ENV MARIADB_MAJOR=10.4
# Tue, 07 Jun 2022 00:44:32 GMT
ARG MARIADB_VERSION=1:10.4.25+maria~focal
# Tue, 07 Jun 2022 00:44:32 GMT
ENV MARIADB_VERSION=1:10.4.25+maria~focal
# Tue, 07 Jun 2022 00:44:32 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
# Tue, 07 Jun 2022 00:44:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 00:44:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 00:44:57 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 00:44:57 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 00:44:57 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Tue, 07 Jun 2022 00:44:58 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 07 Jun 2022 00:44:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 00:44:58 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 00:44:58 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59dcb80bbedb867b19c4eb004e84c86ae3475041d5bd11672bae9ba6be45084f`  
		Last Modified: Tue, 07 Jun 2022 00:48:53 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6c41888e0f25dece871c7e65daad879fc39d7da0a84f6b67ae0d4e1f4a6f8a`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 5.5 MB (5488991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de82bf1cd45986845f81bc71a119bf5ceaec50c145064ea58e5729f4bd6d0d22`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 3.6 MB (3585352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316c0826d235e46a7a9adcfcc3068c004818dc2611a41b69e6e7bea02316b70f`  
		Last Modified: Tue, 07 Jun 2022 00:48:51 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b82e623f5d9ed1cc04e5adc22adc6805abdba4aecc5b427aec6c31223a64dca6`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 2.3 MB (2272315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3daba1f86bc0fd099576f61e5eea0961cdefed1dc443ffb96b6a50c8f054b0b0`  
		Last Modified: Tue, 07 Jun 2022 00:48:49 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d04945d0545a6b71992ae420ca2a5171ff5453e1ecb4dcb614474bb4a02fdcac`  
		Last Modified: Tue, 07 Jun 2022 00:50:17 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3088ccc5e6c7fe86d7b86fed452b51e8207ac99f8b8ba930e398ab3eae8b76b2`  
		Last Modified: Tue, 07 Jun 2022 00:50:30 GMT  
		Size: 85.8 MB (85846325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebdc0a737326c786c882e86038a8e63b0005ba52232e81e0e5a3c749715f0ddc`  
		Last Modified: Tue, 07 Jun 2022 00:50:17 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd995425627004eb949201430def2ef647cfbadcaafcca914f8a82a1ae3242d3`  
		Last Modified: Tue, 07 Jun 2022 00:50:17 GMT  
		Size: 6.7 KB (6692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d92cbc5a67b96abbd56f59c94f2a30e8b9ba2a4538bf9e2b3573b56304bc158`  
		Last Modified: Tue, 07 Jun 2022 00:50:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:b696d9967dde3e1cd9881586f686ee75ea09d06635c8a88b73a7b50c86b6bd44
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123119346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bb619353184ac1a2fe6b631fc37d9bdc3d70c013165aa84f9850808082006b7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:03:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:03:44 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:03:45 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:04:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:04:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:04:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:04:10 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:04:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:07:07 GMT
ARG MARIADB_MAJOR=10.4
# Sat, 30 Apr 2022 00:07:07 GMT
ENV MARIADB_MAJOR=10.4
# Mon, 23 May 2022 18:44:08 GMT
ARG MARIADB_VERSION=1:10.4.25+maria~focal
# Mon, 23 May 2022 18:44:09 GMT
ENV MARIADB_VERSION=1:10.4.25+maria~focal
# Mon, 23 May 2022 18:44:10 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
# Mon, 23 May 2022 18:44:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 23 May 2022 18:44:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 23 May 2022 18:44:33 GMT
VOLUME [/var/lib/mysql]
# Mon, 23 May 2022 18:44:35 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Mon, 23 May 2022 18:44:36 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Mon, 23 May 2022 18:44:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 23 May 2022 18:44:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 18:44:38 GMT
EXPOSE 3306
# Mon, 23 May 2022 18:44:39 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932d0da437931580c9d7f118c259624e1c3ec8e81acb2acf5740d945e511ba78`  
		Last Modified: Sat, 30 Apr 2022 00:11:03 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc35c765a7328bd99273ee471b6b108980755023d4bcb1927fa7717942a9d318`  
		Last Modified: Sat, 30 Apr 2022 00:11:02 GMT  
		Size: 5.3 MB (5320183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88bae007bd9c42610e465ab436d60b2457b10b735a1bc8e5daba38f548c026`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 3.4 MB (3369899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7734d2f7be989dfe94fb891565830b8101d8e9bdbcbce8e5a7e1b1932eb3ac3c`  
		Last Modified: Sat, 30 Apr 2022 00:11:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24600bac48ce2157027e68df9e26a81754edc6f7e099c33c0a89de879dba5d9`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 2.2 MB (2202385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da05700210f681c47e021b8f3ce45f244f696854cfd656f0cd46e59cb8ca9b7d`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d50600df49b6f9bff73723902b349ab11ec42e761d0646fcccff56bf32c7b461`  
		Last Modified: Mon, 23 May 2022 18:50:10 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4051cf72966b8af9e322800c50d38e6d18fff7bfae8492301c61c151613b370`  
		Last Modified: Mon, 23 May 2022 18:50:24 GMT  
		Size: 85.0 MB (85042542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d3ed0aea547876d5b696e38dd81c4806366bb023f220b96f36805a66f754cc`  
		Last Modified: Mon, 23 May 2022 18:50:10 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96a0692ed23e8f88ad2c83869dff9292e7e64bf87f985c8f8878047a63801937`  
		Last Modified: Mon, 23 May 2022 18:50:10 GMT  
		Size: 6.7 KB (6696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149c5fe0fb06642c34e7fff4cab2b43a1a6c934270b6eae11e6178a78b3e20ae`  
		Last Modified: Mon, 23 May 2022 18:50:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4` - linux; ppc64le

```console
$ docker pull mariadb@sha256:29dde019f1b746bd1023b2fdcf9fbe670a2fcc604a4afd1ca4c4c4ad1d6ea064
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.7 MB (136667303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccbf91ef7fbb103d9fffe337e99000912262b5b3bce81e6d91b8d1256422f58a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 07 Jun 2022 05:46:02 GMT
ADD file:86506a94b834ba2b6f10dc0d1955bee539be1cf565e4ccc2c4bc074e0375f115 in / 
# Tue, 07 Jun 2022 05:46:06 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 08:57:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 08:57:48 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 08:57:54 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 08:58:44 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 08:58:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 08:59:09 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 08:59:14 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 08:59:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 09:07:20 GMT
ARG MARIADB_MAJOR=10.4
# Tue, 07 Jun 2022 09:07:22 GMT
ENV MARIADB_MAJOR=10.4
# Tue, 07 Jun 2022 09:07:24 GMT
ARG MARIADB_VERSION=1:10.4.25+maria~focal
# Tue, 07 Jun 2022 09:07:25 GMT
ENV MARIADB_VERSION=1:10.4.25+maria~focal
# Tue, 07 Jun 2022 09:07:27 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
# Tue, 07 Jun 2022 09:07:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 09:08:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 09:09:05 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 09:09:07 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 09:09:08 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Tue, 07 Jun 2022 09:09:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 07 Jun 2022 09:09:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 09:09:19 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 09:09:22 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3f52d061d2d3fdde0d3a099bbeae64080476c9650e9f3ba05de898d5bb5f03e8`  
		Last Modified: Tue, 07 Jun 2022 05:49:10 GMT  
		Size: 33.3 MB (33294345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b33a69d2ff59c89a297c597798ade8ea874f546d95513bd628c17fd7afda14`  
		Last Modified: Tue, 07 Jun 2022 09:17:18 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56a2c22a499e4928a88ae9201c66f507be8b9f10804ea7d0934710a6f91e5ec5`  
		Last Modified: Tue, 07 Jun 2022 09:17:18 GMT  
		Size: 6.7 MB (6667490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892b2ffb492b6d36ce25b68cf708d3c9bc9e0210e0cbbe7f575d3424c35d6b96`  
		Last Modified: Tue, 07 Jun 2022 09:17:17 GMT  
		Size: 3.7 MB (3672362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f80e77ec2bb0d7d685ca6e56f718adc6d253a98e069ebd5439f0c973194758`  
		Last Modified: Tue, 07 Jun 2022 09:17:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b0b3a9b79c49528e8e9da2d5d4954fc4e5392ee848c19c52a4d3369feb63d9`  
		Last Modified: Tue, 07 Jun 2022 09:17:16 GMT  
		Size: 2.6 MB (2568258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617e76c5eb45b560720c75ad4c60429a026cbbcb8467360cc70a7dace9ec4e5a`  
		Last Modified: Tue, 07 Jun 2022 09:17:13 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5bba458690d930a53ffeb4ccb714a0990a3bfabc029d7a06b276745a3d2e26`  
		Last Modified: Tue, 07 Jun 2022 09:19:18 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0972b5680a9853b06b6f6353e0d60b6f0998800c4f73ce013ec84bf222df150e`  
		Last Modified: Tue, 07 Jun 2022 09:19:35 GMT  
		Size: 90.4 MB (90449818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a7a156d8e0364e931c31314f6b4e7cb835a8867b26dca4608b7f98365d36b4`  
		Last Modified: Tue, 07 Jun 2022 09:19:18 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac5a7f6e713b2afa7e54814b43084987f41d4c941859dce87c16da7ba6e3d8e`  
		Last Modified: Tue, 07 Jun 2022 09:19:18 GMT  
		Size: 6.7 KB (6693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f3199d673bdcb32dfefb64ee4096b37863c7baea89f8b140d19ba1e68ad32f1`  
		Last Modified: Tue, 07 Jun 2022 09:19:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4-focal`

```console
$ docker pull mariadb@sha256:d1bd4c46e650e414b54c1667dcaca6ff3e6c044c2682600e477fcbfa4129b1f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:9e962ec1649ede39337396d097572a561dd718cfb8acb99b657facf25ee25cab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.8 MB (125780636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8981e672fce893dc60d226f2969193dbd8139e589df7620eed2c4ff1505d309`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:42:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 00:42:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:42:35 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 00:42:46 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 00:42:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 00:42:53 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:42:53 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 00:42:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 00:44:32 GMT
ARG MARIADB_MAJOR=10.4
# Tue, 07 Jun 2022 00:44:32 GMT
ENV MARIADB_MAJOR=10.4
# Tue, 07 Jun 2022 00:44:32 GMT
ARG MARIADB_VERSION=1:10.4.25+maria~focal
# Tue, 07 Jun 2022 00:44:32 GMT
ENV MARIADB_VERSION=1:10.4.25+maria~focal
# Tue, 07 Jun 2022 00:44:32 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
# Tue, 07 Jun 2022 00:44:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 00:44:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 00:44:57 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 00:44:57 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 00:44:57 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Tue, 07 Jun 2022 00:44:58 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 07 Jun 2022 00:44:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 00:44:58 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 00:44:58 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59dcb80bbedb867b19c4eb004e84c86ae3475041d5bd11672bae9ba6be45084f`  
		Last Modified: Tue, 07 Jun 2022 00:48:53 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6c41888e0f25dece871c7e65daad879fc39d7da0a84f6b67ae0d4e1f4a6f8a`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 5.5 MB (5488991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de82bf1cd45986845f81bc71a119bf5ceaec50c145064ea58e5729f4bd6d0d22`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 3.6 MB (3585352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316c0826d235e46a7a9adcfcc3068c004818dc2611a41b69e6e7bea02316b70f`  
		Last Modified: Tue, 07 Jun 2022 00:48:51 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b82e623f5d9ed1cc04e5adc22adc6805abdba4aecc5b427aec6c31223a64dca6`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 2.3 MB (2272315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3daba1f86bc0fd099576f61e5eea0961cdefed1dc443ffb96b6a50c8f054b0b0`  
		Last Modified: Tue, 07 Jun 2022 00:48:49 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d04945d0545a6b71992ae420ca2a5171ff5453e1ecb4dcb614474bb4a02fdcac`  
		Last Modified: Tue, 07 Jun 2022 00:50:17 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3088ccc5e6c7fe86d7b86fed452b51e8207ac99f8b8ba930e398ab3eae8b76b2`  
		Last Modified: Tue, 07 Jun 2022 00:50:30 GMT  
		Size: 85.8 MB (85846325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebdc0a737326c786c882e86038a8e63b0005ba52232e81e0e5a3c749715f0ddc`  
		Last Modified: Tue, 07 Jun 2022 00:50:17 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd995425627004eb949201430def2ef647cfbadcaafcca914f8a82a1ae3242d3`  
		Last Modified: Tue, 07 Jun 2022 00:50:17 GMT  
		Size: 6.7 KB (6692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d92cbc5a67b96abbd56f59c94f2a30e8b9ba2a4538bf9e2b3573b56304bc158`  
		Last Modified: Tue, 07 Jun 2022 00:50:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:b696d9967dde3e1cd9881586f686ee75ea09d06635c8a88b73a7b50c86b6bd44
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123119346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bb619353184ac1a2fe6b631fc37d9bdc3d70c013165aa84f9850808082006b7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:03:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:03:44 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:03:45 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:04:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:04:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:04:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:04:10 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:04:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:07:07 GMT
ARG MARIADB_MAJOR=10.4
# Sat, 30 Apr 2022 00:07:07 GMT
ENV MARIADB_MAJOR=10.4
# Mon, 23 May 2022 18:44:08 GMT
ARG MARIADB_VERSION=1:10.4.25+maria~focal
# Mon, 23 May 2022 18:44:09 GMT
ENV MARIADB_VERSION=1:10.4.25+maria~focal
# Mon, 23 May 2022 18:44:10 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
# Mon, 23 May 2022 18:44:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 23 May 2022 18:44:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 23 May 2022 18:44:33 GMT
VOLUME [/var/lib/mysql]
# Mon, 23 May 2022 18:44:35 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Mon, 23 May 2022 18:44:36 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Mon, 23 May 2022 18:44:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 23 May 2022 18:44:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 18:44:38 GMT
EXPOSE 3306
# Mon, 23 May 2022 18:44:39 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932d0da437931580c9d7f118c259624e1c3ec8e81acb2acf5740d945e511ba78`  
		Last Modified: Sat, 30 Apr 2022 00:11:03 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc35c765a7328bd99273ee471b6b108980755023d4bcb1927fa7717942a9d318`  
		Last Modified: Sat, 30 Apr 2022 00:11:02 GMT  
		Size: 5.3 MB (5320183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88bae007bd9c42610e465ab436d60b2457b10b735a1bc8e5daba38f548c026`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 3.4 MB (3369899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7734d2f7be989dfe94fb891565830b8101d8e9bdbcbce8e5a7e1b1932eb3ac3c`  
		Last Modified: Sat, 30 Apr 2022 00:11:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24600bac48ce2157027e68df9e26a81754edc6f7e099c33c0a89de879dba5d9`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 2.2 MB (2202385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da05700210f681c47e021b8f3ce45f244f696854cfd656f0cd46e59cb8ca9b7d`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d50600df49b6f9bff73723902b349ab11ec42e761d0646fcccff56bf32c7b461`  
		Last Modified: Mon, 23 May 2022 18:50:10 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4051cf72966b8af9e322800c50d38e6d18fff7bfae8492301c61c151613b370`  
		Last Modified: Mon, 23 May 2022 18:50:24 GMT  
		Size: 85.0 MB (85042542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d3ed0aea547876d5b696e38dd81c4806366bb023f220b96f36805a66f754cc`  
		Last Modified: Mon, 23 May 2022 18:50:10 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96a0692ed23e8f88ad2c83869dff9292e7e64bf87f985c8f8878047a63801937`  
		Last Modified: Mon, 23 May 2022 18:50:10 GMT  
		Size: 6.7 KB (6696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149c5fe0fb06642c34e7fff4cab2b43a1a6c934270b6eae11e6178a78b3e20ae`  
		Last Modified: Mon, 23 May 2022 18:50:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:29dde019f1b746bd1023b2fdcf9fbe670a2fcc604a4afd1ca4c4c4ad1d6ea064
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.7 MB (136667303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccbf91ef7fbb103d9fffe337e99000912262b5b3bce81e6d91b8d1256422f58a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 07 Jun 2022 05:46:02 GMT
ADD file:86506a94b834ba2b6f10dc0d1955bee539be1cf565e4ccc2c4bc074e0375f115 in / 
# Tue, 07 Jun 2022 05:46:06 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 08:57:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 08:57:48 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 08:57:54 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 08:58:44 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 08:58:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 08:59:09 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 08:59:14 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 08:59:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 09:07:20 GMT
ARG MARIADB_MAJOR=10.4
# Tue, 07 Jun 2022 09:07:22 GMT
ENV MARIADB_MAJOR=10.4
# Tue, 07 Jun 2022 09:07:24 GMT
ARG MARIADB_VERSION=1:10.4.25+maria~focal
# Tue, 07 Jun 2022 09:07:25 GMT
ENV MARIADB_VERSION=1:10.4.25+maria~focal
# Tue, 07 Jun 2022 09:07:27 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
# Tue, 07 Jun 2022 09:07:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 09:08:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 09:09:05 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 09:09:07 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 09:09:08 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Tue, 07 Jun 2022 09:09:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 07 Jun 2022 09:09:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 09:09:19 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 09:09:22 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3f52d061d2d3fdde0d3a099bbeae64080476c9650e9f3ba05de898d5bb5f03e8`  
		Last Modified: Tue, 07 Jun 2022 05:49:10 GMT  
		Size: 33.3 MB (33294345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b33a69d2ff59c89a297c597798ade8ea874f546d95513bd628c17fd7afda14`  
		Last Modified: Tue, 07 Jun 2022 09:17:18 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56a2c22a499e4928a88ae9201c66f507be8b9f10804ea7d0934710a6f91e5ec5`  
		Last Modified: Tue, 07 Jun 2022 09:17:18 GMT  
		Size: 6.7 MB (6667490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892b2ffb492b6d36ce25b68cf708d3c9bc9e0210e0cbbe7f575d3424c35d6b96`  
		Last Modified: Tue, 07 Jun 2022 09:17:17 GMT  
		Size: 3.7 MB (3672362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f80e77ec2bb0d7d685ca6e56f718adc6d253a98e069ebd5439f0c973194758`  
		Last Modified: Tue, 07 Jun 2022 09:17:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b0b3a9b79c49528e8e9da2d5d4954fc4e5392ee848c19c52a4d3369feb63d9`  
		Last Modified: Tue, 07 Jun 2022 09:17:16 GMT  
		Size: 2.6 MB (2568258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617e76c5eb45b560720c75ad4c60429a026cbbcb8467360cc70a7dace9ec4e5a`  
		Last Modified: Tue, 07 Jun 2022 09:17:13 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5bba458690d930a53ffeb4ccb714a0990a3bfabc029d7a06b276745a3d2e26`  
		Last Modified: Tue, 07 Jun 2022 09:19:18 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0972b5680a9853b06b6f6353e0d60b6f0998800c4f73ce013ec84bf222df150e`  
		Last Modified: Tue, 07 Jun 2022 09:19:35 GMT  
		Size: 90.4 MB (90449818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a7a156d8e0364e931c31314f6b4e7cb835a8867b26dca4608b7f98365d36b4`  
		Last Modified: Tue, 07 Jun 2022 09:19:18 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac5a7f6e713b2afa7e54814b43084987f41d4c941859dce87c16da7ba6e3d8e`  
		Last Modified: Tue, 07 Jun 2022 09:19:18 GMT  
		Size: 6.7 KB (6693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f3199d673bdcb32dfefb64ee4096b37863c7baea89f8b140d19ba1e68ad32f1`  
		Last Modified: Tue, 07 Jun 2022 09:19:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4.25`

```console
$ docker pull mariadb@sha256:d1bd4c46e650e414b54c1667dcaca6ff3e6c044c2682600e477fcbfa4129b1f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4.25` - linux; amd64

```console
$ docker pull mariadb@sha256:9e962ec1649ede39337396d097572a561dd718cfb8acb99b657facf25ee25cab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.8 MB (125780636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8981e672fce893dc60d226f2969193dbd8139e589df7620eed2c4ff1505d309`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:42:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 00:42:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:42:35 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 00:42:46 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 00:42:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 00:42:53 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:42:53 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 00:42:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 00:44:32 GMT
ARG MARIADB_MAJOR=10.4
# Tue, 07 Jun 2022 00:44:32 GMT
ENV MARIADB_MAJOR=10.4
# Tue, 07 Jun 2022 00:44:32 GMT
ARG MARIADB_VERSION=1:10.4.25+maria~focal
# Tue, 07 Jun 2022 00:44:32 GMT
ENV MARIADB_VERSION=1:10.4.25+maria~focal
# Tue, 07 Jun 2022 00:44:32 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
# Tue, 07 Jun 2022 00:44:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 00:44:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 00:44:57 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 00:44:57 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 00:44:57 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Tue, 07 Jun 2022 00:44:58 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 07 Jun 2022 00:44:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 00:44:58 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 00:44:58 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59dcb80bbedb867b19c4eb004e84c86ae3475041d5bd11672bae9ba6be45084f`  
		Last Modified: Tue, 07 Jun 2022 00:48:53 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6c41888e0f25dece871c7e65daad879fc39d7da0a84f6b67ae0d4e1f4a6f8a`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 5.5 MB (5488991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de82bf1cd45986845f81bc71a119bf5ceaec50c145064ea58e5729f4bd6d0d22`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 3.6 MB (3585352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316c0826d235e46a7a9adcfcc3068c004818dc2611a41b69e6e7bea02316b70f`  
		Last Modified: Tue, 07 Jun 2022 00:48:51 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b82e623f5d9ed1cc04e5adc22adc6805abdba4aecc5b427aec6c31223a64dca6`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 2.3 MB (2272315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3daba1f86bc0fd099576f61e5eea0961cdefed1dc443ffb96b6a50c8f054b0b0`  
		Last Modified: Tue, 07 Jun 2022 00:48:49 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d04945d0545a6b71992ae420ca2a5171ff5453e1ecb4dcb614474bb4a02fdcac`  
		Last Modified: Tue, 07 Jun 2022 00:50:17 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3088ccc5e6c7fe86d7b86fed452b51e8207ac99f8b8ba930e398ab3eae8b76b2`  
		Last Modified: Tue, 07 Jun 2022 00:50:30 GMT  
		Size: 85.8 MB (85846325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebdc0a737326c786c882e86038a8e63b0005ba52232e81e0e5a3c749715f0ddc`  
		Last Modified: Tue, 07 Jun 2022 00:50:17 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd995425627004eb949201430def2ef647cfbadcaafcca914f8a82a1ae3242d3`  
		Last Modified: Tue, 07 Jun 2022 00:50:17 GMT  
		Size: 6.7 KB (6692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d92cbc5a67b96abbd56f59c94f2a30e8b9ba2a4538bf9e2b3573b56304bc158`  
		Last Modified: Tue, 07 Jun 2022 00:50:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.25` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:b696d9967dde3e1cd9881586f686ee75ea09d06635c8a88b73a7b50c86b6bd44
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123119346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bb619353184ac1a2fe6b631fc37d9bdc3d70c013165aa84f9850808082006b7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:03:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:03:44 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:03:45 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:04:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:04:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:04:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:04:10 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:04:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:07:07 GMT
ARG MARIADB_MAJOR=10.4
# Sat, 30 Apr 2022 00:07:07 GMT
ENV MARIADB_MAJOR=10.4
# Mon, 23 May 2022 18:44:08 GMT
ARG MARIADB_VERSION=1:10.4.25+maria~focal
# Mon, 23 May 2022 18:44:09 GMT
ENV MARIADB_VERSION=1:10.4.25+maria~focal
# Mon, 23 May 2022 18:44:10 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
# Mon, 23 May 2022 18:44:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 23 May 2022 18:44:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 23 May 2022 18:44:33 GMT
VOLUME [/var/lib/mysql]
# Mon, 23 May 2022 18:44:35 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Mon, 23 May 2022 18:44:36 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Mon, 23 May 2022 18:44:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 23 May 2022 18:44:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 18:44:38 GMT
EXPOSE 3306
# Mon, 23 May 2022 18:44:39 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932d0da437931580c9d7f118c259624e1c3ec8e81acb2acf5740d945e511ba78`  
		Last Modified: Sat, 30 Apr 2022 00:11:03 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc35c765a7328bd99273ee471b6b108980755023d4bcb1927fa7717942a9d318`  
		Last Modified: Sat, 30 Apr 2022 00:11:02 GMT  
		Size: 5.3 MB (5320183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88bae007bd9c42610e465ab436d60b2457b10b735a1bc8e5daba38f548c026`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 3.4 MB (3369899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7734d2f7be989dfe94fb891565830b8101d8e9bdbcbce8e5a7e1b1932eb3ac3c`  
		Last Modified: Sat, 30 Apr 2022 00:11:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24600bac48ce2157027e68df9e26a81754edc6f7e099c33c0a89de879dba5d9`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 2.2 MB (2202385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da05700210f681c47e021b8f3ce45f244f696854cfd656f0cd46e59cb8ca9b7d`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d50600df49b6f9bff73723902b349ab11ec42e761d0646fcccff56bf32c7b461`  
		Last Modified: Mon, 23 May 2022 18:50:10 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4051cf72966b8af9e322800c50d38e6d18fff7bfae8492301c61c151613b370`  
		Last Modified: Mon, 23 May 2022 18:50:24 GMT  
		Size: 85.0 MB (85042542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d3ed0aea547876d5b696e38dd81c4806366bb023f220b96f36805a66f754cc`  
		Last Modified: Mon, 23 May 2022 18:50:10 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96a0692ed23e8f88ad2c83869dff9292e7e64bf87f985c8f8878047a63801937`  
		Last Modified: Mon, 23 May 2022 18:50:10 GMT  
		Size: 6.7 KB (6696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149c5fe0fb06642c34e7fff4cab2b43a1a6c934270b6eae11e6178a78b3e20ae`  
		Last Modified: Mon, 23 May 2022 18:50:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.25` - linux; ppc64le

```console
$ docker pull mariadb@sha256:29dde019f1b746bd1023b2fdcf9fbe670a2fcc604a4afd1ca4c4c4ad1d6ea064
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.7 MB (136667303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccbf91ef7fbb103d9fffe337e99000912262b5b3bce81e6d91b8d1256422f58a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 07 Jun 2022 05:46:02 GMT
ADD file:86506a94b834ba2b6f10dc0d1955bee539be1cf565e4ccc2c4bc074e0375f115 in / 
# Tue, 07 Jun 2022 05:46:06 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 08:57:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 08:57:48 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 08:57:54 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 08:58:44 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 08:58:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 08:59:09 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 08:59:14 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 08:59:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 09:07:20 GMT
ARG MARIADB_MAJOR=10.4
# Tue, 07 Jun 2022 09:07:22 GMT
ENV MARIADB_MAJOR=10.4
# Tue, 07 Jun 2022 09:07:24 GMT
ARG MARIADB_VERSION=1:10.4.25+maria~focal
# Tue, 07 Jun 2022 09:07:25 GMT
ENV MARIADB_VERSION=1:10.4.25+maria~focal
# Tue, 07 Jun 2022 09:07:27 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
# Tue, 07 Jun 2022 09:07:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 09:08:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 09:09:05 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 09:09:07 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 09:09:08 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Tue, 07 Jun 2022 09:09:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 07 Jun 2022 09:09:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 09:09:19 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 09:09:22 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3f52d061d2d3fdde0d3a099bbeae64080476c9650e9f3ba05de898d5bb5f03e8`  
		Last Modified: Tue, 07 Jun 2022 05:49:10 GMT  
		Size: 33.3 MB (33294345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b33a69d2ff59c89a297c597798ade8ea874f546d95513bd628c17fd7afda14`  
		Last Modified: Tue, 07 Jun 2022 09:17:18 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56a2c22a499e4928a88ae9201c66f507be8b9f10804ea7d0934710a6f91e5ec5`  
		Last Modified: Tue, 07 Jun 2022 09:17:18 GMT  
		Size: 6.7 MB (6667490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892b2ffb492b6d36ce25b68cf708d3c9bc9e0210e0cbbe7f575d3424c35d6b96`  
		Last Modified: Tue, 07 Jun 2022 09:17:17 GMT  
		Size: 3.7 MB (3672362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f80e77ec2bb0d7d685ca6e56f718adc6d253a98e069ebd5439f0c973194758`  
		Last Modified: Tue, 07 Jun 2022 09:17:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b0b3a9b79c49528e8e9da2d5d4954fc4e5392ee848c19c52a4d3369feb63d9`  
		Last Modified: Tue, 07 Jun 2022 09:17:16 GMT  
		Size: 2.6 MB (2568258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617e76c5eb45b560720c75ad4c60429a026cbbcb8467360cc70a7dace9ec4e5a`  
		Last Modified: Tue, 07 Jun 2022 09:17:13 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5bba458690d930a53ffeb4ccb714a0990a3bfabc029d7a06b276745a3d2e26`  
		Last Modified: Tue, 07 Jun 2022 09:19:18 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0972b5680a9853b06b6f6353e0d60b6f0998800c4f73ce013ec84bf222df150e`  
		Last Modified: Tue, 07 Jun 2022 09:19:35 GMT  
		Size: 90.4 MB (90449818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a7a156d8e0364e931c31314f6b4e7cb835a8867b26dca4608b7f98365d36b4`  
		Last Modified: Tue, 07 Jun 2022 09:19:18 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac5a7f6e713b2afa7e54814b43084987f41d4c941859dce87c16da7ba6e3d8e`  
		Last Modified: Tue, 07 Jun 2022 09:19:18 GMT  
		Size: 6.7 KB (6693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f3199d673bdcb32dfefb64ee4096b37863c7baea89f8b140d19ba1e68ad32f1`  
		Last Modified: Tue, 07 Jun 2022 09:19:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4.25-focal`

```console
$ docker pull mariadb@sha256:d1bd4c46e650e414b54c1667dcaca6ff3e6c044c2682600e477fcbfa4129b1f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4.25-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:9e962ec1649ede39337396d097572a561dd718cfb8acb99b657facf25ee25cab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.8 MB (125780636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8981e672fce893dc60d226f2969193dbd8139e589df7620eed2c4ff1505d309`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:42:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 00:42:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:42:35 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 00:42:46 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 00:42:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 00:42:53 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:42:53 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 00:42:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 00:44:32 GMT
ARG MARIADB_MAJOR=10.4
# Tue, 07 Jun 2022 00:44:32 GMT
ENV MARIADB_MAJOR=10.4
# Tue, 07 Jun 2022 00:44:32 GMT
ARG MARIADB_VERSION=1:10.4.25+maria~focal
# Tue, 07 Jun 2022 00:44:32 GMT
ENV MARIADB_VERSION=1:10.4.25+maria~focal
# Tue, 07 Jun 2022 00:44:32 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
# Tue, 07 Jun 2022 00:44:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 00:44:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 00:44:57 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 00:44:57 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 00:44:57 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Tue, 07 Jun 2022 00:44:58 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 07 Jun 2022 00:44:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 00:44:58 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 00:44:58 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59dcb80bbedb867b19c4eb004e84c86ae3475041d5bd11672bae9ba6be45084f`  
		Last Modified: Tue, 07 Jun 2022 00:48:53 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6c41888e0f25dece871c7e65daad879fc39d7da0a84f6b67ae0d4e1f4a6f8a`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 5.5 MB (5488991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de82bf1cd45986845f81bc71a119bf5ceaec50c145064ea58e5729f4bd6d0d22`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 3.6 MB (3585352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316c0826d235e46a7a9adcfcc3068c004818dc2611a41b69e6e7bea02316b70f`  
		Last Modified: Tue, 07 Jun 2022 00:48:51 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b82e623f5d9ed1cc04e5adc22adc6805abdba4aecc5b427aec6c31223a64dca6`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 2.3 MB (2272315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3daba1f86bc0fd099576f61e5eea0961cdefed1dc443ffb96b6a50c8f054b0b0`  
		Last Modified: Tue, 07 Jun 2022 00:48:49 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d04945d0545a6b71992ae420ca2a5171ff5453e1ecb4dcb614474bb4a02fdcac`  
		Last Modified: Tue, 07 Jun 2022 00:50:17 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3088ccc5e6c7fe86d7b86fed452b51e8207ac99f8b8ba930e398ab3eae8b76b2`  
		Last Modified: Tue, 07 Jun 2022 00:50:30 GMT  
		Size: 85.8 MB (85846325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebdc0a737326c786c882e86038a8e63b0005ba52232e81e0e5a3c749715f0ddc`  
		Last Modified: Tue, 07 Jun 2022 00:50:17 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd995425627004eb949201430def2ef647cfbadcaafcca914f8a82a1ae3242d3`  
		Last Modified: Tue, 07 Jun 2022 00:50:17 GMT  
		Size: 6.7 KB (6692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d92cbc5a67b96abbd56f59c94f2a30e8b9ba2a4538bf9e2b3573b56304bc158`  
		Last Modified: Tue, 07 Jun 2022 00:50:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.25-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:b696d9967dde3e1cd9881586f686ee75ea09d06635c8a88b73a7b50c86b6bd44
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123119346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bb619353184ac1a2fe6b631fc37d9bdc3d70c013165aa84f9850808082006b7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:03:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:03:44 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:03:45 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:04:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:04:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:04:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:04:10 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:04:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:07:07 GMT
ARG MARIADB_MAJOR=10.4
# Sat, 30 Apr 2022 00:07:07 GMT
ENV MARIADB_MAJOR=10.4
# Mon, 23 May 2022 18:44:08 GMT
ARG MARIADB_VERSION=1:10.4.25+maria~focal
# Mon, 23 May 2022 18:44:09 GMT
ENV MARIADB_VERSION=1:10.4.25+maria~focal
# Mon, 23 May 2022 18:44:10 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
# Mon, 23 May 2022 18:44:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 23 May 2022 18:44:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 23 May 2022 18:44:33 GMT
VOLUME [/var/lib/mysql]
# Mon, 23 May 2022 18:44:35 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Mon, 23 May 2022 18:44:36 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Mon, 23 May 2022 18:44:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 23 May 2022 18:44:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 18:44:38 GMT
EXPOSE 3306
# Mon, 23 May 2022 18:44:39 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932d0da437931580c9d7f118c259624e1c3ec8e81acb2acf5740d945e511ba78`  
		Last Modified: Sat, 30 Apr 2022 00:11:03 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc35c765a7328bd99273ee471b6b108980755023d4bcb1927fa7717942a9d318`  
		Last Modified: Sat, 30 Apr 2022 00:11:02 GMT  
		Size: 5.3 MB (5320183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88bae007bd9c42610e465ab436d60b2457b10b735a1bc8e5daba38f548c026`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 3.4 MB (3369899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7734d2f7be989dfe94fb891565830b8101d8e9bdbcbce8e5a7e1b1932eb3ac3c`  
		Last Modified: Sat, 30 Apr 2022 00:11:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24600bac48ce2157027e68df9e26a81754edc6f7e099c33c0a89de879dba5d9`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 2.2 MB (2202385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da05700210f681c47e021b8f3ce45f244f696854cfd656f0cd46e59cb8ca9b7d`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d50600df49b6f9bff73723902b349ab11ec42e761d0646fcccff56bf32c7b461`  
		Last Modified: Mon, 23 May 2022 18:50:10 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4051cf72966b8af9e322800c50d38e6d18fff7bfae8492301c61c151613b370`  
		Last Modified: Mon, 23 May 2022 18:50:24 GMT  
		Size: 85.0 MB (85042542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d3ed0aea547876d5b696e38dd81c4806366bb023f220b96f36805a66f754cc`  
		Last Modified: Mon, 23 May 2022 18:50:10 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96a0692ed23e8f88ad2c83869dff9292e7e64bf87f985c8f8878047a63801937`  
		Last Modified: Mon, 23 May 2022 18:50:10 GMT  
		Size: 6.7 KB (6696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149c5fe0fb06642c34e7fff4cab2b43a1a6c934270b6eae11e6178a78b3e20ae`  
		Last Modified: Mon, 23 May 2022 18:50:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.25-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:29dde019f1b746bd1023b2fdcf9fbe670a2fcc604a4afd1ca4c4c4ad1d6ea064
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.7 MB (136667303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccbf91ef7fbb103d9fffe337e99000912262b5b3bce81e6d91b8d1256422f58a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 07 Jun 2022 05:46:02 GMT
ADD file:86506a94b834ba2b6f10dc0d1955bee539be1cf565e4ccc2c4bc074e0375f115 in / 
# Tue, 07 Jun 2022 05:46:06 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 08:57:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 08:57:48 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 08:57:54 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 08:58:44 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 08:58:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 08:59:09 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 08:59:14 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 08:59:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 09:07:20 GMT
ARG MARIADB_MAJOR=10.4
# Tue, 07 Jun 2022 09:07:22 GMT
ENV MARIADB_MAJOR=10.4
# Tue, 07 Jun 2022 09:07:24 GMT
ARG MARIADB_VERSION=1:10.4.25+maria~focal
# Tue, 07 Jun 2022 09:07:25 GMT
ENV MARIADB_VERSION=1:10.4.25+maria~focal
# Tue, 07 Jun 2022 09:07:27 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
# Tue, 07 Jun 2022 09:07:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 09:08:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 09:09:05 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 09:09:07 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 09:09:08 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Tue, 07 Jun 2022 09:09:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.25/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 07 Jun 2022 09:09:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 09:09:19 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 09:09:22 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3f52d061d2d3fdde0d3a099bbeae64080476c9650e9f3ba05de898d5bb5f03e8`  
		Last Modified: Tue, 07 Jun 2022 05:49:10 GMT  
		Size: 33.3 MB (33294345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b33a69d2ff59c89a297c597798ade8ea874f546d95513bd628c17fd7afda14`  
		Last Modified: Tue, 07 Jun 2022 09:17:18 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56a2c22a499e4928a88ae9201c66f507be8b9f10804ea7d0934710a6f91e5ec5`  
		Last Modified: Tue, 07 Jun 2022 09:17:18 GMT  
		Size: 6.7 MB (6667490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892b2ffb492b6d36ce25b68cf708d3c9bc9e0210e0cbbe7f575d3424c35d6b96`  
		Last Modified: Tue, 07 Jun 2022 09:17:17 GMT  
		Size: 3.7 MB (3672362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f80e77ec2bb0d7d685ca6e56f718adc6d253a98e069ebd5439f0c973194758`  
		Last Modified: Tue, 07 Jun 2022 09:17:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b0b3a9b79c49528e8e9da2d5d4954fc4e5392ee848c19c52a4d3369feb63d9`  
		Last Modified: Tue, 07 Jun 2022 09:17:16 GMT  
		Size: 2.6 MB (2568258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617e76c5eb45b560720c75ad4c60429a026cbbcb8467360cc70a7dace9ec4e5a`  
		Last Modified: Tue, 07 Jun 2022 09:17:13 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5bba458690d930a53ffeb4ccb714a0990a3bfabc029d7a06b276745a3d2e26`  
		Last Modified: Tue, 07 Jun 2022 09:19:18 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0972b5680a9853b06b6f6353e0d60b6f0998800c4f73ce013ec84bf222df150e`  
		Last Modified: Tue, 07 Jun 2022 09:19:35 GMT  
		Size: 90.4 MB (90449818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a7a156d8e0364e931c31314f6b4e7cb835a8867b26dca4608b7f98365d36b4`  
		Last Modified: Tue, 07 Jun 2022 09:19:18 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac5a7f6e713b2afa7e54814b43084987f41d4c941859dce87c16da7ba6e3d8e`  
		Last Modified: Tue, 07 Jun 2022 09:19:18 GMT  
		Size: 6.7 KB (6693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f3199d673bdcb32dfefb64ee4096b37863c7baea89f8b140d19ba1e68ad32f1`  
		Last Modified: Tue, 07 Jun 2022 09:19:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5`

```console
$ docker pull mariadb@sha256:ca53a7cd054a66a34377737686753f1c9f9d797c18acc4e6e15ba997faa8b459
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.5` - linux; amd64

```console
$ docker pull mariadb@sha256:5b6b917fd647ee1f288216e78e3065d6e7cf37b2312a7087399a757619870b29
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.0 MB (128034257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b39c42d09fd1eb3753dc3b39271b1e3df2c19cc12ecc7a4124d6dd190ada994`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:42:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 00:42:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:42:35 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 00:42:46 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 00:42:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 00:42:53 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:42:53 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 00:42:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 00:44:04 GMT
ARG MARIADB_MAJOR=10.5
# Tue, 07 Jun 2022 00:44:04 GMT
ENV MARIADB_MAJOR=10.5
# Tue, 07 Jun 2022 00:44:04 GMT
ARG MARIADB_VERSION=1:10.5.16+maria~focal
# Tue, 07 Jun 2022 00:44:04 GMT
ENV MARIADB_VERSION=1:10.5.16+maria~focal
# Tue, 07 Jun 2022 00:44:04 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
# Tue, 07 Jun 2022 00:44:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 00:44:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 00:44:27 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 00:44:27 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 00:44:27 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Tue, 07 Jun 2022 00:44:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 00:44:27 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 00:44:27 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59dcb80bbedb867b19c4eb004e84c86ae3475041d5bd11672bae9ba6be45084f`  
		Last Modified: Tue, 07 Jun 2022 00:48:53 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6c41888e0f25dece871c7e65daad879fc39d7da0a84f6b67ae0d4e1f4a6f8a`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 5.5 MB (5488991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de82bf1cd45986845f81bc71a119bf5ceaec50c145064ea58e5729f4bd6d0d22`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 3.6 MB (3585352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316c0826d235e46a7a9adcfcc3068c004818dc2611a41b69e6e7bea02316b70f`  
		Last Modified: Tue, 07 Jun 2022 00:48:51 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b82e623f5d9ed1cc04e5adc22adc6805abdba4aecc5b427aec6c31223a64dca6`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 2.3 MB (2272315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3daba1f86bc0fd099576f61e5eea0961cdefed1dc443ffb96b6a50c8f054b0b0`  
		Last Modified: Tue, 07 Jun 2022 00:48:49 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa9c00f685bd6cf153c870dc2dd9bcd1e18a855fa57f40e6e41790a91c89117`  
		Last Modified: Tue, 07 Jun 2022 00:49:48 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48a603ad29b0aa206aa9ea8ab73e5750c1198bd28255d8bd8d7c78b97ac3da74`  
		Last Modified: Tue, 07 Jun 2022 00:50:01 GMT  
		Size: 88.1 MB (88100075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac467eecf9aafefbe0051851ef4782a491f9ef0bfe46bd3932eadb8165118c45`  
		Last Modified: Tue, 07 Jun 2022 00:49:48 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d11ea14c479ca40391b72f3c01a4c43be03a6aa941868082e9bb591f1070981`  
		Last Modified: Tue, 07 Jun 2022 00:49:48 GMT  
		Size: 6.7 KB (6689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:7d609f7bc3b1991769a4dca3b0e75e405636069665d18aa9e2738eae4d1eb528
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.3 MB (125291906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2add4e15f7c385964e8ed3c1a6fed4745b2008d9e46005161f00471308eedcc5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:03:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:03:44 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:03:45 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:04:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:04:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:04:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:04:10 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:04:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:06:23 GMT
ARG MARIADB_MAJOR=10.5
# Sat, 30 Apr 2022 00:06:24 GMT
ENV MARIADB_MAJOR=10.5
# Mon, 23 May 2022 18:43:31 GMT
ARG MARIADB_VERSION=1:10.5.16+maria~focal
# Mon, 23 May 2022 18:43:32 GMT
ENV MARIADB_VERSION=1:10.5.16+maria~focal
# Mon, 23 May 2022 18:43:33 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
# Mon, 23 May 2022 18:43:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 23 May 2022 18:43:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 23 May 2022 18:43:56 GMT
VOLUME [/var/lib/mysql]
# Mon, 23 May 2022 18:43:58 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Mon, 23 May 2022 18:43:59 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Mon, 23 May 2022 18:43:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 18:44:00 GMT
EXPOSE 3306
# Mon, 23 May 2022 18:44:01 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932d0da437931580c9d7f118c259624e1c3ec8e81acb2acf5740d945e511ba78`  
		Last Modified: Sat, 30 Apr 2022 00:11:03 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc35c765a7328bd99273ee471b6b108980755023d4bcb1927fa7717942a9d318`  
		Last Modified: Sat, 30 Apr 2022 00:11:02 GMT  
		Size: 5.3 MB (5320183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88bae007bd9c42610e465ab436d60b2457b10b735a1bc8e5daba38f548c026`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 3.4 MB (3369899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7734d2f7be989dfe94fb891565830b8101d8e9bdbcbce8e5a7e1b1932eb3ac3c`  
		Last Modified: Sat, 30 Apr 2022 00:11:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24600bac48ce2157027e68df9e26a81754edc6f7e099c33c0a89de879dba5d9`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 2.2 MB (2202385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da05700210f681c47e021b8f3ce45f244f696854cfd656f0cd46e59cb8ca9b7d`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ffae9fb7abd2928fa97e226250a176df36685529c856c8efbb37f8993bb844`  
		Last Modified: Mon, 23 May 2022 18:49:39 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee99e70137556b16b01eeee55ab2ed41b2d5330fca69b472aaaf1a9097b8bf4f`  
		Last Modified: Mon, 23 May 2022 18:49:52 GMT  
		Size: 87.2 MB (87215227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b1618553dab9fdb059b5f5efef5bcc2d8fb8c949aeb6f6359a36e2bc685dfe`  
		Last Modified: Mon, 23 May 2022 18:49:39 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f0edefce957b3f3e9d22ea3d184d5fd6250c446c0d7510401d669980f31956f`  
		Last Modified: Mon, 23 May 2022 18:49:39 GMT  
		Size: 6.7 KB (6693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; ppc64le

```console
$ docker pull mariadb@sha256:74603051778796eb42860bf97cba78820f1f4aa56a7299405744f498625c13c1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.9 MB (138920706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:910947f81ce0cd41a4a43ec2fcb0c19ba3a42d48b70f386ac8079970f344a371`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 07 Jun 2022 05:46:02 GMT
ADD file:86506a94b834ba2b6f10dc0d1955bee539be1cf565e4ccc2c4bc074e0375f115 in / 
# Tue, 07 Jun 2022 05:46:06 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 08:57:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 08:57:48 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 08:57:54 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 08:58:44 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 08:58:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 08:59:09 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 08:59:14 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 08:59:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 09:05:07 GMT
ARG MARIADB_MAJOR=10.5
# Tue, 07 Jun 2022 09:05:09 GMT
ENV MARIADB_MAJOR=10.5
# Tue, 07 Jun 2022 09:05:11 GMT
ARG MARIADB_VERSION=1:10.5.16+maria~focal
# Tue, 07 Jun 2022 09:05:14 GMT
ENV MARIADB_VERSION=1:10.5.16+maria~focal
# Tue, 07 Jun 2022 09:05:16 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
# Tue, 07 Jun 2022 09:05:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 09:06:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 09:07:00 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 09:07:01 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 09:07:02 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Tue, 07 Jun 2022 09:07:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 09:07:09 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 09:07:11 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3f52d061d2d3fdde0d3a099bbeae64080476c9650e9f3ba05de898d5bb5f03e8`  
		Last Modified: Tue, 07 Jun 2022 05:49:10 GMT  
		Size: 33.3 MB (33294345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b33a69d2ff59c89a297c597798ade8ea874f546d95513bd628c17fd7afda14`  
		Last Modified: Tue, 07 Jun 2022 09:17:18 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56a2c22a499e4928a88ae9201c66f507be8b9f10804ea7d0934710a6f91e5ec5`  
		Last Modified: Tue, 07 Jun 2022 09:17:18 GMT  
		Size: 6.7 MB (6667490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892b2ffb492b6d36ce25b68cf708d3c9bc9e0210e0cbbe7f575d3424c35d6b96`  
		Last Modified: Tue, 07 Jun 2022 09:17:17 GMT  
		Size: 3.7 MB (3672362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f80e77ec2bb0d7d685ca6e56f718adc6d253a98e069ebd5439f0c973194758`  
		Last Modified: Tue, 07 Jun 2022 09:17:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b0b3a9b79c49528e8e9da2d5d4954fc4e5392ee848c19c52a4d3369feb63d9`  
		Last Modified: Tue, 07 Jun 2022 09:17:16 GMT  
		Size: 2.6 MB (2568258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617e76c5eb45b560720c75ad4c60429a026cbbcb8467360cc70a7dace9ec4e5a`  
		Last Modified: Tue, 07 Jun 2022 09:17:13 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a59c27076a9e0b63144b746bf0ff178f849d8439122178341452eb038ce3e4f`  
		Last Modified: Tue, 07 Jun 2022 09:18:37 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd90769a974b7e7cda4cd39253ac95caa7589eebd08ff076bc83131ba7fb8839`  
		Last Modified: Tue, 07 Jun 2022 09:18:56 GMT  
		Size: 92.7 MB (92703341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4c17854aca625521983d66ec897032d27b9b2fac94d0361c43b022895db84d`  
		Last Modified: Tue, 07 Jun 2022 09:18:38 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b4b29126725a609c1392d5fc78c8c7a82a6c7a120d2e709858521aad09d48b`  
		Last Modified: Tue, 07 Jun 2022 09:18:37 GMT  
		Size: 6.7 KB (6693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; s390x

```console
$ docker pull mariadb@sha256:b04ed6dfca4d439554d1186288af3a20277081302a8d92b064191458587e5014
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.3 MB (127263882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d89f53da4f2085522e2510522207f8c4bd3e4c702d16c9b8653bb11008332b3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 07 Jun 2022 04:05:02 GMT
ADD file:6250f895d7d6c591cfe1b9fc991313d21b02167d94c67991db7c5c1c6814c51e in / 
# Tue, 07 Jun 2022 04:05:06 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:49:07 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 06:49:16 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:49:16 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 06:49:29 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 06:49:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 06:49:37 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:49:38 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 06:49:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 06:51:23 GMT
ARG MARIADB_MAJOR=10.5
# Tue, 07 Jun 2022 06:51:24 GMT
ENV MARIADB_MAJOR=10.5
# Tue, 07 Jun 2022 06:51:24 GMT
ARG MARIADB_VERSION=1:10.5.16+maria~focal
# Tue, 07 Jun 2022 06:51:24 GMT
ENV MARIADB_VERSION=1:10.5.16+maria~focal
# Tue, 07 Jun 2022 06:51:24 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
# Tue, 07 Jun 2022 06:51:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 06:52:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 06:52:15 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 06:52:16 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 06:52:16 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Tue, 07 Jun 2022 06:52:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 06:52:17 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 06:52:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2f1fac119b88f55cd8329458ec27c3d6d6cb324b0fe541feacfd9a4ee621a558`  
		Last Modified: Tue, 07 Jun 2022 04:07:45 GMT  
		Size: 27.1 MB (27056020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e11bbd03dcb74b0a89181bc7b5b0c6a1081475b91f09e5b7bd4378245677d0`  
		Last Modified: Tue, 07 Jun 2022 06:54:23 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944609fc08b7430c363765f8d65b07874048d4ee4b4fddc6378410ffbf35a5e4`  
		Last Modified: Tue, 07 Jun 2022 06:54:23 GMT  
		Size: 5.4 MB (5372398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc686e965111a0f5a9fbe0d2fd56fb1cbe1f37cd32ba702e6e181eb8bd952476`  
		Last Modified: Tue, 07 Jun 2022 06:54:22 GMT  
		Size: 3.2 MB (3244071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c6b370e34d40b571955a0831c8669ab35e55a71bc048f8ad7355f3971ba4b3`  
		Last Modified: Tue, 07 Jun 2022 06:54:21 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13a21a85799843063b419b269af229d786c77820174a95c4dcc2363cee9c846`  
		Last Modified: Tue, 07 Jun 2022 06:54:21 GMT  
		Size: 2.2 MB (2183581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed1ebbc1458626d5a4732baab692192158957e9db1cb87eb1e2e23e531a49d6`  
		Last Modified: Tue, 07 Jun 2022 06:54:20 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3ad4eda1b4a8ef767f27722613a4f5c3cf0973e58ed1b051c4d9db476671525`  
		Last Modified: Tue, 07 Jun 2022 06:55:12 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20082cb10cc20f97ee82b3ca5dabc03bd6eb4e8eb09ed6ea11ed9c8c24fa4c05`  
		Last Modified: Tue, 07 Jun 2022 06:55:25 GMT  
		Size: 89.4 MB (89392913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12966bf5bed2405da55c9bb96a369c06bda4b7a26bd2ae38201230d0d4cdee0c`  
		Last Modified: Tue, 07 Jun 2022 06:55:12 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4d5c8e32cb2e967833d9ee92d4276d9a2887ba2388927db51f9666df1d3685d`  
		Last Modified: Tue, 07 Jun 2022 06:55:12 GMT  
		Size: 6.7 KB (6689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5-focal`

```console
$ docker pull mariadb@sha256:ca53a7cd054a66a34377737686753f1c9f9d797c18acc4e6e15ba997faa8b459
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.5-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:5b6b917fd647ee1f288216e78e3065d6e7cf37b2312a7087399a757619870b29
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.0 MB (128034257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b39c42d09fd1eb3753dc3b39271b1e3df2c19cc12ecc7a4124d6dd190ada994`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:42:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 00:42:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:42:35 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 00:42:46 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 00:42:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 00:42:53 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:42:53 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 00:42:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 00:44:04 GMT
ARG MARIADB_MAJOR=10.5
# Tue, 07 Jun 2022 00:44:04 GMT
ENV MARIADB_MAJOR=10.5
# Tue, 07 Jun 2022 00:44:04 GMT
ARG MARIADB_VERSION=1:10.5.16+maria~focal
# Tue, 07 Jun 2022 00:44:04 GMT
ENV MARIADB_VERSION=1:10.5.16+maria~focal
# Tue, 07 Jun 2022 00:44:04 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
# Tue, 07 Jun 2022 00:44:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 00:44:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 00:44:27 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 00:44:27 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 00:44:27 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Tue, 07 Jun 2022 00:44:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 00:44:27 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 00:44:27 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59dcb80bbedb867b19c4eb004e84c86ae3475041d5bd11672bae9ba6be45084f`  
		Last Modified: Tue, 07 Jun 2022 00:48:53 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6c41888e0f25dece871c7e65daad879fc39d7da0a84f6b67ae0d4e1f4a6f8a`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 5.5 MB (5488991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de82bf1cd45986845f81bc71a119bf5ceaec50c145064ea58e5729f4bd6d0d22`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 3.6 MB (3585352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316c0826d235e46a7a9adcfcc3068c004818dc2611a41b69e6e7bea02316b70f`  
		Last Modified: Tue, 07 Jun 2022 00:48:51 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b82e623f5d9ed1cc04e5adc22adc6805abdba4aecc5b427aec6c31223a64dca6`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 2.3 MB (2272315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3daba1f86bc0fd099576f61e5eea0961cdefed1dc443ffb96b6a50c8f054b0b0`  
		Last Modified: Tue, 07 Jun 2022 00:48:49 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa9c00f685bd6cf153c870dc2dd9bcd1e18a855fa57f40e6e41790a91c89117`  
		Last Modified: Tue, 07 Jun 2022 00:49:48 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48a603ad29b0aa206aa9ea8ab73e5750c1198bd28255d8bd8d7c78b97ac3da74`  
		Last Modified: Tue, 07 Jun 2022 00:50:01 GMT  
		Size: 88.1 MB (88100075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac467eecf9aafefbe0051851ef4782a491f9ef0bfe46bd3932eadb8165118c45`  
		Last Modified: Tue, 07 Jun 2022 00:49:48 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d11ea14c479ca40391b72f3c01a4c43be03a6aa941868082e9bb591f1070981`  
		Last Modified: Tue, 07 Jun 2022 00:49:48 GMT  
		Size: 6.7 KB (6689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:7d609f7bc3b1991769a4dca3b0e75e405636069665d18aa9e2738eae4d1eb528
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.3 MB (125291906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2add4e15f7c385964e8ed3c1a6fed4745b2008d9e46005161f00471308eedcc5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:03:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:03:44 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:03:45 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:04:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:04:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:04:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:04:10 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:04:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:06:23 GMT
ARG MARIADB_MAJOR=10.5
# Sat, 30 Apr 2022 00:06:24 GMT
ENV MARIADB_MAJOR=10.5
# Mon, 23 May 2022 18:43:31 GMT
ARG MARIADB_VERSION=1:10.5.16+maria~focal
# Mon, 23 May 2022 18:43:32 GMT
ENV MARIADB_VERSION=1:10.5.16+maria~focal
# Mon, 23 May 2022 18:43:33 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
# Mon, 23 May 2022 18:43:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 23 May 2022 18:43:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 23 May 2022 18:43:56 GMT
VOLUME [/var/lib/mysql]
# Mon, 23 May 2022 18:43:58 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Mon, 23 May 2022 18:43:59 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Mon, 23 May 2022 18:43:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 18:44:00 GMT
EXPOSE 3306
# Mon, 23 May 2022 18:44:01 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932d0da437931580c9d7f118c259624e1c3ec8e81acb2acf5740d945e511ba78`  
		Last Modified: Sat, 30 Apr 2022 00:11:03 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc35c765a7328bd99273ee471b6b108980755023d4bcb1927fa7717942a9d318`  
		Last Modified: Sat, 30 Apr 2022 00:11:02 GMT  
		Size: 5.3 MB (5320183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88bae007bd9c42610e465ab436d60b2457b10b735a1bc8e5daba38f548c026`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 3.4 MB (3369899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7734d2f7be989dfe94fb891565830b8101d8e9bdbcbce8e5a7e1b1932eb3ac3c`  
		Last Modified: Sat, 30 Apr 2022 00:11:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24600bac48ce2157027e68df9e26a81754edc6f7e099c33c0a89de879dba5d9`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 2.2 MB (2202385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da05700210f681c47e021b8f3ce45f244f696854cfd656f0cd46e59cb8ca9b7d`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ffae9fb7abd2928fa97e226250a176df36685529c856c8efbb37f8993bb844`  
		Last Modified: Mon, 23 May 2022 18:49:39 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee99e70137556b16b01eeee55ab2ed41b2d5330fca69b472aaaf1a9097b8bf4f`  
		Last Modified: Mon, 23 May 2022 18:49:52 GMT  
		Size: 87.2 MB (87215227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b1618553dab9fdb059b5f5efef5bcc2d8fb8c949aeb6f6359a36e2bc685dfe`  
		Last Modified: Mon, 23 May 2022 18:49:39 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f0edefce957b3f3e9d22ea3d184d5fd6250c446c0d7510401d669980f31956f`  
		Last Modified: Mon, 23 May 2022 18:49:39 GMT  
		Size: 6.7 KB (6693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:74603051778796eb42860bf97cba78820f1f4aa56a7299405744f498625c13c1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.9 MB (138920706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:910947f81ce0cd41a4a43ec2fcb0c19ba3a42d48b70f386ac8079970f344a371`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 07 Jun 2022 05:46:02 GMT
ADD file:86506a94b834ba2b6f10dc0d1955bee539be1cf565e4ccc2c4bc074e0375f115 in / 
# Tue, 07 Jun 2022 05:46:06 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 08:57:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 08:57:48 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 08:57:54 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 08:58:44 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 08:58:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 08:59:09 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 08:59:14 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 08:59:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 09:05:07 GMT
ARG MARIADB_MAJOR=10.5
# Tue, 07 Jun 2022 09:05:09 GMT
ENV MARIADB_MAJOR=10.5
# Tue, 07 Jun 2022 09:05:11 GMT
ARG MARIADB_VERSION=1:10.5.16+maria~focal
# Tue, 07 Jun 2022 09:05:14 GMT
ENV MARIADB_VERSION=1:10.5.16+maria~focal
# Tue, 07 Jun 2022 09:05:16 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
# Tue, 07 Jun 2022 09:05:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 09:06:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 09:07:00 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 09:07:01 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 09:07:02 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Tue, 07 Jun 2022 09:07:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 09:07:09 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 09:07:11 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3f52d061d2d3fdde0d3a099bbeae64080476c9650e9f3ba05de898d5bb5f03e8`  
		Last Modified: Tue, 07 Jun 2022 05:49:10 GMT  
		Size: 33.3 MB (33294345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b33a69d2ff59c89a297c597798ade8ea874f546d95513bd628c17fd7afda14`  
		Last Modified: Tue, 07 Jun 2022 09:17:18 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56a2c22a499e4928a88ae9201c66f507be8b9f10804ea7d0934710a6f91e5ec5`  
		Last Modified: Tue, 07 Jun 2022 09:17:18 GMT  
		Size: 6.7 MB (6667490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892b2ffb492b6d36ce25b68cf708d3c9bc9e0210e0cbbe7f575d3424c35d6b96`  
		Last Modified: Tue, 07 Jun 2022 09:17:17 GMT  
		Size: 3.7 MB (3672362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f80e77ec2bb0d7d685ca6e56f718adc6d253a98e069ebd5439f0c973194758`  
		Last Modified: Tue, 07 Jun 2022 09:17:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b0b3a9b79c49528e8e9da2d5d4954fc4e5392ee848c19c52a4d3369feb63d9`  
		Last Modified: Tue, 07 Jun 2022 09:17:16 GMT  
		Size: 2.6 MB (2568258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617e76c5eb45b560720c75ad4c60429a026cbbcb8467360cc70a7dace9ec4e5a`  
		Last Modified: Tue, 07 Jun 2022 09:17:13 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a59c27076a9e0b63144b746bf0ff178f849d8439122178341452eb038ce3e4f`  
		Last Modified: Tue, 07 Jun 2022 09:18:37 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd90769a974b7e7cda4cd39253ac95caa7589eebd08ff076bc83131ba7fb8839`  
		Last Modified: Tue, 07 Jun 2022 09:18:56 GMT  
		Size: 92.7 MB (92703341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4c17854aca625521983d66ec897032d27b9b2fac94d0361c43b022895db84d`  
		Last Modified: Tue, 07 Jun 2022 09:18:38 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b4b29126725a609c1392d5fc78c8c7a82a6c7a120d2e709858521aad09d48b`  
		Last Modified: Tue, 07 Jun 2022 09:18:37 GMT  
		Size: 6.7 KB (6693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:b04ed6dfca4d439554d1186288af3a20277081302a8d92b064191458587e5014
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.3 MB (127263882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d89f53da4f2085522e2510522207f8c4bd3e4c702d16c9b8653bb11008332b3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 07 Jun 2022 04:05:02 GMT
ADD file:6250f895d7d6c591cfe1b9fc991313d21b02167d94c67991db7c5c1c6814c51e in / 
# Tue, 07 Jun 2022 04:05:06 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:49:07 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 06:49:16 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:49:16 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 06:49:29 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 06:49:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 06:49:37 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:49:38 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 06:49:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 06:51:23 GMT
ARG MARIADB_MAJOR=10.5
# Tue, 07 Jun 2022 06:51:24 GMT
ENV MARIADB_MAJOR=10.5
# Tue, 07 Jun 2022 06:51:24 GMT
ARG MARIADB_VERSION=1:10.5.16+maria~focal
# Tue, 07 Jun 2022 06:51:24 GMT
ENV MARIADB_VERSION=1:10.5.16+maria~focal
# Tue, 07 Jun 2022 06:51:24 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
# Tue, 07 Jun 2022 06:51:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 06:52:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 06:52:15 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 06:52:16 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 06:52:16 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Tue, 07 Jun 2022 06:52:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 06:52:17 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 06:52:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2f1fac119b88f55cd8329458ec27c3d6d6cb324b0fe541feacfd9a4ee621a558`  
		Last Modified: Tue, 07 Jun 2022 04:07:45 GMT  
		Size: 27.1 MB (27056020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e11bbd03dcb74b0a89181bc7b5b0c6a1081475b91f09e5b7bd4378245677d0`  
		Last Modified: Tue, 07 Jun 2022 06:54:23 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944609fc08b7430c363765f8d65b07874048d4ee4b4fddc6378410ffbf35a5e4`  
		Last Modified: Tue, 07 Jun 2022 06:54:23 GMT  
		Size: 5.4 MB (5372398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc686e965111a0f5a9fbe0d2fd56fb1cbe1f37cd32ba702e6e181eb8bd952476`  
		Last Modified: Tue, 07 Jun 2022 06:54:22 GMT  
		Size: 3.2 MB (3244071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c6b370e34d40b571955a0831c8669ab35e55a71bc048f8ad7355f3971ba4b3`  
		Last Modified: Tue, 07 Jun 2022 06:54:21 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13a21a85799843063b419b269af229d786c77820174a95c4dcc2363cee9c846`  
		Last Modified: Tue, 07 Jun 2022 06:54:21 GMT  
		Size: 2.2 MB (2183581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed1ebbc1458626d5a4732baab692192158957e9db1cb87eb1e2e23e531a49d6`  
		Last Modified: Tue, 07 Jun 2022 06:54:20 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3ad4eda1b4a8ef767f27722613a4f5c3cf0973e58ed1b051c4d9db476671525`  
		Last Modified: Tue, 07 Jun 2022 06:55:12 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20082cb10cc20f97ee82b3ca5dabc03bd6eb4e8eb09ed6ea11ed9c8c24fa4c05`  
		Last Modified: Tue, 07 Jun 2022 06:55:25 GMT  
		Size: 89.4 MB (89392913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12966bf5bed2405da55c9bb96a369c06bda4b7a26bd2ae38201230d0d4cdee0c`  
		Last Modified: Tue, 07 Jun 2022 06:55:12 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4d5c8e32cb2e967833d9ee92d4276d9a2887ba2388927db51f9666df1d3685d`  
		Last Modified: Tue, 07 Jun 2022 06:55:12 GMT  
		Size: 6.7 KB (6689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5.16`

```console
$ docker pull mariadb@sha256:ca53a7cd054a66a34377737686753f1c9f9d797c18acc4e6e15ba997faa8b459
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.5.16` - linux; amd64

```console
$ docker pull mariadb@sha256:5b6b917fd647ee1f288216e78e3065d6e7cf37b2312a7087399a757619870b29
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.0 MB (128034257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b39c42d09fd1eb3753dc3b39271b1e3df2c19cc12ecc7a4124d6dd190ada994`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:42:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 00:42:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:42:35 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 00:42:46 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 00:42:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 00:42:53 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:42:53 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 00:42:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 00:44:04 GMT
ARG MARIADB_MAJOR=10.5
# Tue, 07 Jun 2022 00:44:04 GMT
ENV MARIADB_MAJOR=10.5
# Tue, 07 Jun 2022 00:44:04 GMT
ARG MARIADB_VERSION=1:10.5.16+maria~focal
# Tue, 07 Jun 2022 00:44:04 GMT
ENV MARIADB_VERSION=1:10.5.16+maria~focal
# Tue, 07 Jun 2022 00:44:04 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
# Tue, 07 Jun 2022 00:44:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 00:44:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 00:44:27 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 00:44:27 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 00:44:27 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Tue, 07 Jun 2022 00:44:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 00:44:27 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 00:44:27 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59dcb80bbedb867b19c4eb004e84c86ae3475041d5bd11672bae9ba6be45084f`  
		Last Modified: Tue, 07 Jun 2022 00:48:53 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6c41888e0f25dece871c7e65daad879fc39d7da0a84f6b67ae0d4e1f4a6f8a`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 5.5 MB (5488991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de82bf1cd45986845f81bc71a119bf5ceaec50c145064ea58e5729f4bd6d0d22`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 3.6 MB (3585352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316c0826d235e46a7a9adcfcc3068c004818dc2611a41b69e6e7bea02316b70f`  
		Last Modified: Tue, 07 Jun 2022 00:48:51 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b82e623f5d9ed1cc04e5adc22adc6805abdba4aecc5b427aec6c31223a64dca6`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 2.3 MB (2272315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3daba1f86bc0fd099576f61e5eea0961cdefed1dc443ffb96b6a50c8f054b0b0`  
		Last Modified: Tue, 07 Jun 2022 00:48:49 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa9c00f685bd6cf153c870dc2dd9bcd1e18a855fa57f40e6e41790a91c89117`  
		Last Modified: Tue, 07 Jun 2022 00:49:48 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48a603ad29b0aa206aa9ea8ab73e5750c1198bd28255d8bd8d7c78b97ac3da74`  
		Last Modified: Tue, 07 Jun 2022 00:50:01 GMT  
		Size: 88.1 MB (88100075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac467eecf9aafefbe0051851ef4782a491f9ef0bfe46bd3932eadb8165118c45`  
		Last Modified: Tue, 07 Jun 2022 00:49:48 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d11ea14c479ca40391b72f3c01a4c43be03a6aa941868082e9bb591f1070981`  
		Last Modified: Tue, 07 Jun 2022 00:49:48 GMT  
		Size: 6.7 KB (6689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.16` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:7d609f7bc3b1991769a4dca3b0e75e405636069665d18aa9e2738eae4d1eb528
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.3 MB (125291906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2add4e15f7c385964e8ed3c1a6fed4745b2008d9e46005161f00471308eedcc5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:03:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:03:44 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:03:45 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:04:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:04:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:04:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:04:10 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:04:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:06:23 GMT
ARG MARIADB_MAJOR=10.5
# Sat, 30 Apr 2022 00:06:24 GMT
ENV MARIADB_MAJOR=10.5
# Mon, 23 May 2022 18:43:31 GMT
ARG MARIADB_VERSION=1:10.5.16+maria~focal
# Mon, 23 May 2022 18:43:32 GMT
ENV MARIADB_VERSION=1:10.5.16+maria~focal
# Mon, 23 May 2022 18:43:33 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
# Mon, 23 May 2022 18:43:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 23 May 2022 18:43:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 23 May 2022 18:43:56 GMT
VOLUME [/var/lib/mysql]
# Mon, 23 May 2022 18:43:58 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Mon, 23 May 2022 18:43:59 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Mon, 23 May 2022 18:43:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 18:44:00 GMT
EXPOSE 3306
# Mon, 23 May 2022 18:44:01 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932d0da437931580c9d7f118c259624e1c3ec8e81acb2acf5740d945e511ba78`  
		Last Modified: Sat, 30 Apr 2022 00:11:03 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc35c765a7328bd99273ee471b6b108980755023d4bcb1927fa7717942a9d318`  
		Last Modified: Sat, 30 Apr 2022 00:11:02 GMT  
		Size: 5.3 MB (5320183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88bae007bd9c42610e465ab436d60b2457b10b735a1bc8e5daba38f548c026`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 3.4 MB (3369899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7734d2f7be989dfe94fb891565830b8101d8e9bdbcbce8e5a7e1b1932eb3ac3c`  
		Last Modified: Sat, 30 Apr 2022 00:11:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24600bac48ce2157027e68df9e26a81754edc6f7e099c33c0a89de879dba5d9`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 2.2 MB (2202385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da05700210f681c47e021b8f3ce45f244f696854cfd656f0cd46e59cb8ca9b7d`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ffae9fb7abd2928fa97e226250a176df36685529c856c8efbb37f8993bb844`  
		Last Modified: Mon, 23 May 2022 18:49:39 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee99e70137556b16b01eeee55ab2ed41b2d5330fca69b472aaaf1a9097b8bf4f`  
		Last Modified: Mon, 23 May 2022 18:49:52 GMT  
		Size: 87.2 MB (87215227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b1618553dab9fdb059b5f5efef5bcc2d8fb8c949aeb6f6359a36e2bc685dfe`  
		Last Modified: Mon, 23 May 2022 18:49:39 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f0edefce957b3f3e9d22ea3d184d5fd6250c446c0d7510401d669980f31956f`  
		Last Modified: Mon, 23 May 2022 18:49:39 GMT  
		Size: 6.7 KB (6693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.16` - linux; ppc64le

```console
$ docker pull mariadb@sha256:74603051778796eb42860bf97cba78820f1f4aa56a7299405744f498625c13c1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.9 MB (138920706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:910947f81ce0cd41a4a43ec2fcb0c19ba3a42d48b70f386ac8079970f344a371`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 07 Jun 2022 05:46:02 GMT
ADD file:86506a94b834ba2b6f10dc0d1955bee539be1cf565e4ccc2c4bc074e0375f115 in / 
# Tue, 07 Jun 2022 05:46:06 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 08:57:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 08:57:48 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 08:57:54 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 08:58:44 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 08:58:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 08:59:09 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 08:59:14 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 08:59:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 09:05:07 GMT
ARG MARIADB_MAJOR=10.5
# Tue, 07 Jun 2022 09:05:09 GMT
ENV MARIADB_MAJOR=10.5
# Tue, 07 Jun 2022 09:05:11 GMT
ARG MARIADB_VERSION=1:10.5.16+maria~focal
# Tue, 07 Jun 2022 09:05:14 GMT
ENV MARIADB_VERSION=1:10.5.16+maria~focal
# Tue, 07 Jun 2022 09:05:16 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
# Tue, 07 Jun 2022 09:05:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 09:06:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 09:07:00 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 09:07:01 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 09:07:02 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Tue, 07 Jun 2022 09:07:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 09:07:09 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 09:07:11 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3f52d061d2d3fdde0d3a099bbeae64080476c9650e9f3ba05de898d5bb5f03e8`  
		Last Modified: Tue, 07 Jun 2022 05:49:10 GMT  
		Size: 33.3 MB (33294345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b33a69d2ff59c89a297c597798ade8ea874f546d95513bd628c17fd7afda14`  
		Last Modified: Tue, 07 Jun 2022 09:17:18 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56a2c22a499e4928a88ae9201c66f507be8b9f10804ea7d0934710a6f91e5ec5`  
		Last Modified: Tue, 07 Jun 2022 09:17:18 GMT  
		Size: 6.7 MB (6667490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892b2ffb492b6d36ce25b68cf708d3c9bc9e0210e0cbbe7f575d3424c35d6b96`  
		Last Modified: Tue, 07 Jun 2022 09:17:17 GMT  
		Size: 3.7 MB (3672362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f80e77ec2bb0d7d685ca6e56f718adc6d253a98e069ebd5439f0c973194758`  
		Last Modified: Tue, 07 Jun 2022 09:17:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b0b3a9b79c49528e8e9da2d5d4954fc4e5392ee848c19c52a4d3369feb63d9`  
		Last Modified: Tue, 07 Jun 2022 09:17:16 GMT  
		Size: 2.6 MB (2568258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617e76c5eb45b560720c75ad4c60429a026cbbcb8467360cc70a7dace9ec4e5a`  
		Last Modified: Tue, 07 Jun 2022 09:17:13 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a59c27076a9e0b63144b746bf0ff178f849d8439122178341452eb038ce3e4f`  
		Last Modified: Tue, 07 Jun 2022 09:18:37 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd90769a974b7e7cda4cd39253ac95caa7589eebd08ff076bc83131ba7fb8839`  
		Last Modified: Tue, 07 Jun 2022 09:18:56 GMT  
		Size: 92.7 MB (92703341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4c17854aca625521983d66ec897032d27b9b2fac94d0361c43b022895db84d`  
		Last Modified: Tue, 07 Jun 2022 09:18:38 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b4b29126725a609c1392d5fc78c8c7a82a6c7a120d2e709858521aad09d48b`  
		Last Modified: Tue, 07 Jun 2022 09:18:37 GMT  
		Size: 6.7 KB (6693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.16` - linux; s390x

```console
$ docker pull mariadb@sha256:b04ed6dfca4d439554d1186288af3a20277081302a8d92b064191458587e5014
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.3 MB (127263882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d89f53da4f2085522e2510522207f8c4bd3e4c702d16c9b8653bb11008332b3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 07 Jun 2022 04:05:02 GMT
ADD file:6250f895d7d6c591cfe1b9fc991313d21b02167d94c67991db7c5c1c6814c51e in / 
# Tue, 07 Jun 2022 04:05:06 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:49:07 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 06:49:16 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:49:16 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 06:49:29 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 06:49:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 06:49:37 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:49:38 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 06:49:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 06:51:23 GMT
ARG MARIADB_MAJOR=10.5
# Tue, 07 Jun 2022 06:51:24 GMT
ENV MARIADB_MAJOR=10.5
# Tue, 07 Jun 2022 06:51:24 GMT
ARG MARIADB_VERSION=1:10.5.16+maria~focal
# Tue, 07 Jun 2022 06:51:24 GMT
ENV MARIADB_VERSION=1:10.5.16+maria~focal
# Tue, 07 Jun 2022 06:51:24 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
# Tue, 07 Jun 2022 06:51:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 06:52:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 06:52:15 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 06:52:16 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 06:52:16 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Tue, 07 Jun 2022 06:52:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 06:52:17 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 06:52:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2f1fac119b88f55cd8329458ec27c3d6d6cb324b0fe541feacfd9a4ee621a558`  
		Last Modified: Tue, 07 Jun 2022 04:07:45 GMT  
		Size: 27.1 MB (27056020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e11bbd03dcb74b0a89181bc7b5b0c6a1081475b91f09e5b7bd4378245677d0`  
		Last Modified: Tue, 07 Jun 2022 06:54:23 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944609fc08b7430c363765f8d65b07874048d4ee4b4fddc6378410ffbf35a5e4`  
		Last Modified: Tue, 07 Jun 2022 06:54:23 GMT  
		Size: 5.4 MB (5372398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc686e965111a0f5a9fbe0d2fd56fb1cbe1f37cd32ba702e6e181eb8bd952476`  
		Last Modified: Tue, 07 Jun 2022 06:54:22 GMT  
		Size: 3.2 MB (3244071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c6b370e34d40b571955a0831c8669ab35e55a71bc048f8ad7355f3971ba4b3`  
		Last Modified: Tue, 07 Jun 2022 06:54:21 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13a21a85799843063b419b269af229d786c77820174a95c4dcc2363cee9c846`  
		Last Modified: Tue, 07 Jun 2022 06:54:21 GMT  
		Size: 2.2 MB (2183581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed1ebbc1458626d5a4732baab692192158957e9db1cb87eb1e2e23e531a49d6`  
		Last Modified: Tue, 07 Jun 2022 06:54:20 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3ad4eda1b4a8ef767f27722613a4f5c3cf0973e58ed1b051c4d9db476671525`  
		Last Modified: Tue, 07 Jun 2022 06:55:12 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20082cb10cc20f97ee82b3ca5dabc03bd6eb4e8eb09ed6ea11ed9c8c24fa4c05`  
		Last Modified: Tue, 07 Jun 2022 06:55:25 GMT  
		Size: 89.4 MB (89392913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12966bf5bed2405da55c9bb96a369c06bda4b7a26bd2ae38201230d0d4cdee0c`  
		Last Modified: Tue, 07 Jun 2022 06:55:12 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4d5c8e32cb2e967833d9ee92d4276d9a2887ba2388927db51f9666df1d3685d`  
		Last Modified: Tue, 07 Jun 2022 06:55:12 GMT  
		Size: 6.7 KB (6689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5.16-focal`

```console
$ docker pull mariadb@sha256:ca53a7cd054a66a34377737686753f1c9f9d797c18acc4e6e15ba997faa8b459
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.5.16-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:5b6b917fd647ee1f288216e78e3065d6e7cf37b2312a7087399a757619870b29
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.0 MB (128034257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b39c42d09fd1eb3753dc3b39271b1e3df2c19cc12ecc7a4124d6dd190ada994`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:42:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 00:42:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:42:35 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 00:42:46 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 00:42:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 00:42:53 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:42:53 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 00:42:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 00:44:04 GMT
ARG MARIADB_MAJOR=10.5
# Tue, 07 Jun 2022 00:44:04 GMT
ENV MARIADB_MAJOR=10.5
# Tue, 07 Jun 2022 00:44:04 GMT
ARG MARIADB_VERSION=1:10.5.16+maria~focal
# Tue, 07 Jun 2022 00:44:04 GMT
ENV MARIADB_VERSION=1:10.5.16+maria~focal
# Tue, 07 Jun 2022 00:44:04 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
# Tue, 07 Jun 2022 00:44:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 00:44:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 00:44:27 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 00:44:27 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 00:44:27 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Tue, 07 Jun 2022 00:44:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 00:44:27 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 00:44:27 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59dcb80bbedb867b19c4eb004e84c86ae3475041d5bd11672bae9ba6be45084f`  
		Last Modified: Tue, 07 Jun 2022 00:48:53 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6c41888e0f25dece871c7e65daad879fc39d7da0a84f6b67ae0d4e1f4a6f8a`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 5.5 MB (5488991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de82bf1cd45986845f81bc71a119bf5ceaec50c145064ea58e5729f4bd6d0d22`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 3.6 MB (3585352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316c0826d235e46a7a9adcfcc3068c004818dc2611a41b69e6e7bea02316b70f`  
		Last Modified: Tue, 07 Jun 2022 00:48:51 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b82e623f5d9ed1cc04e5adc22adc6805abdba4aecc5b427aec6c31223a64dca6`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 2.3 MB (2272315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3daba1f86bc0fd099576f61e5eea0961cdefed1dc443ffb96b6a50c8f054b0b0`  
		Last Modified: Tue, 07 Jun 2022 00:48:49 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa9c00f685bd6cf153c870dc2dd9bcd1e18a855fa57f40e6e41790a91c89117`  
		Last Modified: Tue, 07 Jun 2022 00:49:48 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48a603ad29b0aa206aa9ea8ab73e5750c1198bd28255d8bd8d7c78b97ac3da74`  
		Last Modified: Tue, 07 Jun 2022 00:50:01 GMT  
		Size: 88.1 MB (88100075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac467eecf9aafefbe0051851ef4782a491f9ef0bfe46bd3932eadb8165118c45`  
		Last Modified: Tue, 07 Jun 2022 00:49:48 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d11ea14c479ca40391b72f3c01a4c43be03a6aa941868082e9bb591f1070981`  
		Last Modified: Tue, 07 Jun 2022 00:49:48 GMT  
		Size: 6.7 KB (6689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.16-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:7d609f7bc3b1991769a4dca3b0e75e405636069665d18aa9e2738eae4d1eb528
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.3 MB (125291906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2add4e15f7c385964e8ed3c1a6fed4745b2008d9e46005161f00471308eedcc5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:03:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:03:44 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:03:45 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:04:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:04:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:04:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:04:10 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:04:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:06:23 GMT
ARG MARIADB_MAJOR=10.5
# Sat, 30 Apr 2022 00:06:24 GMT
ENV MARIADB_MAJOR=10.5
# Mon, 23 May 2022 18:43:31 GMT
ARG MARIADB_VERSION=1:10.5.16+maria~focal
# Mon, 23 May 2022 18:43:32 GMT
ENV MARIADB_VERSION=1:10.5.16+maria~focal
# Mon, 23 May 2022 18:43:33 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
# Mon, 23 May 2022 18:43:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 23 May 2022 18:43:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 23 May 2022 18:43:56 GMT
VOLUME [/var/lib/mysql]
# Mon, 23 May 2022 18:43:58 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Mon, 23 May 2022 18:43:59 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Mon, 23 May 2022 18:43:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 18:44:00 GMT
EXPOSE 3306
# Mon, 23 May 2022 18:44:01 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932d0da437931580c9d7f118c259624e1c3ec8e81acb2acf5740d945e511ba78`  
		Last Modified: Sat, 30 Apr 2022 00:11:03 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc35c765a7328bd99273ee471b6b108980755023d4bcb1927fa7717942a9d318`  
		Last Modified: Sat, 30 Apr 2022 00:11:02 GMT  
		Size: 5.3 MB (5320183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88bae007bd9c42610e465ab436d60b2457b10b735a1bc8e5daba38f548c026`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 3.4 MB (3369899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7734d2f7be989dfe94fb891565830b8101d8e9bdbcbce8e5a7e1b1932eb3ac3c`  
		Last Modified: Sat, 30 Apr 2022 00:11:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24600bac48ce2157027e68df9e26a81754edc6f7e099c33c0a89de879dba5d9`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 2.2 MB (2202385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da05700210f681c47e021b8f3ce45f244f696854cfd656f0cd46e59cb8ca9b7d`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ffae9fb7abd2928fa97e226250a176df36685529c856c8efbb37f8993bb844`  
		Last Modified: Mon, 23 May 2022 18:49:39 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee99e70137556b16b01eeee55ab2ed41b2d5330fca69b472aaaf1a9097b8bf4f`  
		Last Modified: Mon, 23 May 2022 18:49:52 GMT  
		Size: 87.2 MB (87215227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b1618553dab9fdb059b5f5efef5bcc2d8fb8c949aeb6f6359a36e2bc685dfe`  
		Last Modified: Mon, 23 May 2022 18:49:39 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f0edefce957b3f3e9d22ea3d184d5fd6250c446c0d7510401d669980f31956f`  
		Last Modified: Mon, 23 May 2022 18:49:39 GMT  
		Size: 6.7 KB (6693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.16-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:74603051778796eb42860bf97cba78820f1f4aa56a7299405744f498625c13c1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.9 MB (138920706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:910947f81ce0cd41a4a43ec2fcb0c19ba3a42d48b70f386ac8079970f344a371`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 07 Jun 2022 05:46:02 GMT
ADD file:86506a94b834ba2b6f10dc0d1955bee539be1cf565e4ccc2c4bc074e0375f115 in / 
# Tue, 07 Jun 2022 05:46:06 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 08:57:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 08:57:48 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 08:57:54 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 08:58:44 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 08:58:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 08:59:09 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 08:59:14 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 08:59:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 09:05:07 GMT
ARG MARIADB_MAJOR=10.5
# Tue, 07 Jun 2022 09:05:09 GMT
ENV MARIADB_MAJOR=10.5
# Tue, 07 Jun 2022 09:05:11 GMT
ARG MARIADB_VERSION=1:10.5.16+maria~focal
# Tue, 07 Jun 2022 09:05:14 GMT
ENV MARIADB_VERSION=1:10.5.16+maria~focal
# Tue, 07 Jun 2022 09:05:16 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
# Tue, 07 Jun 2022 09:05:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 09:06:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 09:07:00 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 09:07:01 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 09:07:02 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Tue, 07 Jun 2022 09:07:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 09:07:09 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 09:07:11 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3f52d061d2d3fdde0d3a099bbeae64080476c9650e9f3ba05de898d5bb5f03e8`  
		Last Modified: Tue, 07 Jun 2022 05:49:10 GMT  
		Size: 33.3 MB (33294345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b33a69d2ff59c89a297c597798ade8ea874f546d95513bd628c17fd7afda14`  
		Last Modified: Tue, 07 Jun 2022 09:17:18 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56a2c22a499e4928a88ae9201c66f507be8b9f10804ea7d0934710a6f91e5ec5`  
		Last Modified: Tue, 07 Jun 2022 09:17:18 GMT  
		Size: 6.7 MB (6667490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892b2ffb492b6d36ce25b68cf708d3c9bc9e0210e0cbbe7f575d3424c35d6b96`  
		Last Modified: Tue, 07 Jun 2022 09:17:17 GMT  
		Size: 3.7 MB (3672362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f80e77ec2bb0d7d685ca6e56f718adc6d253a98e069ebd5439f0c973194758`  
		Last Modified: Tue, 07 Jun 2022 09:17:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b0b3a9b79c49528e8e9da2d5d4954fc4e5392ee848c19c52a4d3369feb63d9`  
		Last Modified: Tue, 07 Jun 2022 09:17:16 GMT  
		Size: 2.6 MB (2568258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617e76c5eb45b560720c75ad4c60429a026cbbcb8467360cc70a7dace9ec4e5a`  
		Last Modified: Tue, 07 Jun 2022 09:17:13 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a59c27076a9e0b63144b746bf0ff178f849d8439122178341452eb038ce3e4f`  
		Last Modified: Tue, 07 Jun 2022 09:18:37 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd90769a974b7e7cda4cd39253ac95caa7589eebd08ff076bc83131ba7fb8839`  
		Last Modified: Tue, 07 Jun 2022 09:18:56 GMT  
		Size: 92.7 MB (92703341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4c17854aca625521983d66ec897032d27b9b2fac94d0361c43b022895db84d`  
		Last Modified: Tue, 07 Jun 2022 09:18:38 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b4b29126725a609c1392d5fc78c8c7a82a6c7a120d2e709858521aad09d48b`  
		Last Modified: Tue, 07 Jun 2022 09:18:37 GMT  
		Size: 6.7 KB (6693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.16-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:b04ed6dfca4d439554d1186288af3a20277081302a8d92b064191458587e5014
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.3 MB (127263882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d89f53da4f2085522e2510522207f8c4bd3e4c702d16c9b8653bb11008332b3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 07 Jun 2022 04:05:02 GMT
ADD file:6250f895d7d6c591cfe1b9fc991313d21b02167d94c67991db7c5c1c6814c51e in / 
# Tue, 07 Jun 2022 04:05:06 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:49:07 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 06:49:16 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:49:16 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 06:49:29 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 06:49:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 06:49:37 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:49:38 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 06:49:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 06:51:23 GMT
ARG MARIADB_MAJOR=10.5
# Tue, 07 Jun 2022 06:51:24 GMT
ENV MARIADB_MAJOR=10.5
# Tue, 07 Jun 2022 06:51:24 GMT
ARG MARIADB_VERSION=1:10.5.16+maria~focal
# Tue, 07 Jun 2022 06:51:24 GMT
ENV MARIADB_VERSION=1:10.5.16+maria~focal
# Tue, 07 Jun 2022 06:51:24 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
# Tue, 07 Jun 2022 06:51:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 06:52:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.16/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 06:52:15 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 06:52:16 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 06:52:16 GMT
COPY file:8104832da3dca41b18cf5ee1150e1522c4186f2e9a7f0fdf71d0277ac04ea849 in /usr/local/bin/ 
# Tue, 07 Jun 2022 06:52:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 06:52:17 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 06:52:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2f1fac119b88f55cd8329458ec27c3d6d6cb324b0fe541feacfd9a4ee621a558`  
		Last Modified: Tue, 07 Jun 2022 04:07:45 GMT  
		Size: 27.1 MB (27056020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e11bbd03dcb74b0a89181bc7b5b0c6a1081475b91f09e5b7bd4378245677d0`  
		Last Modified: Tue, 07 Jun 2022 06:54:23 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944609fc08b7430c363765f8d65b07874048d4ee4b4fddc6378410ffbf35a5e4`  
		Last Modified: Tue, 07 Jun 2022 06:54:23 GMT  
		Size: 5.4 MB (5372398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc686e965111a0f5a9fbe0d2fd56fb1cbe1f37cd32ba702e6e181eb8bd952476`  
		Last Modified: Tue, 07 Jun 2022 06:54:22 GMT  
		Size: 3.2 MB (3244071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c6b370e34d40b571955a0831c8669ab35e55a71bc048f8ad7355f3971ba4b3`  
		Last Modified: Tue, 07 Jun 2022 06:54:21 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13a21a85799843063b419b269af229d786c77820174a95c4dcc2363cee9c846`  
		Last Modified: Tue, 07 Jun 2022 06:54:21 GMT  
		Size: 2.2 MB (2183581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed1ebbc1458626d5a4732baab692192158957e9db1cb87eb1e2e23e531a49d6`  
		Last Modified: Tue, 07 Jun 2022 06:54:20 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3ad4eda1b4a8ef767f27722613a4f5c3cf0973e58ed1b051c4d9db476671525`  
		Last Modified: Tue, 07 Jun 2022 06:55:12 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20082cb10cc20f97ee82b3ca5dabc03bd6eb4e8eb09ed6ea11ed9c8c24fa4c05`  
		Last Modified: Tue, 07 Jun 2022 06:55:25 GMT  
		Size: 89.4 MB (89392913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12966bf5bed2405da55c9bb96a369c06bda4b7a26bd2ae38201230d0d4cdee0c`  
		Last Modified: Tue, 07 Jun 2022 06:55:12 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4d5c8e32cb2e967833d9ee92d4276d9a2887ba2388927db51f9666df1d3685d`  
		Last Modified: Tue, 07 Jun 2022 06:55:12 GMT  
		Size: 6.7 KB (6689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.6`

```console
$ docker pull mariadb@sha256:6dc9418a58a9f1e7cdf01e7ce1126a4b28b55896fc0c2b54ba38695e0bdf1277
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.6` - linux; amd64

```console
$ docker pull mariadb@sha256:7819eec13e69628884635961a6d7f89f4572f4ea95a90b0ef978ff3a3f737bc3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.3 MB (128309365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bda4cf409ffca693506ef4fca5b613f0e01839d390f48244aca2da2de114a939`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:42:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 00:42:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:42:35 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 00:42:46 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 00:42:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 00:42:53 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:42:53 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 00:42:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 00:43:35 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 07 Jun 2022 00:43:36 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 07 Jun 2022 00:43:36 GMT
ARG MARIADB_VERSION=1:10.6.8+maria~focal
# Tue, 07 Jun 2022 00:43:36 GMT
ENV MARIADB_VERSION=1:10.6.8+maria~focal
# Tue, 07 Jun 2022 00:43:36 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
# Tue, 07 Jun 2022 00:43:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 00:43:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 00:44:00 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 00:44:00 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 00:44:00 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 07 Jun 2022 00:44:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 00:44:00 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 00:44:00 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59dcb80bbedb867b19c4eb004e84c86ae3475041d5bd11672bae9ba6be45084f`  
		Last Modified: Tue, 07 Jun 2022 00:48:53 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6c41888e0f25dece871c7e65daad879fc39d7da0a84f6b67ae0d4e1f4a6f8a`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 5.5 MB (5488991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de82bf1cd45986845f81bc71a119bf5ceaec50c145064ea58e5729f4bd6d0d22`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 3.6 MB (3585352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316c0826d235e46a7a9adcfcc3068c004818dc2611a41b69e6e7bea02316b70f`  
		Last Modified: Tue, 07 Jun 2022 00:48:51 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b82e623f5d9ed1cc04e5adc22adc6805abdba4aecc5b427aec6c31223a64dca6`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 2.3 MB (2272315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3daba1f86bc0fd099576f61e5eea0961cdefed1dc443ffb96b6a50c8f054b0b0`  
		Last Modified: Tue, 07 Jun 2022 00:48:49 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81411bfac31886b163d372c72f92b47325fe4acae247b86065df7b4a335596af`  
		Last Modified: Tue, 07 Jun 2022 00:49:18 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5393d049295a041d7d52f4b9594a8c074502691fcaf0cddc115a9a8a8bf1a400`  
		Last Modified: Tue, 07 Jun 2022 00:49:32 GMT  
		Size: 88.4 MB (88375172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46020ed440f2aed3b5607767d5f894c6d333e06d739797d7cb285998cec12736`  
		Last Modified: Tue, 07 Jun 2022 00:49:18 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed53f9923e662bb247b209f6dc8ae0610bace4a54d446630c8b04f6e5197cc8f`  
		Last Modified: Tue, 07 Jun 2022 00:49:18 GMT  
		Size: 6.7 KB (6698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:005ec17d9c90bce79e578c244a75c1b4bcd58b6aa25cc98f862403b0f713677e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.4 MB (125350431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54532887d57dda6d4ad134dc385a8b316120b621ffe4d13b6ef9e4d97e7b67f1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:03:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:03:44 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:03:45 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:04:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:04:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:04:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:04:10 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:04:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:05:39 GMT
ARG MARIADB_MAJOR=10.6
# Sat, 30 Apr 2022 00:05:40 GMT
ENV MARIADB_MAJOR=10.6
# Mon, 23 May 2022 18:42:54 GMT
ARG MARIADB_VERSION=1:10.6.8+maria~focal
# Mon, 23 May 2022 18:42:55 GMT
ENV MARIADB_VERSION=1:10.6.8+maria~focal
# Mon, 23 May 2022 18:42:56 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
# Mon, 23 May 2022 18:42:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 23 May 2022 18:43:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 23 May 2022 18:43:20 GMT
VOLUME [/var/lib/mysql]
# Mon, 23 May 2022 18:43:21 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Mon, 23 May 2022 18:43:22 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Mon, 23 May 2022 18:43:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 18:43:23 GMT
EXPOSE 3306
# Mon, 23 May 2022 18:43:24 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932d0da437931580c9d7f118c259624e1c3ec8e81acb2acf5740d945e511ba78`  
		Last Modified: Sat, 30 Apr 2022 00:11:03 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc35c765a7328bd99273ee471b6b108980755023d4bcb1927fa7717942a9d318`  
		Last Modified: Sat, 30 Apr 2022 00:11:02 GMT  
		Size: 5.3 MB (5320183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88bae007bd9c42610e465ab436d60b2457b10b735a1bc8e5daba38f548c026`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 3.4 MB (3369899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7734d2f7be989dfe94fb891565830b8101d8e9bdbcbce8e5a7e1b1932eb3ac3c`  
		Last Modified: Sat, 30 Apr 2022 00:11:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24600bac48ce2157027e68df9e26a81754edc6f7e099c33c0a89de879dba5d9`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 2.2 MB (2202385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da05700210f681c47e021b8f3ce45f244f696854cfd656f0cd46e59cb8ca9b7d`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a04e707f9157288d2518664b72f585be74f80738c3e5d334623bd8f4dfde99b7`  
		Last Modified: Mon, 23 May 2022 18:49:06 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:779a6849160ddb2191bef8873e41d106fd7a9f05607a4711782a1f316450a46d`  
		Last Modified: Mon, 23 May 2022 18:49:20 GMT  
		Size: 87.3 MB (87273747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6601e79019448824b98ca1a7b9263ae9e6dca141455d0317eee0dffb1df8af`  
		Last Modified: Mon, 23 May 2022 18:49:06 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2580a760c284152fef0af2edafdaeebf5833c8072b08e26c6f8f00ccd339a5ee`  
		Last Modified: Mon, 23 May 2022 18:49:07 GMT  
		Size: 6.7 KB (6700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6` - linux; ppc64le

```console
$ docker pull mariadb@sha256:46627532ee7aef79d210470e90e422ac1c194ac32b54ebff10d8a8c11c3a9a95
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.0 MB (138978859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46cf570da4de5cd6bcd27f0bc1d21f601b87be375020bb793793742f69526e69`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 07 Jun 2022 05:46:02 GMT
ADD file:86506a94b834ba2b6f10dc0d1955bee539be1cf565e4ccc2c4bc074e0375f115 in / 
# Tue, 07 Jun 2022 05:46:06 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 08:57:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 08:57:48 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 08:57:54 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 08:58:44 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 08:58:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 08:59:09 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 08:59:14 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 08:59:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 09:02:12 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 07 Jun 2022 09:02:14 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 07 Jun 2022 09:02:18 GMT
ARG MARIADB_VERSION=1:10.6.8+maria~focal
# Tue, 07 Jun 2022 09:02:21 GMT
ENV MARIADB_VERSION=1:10.6.8+maria~focal
# Tue, 07 Jun 2022 09:02:23 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
# Tue, 07 Jun 2022 09:02:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 09:04:35 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 09:04:41 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 09:04:42 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 09:04:43 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 07 Jun 2022 09:04:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 09:04:46 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 09:04:49 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:3f52d061d2d3fdde0d3a099bbeae64080476c9650e9f3ba05de898d5bb5f03e8`  
		Last Modified: Tue, 07 Jun 2022 05:49:10 GMT  
		Size: 33.3 MB (33294345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b33a69d2ff59c89a297c597798ade8ea874f546d95513bd628c17fd7afda14`  
		Last Modified: Tue, 07 Jun 2022 09:17:18 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56a2c22a499e4928a88ae9201c66f507be8b9f10804ea7d0934710a6f91e5ec5`  
		Last Modified: Tue, 07 Jun 2022 09:17:18 GMT  
		Size: 6.7 MB (6667490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892b2ffb492b6d36ce25b68cf708d3c9bc9e0210e0cbbe7f575d3424c35d6b96`  
		Last Modified: Tue, 07 Jun 2022 09:17:17 GMT  
		Size: 3.7 MB (3672362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f80e77ec2bb0d7d685ca6e56f718adc6d253a98e069ebd5439f0c973194758`  
		Last Modified: Tue, 07 Jun 2022 09:17:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b0b3a9b79c49528e8e9da2d5d4954fc4e5392ee848c19c52a4d3369feb63d9`  
		Last Modified: Tue, 07 Jun 2022 09:17:16 GMT  
		Size: 2.6 MB (2568258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617e76c5eb45b560720c75ad4c60429a026cbbcb8467360cc70a7dace9ec4e5a`  
		Last Modified: Tue, 07 Jun 2022 09:17:13 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51097485d982057c87d379feafcbe1d1919349d09a239da19f742e292352da53`  
		Last Modified: Tue, 07 Jun 2022 09:17:59 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8855a4247a5c8216750c0403a57e1c7bcaa78ed396ea922681774e9528bd4e65`  
		Last Modified: Tue, 07 Jun 2022 09:18:17 GMT  
		Size: 92.8 MB (92761496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f780a8c6c967e12e3c99e28ad2bbefff751612fd54aed4740341269dcb4bb198`  
		Last Modified: Tue, 07 Jun 2022 09:17:59 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91380c084c6b0b149781eea18ec91ed28730f07a27346e830d10419cab87f7b5`  
		Last Modified: Tue, 07 Jun 2022 09:17:59 GMT  
		Size: 6.7 KB (6696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6` - linux; s390x

```console
$ docker pull mariadb@sha256:214f3687906b35bea0534fb4267509630eaf1c1b4b8410d0827d0981a52f0cff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.3 MB (127329897 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df253f4cc135aa64fb302a44a9849b2b620ebd4414dc60af0440b6dde07b3141`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 07 Jun 2022 04:05:02 GMT
ADD file:6250f895d7d6c591cfe1b9fc991313d21b02167d94c67991db7c5c1c6814c51e in / 
# Tue, 07 Jun 2022 04:05:06 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:49:07 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 06:49:16 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:49:16 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 06:49:29 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 06:49:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 06:49:37 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:49:38 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 06:49:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 06:50:26 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 07 Jun 2022 06:50:26 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 07 Jun 2022 06:50:26 GMT
ARG MARIADB_VERSION=1:10.6.8+maria~focal
# Tue, 07 Jun 2022 06:50:27 GMT
ENV MARIADB_VERSION=1:10.6.8+maria~focal
# Tue, 07 Jun 2022 06:50:27 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
# Tue, 07 Jun 2022 06:50:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 06:51:01 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 06:51:14 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 06:51:14 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 06:51:14 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 07 Jun 2022 06:51:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 06:51:15 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 06:51:16 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:2f1fac119b88f55cd8329458ec27c3d6d6cb324b0fe541feacfd9a4ee621a558`  
		Last Modified: Tue, 07 Jun 2022 04:07:45 GMT  
		Size: 27.1 MB (27056020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e11bbd03dcb74b0a89181bc7b5b0c6a1081475b91f09e5b7bd4378245677d0`  
		Last Modified: Tue, 07 Jun 2022 06:54:23 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944609fc08b7430c363765f8d65b07874048d4ee4b4fddc6378410ffbf35a5e4`  
		Last Modified: Tue, 07 Jun 2022 06:54:23 GMT  
		Size: 5.4 MB (5372398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc686e965111a0f5a9fbe0d2fd56fb1cbe1f37cd32ba702e6e181eb8bd952476`  
		Last Modified: Tue, 07 Jun 2022 06:54:22 GMT  
		Size: 3.2 MB (3244071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c6b370e34d40b571955a0831c8669ab35e55a71bc048f8ad7355f3971ba4b3`  
		Last Modified: Tue, 07 Jun 2022 06:54:21 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13a21a85799843063b419b269af229d786c77820174a95c4dcc2363cee9c846`  
		Last Modified: Tue, 07 Jun 2022 06:54:21 GMT  
		Size: 2.2 MB (2183581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed1ebbc1458626d5a4732baab692192158957e9db1cb87eb1e2e23e531a49d6`  
		Last Modified: Tue, 07 Jun 2022 06:54:20 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b47aa84fc870e5c06f446069453d141adf0fa22eef7a4fe7cfb9214a24e741d`  
		Last Modified: Tue, 07 Jun 2022 06:54:47 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b635562f4bc8556889bb0f2b9f3ff626d35835290a62846421fe11a8715431c0`  
		Last Modified: Tue, 07 Jun 2022 06:55:00 GMT  
		Size: 89.5 MB (89458920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab733f3f3db269ec38e98e09601a15f589311ec121020e630991c8c53549053`  
		Last Modified: Tue, 07 Jun 2022 06:54:47 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e894f58de8cbfec950d7d9f430b4a6eb9b1c04086571f40b5bd5ef8a606ad0`  
		Last Modified: Tue, 07 Jun 2022 06:54:47 GMT  
		Size: 6.7 KB (6696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.6-focal`

```console
$ docker pull mariadb@sha256:6dc9418a58a9f1e7cdf01e7ce1126a4b28b55896fc0c2b54ba38695e0bdf1277
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.6-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:7819eec13e69628884635961a6d7f89f4572f4ea95a90b0ef978ff3a3f737bc3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.3 MB (128309365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bda4cf409ffca693506ef4fca5b613f0e01839d390f48244aca2da2de114a939`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:42:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 00:42:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:42:35 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 00:42:46 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 00:42:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 00:42:53 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:42:53 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 00:42:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 00:43:35 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 07 Jun 2022 00:43:36 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 07 Jun 2022 00:43:36 GMT
ARG MARIADB_VERSION=1:10.6.8+maria~focal
# Tue, 07 Jun 2022 00:43:36 GMT
ENV MARIADB_VERSION=1:10.6.8+maria~focal
# Tue, 07 Jun 2022 00:43:36 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
# Tue, 07 Jun 2022 00:43:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 00:43:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 00:44:00 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 00:44:00 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 00:44:00 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 07 Jun 2022 00:44:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 00:44:00 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 00:44:00 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59dcb80bbedb867b19c4eb004e84c86ae3475041d5bd11672bae9ba6be45084f`  
		Last Modified: Tue, 07 Jun 2022 00:48:53 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6c41888e0f25dece871c7e65daad879fc39d7da0a84f6b67ae0d4e1f4a6f8a`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 5.5 MB (5488991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de82bf1cd45986845f81bc71a119bf5ceaec50c145064ea58e5729f4bd6d0d22`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 3.6 MB (3585352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316c0826d235e46a7a9adcfcc3068c004818dc2611a41b69e6e7bea02316b70f`  
		Last Modified: Tue, 07 Jun 2022 00:48:51 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b82e623f5d9ed1cc04e5adc22adc6805abdba4aecc5b427aec6c31223a64dca6`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 2.3 MB (2272315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3daba1f86bc0fd099576f61e5eea0961cdefed1dc443ffb96b6a50c8f054b0b0`  
		Last Modified: Tue, 07 Jun 2022 00:48:49 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81411bfac31886b163d372c72f92b47325fe4acae247b86065df7b4a335596af`  
		Last Modified: Tue, 07 Jun 2022 00:49:18 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5393d049295a041d7d52f4b9594a8c074502691fcaf0cddc115a9a8a8bf1a400`  
		Last Modified: Tue, 07 Jun 2022 00:49:32 GMT  
		Size: 88.4 MB (88375172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46020ed440f2aed3b5607767d5f894c6d333e06d739797d7cb285998cec12736`  
		Last Modified: Tue, 07 Jun 2022 00:49:18 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed53f9923e662bb247b209f6dc8ae0610bace4a54d446630c8b04f6e5197cc8f`  
		Last Modified: Tue, 07 Jun 2022 00:49:18 GMT  
		Size: 6.7 KB (6698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:005ec17d9c90bce79e578c244a75c1b4bcd58b6aa25cc98f862403b0f713677e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.4 MB (125350431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54532887d57dda6d4ad134dc385a8b316120b621ffe4d13b6ef9e4d97e7b67f1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:03:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:03:44 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:03:45 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:04:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:04:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:04:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:04:10 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:04:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:05:39 GMT
ARG MARIADB_MAJOR=10.6
# Sat, 30 Apr 2022 00:05:40 GMT
ENV MARIADB_MAJOR=10.6
# Mon, 23 May 2022 18:42:54 GMT
ARG MARIADB_VERSION=1:10.6.8+maria~focal
# Mon, 23 May 2022 18:42:55 GMT
ENV MARIADB_VERSION=1:10.6.8+maria~focal
# Mon, 23 May 2022 18:42:56 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
# Mon, 23 May 2022 18:42:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 23 May 2022 18:43:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 23 May 2022 18:43:20 GMT
VOLUME [/var/lib/mysql]
# Mon, 23 May 2022 18:43:21 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Mon, 23 May 2022 18:43:22 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Mon, 23 May 2022 18:43:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 18:43:23 GMT
EXPOSE 3306
# Mon, 23 May 2022 18:43:24 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932d0da437931580c9d7f118c259624e1c3ec8e81acb2acf5740d945e511ba78`  
		Last Modified: Sat, 30 Apr 2022 00:11:03 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc35c765a7328bd99273ee471b6b108980755023d4bcb1927fa7717942a9d318`  
		Last Modified: Sat, 30 Apr 2022 00:11:02 GMT  
		Size: 5.3 MB (5320183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88bae007bd9c42610e465ab436d60b2457b10b735a1bc8e5daba38f548c026`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 3.4 MB (3369899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7734d2f7be989dfe94fb891565830b8101d8e9bdbcbce8e5a7e1b1932eb3ac3c`  
		Last Modified: Sat, 30 Apr 2022 00:11:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24600bac48ce2157027e68df9e26a81754edc6f7e099c33c0a89de879dba5d9`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 2.2 MB (2202385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da05700210f681c47e021b8f3ce45f244f696854cfd656f0cd46e59cb8ca9b7d`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a04e707f9157288d2518664b72f585be74f80738c3e5d334623bd8f4dfde99b7`  
		Last Modified: Mon, 23 May 2022 18:49:06 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:779a6849160ddb2191bef8873e41d106fd7a9f05607a4711782a1f316450a46d`  
		Last Modified: Mon, 23 May 2022 18:49:20 GMT  
		Size: 87.3 MB (87273747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6601e79019448824b98ca1a7b9263ae9e6dca141455d0317eee0dffb1df8af`  
		Last Modified: Mon, 23 May 2022 18:49:06 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2580a760c284152fef0af2edafdaeebf5833c8072b08e26c6f8f00ccd339a5ee`  
		Last Modified: Mon, 23 May 2022 18:49:07 GMT  
		Size: 6.7 KB (6700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:46627532ee7aef79d210470e90e422ac1c194ac32b54ebff10d8a8c11c3a9a95
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.0 MB (138978859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46cf570da4de5cd6bcd27f0bc1d21f601b87be375020bb793793742f69526e69`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 07 Jun 2022 05:46:02 GMT
ADD file:86506a94b834ba2b6f10dc0d1955bee539be1cf565e4ccc2c4bc074e0375f115 in / 
# Tue, 07 Jun 2022 05:46:06 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 08:57:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 08:57:48 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 08:57:54 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 08:58:44 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 08:58:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 08:59:09 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 08:59:14 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 08:59:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 09:02:12 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 07 Jun 2022 09:02:14 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 07 Jun 2022 09:02:18 GMT
ARG MARIADB_VERSION=1:10.6.8+maria~focal
# Tue, 07 Jun 2022 09:02:21 GMT
ENV MARIADB_VERSION=1:10.6.8+maria~focal
# Tue, 07 Jun 2022 09:02:23 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
# Tue, 07 Jun 2022 09:02:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 09:04:35 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 09:04:41 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 09:04:42 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 09:04:43 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 07 Jun 2022 09:04:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 09:04:46 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 09:04:49 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:3f52d061d2d3fdde0d3a099bbeae64080476c9650e9f3ba05de898d5bb5f03e8`  
		Last Modified: Tue, 07 Jun 2022 05:49:10 GMT  
		Size: 33.3 MB (33294345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b33a69d2ff59c89a297c597798ade8ea874f546d95513bd628c17fd7afda14`  
		Last Modified: Tue, 07 Jun 2022 09:17:18 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56a2c22a499e4928a88ae9201c66f507be8b9f10804ea7d0934710a6f91e5ec5`  
		Last Modified: Tue, 07 Jun 2022 09:17:18 GMT  
		Size: 6.7 MB (6667490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892b2ffb492b6d36ce25b68cf708d3c9bc9e0210e0cbbe7f575d3424c35d6b96`  
		Last Modified: Tue, 07 Jun 2022 09:17:17 GMT  
		Size: 3.7 MB (3672362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f80e77ec2bb0d7d685ca6e56f718adc6d253a98e069ebd5439f0c973194758`  
		Last Modified: Tue, 07 Jun 2022 09:17:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b0b3a9b79c49528e8e9da2d5d4954fc4e5392ee848c19c52a4d3369feb63d9`  
		Last Modified: Tue, 07 Jun 2022 09:17:16 GMT  
		Size: 2.6 MB (2568258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617e76c5eb45b560720c75ad4c60429a026cbbcb8467360cc70a7dace9ec4e5a`  
		Last Modified: Tue, 07 Jun 2022 09:17:13 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51097485d982057c87d379feafcbe1d1919349d09a239da19f742e292352da53`  
		Last Modified: Tue, 07 Jun 2022 09:17:59 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8855a4247a5c8216750c0403a57e1c7bcaa78ed396ea922681774e9528bd4e65`  
		Last Modified: Tue, 07 Jun 2022 09:18:17 GMT  
		Size: 92.8 MB (92761496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f780a8c6c967e12e3c99e28ad2bbefff751612fd54aed4740341269dcb4bb198`  
		Last Modified: Tue, 07 Jun 2022 09:17:59 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91380c084c6b0b149781eea18ec91ed28730f07a27346e830d10419cab87f7b5`  
		Last Modified: Tue, 07 Jun 2022 09:17:59 GMT  
		Size: 6.7 KB (6696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:214f3687906b35bea0534fb4267509630eaf1c1b4b8410d0827d0981a52f0cff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.3 MB (127329897 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df253f4cc135aa64fb302a44a9849b2b620ebd4414dc60af0440b6dde07b3141`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 07 Jun 2022 04:05:02 GMT
ADD file:6250f895d7d6c591cfe1b9fc991313d21b02167d94c67991db7c5c1c6814c51e in / 
# Tue, 07 Jun 2022 04:05:06 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:49:07 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 06:49:16 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:49:16 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 06:49:29 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 06:49:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 06:49:37 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:49:38 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 06:49:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 06:50:26 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 07 Jun 2022 06:50:26 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 07 Jun 2022 06:50:26 GMT
ARG MARIADB_VERSION=1:10.6.8+maria~focal
# Tue, 07 Jun 2022 06:50:27 GMT
ENV MARIADB_VERSION=1:10.6.8+maria~focal
# Tue, 07 Jun 2022 06:50:27 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
# Tue, 07 Jun 2022 06:50:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 06:51:01 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 06:51:14 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 06:51:14 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 06:51:14 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 07 Jun 2022 06:51:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 06:51:15 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 06:51:16 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:2f1fac119b88f55cd8329458ec27c3d6d6cb324b0fe541feacfd9a4ee621a558`  
		Last Modified: Tue, 07 Jun 2022 04:07:45 GMT  
		Size: 27.1 MB (27056020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e11bbd03dcb74b0a89181bc7b5b0c6a1081475b91f09e5b7bd4378245677d0`  
		Last Modified: Tue, 07 Jun 2022 06:54:23 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944609fc08b7430c363765f8d65b07874048d4ee4b4fddc6378410ffbf35a5e4`  
		Last Modified: Tue, 07 Jun 2022 06:54:23 GMT  
		Size: 5.4 MB (5372398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc686e965111a0f5a9fbe0d2fd56fb1cbe1f37cd32ba702e6e181eb8bd952476`  
		Last Modified: Tue, 07 Jun 2022 06:54:22 GMT  
		Size: 3.2 MB (3244071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c6b370e34d40b571955a0831c8669ab35e55a71bc048f8ad7355f3971ba4b3`  
		Last Modified: Tue, 07 Jun 2022 06:54:21 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13a21a85799843063b419b269af229d786c77820174a95c4dcc2363cee9c846`  
		Last Modified: Tue, 07 Jun 2022 06:54:21 GMT  
		Size: 2.2 MB (2183581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed1ebbc1458626d5a4732baab692192158957e9db1cb87eb1e2e23e531a49d6`  
		Last Modified: Tue, 07 Jun 2022 06:54:20 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b47aa84fc870e5c06f446069453d141adf0fa22eef7a4fe7cfb9214a24e741d`  
		Last Modified: Tue, 07 Jun 2022 06:54:47 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b635562f4bc8556889bb0f2b9f3ff626d35835290a62846421fe11a8715431c0`  
		Last Modified: Tue, 07 Jun 2022 06:55:00 GMT  
		Size: 89.5 MB (89458920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab733f3f3db269ec38e98e09601a15f589311ec121020e630991c8c53549053`  
		Last Modified: Tue, 07 Jun 2022 06:54:47 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e894f58de8cbfec950d7d9f430b4a6eb9b1c04086571f40b5bd5ef8a606ad0`  
		Last Modified: Tue, 07 Jun 2022 06:54:47 GMT  
		Size: 6.7 KB (6696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.6.8`

```console
$ docker pull mariadb@sha256:6dc9418a58a9f1e7cdf01e7ce1126a4b28b55896fc0c2b54ba38695e0bdf1277
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.6.8` - linux; amd64

```console
$ docker pull mariadb@sha256:7819eec13e69628884635961a6d7f89f4572f4ea95a90b0ef978ff3a3f737bc3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.3 MB (128309365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bda4cf409ffca693506ef4fca5b613f0e01839d390f48244aca2da2de114a939`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:42:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 00:42:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:42:35 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 00:42:46 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 00:42:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 00:42:53 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:42:53 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 00:42:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 00:43:35 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 07 Jun 2022 00:43:36 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 07 Jun 2022 00:43:36 GMT
ARG MARIADB_VERSION=1:10.6.8+maria~focal
# Tue, 07 Jun 2022 00:43:36 GMT
ENV MARIADB_VERSION=1:10.6.8+maria~focal
# Tue, 07 Jun 2022 00:43:36 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
# Tue, 07 Jun 2022 00:43:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 00:43:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 00:44:00 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 00:44:00 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 00:44:00 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 07 Jun 2022 00:44:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 00:44:00 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 00:44:00 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59dcb80bbedb867b19c4eb004e84c86ae3475041d5bd11672bae9ba6be45084f`  
		Last Modified: Tue, 07 Jun 2022 00:48:53 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6c41888e0f25dece871c7e65daad879fc39d7da0a84f6b67ae0d4e1f4a6f8a`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 5.5 MB (5488991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de82bf1cd45986845f81bc71a119bf5ceaec50c145064ea58e5729f4bd6d0d22`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 3.6 MB (3585352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316c0826d235e46a7a9adcfcc3068c004818dc2611a41b69e6e7bea02316b70f`  
		Last Modified: Tue, 07 Jun 2022 00:48:51 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b82e623f5d9ed1cc04e5adc22adc6805abdba4aecc5b427aec6c31223a64dca6`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 2.3 MB (2272315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3daba1f86bc0fd099576f61e5eea0961cdefed1dc443ffb96b6a50c8f054b0b0`  
		Last Modified: Tue, 07 Jun 2022 00:48:49 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81411bfac31886b163d372c72f92b47325fe4acae247b86065df7b4a335596af`  
		Last Modified: Tue, 07 Jun 2022 00:49:18 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5393d049295a041d7d52f4b9594a8c074502691fcaf0cddc115a9a8a8bf1a400`  
		Last Modified: Tue, 07 Jun 2022 00:49:32 GMT  
		Size: 88.4 MB (88375172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46020ed440f2aed3b5607767d5f894c6d333e06d739797d7cb285998cec12736`  
		Last Modified: Tue, 07 Jun 2022 00:49:18 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed53f9923e662bb247b209f6dc8ae0610bace4a54d446630c8b04f6e5197cc8f`  
		Last Modified: Tue, 07 Jun 2022 00:49:18 GMT  
		Size: 6.7 KB (6698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6.8` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:005ec17d9c90bce79e578c244a75c1b4bcd58b6aa25cc98f862403b0f713677e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.4 MB (125350431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54532887d57dda6d4ad134dc385a8b316120b621ffe4d13b6ef9e4d97e7b67f1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:03:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:03:44 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:03:45 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:04:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:04:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:04:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:04:10 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:04:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:05:39 GMT
ARG MARIADB_MAJOR=10.6
# Sat, 30 Apr 2022 00:05:40 GMT
ENV MARIADB_MAJOR=10.6
# Mon, 23 May 2022 18:42:54 GMT
ARG MARIADB_VERSION=1:10.6.8+maria~focal
# Mon, 23 May 2022 18:42:55 GMT
ENV MARIADB_VERSION=1:10.6.8+maria~focal
# Mon, 23 May 2022 18:42:56 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
# Mon, 23 May 2022 18:42:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 23 May 2022 18:43:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 23 May 2022 18:43:20 GMT
VOLUME [/var/lib/mysql]
# Mon, 23 May 2022 18:43:21 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Mon, 23 May 2022 18:43:22 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Mon, 23 May 2022 18:43:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 18:43:23 GMT
EXPOSE 3306
# Mon, 23 May 2022 18:43:24 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932d0da437931580c9d7f118c259624e1c3ec8e81acb2acf5740d945e511ba78`  
		Last Modified: Sat, 30 Apr 2022 00:11:03 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc35c765a7328bd99273ee471b6b108980755023d4bcb1927fa7717942a9d318`  
		Last Modified: Sat, 30 Apr 2022 00:11:02 GMT  
		Size: 5.3 MB (5320183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88bae007bd9c42610e465ab436d60b2457b10b735a1bc8e5daba38f548c026`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 3.4 MB (3369899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7734d2f7be989dfe94fb891565830b8101d8e9bdbcbce8e5a7e1b1932eb3ac3c`  
		Last Modified: Sat, 30 Apr 2022 00:11:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24600bac48ce2157027e68df9e26a81754edc6f7e099c33c0a89de879dba5d9`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 2.2 MB (2202385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da05700210f681c47e021b8f3ce45f244f696854cfd656f0cd46e59cb8ca9b7d`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a04e707f9157288d2518664b72f585be74f80738c3e5d334623bd8f4dfde99b7`  
		Last Modified: Mon, 23 May 2022 18:49:06 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:779a6849160ddb2191bef8873e41d106fd7a9f05607a4711782a1f316450a46d`  
		Last Modified: Mon, 23 May 2022 18:49:20 GMT  
		Size: 87.3 MB (87273747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6601e79019448824b98ca1a7b9263ae9e6dca141455d0317eee0dffb1df8af`  
		Last Modified: Mon, 23 May 2022 18:49:06 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2580a760c284152fef0af2edafdaeebf5833c8072b08e26c6f8f00ccd339a5ee`  
		Last Modified: Mon, 23 May 2022 18:49:07 GMT  
		Size: 6.7 KB (6700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6.8` - linux; ppc64le

```console
$ docker pull mariadb@sha256:46627532ee7aef79d210470e90e422ac1c194ac32b54ebff10d8a8c11c3a9a95
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.0 MB (138978859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46cf570da4de5cd6bcd27f0bc1d21f601b87be375020bb793793742f69526e69`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 07 Jun 2022 05:46:02 GMT
ADD file:86506a94b834ba2b6f10dc0d1955bee539be1cf565e4ccc2c4bc074e0375f115 in / 
# Tue, 07 Jun 2022 05:46:06 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 08:57:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 08:57:48 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 08:57:54 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 08:58:44 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 08:58:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 08:59:09 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 08:59:14 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 08:59:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 09:02:12 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 07 Jun 2022 09:02:14 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 07 Jun 2022 09:02:18 GMT
ARG MARIADB_VERSION=1:10.6.8+maria~focal
# Tue, 07 Jun 2022 09:02:21 GMT
ENV MARIADB_VERSION=1:10.6.8+maria~focal
# Tue, 07 Jun 2022 09:02:23 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
# Tue, 07 Jun 2022 09:02:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 09:04:35 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 09:04:41 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 09:04:42 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 09:04:43 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 07 Jun 2022 09:04:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 09:04:46 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 09:04:49 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:3f52d061d2d3fdde0d3a099bbeae64080476c9650e9f3ba05de898d5bb5f03e8`  
		Last Modified: Tue, 07 Jun 2022 05:49:10 GMT  
		Size: 33.3 MB (33294345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b33a69d2ff59c89a297c597798ade8ea874f546d95513bd628c17fd7afda14`  
		Last Modified: Tue, 07 Jun 2022 09:17:18 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56a2c22a499e4928a88ae9201c66f507be8b9f10804ea7d0934710a6f91e5ec5`  
		Last Modified: Tue, 07 Jun 2022 09:17:18 GMT  
		Size: 6.7 MB (6667490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892b2ffb492b6d36ce25b68cf708d3c9bc9e0210e0cbbe7f575d3424c35d6b96`  
		Last Modified: Tue, 07 Jun 2022 09:17:17 GMT  
		Size: 3.7 MB (3672362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f80e77ec2bb0d7d685ca6e56f718adc6d253a98e069ebd5439f0c973194758`  
		Last Modified: Tue, 07 Jun 2022 09:17:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b0b3a9b79c49528e8e9da2d5d4954fc4e5392ee848c19c52a4d3369feb63d9`  
		Last Modified: Tue, 07 Jun 2022 09:17:16 GMT  
		Size: 2.6 MB (2568258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617e76c5eb45b560720c75ad4c60429a026cbbcb8467360cc70a7dace9ec4e5a`  
		Last Modified: Tue, 07 Jun 2022 09:17:13 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51097485d982057c87d379feafcbe1d1919349d09a239da19f742e292352da53`  
		Last Modified: Tue, 07 Jun 2022 09:17:59 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8855a4247a5c8216750c0403a57e1c7bcaa78ed396ea922681774e9528bd4e65`  
		Last Modified: Tue, 07 Jun 2022 09:18:17 GMT  
		Size: 92.8 MB (92761496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f780a8c6c967e12e3c99e28ad2bbefff751612fd54aed4740341269dcb4bb198`  
		Last Modified: Tue, 07 Jun 2022 09:17:59 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91380c084c6b0b149781eea18ec91ed28730f07a27346e830d10419cab87f7b5`  
		Last Modified: Tue, 07 Jun 2022 09:17:59 GMT  
		Size: 6.7 KB (6696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6.8` - linux; s390x

```console
$ docker pull mariadb@sha256:214f3687906b35bea0534fb4267509630eaf1c1b4b8410d0827d0981a52f0cff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.3 MB (127329897 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df253f4cc135aa64fb302a44a9849b2b620ebd4414dc60af0440b6dde07b3141`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 07 Jun 2022 04:05:02 GMT
ADD file:6250f895d7d6c591cfe1b9fc991313d21b02167d94c67991db7c5c1c6814c51e in / 
# Tue, 07 Jun 2022 04:05:06 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:49:07 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 06:49:16 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:49:16 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 06:49:29 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 06:49:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 06:49:37 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:49:38 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 06:49:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 06:50:26 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 07 Jun 2022 06:50:26 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 07 Jun 2022 06:50:26 GMT
ARG MARIADB_VERSION=1:10.6.8+maria~focal
# Tue, 07 Jun 2022 06:50:27 GMT
ENV MARIADB_VERSION=1:10.6.8+maria~focal
# Tue, 07 Jun 2022 06:50:27 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
# Tue, 07 Jun 2022 06:50:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 06:51:01 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 06:51:14 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 06:51:14 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 06:51:14 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 07 Jun 2022 06:51:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 06:51:15 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 06:51:16 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:2f1fac119b88f55cd8329458ec27c3d6d6cb324b0fe541feacfd9a4ee621a558`  
		Last Modified: Tue, 07 Jun 2022 04:07:45 GMT  
		Size: 27.1 MB (27056020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e11bbd03dcb74b0a89181bc7b5b0c6a1081475b91f09e5b7bd4378245677d0`  
		Last Modified: Tue, 07 Jun 2022 06:54:23 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944609fc08b7430c363765f8d65b07874048d4ee4b4fddc6378410ffbf35a5e4`  
		Last Modified: Tue, 07 Jun 2022 06:54:23 GMT  
		Size: 5.4 MB (5372398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc686e965111a0f5a9fbe0d2fd56fb1cbe1f37cd32ba702e6e181eb8bd952476`  
		Last Modified: Tue, 07 Jun 2022 06:54:22 GMT  
		Size: 3.2 MB (3244071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c6b370e34d40b571955a0831c8669ab35e55a71bc048f8ad7355f3971ba4b3`  
		Last Modified: Tue, 07 Jun 2022 06:54:21 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13a21a85799843063b419b269af229d786c77820174a95c4dcc2363cee9c846`  
		Last Modified: Tue, 07 Jun 2022 06:54:21 GMT  
		Size: 2.2 MB (2183581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed1ebbc1458626d5a4732baab692192158957e9db1cb87eb1e2e23e531a49d6`  
		Last Modified: Tue, 07 Jun 2022 06:54:20 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b47aa84fc870e5c06f446069453d141adf0fa22eef7a4fe7cfb9214a24e741d`  
		Last Modified: Tue, 07 Jun 2022 06:54:47 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b635562f4bc8556889bb0f2b9f3ff626d35835290a62846421fe11a8715431c0`  
		Last Modified: Tue, 07 Jun 2022 06:55:00 GMT  
		Size: 89.5 MB (89458920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab733f3f3db269ec38e98e09601a15f589311ec121020e630991c8c53549053`  
		Last Modified: Tue, 07 Jun 2022 06:54:47 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e894f58de8cbfec950d7d9f430b4a6eb9b1c04086571f40b5bd5ef8a606ad0`  
		Last Modified: Tue, 07 Jun 2022 06:54:47 GMT  
		Size: 6.7 KB (6696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.6.8-focal`

```console
$ docker pull mariadb@sha256:6dc9418a58a9f1e7cdf01e7ce1126a4b28b55896fc0c2b54ba38695e0bdf1277
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.6.8-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:7819eec13e69628884635961a6d7f89f4572f4ea95a90b0ef978ff3a3f737bc3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.3 MB (128309365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bda4cf409ffca693506ef4fca5b613f0e01839d390f48244aca2da2de114a939`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:42:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 00:42:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:42:35 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 00:42:46 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 00:42:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 00:42:53 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:42:53 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 00:42:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 00:43:35 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 07 Jun 2022 00:43:36 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 07 Jun 2022 00:43:36 GMT
ARG MARIADB_VERSION=1:10.6.8+maria~focal
# Tue, 07 Jun 2022 00:43:36 GMT
ENV MARIADB_VERSION=1:10.6.8+maria~focal
# Tue, 07 Jun 2022 00:43:36 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
# Tue, 07 Jun 2022 00:43:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 00:43:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 00:44:00 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 00:44:00 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 00:44:00 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 07 Jun 2022 00:44:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 00:44:00 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 00:44:00 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59dcb80bbedb867b19c4eb004e84c86ae3475041d5bd11672bae9ba6be45084f`  
		Last Modified: Tue, 07 Jun 2022 00:48:53 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6c41888e0f25dece871c7e65daad879fc39d7da0a84f6b67ae0d4e1f4a6f8a`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 5.5 MB (5488991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de82bf1cd45986845f81bc71a119bf5ceaec50c145064ea58e5729f4bd6d0d22`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 3.6 MB (3585352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316c0826d235e46a7a9adcfcc3068c004818dc2611a41b69e6e7bea02316b70f`  
		Last Modified: Tue, 07 Jun 2022 00:48:51 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b82e623f5d9ed1cc04e5adc22adc6805abdba4aecc5b427aec6c31223a64dca6`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 2.3 MB (2272315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3daba1f86bc0fd099576f61e5eea0961cdefed1dc443ffb96b6a50c8f054b0b0`  
		Last Modified: Tue, 07 Jun 2022 00:48:49 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81411bfac31886b163d372c72f92b47325fe4acae247b86065df7b4a335596af`  
		Last Modified: Tue, 07 Jun 2022 00:49:18 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5393d049295a041d7d52f4b9594a8c074502691fcaf0cddc115a9a8a8bf1a400`  
		Last Modified: Tue, 07 Jun 2022 00:49:32 GMT  
		Size: 88.4 MB (88375172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46020ed440f2aed3b5607767d5f894c6d333e06d739797d7cb285998cec12736`  
		Last Modified: Tue, 07 Jun 2022 00:49:18 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed53f9923e662bb247b209f6dc8ae0610bace4a54d446630c8b04f6e5197cc8f`  
		Last Modified: Tue, 07 Jun 2022 00:49:18 GMT  
		Size: 6.7 KB (6698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6.8-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:005ec17d9c90bce79e578c244a75c1b4bcd58b6aa25cc98f862403b0f713677e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.4 MB (125350431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54532887d57dda6d4ad134dc385a8b316120b621ffe4d13b6ef9e4d97e7b67f1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:03:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:03:44 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:03:45 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:04:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:04:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:04:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:04:10 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:04:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:05:39 GMT
ARG MARIADB_MAJOR=10.6
# Sat, 30 Apr 2022 00:05:40 GMT
ENV MARIADB_MAJOR=10.6
# Mon, 23 May 2022 18:42:54 GMT
ARG MARIADB_VERSION=1:10.6.8+maria~focal
# Mon, 23 May 2022 18:42:55 GMT
ENV MARIADB_VERSION=1:10.6.8+maria~focal
# Mon, 23 May 2022 18:42:56 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
# Mon, 23 May 2022 18:42:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 23 May 2022 18:43:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 23 May 2022 18:43:20 GMT
VOLUME [/var/lib/mysql]
# Mon, 23 May 2022 18:43:21 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Mon, 23 May 2022 18:43:22 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Mon, 23 May 2022 18:43:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 18:43:23 GMT
EXPOSE 3306
# Mon, 23 May 2022 18:43:24 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932d0da437931580c9d7f118c259624e1c3ec8e81acb2acf5740d945e511ba78`  
		Last Modified: Sat, 30 Apr 2022 00:11:03 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc35c765a7328bd99273ee471b6b108980755023d4bcb1927fa7717942a9d318`  
		Last Modified: Sat, 30 Apr 2022 00:11:02 GMT  
		Size: 5.3 MB (5320183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88bae007bd9c42610e465ab436d60b2457b10b735a1bc8e5daba38f548c026`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 3.4 MB (3369899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7734d2f7be989dfe94fb891565830b8101d8e9bdbcbce8e5a7e1b1932eb3ac3c`  
		Last Modified: Sat, 30 Apr 2022 00:11:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24600bac48ce2157027e68df9e26a81754edc6f7e099c33c0a89de879dba5d9`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 2.2 MB (2202385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da05700210f681c47e021b8f3ce45f244f696854cfd656f0cd46e59cb8ca9b7d`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a04e707f9157288d2518664b72f585be74f80738c3e5d334623bd8f4dfde99b7`  
		Last Modified: Mon, 23 May 2022 18:49:06 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:779a6849160ddb2191bef8873e41d106fd7a9f05607a4711782a1f316450a46d`  
		Last Modified: Mon, 23 May 2022 18:49:20 GMT  
		Size: 87.3 MB (87273747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6601e79019448824b98ca1a7b9263ae9e6dca141455d0317eee0dffb1df8af`  
		Last Modified: Mon, 23 May 2022 18:49:06 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2580a760c284152fef0af2edafdaeebf5833c8072b08e26c6f8f00ccd339a5ee`  
		Last Modified: Mon, 23 May 2022 18:49:07 GMT  
		Size: 6.7 KB (6700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6.8-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:46627532ee7aef79d210470e90e422ac1c194ac32b54ebff10d8a8c11c3a9a95
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.0 MB (138978859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46cf570da4de5cd6bcd27f0bc1d21f601b87be375020bb793793742f69526e69`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 07 Jun 2022 05:46:02 GMT
ADD file:86506a94b834ba2b6f10dc0d1955bee539be1cf565e4ccc2c4bc074e0375f115 in / 
# Tue, 07 Jun 2022 05:46:06 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 08:57:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 08:57:48 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 08:57:54 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 08:58:44 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 08:58:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 08:59:09 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 08:59:14 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 08:59:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 09:02:12 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 07 Jun 2022 09:02:14 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 07 Jun 2022 09:02:18 GMT
ARG MARIADB_VERSION=1:10.6.8+maria~focal
# Tue, 07 Jun 2022 09:02:21 GMT
ENV MARIADB_VERSION=1:10.6.8+maria~focal
# Tue, 07 Jun 2022 09:02:23 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
# Tue, 07 Jun 2022 09:02:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 09:04:35 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 09:04:41 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 09:04:42 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 09:04:43 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 07 Jun 2022 09:04:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 09:04:46 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 09:04:49 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:3f52d061d2d3fdde0d3a099bbeae64080476c9650e9f3ba05de898d5bb5f03e8`  
		Last Modified: Tue, 07 Jun 2022 05:49:10 GMT  
		Size: 33.3 MB (33294345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b33a69d2ff59c89a297c597798ade8ea874f546d95513bd628c17fd7afda14`  
		Last Modified: Tue, 07 Jun 2022 09:17:18 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56a2c22a499e4928a88ae9201c66f507be8b9f10804ea7d0934710a6f91e5ec5`  
		Last Modified: Tue, 07 Jun 2022 09:17:18 GMT  
		Size: 6.7 MB (6667490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892b2ffb492b6d36ce25b68cf708d3c9bc9e0210e0cbbe7f575d3424c35d6b96`  
		Last Modified: Tue, 07 Jun 2022 09:17:17 GMT  
		Size: 3.7 MB (3672362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f80e77ec2bb0d7d685ca6e56f718adc6d253a98e069ebd5439f0c973194758`  
		Last Modified: Tue, 07 Jun 2022 09:17:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b0b3a9b79c49528e8e9da2d5d4954fc4e5392ee848c19c52a4d3369feb63d9`  
		Last Modified: Tue, 07 Jun 2022 09:17:16 GMT  
		Size: 2.6 MB (2568258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617e76c5eb45b560720c75ad4c60429a026cbbcb8467360cc70a7dace9ec4e5a`  
		Last Modified: Tue, 07 Jun 2022 09:17:13 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51097485d982057c87d379feafcbe1d1919349d09a239da19f742e292352da53`  
		Last Modified: Tue, 07 Jun 2022 09:17:59 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8855a4247a5c8216750c0403a57e1c7bcaa78ed396ea922681774e9528bd4e65`  
		Last Modified: Tue, 07 Jun 2022 09:18:17 GMT  
		Size: 92.8 MB (92761496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f780a8c6c967e12e3c99e28ad2bbefff751612fd54aed4740341269dcb4bb198`  
		Last Modified: Tue, 07 Jun 2022 09:17:59 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91380c084c6b0b149781eea18ec91ed28730f07a27346e830d10419cab87f7b5`  
		Last Modified: Tue, 07 Jun 2022 09:17:59 GMT  
		Size: 6.7 KB (6696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6.8-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:214f3687906b35bea0534fb4267509630eaf1c1b4b8410d0827d0981a52f0cff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.3 MB (127329897 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df253f4cc135aa64fb302a44a9849b2b620ebd4414dc60af0440b6dde07b3141`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 07 Jun 2022 04:05:02 GMT
ADD file:6250f895d7d6c591cfe1b9fc991313d21b02167d94c67991db7c5c1c6814c51e in / 
# Tue, 07 Jun 2022 04:05:06 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:49:07 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 06:49:16 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:49:16 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 06:49:29 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 06:49:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 06:49:37 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:49:38 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 06:49:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 06:50:26 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 07 Jun 2022 06:50:26 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 07 Jun 2022 06:50:26 GMT
ARG MARIADB_VERSION=1:10.6.8+maria~focal
# Tue, 07 Jun 2022 06:50:27 GMT
ENV MARIADB_VERSION=1:10.6.8+maria~focal
# Tue, 07 Jun 2022 06:50:27 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
# Tue, 07 Jun 2022 06:50:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 06:51:01 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.8/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 06:51:14 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 06:51:14 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 06:51:14 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 07 Jun 2022 06:51:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 06:51:15 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 06:51:16 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:2f1fac119b88f55cd8329458ec27c3d6d6cb324b0fe541feacfd9a4ee621a558`  
		Last Modified: Tue, 07 Jun 2022 04:07:45 GMT  
		Size: 27.1 MB (27056020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e11bbd03dcb74b0a89181bc7b5b0c6a1081475b91f09e5b7bd4378245677d0`  
		Last Modified: Tue, 07 Jun 2022 06:54:23 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944609fc08b7430c363765f8d65b07874048d4ee4b4fddc6378410ffbf35a5e4`  
		Last Modified: Tue, 07 Jun 2022 06:54:23 GMT  
		Size: 5.4 MB (5372398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc686e965111a0f5a9fbe0d2fd56fb1cbe1f37cd32ba702e6e181eb8bd952476`  
		Last Modified: Tue, 07 Jun 2022 06:54:22 GMT  
		Size: 3.2 MB (3244071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c6b370e34d40b571955a0831c8669ab35e55a71bc048f8ad7355f3971ba4b3`  
		Last Modified: Tue, 07 Jun 2022 06:54:21 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13a21a85799843063b419b269af229d786c77820174a95c4dcc2363cee9c846`  
		Last Modified: Tue, 07 Jun 2022 06:54:21 GMT  
		Size: 2.2 MB (2183581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed1ebbc1458626d5a4732baab692192158957e9db1cb87eb1e2e23e531a49d6`  
		Last Modified: Tue, 07 Jun 2022 06:54:20 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b47aa84fc870e5c06f446069453d141adf0fa22eef7a4fe7cfb9214a24e741d`  
		Last Modified: Tue, 07 Jun 2022 06:54:47 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b635562f4bc8556889bb0f2b9f3ff626d35835290a62846421fe11a8715431c0`  
		Last Modified: Tue, 07 Jun 2022 06:55:00 GMT  
		Size: 89.5 MB (89458920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab733f3f3db269ec38e98e09601a15f589311ec121020e630991c8c53549053`  
		Last Modified: Tue, 07 Jun 2022 06:54:47 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e894f58de8cbfec950d7d9f430b4a6eb9b1c04086571f40b5bd5ef8a606ad0`  
		Last Modified: Tue, 07 Jun 2022 06:54:47 GMT  
		Size: 6.7 KB (6696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.7`

```console
$ docker pull mariadb@sha256:a9f685f2d30a09cc7f1bed4071127a2a53ca35d3fb5f6bf145b94d6c7fdd154a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.7` - linux; amd64

```console
$ docker pull mariadb@sha256:063bad1f3f13ff0ab434aa51a8efc9b808bc4be4471083f6c1ba19df4c32c2bd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.8 MB (128787566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e5b7dee917c8bfbf742bebf59235e222e0af1289e5735ee18189d3066ae00b0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:42:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 00:42:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:42:35 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 00:42:46 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 00:42:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 00:42:53 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:42:53 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 00:42:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 00:42:55 GMT
ARG MARIADB_MAJOR=10.7
# Tue, 07 Jun 2022 00:42:55 GMT
ENV MARIADB_MAJOR=10.7
# Tue, 07 Jun 2022 00:42:55 GMT
ARG MARIADB_VERSION=1:10.7.4+maria~focal
# Tue, 07 Jun 2022 00:42:55 GMT
ENV MARIADB_VERSION=1:10.7.4+maria~focal
# Tue, 07 Jun 2022 00:42:55 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
# Tue, 07 Jun 2022 00:42:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 00:43:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 00:43:28 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 00:43:28 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 00:43:28 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 07 Jun 2022 00:43:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 00:43:28 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 00:43:28 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59dcb80bbedb867b19c4eb004e84c86ae3475041d5bd11672bae9ba6be45084f`  
		Last Modified: Tue, 07 Jun 2022 00:48:53 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6c41888e0f25dece871c7e65daad879fc39d7da0a84f6b67ae0d4e1f4a6f8a`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 5.5 MB (5488991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de82bf1cd45986845f81bc71a119bf5ceaec50c145064ea58e5729f4bd6d0d22`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 3.6 MB (3585352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316c0826d235e46a7a9adcfcc3068c004818dc2611a41b69e6e7bea02316b70f`  
		Last Modified: Tue, 07 Jun 2022 00:48:51 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b82e623f5d9ed1cc04e5adc22adc6805abdba4aecc5b427aec6c31223a64dca6`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 2.3 MB (2272315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3daba1f86bc0fd099576f61e5eea0961cdefed1dc443ffb96b6a50c8f054b0b0`  
		Last Modified: Tue, 07 Jun 2022 00:48:49 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e8476dc2efc09cae7593c6a3d696b8e8ee9d2b5e075927e121bc87f2f68ae1`  
		Last Modified: Tue, 07 Jun 2022 00:48:49 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2198a08f437cfafdfa1afc179a3e3e1da7b5a1dd3c24d6237188166037331d03`  
		Last Modified: Tue, 07 Jun 2022 00:49:02 GMT  
		Size: 88.9 MB (88853372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c4b1aed2f13a70811ce5115b57c8cfc2a389fb845540554697c2c557bc5cd03`  
		Last Modified: Tue, 07 Jun 2022 00:48:49 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3854f5d284b098116938d30f8452e5bd6d0efe07b08bfd262c61335935f776d7`  
		Last Modified: Tue, 07 Jun 2022 00:48:49 GMT  
		Size: 6.7 KB (6699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:8ebc0a5db16adf3c079af69d6c1bfaab3ff796f226d5bf4f48bd4097bcaa8f76
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.8 MB (125845258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ea923363e21a31355aeb311cf607458a24e7777e5802f842a6c20747597896c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:03:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:03:44 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:03:45 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:04:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:04:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:04:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:04:10 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:04:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:04:59 GMT
ARG MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 00:05:00 GMT
ENV MARIADB_MAJOR=10.7
# Mon, 23 May 2022 18:42:18 GMT
ARG MARIADB_VERSION=1:10.7.4+maria~focal
# Mon, 23 May 2022 18:42:18 GMT
ENV MARIADB_VERSION=1:10.7.4+maria~focal
# Mon, 23 May 2022 18:42:19 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
# Mon, 23 May 2022 18:42:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 23 May 2022 18:42:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 23 May 2022 18:42:43 GMT
VOLUME [/var/lib/mysql]
# Mon, 23 May 2022 18:42:45 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Mon, 23 May 2022 18:42:46 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Mon, 23 May 2022 18:42:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 18:42:47 GMT
EXPOSE 3306
# Mon, 23 May 2022 18:42:48 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932d0da437931580c9d7f118c259624e1c3ec8e81acb2acf5740d945e511ba78`  
		Last Modified: Sat, 30 Apr 2022 00:11:03 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc35c765a7328bd99273ee471b6b108980755023d4bcb1927fa7717942a9d318`  
		Last Modified: Sat, 30 Apr 2022 00:11:02 GMT  
		Size: 5.3 MB (5320183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88bae007bd9c42610e465ab436d60b2457b10b735a1bc8e5daba38f548c026`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 3.4 MB (3369899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7734d2f7be989dfe94fb891565830b8101d8e9bdbcbce8e5a7e1b1932eb3ac3c`  
		Last Modified: Sat, 30 Apr 2022 00:11:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24600bac48ce2157027e68df9e26a81754edc6f7e099c33c0a89de879dba5d9`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 2.2 MB (2202385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da05700210f681c47e021b8f3ce45f244f696854cfd656f0cd46e59cb8ca9b7d`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feec96e115e3570a3306a7f9fe5bd8ad126e034793081ed6a8a7935f0a81da36`  
		Last Modified: Mon, 23 May 2022 18:48:33 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf112c240f24966420594c548dea9f09a863a4d0bdb310880b9aed7da339b3ca`  
		Last Modified: Mon, 23 May 2022 18:48:47 GMT  
		Size: 87.8 MB (87768578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a92fe4d3412152aa6b8e9d74163065fda41b4c77227f5f9c30b5fc8d0d16f26`  
		Last Modified: Mon, 23 May 2022 18:48:33 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ce92a382f8ee5355dddd6244487ef5246bdb325dc5dddd25d55afc14fc1a54`  
		Last Modified: Mon, 23 May 2022 18:48:33 GMT  
		Size: 6.7 KB (6698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7` - linux; ppc64le

```console
$ docker pull mariadb@sha256:f0f70714b5114255e26aa78a9e83aaa4083aea06669123adc7514c62f05cfe06
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.7 MB (139693601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cefbf84ce293c6509be6031be3e13dbb9c055c60e6f8821f4e049d61667d9f6a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 07 Jun 2022 05:46:02 GMT
ADD file:86506a94b834ba2b6f10dc0d1955bee539be1cf565e4ccc2c4bc074e0375f115 in / 
# Tue, 07 Jun 2022 05:46:06 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 08:57:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 08:57:48 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 08:57:54 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 08:58:44 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 08:58:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 08:59:09 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 08:59:14 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 08:59:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 08:59:22 GMT
ARG MARIADB_MAJOR=10.7
# Tue, 07 Jun 2022 08:59:24 GMT
ENV MARIADB_MAJOR=10.7
# Tue, 07 Jun 2022 08:59:26 GMT
ARG MARIADB_VERSION=1:10.7.4+maria~focal
# Tue, 07 Jun 2022 08:59:28 GMT
ENV MARIADB_VERSION=1:10.7.4+maria~focal
# Tue, 07 Jun 2022 08:59:30 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
# Tue, 07 Jun 2022 08:59:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 09:01:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 09:01:47 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 09:01:48 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 09:01:49 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 07 Jun 2022 09:01:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 09:01:52 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 09:01:54 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:3f52d061d2d3fdde0d3a099bbeae64080476c9650e9f3ba05de898d5bb5f03e8`  
		Last Modified: Tue, 07 Jun 2022 05:49:10 GMT  
		Size: 33.3 MB (33294345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b33a69d2ff59c89a297c597798ade8ea874f546d95513bd628c17fd7afda14`  
		Last Modified: Tue, 07 Jun 2022 09:17:18 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56a2c22a499e4928a88ae9201c66f507be8b9f10804ea7d0934710a6f91e5ec5`  
		Last Modified: Tue, 07 Jun 2022 09:17:18 GMT  
		Size: 6.7 MB (6667490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892b2ffb492b6d36ce25b68cf708d3c9bc9e0210e0cbbe7f575d3424c35d6b96`  
		Last Modified: Tue, 07 Jun 2022 09:17:17 GMT  
		Size: 3.7 MB (3672362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f80e77ec2bb0d7d685ca6e56f718adc6d253a98e069ebd5439f0c973194758`  
		Last Modified: Tue, 07 Jun 2022 09:17:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b0b3a9b79c49528e8e9da2d5d4954fc4e5392ee848c19c52a4d3369feb63d9`  
		Last Modified: Tue, 07 Jun 2022 09:17:16 GMT  
		Size: 2.6 MB (2568258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617e76c5eb45b560720c75ad4c60429a026cbbcb8467360cc70a7dace9ec4e5a`  
		Last Modified: Tue, 07 Jun 2022 09:17:13 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdca053f77be7bc367cfebaa53d5d08d532c59d7867e9f8436c5651cc9c5f8ef`  
		Last Modified: Tue, 07 Jun 2022 09:17:13 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d69be38bbc5789b34366e29735d472e14e54d1b3c97313551af15f328d3fb72`  
		Last Modified: Tue, 07 Jun 2022 09:17:31 GMT  
		Size: 93.5 MB (93476234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82950130e7684751a042dd1e5177805716aafdfd4fa8ac77491c8939fe5a9c8`  
		Last Modified: Tue, 07 Jun 2022 09:17:13 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89d9db175b30507163abf1cdc26b76007778c64a4c96c18cd17eaff8824c054c`  
		Last Modified: Tue, 07 Jun 2022 09:17:13 GMT  
		Size: 6.7 KB (6699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7` - linux; s390x

```console
$ docker pull mariadb@sha256:72391e15ca5a5950d33f63a7738d6f48aae2b9636f5924d433408f7c9d29e9db
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127831817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd0821e52e397086f99ac4ad7f44c185b0f53a7d0b0f9d12c307c90ad1581ba5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 07 Jun 2022 04:05:02 GMT
ADD file:6250f895d7d6c591cfe1b9fc991313d21b02167d94c67991db7c5c1c6814c51e in / 
# Tue, 07 Jun 2022 04:05:06 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:49:07 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 06:49:16 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:49:16 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 06:49:29 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 06:49:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 06:49:37 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:49:38 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 06:49:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 06:49:40 GMT
ARG MARIADB_MAJOR=10.7
# Tue, 07 Jun 2022 06:49:40 GMT
ENV MARIADB_MAJOR=10.7
# Tue, 07 Jun 2022 06:49:40 GMT
ARG MARIADB_VERSION=1:10.7.4+maria~focal
# Tue, 07 Jun 2022 06:49:40 GMT
ENV MARIADB_VERSION=1:10.7.4+maria~focal
# Tue, 07 Jun 2022 06:49:40 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
# Tue, 07 Jun 2022 06:49:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 06:50:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 06:50:16 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 06:50:16 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 06:50:16 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 07 Jun 2022 06:50:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 06:50:17 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 06:50:17 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:2f1fac119b88f55cd8329458ec27c3d6d6cb324b0fe541feacfd9a4ee621a558`  
		Last Modified: Tue, 07 Jun 2022 04:07:45 GMT  
		Size: 27.1 MB (27056020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e11bbd03dcb74b0a89181bc7b5b0c6a1081475b91f09e5b7bd4378245677d0`  
		Last Modified: Tue, 07 Jun 2022 06:54:23 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944609fc08b7430c363765f8d65b07874048d4ee4b4fddc6378410ffbf35a5e4`  
		Last Modified: Tue, 07 Jun 2022 06:54:23 GMT  
		Size: 5.4 MB (5372398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc686e965111a0f5a9fbe0d2fd56fb1cbe1f37cd32ba702e6e181eb8bd952476`  
		Last Modified: Tue, 07 Jun 2022 06:54:22 GMT  
		Size: 3.2 MB (3244071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c6b370e34d40b571955a0831c8669ab35e55a71bc048f8ad7355f3971ba4b3`  
		Last Modified: Tue, 07 Jun 2022 06:54:21 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13a21a85799843063b419b269af229d786c77820174a95c4dcc2363cee9c846`  
		Last Modified: Tue, 07 Jun 2022 06:54:21 GMT  
		Size: 2.2 MB (2183581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed1ebbc1458626d5a4732baab692192158957e9db1cb87eb1e2e23e531a49d6`  
		Last Modified: Tue, 07 Jun 2022 06:54:20 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614db198dacca8ed6c52535c1fdbc85888ddaca6024101b2e403e3fc7c550dd3`  
		Last Modified: Tue, 07 Jun 2022 06:54:20 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112513282991ee2bec84e541f18f8fbb8961896a677c73bde70e69eea1f436e8`  
		Last Modified: Tue, 07 Jun 2022 06:54:33 GMT  
		Size: 90.0 MB (89960845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5cafa0af9b9996a5eafb36ef91ceff006096f9aa6a9fae2986ce92c8e135702`  
		Last Modified: Tue, 07 Jun 2022 06:54:20 GMT  
		Size: 3.5 KB (3487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5260a94f7c359d31abc893fee220479be3853fe10d1e5e5fd44ed934e6774551`  
		Last Modified: Tue, 07 Jun 2022 06:54:20 GMT  
		Size: 6.7 KB (6695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.7-focal`

```console
$ docker pull mariadb@sha256:a9f685f2d30a09cc7f1bed4071127a2a53ca35d3fb5f6bf145b94d6c7fdd154a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.7-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:063bad1f3f13ff0ab434aa51a8efc9b808bc4be4471083f6c1ba19df4c32c2bd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.8 MB (128787566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e5b7dee917c8bfbf742bebf59235e222e0af1289e5735ee18189d3066ae00b0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:42:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 00:42:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:42:35 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 00:42:46 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 00:42:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 00:42:53 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:42:53 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 00:42:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 00:42:55 GMT
ARG MARIADB_MAJOR=10.7
# Tue, 07 Jun 2022 00:42:55 GMT
ENV MARIADB_MAJOR=10.7
# Tue, 07 Jun 2022 00:42:55 GMT
ARG MARIADB_VERSION=1:10.7.4+maria~focal
# Tue, 07 Jun 2022 00:42:55 GMT
ENV MARIADB_VERSION=1:10.7.4+maria~focal
# Tue, 07 Jun 2022 00:42:55 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
# Tue, 07 Jun 2022 00:42:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 00:43:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 00:43:28 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 00:43:28 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 00:43:28 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 07 Jun 2022 00:43:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 00:43:28 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 00:43:28 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59dcb80bbedb867b19c4eb004e84c86ae3475041d5bd11672bae9ba6be45084f`  
		Last Modified: Tue, 07 Jun 2022 00:48:53 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6c41888e0f25dece871c7e65daad879fc39d7da0a84f6b67ae0d4e1f4a6f8a`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 5.5 MB (5488991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de82bf1cd45986845f81bc71a119bf5ceaec50c145064ea58e5729f4bd6d0d22`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 3.6 MB (3585352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316c0826d235e46a7a9adcfcc3068c004818dc2611a41b69e6e7bea02316b70f`  
		Last Modified: Tue, 07 Jun 2022 00:48:51 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b82e623f5d9ed1cc04e5adc22adc6805abdba4aecc5b427aec6c31223a64dca6`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 2.3 MB (2272315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3daba1f86bc0fd099576f61e5eea0961cdefed1dc443ffb96b6a50c8f054b0b0`  
		Last Modified: Tue, 07 Jun 2022 00:48:49 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e8476dc2efc09cae7593c6a3d696b8e8ee9d2b5e075927e121bc87f2f68ae1`  
		Last Modified: Tue, 07 Jun 2022 00:48:49 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2198a08f437cfafdfa1afc179a3e3e1da7b5a1dd3c24d6237188166037331d03`  
		Last Modified: Tue, 07 Jun 2022 00:49:02 GMT  
		Size: 88.9 MB (88853372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c4b1aed2f13a70811ce5115b57c8cfc2a389fb845540554697c2c557bc5cd03`  
		Last Modified: Tue, 07 Jun 2022 00:48:49 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3854f5d284b098116938d30f8452e5bd6d0efe07b08bfd262c61335935f776d7`  
		Last Modified: Tue, 07 Jun 2022 00:48:49 GMT  
		Size: 6.7 KB (6699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:8ebc0a5db16adf3c079af69d6c1bfaab3ff796f226d5bf4f48bd4097bcaa8f76
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.8 MB (125845258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ea923363e21a31355aeb311cf607458a24e7777e5802f842a6c20747597896c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:03:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:03:44 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:03:45 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:04:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:04:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:04:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:04:10 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:04:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:04:59 GMT
ARG MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 00:05:00 GMT
ENV MARIADB_MAJOR=10.7
# Mon, 23 May 2022 18:42:18 GMT
ARG MARIADB_VERSION=1:10.7.4+maria~focal
# Mon, 23 May 2022 18:42:18 GMT
ENV MARIADB_VERSION=1:10.7.4+maria~focal
# Mon, 23 May 2022 18:42:19 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
# Mon, 23 May 2022 18:42:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 23 May 2022 18:42:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 23 May 2022 18:42:43 GMT
VOLUME [/var/lib/mysql]
# Mon, 23 May 2022 18:42:45 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Mon, 23 May 2022 18:42:46 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Mon, 23 May 2022 18:42:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 18:42:47 GMT
EXPOSE 3306
# Mon, 23 May 2022 18:42:48 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932d0da437931580c9d7f118c259624e1c3ec8e81acb2acf5740d945e511ba78`  
		Last Modified: Sat, 30 Apr 2022 00:11:03 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc35c765a7328bd99273ee471b6b108980755023d4bcb1927fa7717942a9d318`  
		Last Modified: Sat, 30 Apr 2022 00:11:02 GMT  
		Size: 5.3 MB (5320183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88bae007bd9c42610e465ab436d60b2457b10b735a1bc8e5daba38f548c026`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 3.4 MB (3369899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7734d2f7be989dfe94fb891565830b8101d8e9bdbcbce8e5a7e1b1932eb3ac3c`  
		Last Modified: Sat, 30 Apr 2022 00:11:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24600bac48ce2157027e68df9e26a81754edc6f7e099c33c0a89de879dba5d9`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 2.2 MB (2202385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da05700210f681c47e021b8f3ce45f244f696854cfd656f0cd46e59cb8ca9b7d`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feec96e115e3570a3306a7f9fe5bd8ad126e034793081ed6a8a7935f0a81da36`  
		Last Modified: Mon, 23 May 2022 18:48:33 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf112c240f24966420594c548dea9f09a863a4d0bdb310880b9aed7da339b3ca`  
		Last Modified: Mon, 23 May 2022 18:48:47 GMT  
		Size: 87.8 MB (87768578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a92fe4d3412152aa6b8e9d74163065fda41b4c77227f5f9c30b5fc8d0d16f26`  
		Last Modified: Mon, 23 May 2022 18:48:33 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ce92a382f8ee5355dddd6244487ef5246bdb325dc5dddd25d55afc14fc1a54`  
		Last Modified: Mon, 23 May 2022 18:48:33 GMT  
		Size: 6.7 KB (6698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:f0f70714b5114255e26aa78a9e83aaa4083aea06669123adc7514c62f05cfe06
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.7 MB (139693601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cefbf84ce293c6509be6031be3e13dbb9c055c60e6f8821f4e049d61667d9f6a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 07 Jun 2022 05:46:02 GMT
ADD file:86506a94b834ba2b6f10dc0d1955bee539be1cf565e4ccc2c4bc074e0375f115 in / 
# Tue, 07 Jun 2022 05:46:06 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 08:57:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 08:57:48 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 08:57:54 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 08:58:44 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 08:58:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 08:59:09 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 08:59:14 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 08:59:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 08:59:22 GMT
ARG MARIADB_MAJOR=10.7
# Tue, 07 Jun 2022 08:59:24 GMT
ENV MARIADB_MAJOR=10.7
# Tue, 07 Jun 2022 08:59:26 GMT
ARG MARIADB_VERSION=1:10.7.4+maria~focal
# Tue, 07 Jun 2022 08:59:28 GMT
ENV MARIADB_VERSION=1:10.7.4+maria~focal
# Tue, 07 Jun 2022 08:59:30 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
# Tue, 07 Jun 2022 08:59:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 09:01:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 09:01:47 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 09:01:48 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 09:01:49 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 07 Jun 2022 09:01:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 09:01:52 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 09:01:54 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:3f52d061d2d3fdde0d3a099bbeae64080476c9650e9f3ba05de898d5bb5f03e8`  
		Last Modified: Tue, 07 Jun 2022 05:49:10 GMT  
		Size: 33.3 MB (33294345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b33a69d2ff59c89a297c597798ade8ea874f546d95513bd628c17fd7afda14`  
		Last Modified: Tue, 07 Jun 2022 09:17:18 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56a2c22a499e4928a88ae9201c66f507be8b9f10804ea7d0934710a6f91e5ec5`  
		Last Modified: Tue, 07 Jun 2022 09:17:18 GMT  
		Size: 6.7 MB (6667490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892b2ffb492b6d36ce25b68cf708d3c9bc9e0210e0cbbe7f575d3424c35d6b96`  
		Last Modified: Tue, 07 Jun 2022 09:17:17 GMT  
		Size: 3.7 MB (3672362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f80e77ec2bb0d7d685ca6e56f718adc6d253a98e069ebd5439f0c973194758`  
		Last Modified: Tue, 07 Jun 2022 09:17:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b0b3a9b79c49528e8e9da2d5d4954fc4e5392ee848c19c52a4d3369feb63d9`  
		Last Modified: Tue, 07 Jun 2022 09:17:16 GMT  
		Size: 2.6 MB (2568258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617e76c5eb45b560720c75ad4c60429a026cbbcb8467360cc70a7dace9ec4e5a`  
		Last Modified: Tue, 07 Jun 2022 09:17:13 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdca053f77be7bc367cfebaa53d5d08d532c59d7867e9f8436c5651cc9c5f8ef`  
		Last Modified: Tue, 07 Jun 2022 09:17:13 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d69be38bbc5789b34366e29735d472e14e54d1b3c97313551af15f328d3fb72`  
		Last Modified: Tue, 07 Jun 2022 09:17:31 GMT  
		Size: 93.5 MB (93476234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82950130e7684751a042dd1e5177805716aafdfd4fa8ac77491c8939fe5a9c8`  
		Last Modified: Tue, 07 Jun 2022 09:17:13 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89d9db175b30507163abf1cdc26b76007778c64a4c96c18cd17eaff8824c054c`  
		Last Modified: Tue, 07 Jun 2022 09:17:13 GMT  
		Size: 6.7 KB (6699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:72391e15ca5a5950d33f63a7738d6f48aae2b9636f5924d433408f7c9d29e9db
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127831817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd0821e52e397086f99ac4ad7f44c185b0f53a7d0b0f9d12c307c90ad1581ba5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 07 Jun 2022 04:05:02 GMT
ADD file:6250f895d7d6c591cfe1b9fc991313d21b02167d94c67991db7c5c1c6814c51e in / 
# Tue, 07 Jun 2022 04:05:06 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:49:07 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 06:49:16 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:49:16 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 06:49:29 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 06:49:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 06:49:37 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:49:38 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 06:49:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 06:49:40 GMT
ARG MARIADB_MAJOR=10.7
# Tue, 07 Jun 2022 06:49:40 GMT
ENV MARIADB_MAJOR=10.7
# Tue, 07 Jun 2022 06:49:40 GMT
ARG MARIADB_VERSION=1:10.7.4+maria~focal
# Tue, 07 Jun 2022 06:49:40 GMT
ENV MARIADB_VERSION=1:10.7.4+maria~focal
# Tue, 07 Jun 2022 06:49:40 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
# Tue, 07 Jun 2022 06:49:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 06:50:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 06:50:16 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 06:50:16 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 06:50:16 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 07 Jun 2022 06:50:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 06:50:17 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 06:50:17 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:2f1fac119b88f55cd8329458ec27c3d6d6cb324b0fe541feacfd9a4ee621a558`  
		Last Modified: Tue, 07 Jun 2022 04:07:45 GMT  
		Size: 27.1 MB (27056020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e11bbd03dcb74b0a89181bc7b5b0c6a1081475b91f09e5b7bd4378245677d0`  
		Last Modified: Tue, 07 Jun 2022 06:54:23 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944609fc08b7430c363765f8d65b07874048d4ee4b4fddc6378410ffbf35a5e4`  
		Last Modified: Tue, 07 Jun 2022 06:54:23 GMT  
		Size: 5.4 MB (5372398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc686e965111a0f5a9fbe0d2fd56fb1cbe1f37cd32ba702e6e181eb8bd952476`  
		Last Modified: Tue, 07 Jun 2022 06:54:22 GMT  
		Size: 3.2 MB (3244071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c6b370e34d40b571955a0831c8669ab35e55a71bc048f8ad7355f3971ba4b3`  
		Last Modified: Tue, 07 Jun 2022 06:54:21 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13a21a85799843063b419b269af229d786c77820174a95c4dcc2363cee9c846`  
		Last Modified: Tue, 07 Jun 2022 06:54:21 GMT  
		Size: 2.2 MB (2183581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed1ebbc1458626d5a4732baab692192158957e9db1cb87eb1e2e23e531a49d6`  
		Last Modified: Tue, 07 Jun 2022 06:54:20 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614db198dacca8ed6c52535c1fdbc85888ddaca6024101b2e403e3fc7c550dd3`  
		Last Modified: Tue, 07 Jun 2022 06:54:20 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112513282991ee2bec84e541f18f8fbb8961896a677c73bde70e69eea1f436e8`  
		Last Modified: Tue, 07 Jun 2022 06:54:33 GMT  
		Size: 90.0 MB (89960845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5cafa0af9b9996a5eafb36ef91ceff006096f9aa6a9fae2986ce92c8e135702`  
		Last Modified: Tue, 07 Jun 2022 06:54:20 GMT  
		Size: 3.5 KB (3487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5260a94f7c359d31abc893fee220479be3853fe10d1e5e5fd44ed934e6774551`  
		Last Modified: Tue, 07 Jun 2022 06:54:20 GMT  
		Size: 6.7 KB (6695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.7.4`

```console
$ docker pull mariadb@sha256:a9f685f2d30a09cc7f1bed4071127a2a53ca35d3fb5f6bf145b94d6c7fdd154a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.7.4` - linux; amd64

```console
$ docker pull mariadb@sha256:063bad1f3f13ff0ab434aa51a8efc9b808bc4be4471083f6c1ba19df4c32c2bd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.8 MB (128787566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e5b7dee917c8bfbf742bebf59235e222e0af1289e5735ee18189d3066ae00b0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:42:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 00:42:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:42:35 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 00:42:46 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 00:42:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 00:42:53 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:42:53 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 00:42:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 00:42:55 GMT
ARG MARIADB_MAJOR=10.7
# Tue, 07 Jun 2022 00:42:55 GMT
ENV MARIADB_MAJOR=10.7
# Tue, 07 Jun 2022 00:42:55 GMT
ARG MARIADB_VERSION=1:10.7.4+maria~focal
# Tue, 07 Jun 2022 00:42:55 GMT
ENV MARIADB_VERSION=1:10.7.4+maria~focal
# Tue, 07 Jun 2022 00:42:55 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
# Tue, 07 Jun 2022 00:42:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 00:43:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 00:43:28 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 00:43:28 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 00:43:28 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 07 Jun 2022 00:43:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 00:43:28 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 00:43:28 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59dcb80bbedb867b19c4eb004e84c86ae3475041d5bd11672bae9ba6be45084f`  
		Last Modified: Tue, 07 Jun 2022 00:48:53 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6c41888e0f25dece871c7e65daad879fc39d7da0a84f6b67ae0d4e1f4a6f8a`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 5.5 MB (5488991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de82bf1cd45986845f81bc71a119bf5ceaec50c145064ea58e5729f4bd6d0d22`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 3.6 MB (3585352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316c0826d235e46a7a9adcfcc3068c004818dc2611a41b69e6e7bea02316b70f`  
		Last Modified: Tue, 07 Jun 2022 00:48:51 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b82e623f5d9ed1cc04e5adc22adc6805abdba4aecc5b427aec6c31223a64dca6`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 2.3 MB (2272315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3daba1f86bc0fd099576f61e5eea0961cdefed1dc443ffb96b6a50c8f054b0b0`  
		Last Modified: Tue, 07 Jun 2022 00:48:49 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e8476dc2efc09cae7593c6a3d696b8e8ee9d2b5e075927e121bc87f2f68ae1`  
		Last Modified: Tue, 07 Jun 2022 00:48:49 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2198a08f437cfafdfa1afc179a3e3e1da7b5a1dd3c24d6237188166037331d03`  
		Last Modified: Tue, 07 Jun 2022 00:49:02 GMT  
		Size: 88.9 MB (88853372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c4b1aed2f13a70811ce5115b57c8cfc2a389fb845540554697c2c557bc5cd03`  
		Last Modified: Tue, 07 Jun 2022 00:48:49 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3854f5d284b098116938d30f8452e5bd6d0efe07b08bfd262c61335935f776d7`  
		Last Modified: Tue, 07 Jun 2022 00:48:49 GMT  
		Size: 6.7 KB (6699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7.4` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:8ebc0a5db16adf3c079af69d6c1bfaab3ff796f226d5bf4f48bd4097bcaa8f76
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.8 MB (125845258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ea923363e21a31355aeb311cf607458a24e7777e5802f842a6c20747597896c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:03:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:03:44 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:03:45 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:04:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:04:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:04:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:04:10 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:04:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:04:59 GMT
ARG MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 00:05:00 GMT
ENV MARIADB_MAJOR=10.7
# Mon, 23 May 2022 18:42:18 GMT
ARG MARIADB_VERSION=1:10.7.4+maria~focal
# Mon, 23 May 2022 18:42:18 GMT
ENV MARIADB_VERSION=1:10.7.4+maria~focal
# Mon, 23 May 2022 18:42:19 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
# Mon, 23 May 2022 18:42:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 23 May 2022 18:42:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 23 May 2022 18:42:43 GMT
VOLUME [/var/lib/mysql]
# Mon, 23 May 2022 18:42:45 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Mon, 23 May 2022 18:42:46 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Mon, 23 May 2022 18:42:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 18:42:47 GMT
EXPOSE 3306
# Mon, 23 May 2022 18:42:48 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932d0da437931580c9d7f118c259624e1c3ec8e81acb2acf5740d945e511ba78`  
		Last Modified: Sat, 30 Apr 2022 00:11:03 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc35c765a7328bd99273ee471b6b108980755023d4bcb1927fa7717942a9d318`  
		Last Modified: Sat, 30 Apr 2022 00:11:02 GMT  
		Size: 5.3 MB (5320183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88bae007bd9c42610e465ab436d60b2457b10b735a1bc8e5daba38f548c026`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 3.4 MB (3369899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7734d2f7be989dfe94fb891565830b8101d8e9bdbcbce8e5a7e1b1932eb3ac3c`  
		Last Modified: Sat, 30 Apr 2022 00:11:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24600bac48ce2157027e68df9e26a81754edc6f7e099c33c0a89de879dba5d9`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 2.2 MB (2202385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da05700210f681c47e021b8f3ce45f244f696854cfd656f0cd46e59cb8ca9b7d`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feec96e115e3570a3306a7f9fe5bd8ad126e034793081ed6a8a7935f0a81da36`  
		Last Modified: Mon, 23 May 2022 18:48:33 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf112c240f24966420594c548dea9f09a863a4d0bdb310880b9aed7da339b3ca`  
		Last Modified: Mon, 23 May 2022 18:48:47 GMT  
		Size: 87.8 MB (87768578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a92fe4d3412152aa6b8e9d74163065fda41b4c77227f5f9c30b5fc8d0d16f26`  
		Last Modified: Mon, 23 May 2022 18:48:33 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ce92a382f8ee5355dddd6244487ef5246bdb325dc5dddd25d55afc14fc1a54`  
		Last Modified: Mon, 23 May 2022 18:48:33 GMT  
		Size: 6.7 KB (6698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7.4` - linux; ppc64le

```console
$ docker pull mariadb@sha256:f0f70714b5114255e26aa78a9e83aaa4083aea06669123adc7514c62f05cfe06
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.7 MB (139693601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cefbf84ce293c6509be6031be3e13dbb9c055c60e6f8821f4e049d61667d9f6a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 07 Jun 2022 05:46:02 GMT
ADD file:86506a94b834ba2b6f10dc0d1955bee539be1cf565e4ccc2c4bc074e0375f115 in / 
# Tue, 07 Jun 2022 05:46:06 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 08:57:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 08:57:48 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 08:57:54 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 08:58:44 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 08:58:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 08:59:09 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 08:59:14 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 08:59:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 08:59:22 GMT
ARG MARIADB_MAJOR=10.7
# Tue, 07 Jun 2022 08:59:24 GMT
ENV MARIADB_MAJOR=10.7
# Tue, 07 Jun 2022 08:59:26 GMT
ARG MARIADB_VERSION=1:10.7.4+maria~focal
# Tue, 07 Jun 2022 08:59:28 GMT
ENV MARIADB_VERSION=1:10.7.4+maria~focal
# Tue, 07 Jun 2022 08:59:30 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
# Tue, 07 Jun 2022 08:59:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 09:01:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 09:01:47 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 09:01:48 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 09:01:49 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 07 Jun 2022 09:01:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 09:01:52 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 09:01:54 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:3f52d061d2d3fdde0d3a099bbeae64080476c9650e9f3ba05de898d5bb5f03e8`  
		Last Modified: Tue, 07 Jun 2022 05:49:10 GMT  
		Size: 33.3 MB (33294345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b33a69d2ff59c89a297c597798ade8ea874f546d95513bd628c17fd7afda14`  
		Last Modified: Tue, 07 Jun 2022 09:17:18 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56a2c22a499e4928a88ae9201c66f507be8b9f10804ea7d0934710a6f91e5ec5`  
		Last Modified: Tue, 07 Jun 2022 09:17:18 GMT  
		Size: 6.7 MB (6667490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892b2ffb492b6d36ce25b68cf708d3c9bc9e0210e0cbbe7f575d3424c35d6b96`  
		Last Modified: Tue, 07 Jun 2022 09:17:17 GMT  
		Size: 3.7 MB (3672362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f80e77ec2bb0d7d685ca6e56f718adc6d253a98e069ebd5439f0c973194758`  
		Last Modified: Tue, 07 Jun 2022 09:17:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b0b3a9b79c49528e8e9da2d5d4954fc4e5392ee848c19c52a4d3369feb63d9`  
		Last Modified: Tue, 07 Jun 2022 09:17:16 GMT  
		Size: 2.6 MB (2568258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617e76c5eb45b560720c75ad4c60429a026cbbcb8467360cc70a7dace9ec4e5a`  
		Last Modified: Tue, 07 Jun 2022 09:17:13 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdca053f77be7bc367cfebaa53d5d08d532c59d7867e9f8436c5651cc9c5f8ef`  
		Last Modified: Tue, 07 Jun 2022 09:17:13 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d69be38bbc5789b34366e29735d472e14e54d1b3c97313551af15f328d3fb72`  
		Last Modified: Tue, 07 Jun 2022 09:17:31 GMT  
		Size: 93.5 MB (93476234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82950130e7684751a042dd1e5177805716aafdfd4fa8ac77491c8939fe5a9c8`  
		Last Modified: Tue, 07 Jun 2022 09:17:13 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89d9db175b30507163abf1cdc26b76007778c64a4c96c18cd17eaff8824c054c`  
		Last Modified: Tue, 07 Jun 2022 09:17:13 GMT  
		Size: 6.7 KB (6699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7.4` - linux; s390x

```console
$ docker pull mariadb@sha256:72391e15ca5a5950d33f63a7738d6f48aae2b9636f5924d433408f7c9d29e9db
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127831817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd0821e52e397086f99ac4ad7f44c185b0f53a7d0b0f9d12c307c90ad1581ba5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 07 Jun 2022 04:05:02 GMT
ADD file:6250f895d7d6c591cfe1b9fc991313d21b02167d94c67991db7c5c1c6814c51e in / 
# Tue, 07 Jun 2022 04:05:06 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:49:07 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 06:49:16 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:49:16 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 06:49:29 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 06:49:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 06:49:37 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:49:38 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 06:49:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 06:49:40 GMT
ARG MARIADB_MAJOR=10.7
# Tue, 07 Jun 2022 06:49:40 GMT
ENV MARIADB_MAJOR=10.7
# Tue, 07 Jun 2022 06:49:40 GMT
ARG MARIADB_VERSION=1:10.7.4+maria~focal
# Tue, 07 Jun 2022 06:49:40 GMT
ENV MARIADB_VERSION=1:10.7.4+maria~focal
# Tue, 07 Jun 2022 06:49:40 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
# Tue, 07 Jun 2022 06:49:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 06:50:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 06:50:16 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 06:50:16 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 06:50:16 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 07 Jun 2022 06:50:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 06:50:17 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 06:50:17 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:2f1fac119b88f55cd8329458ec27c3d6d6cb324b0fe541feacfd9a4ee621a558`  
		Last Modified: Tue, 07 Jun 2022 04:07:45 GMT  
		Size: 27.1 MB (27056020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e11bbd03dcb74b0a89181bc7b5b0c6a1081475b91f09e5b7bd4378245677d0`  
		Last Modified: Tue, 07 Jun 2022 06:54:23 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944609fc08b7430c363765f8d65b07874048d4ee4b4fddc6378410ffbf35a5e4`  
		Last Modified: Tue, 07 Jun 2022 06:54:23 GMT  
		Size: 5.4 MB (5372398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc686e965111a0f5a9fbe0d2fd56fb1cbe1f37cd32ba702e6e181eb8bd952476`  
		Last Modified: Tue, 07 Jun 2022 06:54:22 GMT  
		Size: 3.2 MB (3244071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c6b370e34d40b571955a0831c8669ab35e55a71bc048f8ad7355f3971ba4b3`  
		Last Modified: Tue, 07 Jun 2022 06:54:21 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13a21a85799843063b419b269af229d786c77820174a95c4dcc2363cee9c846`  
		Last Modified: Tue, 07 Jun 2022 06:54:21 GMT  
		Size: 2.2 MB (2183581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed1ebbc1458626d5a4732baab692192158957e9db1cb87eb1e2e23e531a49d6`  
		Last Modified: Tue, 07 Jun 2022 06:54:20 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614db198dacca8ed6c52535c1fdbc85888ddaca6024101b2e403e3fc7c550dd3`  
		Last Modified: Tue, 07 Jun 2022 06:54:20 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112513282991ee2bec84e541f18f8fbb8961896a677c73bde70e69eea1f436e8`  
		Last Modified: Tue, 07 Jun 2022 06:54:33 GMT  
		Size: 90.0 MB (89960845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5cafa0af9b9996a5eafb36ef91ceff006096f9aa6a9fae2986ce92c8e135702`  
		Last Modified: Tue, 07 Jun 2022 06:54:20 GMT  
		Size: 3.5 KB (3487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5260a94f7c359d31abc893fee220479be3853fe10d1e5e5fd44ed934e6774551`  
		Last Modified: Tue, 07 Jun 2022 06:54:20 GMT  
		Size: 6.7 KB (6695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.7.4-focal`

```console
$ docker pull mariadb@sha256:a9f685f2d30a09cc7f1bed4071127a2a53ca35d3fb5f6bf145b94d6c7fdd154a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.7.4-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:063bad1f3f13ff0ab434aa51a8efc9b808bc4be4471083f6c1ba19df4c32c2bd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.8 MB (128787566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e5b7dee917c8bfbf742bebf59235e222e0af1289e5735ee18189d3066ae00b0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:42:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 00:42:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:42:35 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 00:42:46 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 00:42:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 00:42:53 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:42:53 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 00:42:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 00:42:55 GMT
ARG MARIADB_MAJOR=10.7
# Tue, 07 Jun 2022 00:42:55 GMT
ENV MARIADB_MAJOR=10.7
# Tue, 07 Jun 2022 00:42:55 GMT
ARG MARIADB_VERSION=1:10.7.4+maria~focal
# Tue, 07 Jun 2022 00:42:55 GMT
ENV MARIADB_VERSION=1:10.7.4+maria~focal
# Tue, 07 Jun 2022 00:42:55 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
# Tue, 07 Jun 2022 00:42:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 00:43:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 00:43:28 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 00:43:28 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 00:43:28 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 07 Jun 2022 00:43:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 00:43:28 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 00:43:28 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59dcb80bbedb867b19c4eb004e84c86ae3475041d5bd11672bae9ba6be45084f`  
		Last Modified: Tue, 07 Jun 2022 00:48:53 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6c41888e0f25dece871c7e65daad879fc39d7da0a84f6b67ae0d4e1f4a6f8a`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 5.5 MB (5488991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de82bf1cd45986845f81bc71a119bf5ceaec50c145064ea58e5729f4bd6d0d22`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 3.6 MB (3585352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316c0826d235e46a7a9adcfcc3068c004818dc2611a41b69e6e7bea02316b70f`  
		Last Modified: Tue, 07 Jun 2022 00:48:51 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b82e623f5d9ed1cc04e5adc22adc6805abdba4aecc5b427aec6c31223a64dca6`  
		Last Modified: Tue, 07 Jun 2022 00:48:52 GMT  
		Size: 2.3 MB (2272315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3daba1f86bc0fd099576f61e5eea0961cdefed1dc443ffb96b6a50c8f054b0b0`  
		Last Modified: Tue, 07 Jun 2022 00:48:49 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e8476dc2efc09cae7593c6a3d696b8e8ee9d2b5e075927e121bc87f2f68ae1`  
		Last Modified: Tue, 07 Jun 2022 00:48:49 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2198a08f437cfafdfa1afc179a3e3e1da7b5a1dd3c24d6237188166037331d03`  
		Last Modified: Tue, 07 Jun 2022 00:49:02 GMT  
		Size: 88.9 MB (88853372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c4b1aed2f13a70811ce5115b57c8cfc2a389fb845540554697c2c557bc5cd03`  
		Last Modified: Tue, 07 Jun 2022 00:48:49 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3854f5d284b098116938d30f8452e5bd6d0efe07b08bfd262c61335935f776d7`  
		Last Modified: Tue, 07 Jun 2022 00:48:49 GMT  
		Size: 6.7 KB (6699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7.4-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:8ebc0a5db16adf3c079af69d6c1bfaab3ff796f226d5bf4f48bd4097bcaa8f76
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.8 MB (125845258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ea923363e21a31355aeb311cf607458a24e7777e5802f842a6c20747597896c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:03:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:03:44 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:03:45 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:04:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:04:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:04:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:04:10 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:04:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:04:59 GMT
ARG MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 00:05:00 GMT
ENV MARIADB_MAJOR=10.7
# Mon, 23 May 2022 18:42:18 GMT
ARG MARIADB_VERSION=1:10.7.4+maria~focal
# Mon, 23 May 2022 18:42:18 GMT
ENV MARIADB_VERSION=1:10.7.4+maria~focal
# Mon, 23 May 2022 18:42:19 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
# Mon, 23 May 2022 18:42:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 23 May 2022 18:42:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 23 May 2022 18:42:43 GMT
VOLUME [/var/lib/mysql]
# Mon, 23 May 2022 18:42:45 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Mon, 23 May 2022 18:42:46 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Mon, 23 May 2022 18:42:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 18:42:47 GMT
EXPOSE 3306
# Mon, 23 May 2022 18:42:48 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932d0da437931580c9d7f118c259624e1c3ec8e81acb2acf5740d945e511ba78`  
		Last Modified: Sat, 30 Apr 2022 00:11:03 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc35c765a7328bd99273ee471b6b108980755023d4bcb1927fa7717942a9d318`  
		Last Modified: Sat, 30 Apr 2022 00:11:02 GMT  
		Size: 5.3 MB (5320183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88bae007bd9c42610e465ab436d60b2457b10b735a1bc8e5daba38f548c026`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 3.4 MB (3369899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7734d2f7be989dfe94fb891565830b8101d8e9bdbcbce8e5a7e1b1932eb3ac3c`  
		Last Modified: Sat, 30 Apr 2022 00:11:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24600bac48ce2157027e68df9e26a81754edc6f7e099c33c0a89de879dba5d9`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 2.2 MB (2202385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da05700210f681c47e021b8f3ce45f244f696854cfd656f0cd46e59cb8ca9b7d`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feec96e115e3570a3306a7f9fe5bd8ad126e034793081ed6a8a7935f0a81da36`  
		Last Modified: Mon, 23 May 2022 18:48:33 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf112c240f24966420594c548dea9f09a863a4d0bdb310880b9aed7da339b3ca`  
		Last Modified: Mon, 23 May 2022 18:48:47 GMT  
		Size: 87.8 MB (87768578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a92fe4d3412152aa6b8e9d74163065fda41b4c77227f5f9c30b5fc8d0d16f26`  
		Last Modified: Mon, 23 May 2022 18:48:33 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ce92a382f8ee5355dddd6244487ef5246bdb325dc5dddd25d55afc14fc1a54`  
		Last Modified: Mon, 23 May 2022 18:48:33 GMT  
		Size: 6.7 KB (6698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7.4-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:f0f70714b5114255e26aa78a9e83aaa4083aea06669123adc7514c62f05cfe06
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.7 MB (139693601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cefbf84ce293c6509be6031be3e13dbb9c055c60e6f8821f4e049d61667d9f6a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 07 Jun 2022 05:46:02 GMT
ADD file:86506a94b834ba2b6f10dc0d1955bee539be1cf565e4ccc2c4bc074e0375f115 in / 
# Tue, 07 Jun 2022 05:46:06 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 08:57:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 08:57:48 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 08:57:54 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 08:58:44 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 08:58:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 08:59:09 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 08:59:14 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 08:59:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 08:59:22 GMT
ARG MARIADB_MAJOR=10.7
# Tue, 07 Jun 2022 08:59:24 GMT
ENV MARIADB_MAJOR=10.7
# Tue, 07 Jun 2022 08:59:26 GMT
ARG MARIADB_VERSION=1:10.7.4+maria~focal
# Tue, 07 Jun 2022 08:59:28 GMT
ENV MARIADB_VERSION=1:10.7.4+maria~focal
# Tue, 07 Jun 2022 08:59:30 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
# Tue, 07 Jun 2022 08:59:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 09:01:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 09:01:47 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 09:01:48 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 09:01:49 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 07 Jun 2022 09:01:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 09:01:52 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 09:01:54 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:3f52d061d2d3fdde0d3a099bbeae64080476c9650e9f3ba05de898d5bb5f03e8`  
		Last Modified: Tue, 07 Jun 2022 05:49:10 GMT  
		Size: 33.3 MB (33294345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b33a69d2ff59c89a297c597798ade8ea874f546d95513bd628c17fd7afda14`  
		Last Modified: Tue, 07 Jun 2022 09:17:18 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56a2c22a499e4928a88ae9201c66f507be8b9f10804ea7d0934710a6f91e5ec5`  
		Last Modified: Tue, 07 Jun 2022 09:17:18 GMT  
		Size: 6.7 MB (6667490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892b2ffb492b6d36ce25b68cf708d3c9bc9e0210e0cbbe7f575d3424c35d6b96`  
		Last Modified: Tue, 07 Jun 2022 09:17:17 GMT  
		Size: 3.7 MB (3672362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f80e77ec2bb0d7d685ca6e56f718adc6d253a98e069ebd5439f0c973194758`  
		Last Modified: Tue, 07 Jun 2022 09:17:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b0b3a9b79c49528e8e9da2d5d4954fc4e5392ee848c19c52a4d3369feb63d9`  
		Last Modified: Tue, 07 Jun 2022 09:17:16 GMT  
		Size: 2.6 MB (2568258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617e76c5eb45b560720c75ad4c60429a026cbbcb8467360cc70a7dace9ec4e5a`  
		Last Modified: Tue, 07 Jun 2022 09:17:13 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdca053f77be7bc367cfebaa53d5d08d532c59d7867e9f8436c5651cc9c5f8ef`  
		Last Modified: Tue, 07 Jun 2022 09:17:13 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d69be38bbc5789b34366e29735d472e14e54d1b3c97313551af15f328d3fb72`  
		Last Modified: Tue, 07 Jun 2022 09:17:31 GMT  
		Size: 93.5 MB (93476234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82950130e7684751a042dd1e5177805716aafdfd4fa8ac77491c8939fe5a9c8`  
		Last Modified: Tue, 07 Jun 2022 09:17:13 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89d9db175b30507163abf1cdc26b76007778c64a4c96c18cd17eaff8824c054c`  
		Last Modified: Tue, 07 Jun 2022 09:17:13 GMT  
		Size: 6.7 KB (6699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7.4-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:72391e15ca5a5950d33f63a7738d6f48aae2b9636f5924d433408f7c9d29e9db
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127831817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd0821e52e397086f99ac4ad7f44c185b0f53a7d0b0f9d12c307c90ad1581ba5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 07 Jun 2022 04:05:02 GMT
ADD file:6250f895d7d6c591cfe1b9fc991313d21b02167d94c67991db7c5c1c6814c51e in / 
# Tue, 07 Jun 2022 04:05:06 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:49:07 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 06:49:16 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:49:16 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 06:49:29 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 06:49:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 06:49:37 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:49:38 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 06:49:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 06:49:40 GMT
ARG MARIADB_MAJOR=10.7
# Tue, 07 Jun 2022 06:49:40 GMT
ENV MARIADB_MAJOR=10.7
# Tue, 07 Jun 2022 06:49:40 GMT
ARG MARIADB_VERSION=1:10.7.4+maria~focal
# Tue, 07 Jun 2022 06:49:40 GMT
ENV MARIADB_VERSION=1:10.7.4+maria~focal
# Tue, 07 Jun 2022 06:49:40 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
# Tue, 07 Jun 2022 06:49:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 06:50:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.4/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 06:50:16 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 06:50:16 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 06:50:16 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 07 Jun 2022 06:50:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 06:50:17 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 06:50:17 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:2f1fac119b88f55cd8329458ec27c3d6d6cb324b0fe541feacfd9a4ee621a558`  
		Last Modified: Tue, 07 Jun 2022 04:07:45 GMT  
		Size: 27.1 MB (27056020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e11bbd03dcb74b0a89181bc7b5b0c6a1081475b91f09e5b7bd4378245677d0`  
		Last Modified: Tue, 07 Jun 2022 06:54:23 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944609fc08b7430c363765f8d65b07874048d4ee4b4fddc6378410ffbf35a5e4`  
		Last Modified: Tue, 07 Jun 2022 06:54:23 GMT  
		Size: 5.4 MB (5372398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc686e965111a0f5a9fbe0d2fd56fb1cbe1f37cd32ba702e6e181eb8bd952476`  
		Last Modified: Tue, 07 Jun 2022 06:54:22 GMT  
		Size: 3.2 MB (3244071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c6b370e34d40b571955a0831c8669ab35e55a71bc048f8ad7355f3971ba4b3`  
		Last Modified: Tue, 07 Jun 2022 06:54:21 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13a21a85799843063b419b269af229d786c77820174a95c4dcc2363cee9c846`  
		Last Modified: Tue, 07 Jun 2022 06:54:21 GMT  
		Size: 2.2 MB (2183581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed1ebbc1458626d5a4732baab692192158957e9db1cb87eb1e2e23e531a49d6`  
		Last Modified: Tue, 07 Jun 2022 06:54:20 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614db198dacca8ed6c52535c1fdbc85888ddaca6024101b2e403e3fc7c550dd3`  
		Last Modified: Tue, 07 Jun 2022 06:54:20 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112513282991ee2bec84e541f18f8fbb8961896a677c73bde70e69eea1f436e8`  
		Last Modified: Tue, 07 Jun 2022 06:54:33 GMT  
		Size: 90.0 MB (89960845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5cafa0af9b9996a5eafb36ef91ceff006096f9aa6a9fae2986ce92c8e135702`  
		Last Modified: Tue, 07 Jun 2022 06:54:20 GMT  
		Size: 3.5 KB (3487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5260a94f7c359d31abc893fee220479be3853fe10d1e5e5fd44ed934e6774551`  
		Last Modified: Tue, 07 Jun 2022 06:54:20 GMT  
		Size: 6.7 KB (6695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.8`

```console
$ docker pull mariadb@sha256:49dd7a8f3092929fb9dbc9dd10c28d1e94a7e1e031060971dab741ba7221f807
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.8` - linux; amd64

```console
$ docker pull mariadb@sha256:483a080b5bcdf0a898ef4574209080f7a42896c7134c60c55b4d4cb5ab3a8d6f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.9 MB (123859860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea81af801379dae14e596b55612f355a63cfca2ed53cf27d047340f4890cf25c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:25 GMT
ADD file:11157b07dde10107f3f6f2b892c869ea83868475d5825167b5f466a7e410eb05 in / 
# Mon, 06 Jun 2022 22:21:26 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:40:40 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 00:40:56 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:40:56 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 00:41:06 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 00:41:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 00:41:13 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:41:13 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 00:41:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 00:42:02 GMT
ARG MARIADB_MAJOR=10.8
# Tue, 07 Jun 2022 00:42:03 GMT
ENV MARIADB_MAJOR=10.8
# Tue, 07 Jun 2022 00:42:03 GMT
ARG MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 07 Jun 2022 00:42:03 GMT
ENV MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 07 Jun 2022 00:42:03 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
# Tue, 07 Jun 2022 00:42:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 00:42:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 00:42:23 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 00:42:23 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 00:42:23 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 07 Jun 2022 00:42:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 00:42:23 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 00:42:23 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:405f018f9d1d0f351c196b841a7c7f226fb8ea448acd6339a9ed8741600275a2`  
		Last Modified: Wed, 01 Jun 2022 03:03:39 GMT  
		Size: 30.4 MB (30423715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a85079b8234f1744aeed618170b84c2f6b970a320e10616ff031d3be24b5cd4`  
		Last Modified: Tue, 07 Jun 2022 00:47:43 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:579c7ff691b1abc2640eb61104ca92a223103daf11214a248cc580163536e70d`  
		Last Modified: Tue, 07 Jun 2022 00:47:42 GMT  
		Size: 3.8 MB (3765124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4976663b5d6daa78634cc56c60cb837f47e79832759e9bdb8f1c592b194411bf`  
		Last Modified: Tue, 07 Jun 2022 00:47:42 GMT  
		Size: 2.0 MB (1991845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:169024b1fb136785c2ed5f758e9707ce456f38d8007d568f863be47b0873afd7`  
		Last Modified: Tue, 07 Jun 2022 00:47:41 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ffe8ce897f6bfdab5ac2fa06b95c2a6187161ced620b3b00e71b31e7b75e47`  
		Last Modified: Tue, 07 Jun 2022 00:47:42 GMT  
		Size: 2.3 MB (2297483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b583c09d23c314a64c34258bda89aaefc6c4b3a488297892863af1dd61bb4113`  
		Last Modified: Tue, 07 Jun 2022 00:47:39 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b9f0c08d08f4ae53297606d8c0aea35c96566d2e544a8a32efb72eebc3749b6`  
		Last Modified: Tue, 07 Jun 2022 00:48:08 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cd51f98458654de3ea7c535ee562e9f9251fd6a0818629346bcadaaa768b71a`  
		Last Modified: Tue, 07 Jun 2022 00:48:20 GMT  
		Size: 85.4 MB (85366786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f506bb8acafbb672f41df13b1d99173b9217140c8137ecc9daec14c4e00f70`  
		Last Modified: Tue, 07 Jun 2022 00:48:08 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d689f79ba4ea066cd24d5c7f7ae294a524fc166bb7f9e8b60d48472f35277a`  
		Last Modified: Tue, 07 Jun 2022 00:48:08 GMT  
		Size: 6.7 KB (6699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:b6764b02b5eb8d6274207dbb827317cafc8694c1505185aa092d5551f8a793f2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.5 MB (104543896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecc004eed0c26ad5c4e0d75baff2cb4e7fdc144f713d053c256f6455b608d280`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:52 GMT
ADD file:1e18e22e32f06a7e93275cf3a2eb2a1d3892be27628bdae2de4b2aadb992bd50 in / 
# Fri, 29 Apr 2022 22:49:53 GMT
CMD ["bash"]
# Mon, 23 May 2022 18:40:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Mon, 23 May 2022 18:40:25 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 23 May 2022 18:40:26 GMT
ENV GOSU_VERSION=1.14
# Mon, 23 May 2022 18:40:43 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 23 May 2022 18:40:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 23 May 2022 18:40:53 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 23 May 2022 18:40:53 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Mon, 23 May 2022 18:40:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Mon, 23 May 2022 18:41:40 GMT
ARG MARIADB_MAJOR=10.8
# Mon, 23 May 2022 18:41:41 GMT
ENV MARIADB_MAJOR=10.8
# Mon, 23 May 2022 18:41:42 GMT
ARG MARIADB_VERSION=1:10.8.3+maria~jammy
# Mon, 23 May 2022 18:41:43 GMT
ENV MARIADB_VERSION=1:10.8.3+maria~jammy
# Mon, 23 May 2022 18:41:44 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
# Mon, 23 May 2022 18:41:45 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 23 May 2022 18:42:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 23 May 2022 18:42:04 GMT
VOLUME [/var/lib/mysql]
# Mon, 23 May 2022 18:42:06 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Mon, 23 May 2022 18:42:07 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Mon, 23 May 2022 18:42:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 18:42:08 GMT
EXPOSE 3306
# Mon, 23 May 2022 18:42:09 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:b84950154c181a602d2e93b68e84660f96dc78f94ae36f3df2db8d5701abb6a5`  
		Last Modified: Fri, 29 Apr 2022 22:52:07 GMT  
		Size: 28.4 MB (28376457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ae07faadba444656d4d080edc85dcaba97c3ac8f3ac415b136c2add7ff5393`  
		Last Modified: Mon, 23 May 2022 18:47:26 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46428e702eff2922592a3c96fbe5e3764cbca14a5a770718e36a51ad4c9dc906`  
		Last Modified: Mon, 23 May 2022 18:47:25 GMT  
		Size: 3.6 MB (3592731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e775e0ed5a0037f1c4cce3ef74f7025c80ec7e27e1e60a27c1f39d53e944c75`  
		Last Modified: Mon, 23 May 2022 18:47:25 GMT  
		Size: 4.0 MB (4014468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:031c54d0d9d9d4a999c13ba6733390868914e2c9c66b3ee2feb98e2a93de5d99`  
		Last Modified: Mon, 23 May 2022 18:47:24 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602265dc68e116e160f1e4da3863e9ff8313798a78e0d68554915d7cb1d970b9`  
		Last Modified: Mon, 23 May 2022 18:47:25 GMT  
		Size: 2.2 MB (2210433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d1d131fb6cb45f460fd0eb002edad2f1273dd1d769fff5ad071a2356a239edc`  
		Last Modified: Mon, 23 May 2022 18:47:22 GMT  
		Size: 2.5 KB (2470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a33ea1b30434b058f9b0ea3af9c9638014b6e11714eaa4888fceb806344fe49`  
		Last Modified: Mon, 23 May 2022 18:47:50 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9539c6148f07eaa2bb03fae3339771575a22824c8b4d9a6ab5cc10210d114a0c`  
		Last Modified: Mon, 23 May 2022 18:48:01 GMT  
		Size: 66.3 MB (66334981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38aa29868643c4f4f19f60129f5a981a1b09518e1621b1ffdcdf6f06c8261231`  
		Last Modified: Mon, 23 May 2022 18:47:50 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3702214dffba8174c27ba1d8d97eebb416c8b984871b3a18b8c497c26b227a77`  
		Last Modified: Mon, 23 May 2022 18:47:50 GMT  
		Size: 6.7 KB (6700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8` - linux; ppc64le

```console
$ docker pull mariadb@sha256:8b4854c6f329ab0812364a165568b8cba4d1e940e1c1241c62041f2f435c4b5b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.6 MB (139615228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1bb143b9b1f3a3b9a762e3ddbcaccba2aacae05432156b2097ff5f92be36c5f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 03:50:21 GMT
ADD file:e27da75ca1655de0ac82ef9879f868863388ea992e031aeace61195495bc21bc in / 
# Wed, 02 Feb 2022 03:50:25 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 06:07:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 06:08:34 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:08:37 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 06:09:21 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 06:09:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 06:09:52 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:09:55 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 06:10:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 25 Feb 2022 19:12:24 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 25 Feb 2022 19:12:32 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 25 Feb 2022 19:12:36 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 25 Feb 2022 19:12:40 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 25 Feb 2022 19:12:44 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 19:12:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 19:17:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 19:17:49 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 19:17:51 GMT
COPY file:f693e5845f70db80415072fbc1b9ad23eb585c105d71de03f85effee169e3220 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 19:17:52 GMT
COPY file:d5d79d09980467bc2d89c305ca6c877b5500a08d8bfc8e1accc338acff89339f in /usr/local/bin/ 
# Fri, 25 Feb 2022 19:17:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 19:18:02 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 19:18:07 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:e4ad98202983f0b602991305f807e9b8460bb3fdb617889c276ccbd4b92c69b4`  
		Last Modified: Wed, 02 Feb 2022 03:53:11 GMT  
		Size: 33.3 MB (33284717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eaa6ddf04a6d9ff5571f3581411a5c5599f359efc06218aa8d7c98b19a55901`  
		Last Modified: Wed, 02 Feb 2022 06:39:04 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ae472154410dbc918378510614e56d08dd8a080b560ff9c32dda5245513274`  
		Last Modified: Wed, 02 Feb 2022 06:39:05 GMT  
		Size: 6.7 MB (6667616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98e257a32b5e76c486ebf42a085bb256e66387304f2229a5ea755f81fd4ff043`  
		Last Modified: Wed, 02 Feb 2022 06:39:04 GMT  
		Size: 3.7 MB (3672907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4ba19c6c72ddf1ef6540af7465f5ebce217aa9ae4262681c6f8dab092d1c4f2`  
		Last Modified: Wed, 02 Feb 2022 06:39:03 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a1d4520ce5fb6b4de48cceee5ec288b0d16ed237ac7a5803a60e47a5b30485`  
		Last Modified: Wed, 02 Feb 2022 06:39:01 GMT  
		Size: 2.6 MB (2568961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e484cec9b927076854980caeef8520dfe1aa90b9caf1af6321de484c1afd41`  
		Last Modified: Wed, 02 Feb 2022 06:39:00 GMT  
		Size: 2.5 KB (2488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a14a5fccb8be7a86c2f4525978a4f9f4ec12c4668c23e02907143a1a13f41fd3`  
		Last Modified: Fri, 25 Feb 2022 19:52:19 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf158610bdc2ebfd56532e3fededc58199585a4a16fc1b7e5e714002e933f45a`  
		Last Modified: Fri, 25 Feb 2022 19:53:26 GMT  
		Size: 93.4 MB (93406255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a199944b754064fbac0e033d57b08b5ce81a70d6411b5ce343325675d9bd71b`  
		Last Modified: Fri, 25 Feb 2022 19:52:19 GMT  
		Size: 3.5 KB (3459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3184fee01c5918dfc2ec03530903011dd49caf120d5fc685f055bdd0710e51`  
		Last Modified: Fri, 25 Feb 2022 19:52:19 GMT  
		Size: 6.6 KB (6599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8` - linux; s390x

```console
$ docker pull mariadb@sha256:a9c536d0da138dacf56fd611cd76171a5e7f21b2c254495939f45200a2d2ec7e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (104950766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fad948eb6c3a1c6724e95ac01927251304a6d53ddb9014a73f6964b6092b994`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 07 Jun 2022 04:05:41 GMT
ADD file:5412b0d16961079a78b96411ca23f1838ac09c2fae839829476380b5389e49f8 in / 
# Tue, 07 Jun 2022 04:05:45 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:46:42 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 06:46:54 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:46:55 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 06:47:15 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 06:47:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 06:47:27 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:47:27 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 06:47:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 06:48:14 GMT
ARG MARIADB_MAJOR=10.8
# Tue, 07 Jun 2022 06:48:15 GMT
ENV MARIADB_MAJOR=10.8
# Tue, 07 Jun 2022 06:48:15 GMT
ARG MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 07 Jun 2022 06:48:15 GMT
ENV MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 07 Jun 2022 06:48:15 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
# Tue, 07 Jun 2022 06:48:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 06:48:49 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 06:48:56 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 06:48:56 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 06:48:56 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 07 Jun 2022 06:48:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 06:48:57 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 06:48:57 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:6fa1296f44090f6150dfb96d6ae217a58b9d66c56d7a986c35657df6bd1a89f0`  
		Last Modified: Tue, 07 Jun 2022 04:08:13 GMT  
		Size: 28.6 MB (28638482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e980d0c8e278a504f0f8cb00cbb715bc7239eb7e9e13f635db0c77b7e9625c`  
		Last Modified: Tue, 07 Jun 2022 06:53:30 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec96ea557bfa670cf2072437f6b01b817a185da1ef3e1b694d61b29c5da1561e`  
		Last Modified: Tue, 07 Jun 2022 06:53:29 GMT  
		Size: 3.7 MB (3674855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:726015530ec97a71af69b3bda1ced0b4bbdb013fc074478728335d1c714e1ed0`  
		Last Modified: Tue, 07 Jun 2022 06:53:29 GMT  
		Size: 2.0 MB (1954988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b4bef35a73fc4bcfe6311f2e5045128a3861bcd38b075463b870d13c0967b9`  
		Last Modified: Tue, 07 Jun 2022 06:53:29 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe29a6e8adabddd30630efcb94fa1700cbd3c96aa623c45d34e889d00358fc07`  
		Last Modified: Tue, 07 Jun 2022 06:53:29 GMT  
		Size: 2.2 MB (2215965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3784b0c624b488911de05f153cfb7a59247ee32628f054fc1672d59c993907b8`  
		Last Modified: Tue, 07 Jun 2022 06:53:28 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1811da06c80a8ea4d1138022303a2aee104a2e92377d041edeeea75286fc8df9`  
		Last Modified: Tue, 07 Jun 2022 06:53:50 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b002fb05e958857048b5e3de1eaf8add56ee8be42579108a53beda62649599c`  
		Last Modified: Tue, 07 Jun 2022 06:53:59 GMT  
		Size: 68.5 MB (68451571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12dfba249abcff12b977205f137dffac3b7456bee31377d44e3c935b68ae5e7`  
		Last Modified: Tue, 07 Jun 2022 06:53:50 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fecfeca76a356593a14b01d27c7d0301e7f5b59b14fe638cc7c1b2c0e3dfdeb8`  
		Last Modified: Tue, 07 Jun 2022 06:53:50 GMT  
		Size: 6.7 KB (6694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.8-jammy`

```console
$ docker pull mariadb@sha256:8be45db6728d9f755064b1553a20475120a962e49db52dff30f77c487c2da60d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mariadb:10.8-jammy` - linux; amd64

```console
$ docker pull mariadb@sha256:483a080b5bcdf0a898ef4574209080f7a42896c7134c60c55b4d4cb5ab3a8d6f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.9 MB (123859860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea81af801379dae14e596b55612f355a63cfca2ed53cf27d047340f4890cf25c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:25 GMT
ADD file:11157b07dde10107f3f6f2b892c869ea83868475d5825167b5f466a7e410eb05 in / 
# Mon, 06 Jun 2022 22:21:26 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:40:40 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 00:40:56 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:40:56 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 00:41:06 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 00:41:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 00:41:13 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:41:13 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 00:41:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 00:42:02 GMT
ARG MARIADB_MAJOR=10.8
# Tue, 07 Jun 2022 00:42:03 GMT
ENV MARIADB_MAJOR=10.8
# Tue, 07 Jun 2022 00:42:03 GMT
ARG MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 07 Jun 2022 00:42:03 GMT
ENV MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 07 Jun 2022 00:42:03 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
# Tue, 07 Jun 2022 00:42:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 00:42:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 00:42:23 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 00:42:23 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 00:42:23 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 07 Jun 2022 00:42:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 00:42:23 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 00:42:23 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:405f018f9d1d0f351c196b841a7c7f226fb8ea448acd6339a9ed8741600275a2`  
		Last Modified: Wed, 01 Jun 2022 03:03:39 GMT  
		Size: 30.4 MB (30423715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a85079b8234f1744aeed618170b84c2f6b970a320e10616ff031d3be24b5cd4`  
		Last Modified: Tue, 07 Jun 2022 00:47:43 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:579c7ff691b1abc2640eb61104ca92a223103daf11214a248cc580163536e70d`  
		Last Modified: Tue, 07 Jun 2022 00:47:42 GMT  
		Size: 3.8 MB (3765124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4976663b5d6daa78634cc56c60cb837f47e79832759e9bdb8f1c592b194411bf`  
		Last Modified: Tue, 07 Jun 2022 00:47:42 GMT  
		Size: 2.0 MB (1991845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:169024b1fb136785c2ed5f758e9707ce456f38d8007d568f863be47b0873afd7`  
		Last Modified: Tue, 07 Jun 2022 00:47:41 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ffe8ce897f6bfdab5ac2fa06b95c2a6187161ced620b3b00e71b31e7b75e47`  
		Last Modified: Tue, 07 Jun 2022 00:47:42 GMT  
		Size: 2.3 MB (2297483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b583c09d23c314a64c34258bda89aaefc6c4b3a488297892863af1dd61bb4113`  
		Last Modified: Tue, 07 Jun 2022 00:47:39 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b9f0c08d08f4ae53297606d8c0aea35c96566d2e544a8a32efb72eebc3749b6`  
		Last Modified: Tue, 07 Jun 2022 00:48:08 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cd51f98458654de3ea7c535ee562e9f9251fd6a0818629346bcadaaa768b71a`  
		Last Modified: Tue, 07 Jun 2022 00:48:20 GMT  
		Size: 85.4 MB (85366786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f506bb8acafbb672f41df13b1d99173b9217140c8137ecc9daec14c4e00f70`  
		Last Modified: Tue, 07 Jun 2022 00:48:08 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d689f79ba4ea066cd24d5c7f7ae294a524fc166bb7f9e8b60d48472f35277a`  
		Last Modified: Tue, 07 Jun 2022 00:48:08 GMT  
		Size: 6.7 KB (6699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8-jammy` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:b6764b02b5eb8d6274207dbb827317cafc8694c1505185aa092d5551f8a793f2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.5 MB (104543896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecc004eed0c26ad5c4e0d75baff2cb4e7fdc144f713d053c256f6455b608d280`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:52 GMT
ADD file:1e18e22e32f06a7e93275cf3a2eb2a1d3892be27628bdae2de4b2aadb992bd50 in / 
# Fri, 29 Apr 2022 22:49:53 GMT
CMD ["bash"]
# Mon, 23 May 2022 18:40:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Mon, 23 May 2022 18:40:25 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 23 May 2022 18:40:26 GMT
ENV GOSU_VERSION=1.14
# Mon, 23 May 2022 18:40:43 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 23 May 2022 18:40:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 23 May 2022 18:40:53 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 23 May 2022 18:40:53 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Mon, 23 May 2022 18:40:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Mon, 23 May 2022 18:41:40 GMT
ARG MARIADB_MAJOR=10.8
# Mon, 23 May 2022 18:41:41 GMT
ENV MARIADB_MAJOR=10.8
# Mon, 23 May 2022 18:41:42 GMT
ARG MARIADB_VERSION=1:10.8.3+maria~jammy
# Mon, 23 May 2022 18:41:43 GMT
ENV MARIADB_VERSION=1:10.8.3+maria~jammy
# Mon, 23 May 2022 18:41:44 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
# Mon, 23 May 2022 18:41:45 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 23 May 2022 18:42:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 23 May 2022 18:42:04 GMT
VOLUME [/var/lib/mysql]
# Mon, 23 May 2022 18:42:06 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Mon, 23 May 2022 18:42:07 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Mon, 23 May 2022 18:42:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 18:42:08 GMT
EXPOSE 3306
# Mon, 23 May 2022 18:42:09 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:b84950154c181a602d2e93b68e84660f96dc78f94ae36f3df2db8d5701abb6a5`  
		Last Modified: Fri, 29 Apr 2022 22:52:07 GMT  
		Size: 28.4 MB (28376457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ae07faadba444656d4d080edc85dcaba97c3ac8f3ac415b136c2add7ff5393`  
		Last Modified: Mon, 23 May 2022 18:47:26 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46428e702eff2922592a3c96fbe5e3764cbca14a5a770718e36a51ad4c9dc906`  
		Last Modified: Mon, 23 May 2022 18:47:25 GMT  
		Size: 3.6 MB (3592731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e775e0ed5a0037f1c4cce3ef74f7025c80ec7e27e1e60a27c1f39d53e944c75`  
		Last Modified: Mon, 23 May 2022 18:47:25 GMT  
		Size: 4.0 MB (4014468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:031c54d0d9d9d4a999c13ba6733390868914e2c9c66b3ee2feb98e2a93de5d99`  
		Last Modified: Mon, 23 May 2022 18:47:24 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602265dc68e116e160f1e4da3863e9ff8313798a78e0d68554915d7cb1d970b9`  
		Last Modified: Mon, 23 May 2022 18:47:25 GMT  
		Size: 2.2 MB (2210433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d1d131fb6cb45f460fd0eb002edad2f1273dd1d769fff5ad071a2356a239edc`  
		Last Modified: Mon, 23 May 2022 18:47:22 GMT  
		Size: 2.5 KB (2470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a33ea1b30434b058f9b0ea3af9c9638014b6e11714eaa4888fceb806344fe49`  
		Last Modified: Mon, 23 May 2022 18:47:50 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9539c6148f07eaa2bb03fae3339771575a22824c8b4d9a6ab5cc10210d114a0c`  
		Last Modified: Mon, 23 May 2022 18:48:01 GMT  
		Size: 66.3 MB (66334981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38aa29868643c4f4f19f60129f5a981a1b09518e1621b1ffdcdf6f06c8261231`  
		Last Modified: Mon, 23 May 2022 18:47:50 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3702214dffba8174c27ba1d8d97eebb416c8b984871b3a18b8c497c26b227a77`  
		Last Modified: Mon, 23 May 2022 18:47:50 GMT  
		Size: 6.7 KB (6700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8-jammy` - linux; s390x

```console
$ docker pull mariadb@sha256:a9c536d0da138dacf56fd611cd76171a5e7f21b2c254495939f45200a2d2ec7e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (104950766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fad948eb6c3a1c6724e95ac01927251304a6d53ddb9014a73f6964b6092b994`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 07 Jun 2022 04:05:41 GMT
ADD file:5412b0d16961079a78b96411ca23f1838ac09c2fae839829476380b5389e49f8 in / 
# Tue, 07 Jun 2022 04:05:45 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:46:42 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 06:46:54 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:46:55 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 06:47:15 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 06:47:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 06:47:27 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:47:27 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 06:47:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 06:48:14 GMT
ARG MARIADB_MAJOR=10.8
# Tue, 07 Jun 2022 06:48:15 GMT
ENV MARIADB_MAJOR=10.8
# Tue, 07 Jun 2022 06:48:15 GMT
ARG MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 07 Jun 2022 06:48:15 GMT
ENV MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 07 Jun 2022 06:48:15 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
# Tue, 07 Jun 2022 06:48:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 06:48:49 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 06:48:56 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 06:48:56 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 06:48:56 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 07 Jun 2022 06:48:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 06:48:57 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 06:48:57 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:6fa1296f44090f6150dfb96d6ae217a58b9d66c56d7a986c35657df6bd1a89f0`  
		Last Modified: Tue, 07 Jun 2022 04:08:13 GMT  
		Size: 28.6 MB (28638482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e980d0c8e278a504f0f8cb00cbb715bc7239eb7e9e13f635db0c77b7e9625c`  
		Last Modified: Tue, 07 Jun 2022 06:53:30 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec96ea557bfa670cf2072437f6b01b817a185da1ef3e1b694d61b29c5da1561e`  
		Last Modified: Tue, 07 Jun 2022 06:53:29 GMT  
		Size: 3.7 MB (3674855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:726015530ec97a71af69b3bda1ced0b4bbdb013fc074478728335d1c714e1ed0`  
		Last Modified: Tue, 07 Jun 2022 06:53:29 GMT  
		Size: 2.0 MB (1954988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b4bef35a73fc4bcfe6311f2e5045128a3861bcd38b075463b870d13c0967b9`  
		Last Modified: Tue, 07 Jun 2022 06:53:29 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe29a6e8adabddd30630efcb94fa1700cbd3c96aa623c45d34e889d00358fc07`  
		Last Modified: Tue, 07 Jun 2022 06:53:29 GMT  
		Size: 2.2 MB (2215965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3784b0c624b488911de05f153cfb7a59247ee32628f054fc1672d59c993907b8`  
		Last Modified: Tue, 07 Jun 2022 06:53:28 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1811da06c80a8ea4d1138022303a2aee104a2e92377d041edeeea75286fc8df9`  
		Last Modified: Tue, 07 Jun 2022 06:53:50 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b002fb05e958857048b5e3de1eaf8add56ee8be42579108a53beda62649599c`  
		Last Modified: Tue, 07 Jun 2022 06:53:59 GMT  
		Size: 68.5 MB (68451571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12dfba249abcff12b977205f137dffac3b7456bee31377d44e3c935b68ae5e7`  
		Last Modified: Tue, 07 Jun 2022 06:53:50 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fecfeca76a356593a14b01d27c7d0301e7f5b59b14fe638cc7c1b2c0e3dfdeb8`  
		Last Modified: Tue, 07 Jun 2022 06:53:50 GMT  
		Size: 6.7 KB (6694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.8.3`

```console
$ docker pull mariadb@sha256:8be45db6728d9f755064b1553a20475120a962e49db52dff30f77c487c2da60d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mariadb:10.8.3` - linux; amd64

```console
$ docker pull mariadb@sha256:483a080b5bcdf0a898ef4574209080f7a42896c7134c60c55b4d4cb5ab3a8d6f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.9 MB (123859860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea81af801379dae14e596b55612f355a63cfca2ed53cf27d047340f4890cf25c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:25 GMT
ADD file:11157b07dde10107f3f6f2b892c869ea83868475d5825167b5f466a7e410eb05 in / 
# Mon, 06 Jun 2022 22:21:26 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:40:40 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 00:40:56 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:40:56 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 00:41:06 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 00:41:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 00:41:13 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:41:13 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 00:41:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 00:42:02 GMT
ARG MARIADB_MAJOR=10.8
# Tue, 07 Jun 2022 00:42:03 GMT
ENV MARIADB_MAJOR=10.8
# Tue, 07 Jun 2022 00:42:03 GMT
ARG MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 07 Jun 2022 00:42:03 GMT
ENV MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 07 Jun 2022 00:42:03 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
# Tue, 07 Jun 2022 00:42:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 00:42:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 00:42:23 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 00:42:23 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 00:42:23 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 07 Jun 2022 00:42:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 00:42:23 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 00:42:23 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:405f018f9d1d0f351c196b841a7c7f226fb8ea448acd6339a9ed8741600275a2`  
		Last Modified: Wed, 01 Jun 2022 03:03:39 GMT  
		Size: 30.4 MB (30423715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a85079b8234f1744aeed618170b84c2f6b970a320e10616ff031d3be24b5cd4`  
		Last Modified: Tue, 07 Jun 2022 00:47:43 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:579c7ff691b1abc2640eb61104ca92a223103daf11214a248cc580163536e70d`  
		Last Modified: Tue, 07 Jun 2022 00:47:42 GMT  
		Size: 3.8 MB (3765124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4976663b5d6daa78634cc56c60cb837f47e79832759e9bdb8f1c592b194411bf`  
		Last Modified: Tue, 07 Jun 2022 00:47:42 GMT  
		Size: 2.0 MB (1991845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:169024b1fb136785c2ed5f758e9707ce456f38d8007d568f863be47b0873afd7`  
		Last Modified: Tue, 07 Jun 2022 00:47:41 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ffe8ce897f6bfdab5ac2fa06b95c2a6187161ced620b3b00e71b31e7b75e47`  
		Last Modified: Tue, 07 Jun 2022 00:47:42 GMT  
		Size: 2.3 MB (2297483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b583c09d23c314a64c34258bda89aaefc6c4b3a488297892863af1dd61bb4113`  
		Last Modified: Tue, 07 Jun 2022 00:47:39 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b9f0c08d08f4ae53297606d8c0aea35c96566d2e544a8a32efb72eebc3749b6`  
		Last Modified: Tue, 07 Jun 2022 00:48:08 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cd51f98458654de3ea7c535ee562e9f9251fd6a0818629346bcadaaa768b71a`  
		Last Modified: Tue, 07 Jun 2022 00:48:20 GMT  
		Size: 85.4 MB (85366786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f506bb8acafbb672f41df13b1d99173b9217140c8137ecc9daec14c4e00f70`  
		Last Modified: Tue, 07 Jun 2022 00:48:08 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d689f79ba4ea066cd24d5c7f7ae294a524fc166bb7f9e8b60d48472f35277a`  
		Last Modified: Tue, 07 Jun 2022 00:48:08 GMT  
		Size: 6.7 KB (6699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8.3` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:b6764b02b5eb8d6274207dbb827317cafc8694c1505185aa092d5551f8a793f2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.5 MB (104543896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecc004eed0c26ad5c4e0d75baff2cb4e7fdc144f713d053c256f6455b608d280`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:52 GMT
ADD file:1e18e22e32f06a7e93275cf3a2eb2a1d3892be27628bdae2de4b2aadb992bd50 in / 
# Fri, 29 Apr 2022 22:49:53 GMT
CMD ["bash"]
# Mon, 23 May 2022 18:40:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Mon, 23 May 2022 18:40:25 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 23 May 2022 18:40:26 GMT
ENV GOSU_VERSION=1.14
# Mon, 23 May 2022 18:40:43 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 23 May 2022 18:40:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 23 May 2022 18:40:53 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 23 May 2022 18:40:53 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Mon, 23 May 2022 18:40:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Mon, 23 May 2022 18:41:40 GMT
ARG MARIADB_MAJOR=10.8
# Mon, 23 May 2022 18:41:41 GMT
ENV MARIADB_MAJOR=10.8
# Mon, 23 May 2022 18:41:42 GMT
ARG MARIADB_VERSION=1:10.8.3+maria~jammy
# Mon, 23 May 2022 18:41:43 GMT
ENV MARIADB_VERSION=1:10.8.3+maria~jammy
# Mon, 23 May 2022 18:41:44 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
# Mon, 23 May 2022 18:41:45 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 23 May 2022 18:42:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 23 May 2022 18:42:04 GMT
VOLUME [/var/lib/mysql]
# Mon, 23 May 2022 18:42:06 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Mon, 23 May 2022 18:42:07 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Mon, 23 May 2022 18:42:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 18:42:08 GMT
EXPOSE 3306
# Mon, 23 May 2022 18:42:09 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:b84950154c181a602d2e93b68e84660f96dc78f94ae36f3df2db8d5701abb6a5`  
		Last Modified: Fri, 29 Apr 2022 22:52:07 GMT  
		Size: 28.4 MB (28376457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ae07faadba444656d4d080edc85dcaba97c3ac8f3ac415b136c2add7ff5393`  
		Last Modified: Mon, 23 May 2022 18:47:26 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46428e702eff2922592a3c96fbe5e3764cbca14a5a770718e36a51ad4c9dc906`  
		Last Modified: Mon, 23 May 2022 18:47:25 GMT  
		Size: 3.6 MB (3592731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e775e0ed5a0037f1c4cce3ef74f7025c80ec7e27e1e60a27c1f39d53e944c75`  
		Last Modified: Mon, 23 May 2022 18:47:25 GMT  
		Size: 4.0 MB (4014468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:031c54d0d9d9d4a999c13ba6733390868914e2c9c66b3ee2feb98e2a93de5d99`  
		Last Modified: Mon, 23 May 2022 18:47:24 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602265dc68e116e160f1e4da3863e9ff8313798a78e0d68554915d7cb1d970b9`  
		Last Modified: Mon, 23 May 2022 18:47:25 GMT  
		Size: 2.2 MB (2210433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d1d131fb6cb45f460fd0eb002edad2f1273dd1d769fff5ad071a2356a239edc`  
		Last Modified: Mon, 23 May 2022 18:47:22 GMT  
		Size: 2.5 KB (2470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a33ea1b30434b058f9b0ea3af9c9638014b6e11714eaa4888fceb806344fe49`  
		Last Modified: Mon, 23 May 2022 18:47:50 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9539c6148f07eaa2bb03fae3339771575a22824c8b4d9a6ab5cc10210d114a0c`  
		Last Modified: Mon, 23 May 2022 18:48:01 GMT  
		Size: 66.3 MB (66334981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38aa29868643c4f4f19f60129f5a981a1b09518e1621b1ffdcdf6f06c8261231`  
		Last Modified: Mon, 23 May 2022 18:47:50 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3702214dffba8174c27ba1d8d97eebb416c8b984871b3a18b8c497c26b227a77`  
		Last Modified: Mon, 23 May 2022 18:47:50 GMT  
		Size: 6.7 KB (6700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8.3` - linux; s390x

```console
$ docker pull mariadb@sha256:a9c536d0da138dacf56fd611cd76171a5e7f21b2c254495939f45200a2d2ec7e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (104950766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fad948eb6c3a1c6724e95ac01927251304a6d53ddb9014a73f6964b6092b994`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 07 Jun 2022 04:05:41 GMT
ADD file:5412b0d16961079a78b96411ca23f1838ac09c2fae839829476380b5389e49f8 in / 
# Tue, 07 Jun 2022 04:05:45 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:46:42 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 06:46:54 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:46:55 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 06:47:15 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 06:47:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 06:47:27 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:47:27 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 06:47:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 06:48:14 GMT
ARG MARIADB_MAJOR=10.8
# Tue, 07 Jun 2022 06:48:15 GMT
ENV MARIADB_MAJOR=10.8
# Tue, 07 Jun 2022 06:48:15 GMT
ARG MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 07 Jun 2022 06:48:15 GMT
ENV MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 07 Jun 2022 06:48:15 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
# Tue, 07 Jun 2022 06:48:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 06:48:49 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 06:48:56 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 06:48:56 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 06:48:56 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 07 Jun 2022 06:48:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 06:48:57 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 06:48:57 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:6fa1296f44090f6150dfb96d6ae217a58b9d66c56d7a986c35657df6bd1a89f0`  
		Last Modified: Tue, 07 Jun 2022 04:08:13 GMT  
		Size: 28.6 MB (28638482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e980d0c8e278a504f0f8cb00cbb715bc7239eb7e9e13f635db0c77b7e9625c`  
		Last Modified: Tue, 07 Jun 2022 06:53:30 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec96ea557bfa670cf2072437f6b01b817a185da1ef3e1b694d61b29c5da1561e`  
		Last Modified: Tue, 07 Jun 2022 06:53:29 GMT  
		Size: 3.7 MB (3674855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:726015530ec97a71af69b3bda1ced0b4bbdb013fc074478728335d1c714e1ed0`  
		Last Modified: Tue, 07 Jun 2022 06:53:29 GMT  
		Size: 2.0 MB (1954988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b4bef35a73fc4bcfe6311f2e5045128a3861bcd38b075463b870d13c0967b9`  
		Last Modified: Tue, 07 Jun 2022 06:53:29 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe29a6e8adabddd30630efcb94fa1700cbd3c96aa623c45d34e889d00358fc07`  
		Last Modified: Tue, 07 Jun 2022 06:53:29 GMT  
		Size: 2.2 MB (2215965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3784b0c624b488911de05f153cfb7a59247ee32628f054fc1672d59c993907b8`  
		Last Modified: Tue, 07 Jun 2022 06:53:28 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1811da06c80a8ea4d1138022303a2aee104a2e92377d041edeeea75286fc8df9`  
		Last Modified: Tue, 07 Jun 2022 06:53:50 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b002fb05e958857048b5e3de1eaf8add56ee8be42579108a53beda62649599c`  
		Last Modified: Tue, 07 Jun 2022 06:53:59 GMT  
		Size: 68.5 MB (68451571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12dfba249abcff12b977205f137dffac3b7456bee31377d44e3c935b68ae5e7`  
		Last Modified: Tue, 07 Jun 2022 06:53:50 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fecfeca76a356593a14b01d27c7d0301e7f5b59b14fe638cc7c1b2c0e3dfdeb8`  
		Last Modified: Tue, 07 Jun 2022 06:53:50 GMT  
		Size: 6.7 KB (6694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.8.3-jammy`

```console
$ docker pull mariadb@sha256:8be45db6728d9f755064b1553a20475120a962e49db52dff30f77c487c2da60d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mariadb:10.8.3-jammy` - linux; amd64

```console
$ docker pull mariadb@sha256:483a080b5bcdf0a898ef4574209080f7a42896c7134c60c55b4d4cb5ab3a8d6f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.9 MB (123859860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea81af801379dae14e596b55612f355a63cfca2ed53cf27d047340f4890cf25c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:25 GMT
ADD file:11157b07dde10107f3f6f2b892c869ea83868475d5825167b5f466a7e410eb05 in / 
# Mon, 06 Jun 2022 22:21:26 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:40:40 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 00:40:56 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:40:56 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 00:41:06 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 00:41:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 00:41:13 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:41:13 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 00:41:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 00:42:02 GMT
ARG MARIADB_MAJOR=10.8
# Tue, 07 Jun 2022 00:42:03 GMT
ENV MARIADB_MAJOR=10.8
# Tue, 07 Jun 2022 00:42:03 GMT
ARG MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 07 Jun 2022 00:42:03 GMT
ENV MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 07 Jun 2022 00:42:03 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
# Tue, 07 Jun 2022 00:42:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 00:42:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 00:42:23 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 00:42:23 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 00:42:23 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 07 Jun 2022 00:42:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 00:42:23 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 00:42:23 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:405f018f9d1d0f351c196b841a7c7f226fb8ea448acd6339a9ed8741600275a2`  
		Last Modified: Wed, 01 Jun 2022 03:03:39 GMT  
		Size: 30.4 MB (30423715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a85079b8234f1744aeed618170b84c2f6b970a320e10616ff031d3be24b5cd4`  
		Last Modified: Tue, 07 Jun 2022 00:47:43 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:579c7ff691b1abc2640eb61104ca92a223103daf11214a248cc580163536e70d`  
		Last Modified: Tue, 07 Jun 2022 00:47:42 GMT  
		Size: 3.8 MB (3765124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4976663b5d6daa78634cc56c60cb837f47e79832759e9bdb8f1c592b194411bf`  
		Last Modified: Tue, 07 Jun 2022 00:47:42 GMT  
		Size: 2.0 MB (1991845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:169024b1fb136785c2ed5f758e9707ce456f38d8007d568f863be47b0873afd7`  
		Last Modified: Tue, 07 Jun 2022 00:47:41 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ffe8ce897f6bfdab5ac2fa06b95c2a6187161ced620b3b00e71b31e7b75e47`  
		Last Modified: Tue, 07 Jun 2022 00:47:42 GMT  
		Size: 2.3 MB (2297483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b583c09d23c314a64c34258bda89aaefc6c4b3a488297892863af1dd61bb4113`  
		Last Modified: Tue, 07 Jun 2022 00:47:39 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b9f0c08d08f4ae53297606d8c0aea35c96566d2e544a8a32efb72eebc3749b6`  
		Last Modified: Tue, 07 Jun 2022 00:48:08 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cd51f98458654de3ea7c535ee562e9f9251fd6a0818629346bcadaaa768b71a`  
		Last Modified: Tue, 07 Jun 2022 00:48:20 GMT  
		Size: 85.4 MB (85366786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f506bb8acafbb672f41df13b1d99173b9217140c8137ecc9daec14c4e00f70`  
		Last Modified: Tue, 07 Jun 2022 00:48:08 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d689f79ba4ea066cd24d5c7f7ae294a524fc166bb7f9e8b60d48472f35277a`  
		Last Modified: Tue, 07 Jun 2022 00:48:08 GMT  
		Size: 6.7 KB (6699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8.3-jammy` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:b6764b02b5eb8d6274207dbb827317cafc8694c1505185aa092d5551f8a793f2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.5 MB (104543896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecc004eed0c26ad5c4e0d75baff2cb4e7fdc144f713d053c256f6455b608d280`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:52 GMT
ADD file:1e18e22e32f06a7e93275cf3a2eb2a1d3892be27628bdae2de4b2aadb992bd50 in / 
# Fri, 29 Apr 2022 22:49:53 GMT
CMD ["bash"]
# Mon, 23 May 2022 18:40:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Mon, 23 May 2022 18:40:25 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 23 May 2022 18:40:26 GMT
ENV GOSU_VERSION=1.14
# Mon, 23 May 2022 18:40:43 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 23 May 2022 18:40:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 23 May 2022 18:40:53 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 23 May 2022 18:40:53 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Mon, 23 May 2022 18:40:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Mon, 23 May 2022 18:41:40 GMT
ARG MARIADB_MAJOR=10.8
# Mon, 23 May 2022 18:41:41 GMT
ENV MARIADB_MAJOR=10.8
# Mon, 23 May 2022 18:41:42 GMT
ARG MARIADB_VERSION=1:10.8.3+maria~jammy
# Mon, 23 May 2022 18:41:43 GMT
ENV MARIADB_VERSION=1:10.8.3+maria~jammy
# Mon, 23 May 2022 18:41:44 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
# Mon, 23 May 2022 18:41:45 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 23 May 2022 18:42:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 23 May 2022 18:42:04 GMT
VOLUME [/var/lib/mysql]
# Mon, 23 May 2022 18:42:06 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Mon, 23 May 2022 18:42:07 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Mon, 23 May 2022 18:42:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 18:42:08 GMT
EXPOSE 3306
# Mon, 23 May 2022 18:42:09 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:b84950154c181a602d2e93b68e84660f96dc78f94ae36f3df2db8d5701abb6a5`  
		Last Modified: Fri, 29 Apr 2022 22:52:07 GMT  
		Size: 28.4 MB (28376457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ae07faadba444656d4d080edc85dcaba97c3ac8f3ac415b136c2add7ff5393`  
		Last Modified: Mon, 23 May 2022 18:47:26 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46428e702eff2922592a3c96fbe5e3764cbca14a5a770718e36a51ad4c9dc906`  
		Last Modified: Mon, 23 May 2022 18:47:25 GMT  
		Size: 3.6 MB (3592731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e775e0ed5a0037f1c4cce3ef74f7025c80ec7e27e1e60a27c1f39d53e944c75`  
		Last Modified: Mon, 23 May 2022 18:47:25 GMT  
		Size: 4.0 MB (4014468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:031c54d0d9d9d4a999c13ba6733390868914e2c9c66b3ee2feb98e2a93de5d99`  
		Last Modified: Mon, 23 May 2022 18:47:24 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602265dc68e116e160f1e4da3863e9ff8313798a78e0d68554915d7cb1d970b9`  
		Last Modified: Mon, 23 May 2022 18:47:25 GMT  
		Size: 2.2 MB (2210433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d1d131fb6cb45f460fd0eb002edad2f1273dd1d769fff5ad071a2356a239edc`  
		Last Modified: Mon, 23 May 2022 18:47:22 GMT  
		Size: 2.5 KB (2470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a33ea1b30434b058f9b0ea3af9c9638014b6e11714eaa4888fceb806344fe49`  
		Last Modified: Mon, 23 May 2022 18:47:50 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9539c6148f07eaa2bb03fae3339771575a22824c8b4d9a6ab5cc10210d114a0c`  
		Last Modified: Mon, 23 May 2022 18:48:01 GMT  
		Size: 66.3 MB (66334981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38aa29868643c4f4f19f60129f5a981a1b09518e1621b1ffdcdf6f06c8261231`  
		Last Modified: Mon, 23 May 2022 18:47:50 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3702214dffba8174c27ba1d8d97eebb416c8b984871b3a18b8c497c26b227a77`  
		Last Modified: Mon, 23 May 2022 18:47:50 GMT  
		Size: 6.7 KB (6700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8.3-jammy` - linux; s390x

```console
$ docker pull mariadb@sha256:a9c536d0da138dacf56fd611cd76171a5e7f21b2c254495939f45200a2d2ec7e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (104950766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fad948eb6c3a1c6724e95ac01927251304a6d53ddb9014a73f6964b6092b994`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 07 Jun 2022 04:05:41 GMT
ADD file:5412b0d16961079a78b96411ca23f1838ac09c2fae839829476380b5389e49f8 in / 
# Tue, 07 Jun 2022 04:05:45 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:46:42 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 06:46:54 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:46:55 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 06:47:15 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 06:47:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 06:47:27 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:47:27 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 06:47:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 06:48:14 GMT
ARG MARIADB_MAJOR=10.8
# Tue, 07 Jun 2022 06:48:15 GMT
ENV MARIADB_MAJOR=10.8
# Tue, 07 Jun 2022 06:48:15 GMT
ARG MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 07 Jun 2022 06:48:15 GMT
ENV MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 07 Jun 2022 06:48:15 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
# Tue, 07 Jun 2022 06:48:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 06:48:49 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 06:48:56 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 06:48:56 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 06:48:56 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 07 Jun 2022 06:48:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 06:48:57 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 06:48:57 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:6fa1296f44090f6150dfb96d6ae217a58b9d66c56d7a986c35657df6bd1a89f0`  
		Last Modified: Tue, 07 Jun 2022 04:08:13 GMT  
		Size: 28.6 MB (28638482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e980d0c8e278a504f0f8cb00cbb715bc7239eb7e9e13f635db0c77b7e9625c`  
		Last Modified: Tue, 07 Jun 2022 06:53:30 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec96ea557bfa670cf2072437f6b01b817a185da1ef3e1b694d61b29c5da1561e`  
		Last Modified: Tue, 07 Jun 2022 06:53:29 GMT  
		Size: 3.7 MB (3674855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:726015530ec97a71af69b3bda1ced0b4bbdb013fc074478728335d1c714e1ed0`  
		Last Modified: Tue, 07 Jun 2022 06:53:29 GMT  
		Size: 2.0 MB (1954988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b4bef35a73fc4bcfe6311f2e5045128a3861bcd38b075463b870d13c0967b9`  
		Last Modified: Tue, 07 Jun 2022 06:53:29 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe29a6e8adabddd30630efcb94fa1700cbd3c96aa623c45d34e889d00358fc07`  
		Last Modified: Tue, 07 Jun 2022 06:53:29 GMT  
		Size: 2.2 MB (2215965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3784b0c624b488911de05f153cfb7a59247ee32628f054fc1672d59c993907b8`  
		Last Modified: Tue, 07 Jun 2022 06:53:28 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1811da06c80a8ea4d1138022303a2aee104a2e92377d041edeeea75286fc8df9`  
		Last Modified: Tue, 07 Jun 2022 06:53:50 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b002fb05e958857048b5e3de1eaf8add56ee8be42579108a53beda62649599c`  
		Last Modified: Tue, 07 Jun 2022 06:53:59 GMT  
		Size: 68.5 MB (68451571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12dfba249abcff12b977205f137dffac3b7456bee31377d44e3c935b68ae5e7`  
		Last Modified: Tue, 07 Jun 2022 06:53:50 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fecfeca76a356593a14b01d27c7d0301e7f5b59b14fe638cc7c1b2c0e3dfdeb8`  
		Last Modified: Tue, 07 Jun 2022 06:53:50 GMT  
		Size: 6.7 KB (6694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.9-rc`

```console
$ docker pull mariadb@sha256:bb6ba67eed729d1bf0fc5460d8a1fdc32074af00af57db5db49822535df2e668
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mariadb:10.9-rc` - linux; amd64

```console
$ docker pull mariadb@sha256:dd4cb21a789492015492bd88fcd1b3cb5f01066f2a29394b27693ddadb350a57
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.9 MB (123936501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77fb598a35cd191ab4df137b017094f130450bb1422879aaad55ccceaf3269a4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:25 GMT
ADD file:11157b07dde10107f3f6f2b892c869ea83868475d5825167b5f466a7e410eb05 in / 
# Mon, 06 Jun 2022 22:21:26 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:40:40 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 00:40:56 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:40:56 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 00:41:06 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 00:41:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 00:41:13 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:41:13 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 00:41:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 00:41:14 GMT
ARG MARIADB_VERSION=1:10.9.1+maria~jammy
# Tue, 07 Jun 2022 00:41:14 GMT
ENV MARIADB_VERSION=1:10.9.1+maria~jammy
# Tue, 07 Jun 2022 00:41:15 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.1/repo/ubuntu/ jammy main
# Tue, 07 Jun 2022 00:41:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 00:41:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 00:41:54 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 00:41:54 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 00:41:54 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 07 Jun 2022 00:41:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 00:41:54 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 00:41:55 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:405f018f9d1d0f351c196b841a7c7f226fb8ea448acd6339a9ed8741600275a2`  
		Last Modified: Wed, 01 Jun 2022 03:03:39 GMT  
		Size: 30.4 MB (30423715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a85079b8234f1744aeed618170b84c2f6b970a320e10616ff031d3be24b5cd4`  
		Last Modified: Tue, 07 Jun 2022 00:47:43 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:579c7ff691b1abc2640eb61104ca92a223103daf11214a248cc580163536e70d`  
		Last Modified: Tue, 07 Jun 2022 00:47:42 GMT  
		Size: 3.8 MB (3765124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4976663b5d6daa78634cc56c60cb837f47e79832759e9bdb8f1c592b194411bf`  
		Last Modified: Tue, 07 Jun 2022 00:47:42 GMT  
		Size: 2.0 MB (1991845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:169024b1fb136785c2ed5f758e9707ce456f38d8007d568f863be47b0873afd7`  
		Last Modified: Tue, 07 Jun 2022 00:47:41 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ffe8ce897f6bfdab5ac2fa06b95c2a6187161ced620b3b00e71b31e7b75e47`  
		Last Modified: Tue, 07 Jun 2022 00:47:42 GMT  
		Size: 2.3 MB (2297483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b583c09d23c314a64c34258bda89aaefc6c4b3a488297892863af1dd61bb4113`  
		Last Modified: Tue, 07 Jun 2022 00:47:39 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b087a1c18065759c32e97ec3bdd17826b56e9584329a56f3b2d20ab8107fb12`  
		Last Modified: Tue, 07 Jun 2022 00:47:39 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2228bf46e3619c0bbabb8e69829d07d7d8d1d16b5325308b35ac322045ad9587`  
		Last Modified: Tue, 07 Jun 2022 00:47:51 GMT  
		Size: 85.4 MB (85443427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2bafc0c77fc31ce9c7ce1487965b647df0899aa73e7d98e1ae996edcd18fe6`  
		Last Modified: Tue, 07 Jun 2022 00:47:39 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36c033aae7e5619d18477f364b36b3a4352faf1b358cf8610459ef0d1725b2ed`  
		Last Modified: Tue, 07 Jun 2022 00:47:39 GMT  
		Size: 6.7 KB (6699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.9-rc` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:9c549fd6b1de0638cd66bb479a66b5e0f8754ff38b56f38847c4feee31c3bf87
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.6 MB (104649846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79226ff3061b39f0ab904ed5aa410a2907783a36f773e484ede8b8fa78e32289`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:52 GMT
ADD file:1e18e22e32f06a7e93275cf3a2eb2a1d3892be27628bdae2de4b2aadb992bd50 in / 
# Fri, 29 Apr 2022 22:49:53 GMT
CMD ["bash"]
# Mon, 23 May 2022 18:40:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Mon, 23 May 2022 18:40:25 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 23 May 2022 18:40:26 GMT
ENV GOSU_VERSION=1.14
# Mon, 23 May 2022 18:40:43 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 23 May 2022 18:40:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 23 May 2022 18:40:53 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 23 May 2022 18:40:53 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Mon, 23 May 2022 18:40:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Mon, 23 May 2022 18:40:56 GMT
ARG MARIADB_VERSION=1:10.9.1+maria~jammy
# Mon, 23 May 2022 18:40:57 GMT
ENV MARIADB_VERSION=1:10.9.1+maria~jammy
# Mon, 23 May 2022 18:40:58 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.1/repo/ubuntu/ jammy main
# Mon, 23 May 2022 18:40:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 23 May 2022 18:41:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 23 May 2022 18:41:19 GMT
VOLUME [/var/lib/mysql]
# Mon, 23 May 2022 18:41:20 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Mon, 23 May 2022 18:41:21 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Mon, 23 May 2022 18:41:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 18:41:22 GMT
EXPOSE 3306
# Mon, 23 May 2022 18:41:23 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:b84950154c181a602d2e93b68e84660f96dc78f94ae36f3df2db8d5701abb6a5`  
		Last Modified: Fri, 29 Apr 2022 22:52:07 GMT  
		Size: 28.4 MB (28376457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ae07faadba444656d4d080edc85dcaba97c3ac8f3ac415b136c2add7ff5393`  
		Last Modified: Mon, 23 May 2022 18:47:26 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46428e702eff2922592a3c96fbe5e3764cbca14a5a770718e36a51ad4c9dc906`  
		Last Modified: Mon, 23 May 2022 18:47:25 GMT  
		Size: 3.6 MB (3592731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e775e0ed5a0037f1c4cce3ef74f7025c80ec7e27e1e60a27c1f39d53e944c75`  
		Last Modified: Mon, 23 May 2022 18:47:25 GMT  
		Size: 4.0 MB (4014468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:031c54d0d9d9d4a999c13ba6733390868914e2c9c66b3ee2feb98e2a93de5d99`  
		Last Modified: Mon, 23 May 2022 18:47:24 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602265dc68e116e160f1e4da3863e9ff8313798a78e0d68554915d7cb1d970b9`  
		Last Modified: Mon, 23 May 2022 18:47:25 GMT  
		Size: 2.2 MB (2210433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d1d131fb6cb45f460fd0eb002edad2f1273dd1d769fff5ad071a2356a239edc`  
		Last Modified: Mon, 23 May 2022 18:47:22 GMT  
		Size: 2.5 KB (2470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a472a231b9bc32ef187c8c40f82604479c8a70ba51f185c27f08ecdacbea74`  
		Last Modified: Mon, 23 May 2022 18:47:22 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b206b9b7f2426f95ff0c1c8ab3e228ab2a6550f12fcab51fae66bce0e073028`  
		Last Modified: Mon, 23 May 2022 18:47:32 GMT  
		Size: 66.4 MB (66440929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83954d0fd1371eec503150a70054b803a3ef6d5cfdbcb6292712ecf1834b5f0a`  
		Last Modified: Mon, 23 May 2022 18:47:22 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c624ab0a5fc6c924c38bd2ec5ab26dd0f83ac9e8d0ec4aeb46590d5920fb81`  
		Last Modified: Mon, 23 May 2022 18:47:22 GMT  
		Size: 6.7 KB (6699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.9-rc` - linux; s390x

```console
$ docker pull mariadb@sha256:33538e6a86f234d1e45ae0f2c9b3f9dbfb0885fc74ca39eb91273fa2cd7fe142
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (105019606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c1caded8d0213b371f298a00ae52666860fc6794d601e88a0818002d37ce5d4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 07 Jun 2022 04:05:41 GMT
ADD file:5412b0d16961079a78b96411ca23f1838ac09c2fae839829476380b5389e49f8 in / 
# Tue, 07 Jun 2022 04:05:45 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:46:42 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 06:46:54 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:46:55 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 06:47:15 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 06:47:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 06:47:27 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:47:27 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 06:47:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 06:47:30 GMT
ARG MARIADB_VERSION=1:10.9.1+maria~jammy
# Tue, 07 Jun 2022 06:47:30 GMT
ENV MARIADB_VERSION=1:10.9.1+maria~jammy
# Tue, 07 Jun 2022 06:47:31 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.1/repo/ubuntu/ jammy main
# Tue, 07 Jun 2022 06:47:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 06:47:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 06:48:01 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 06:48:01 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 06:48:02 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 07 Jun 2022 06:48:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 06:48:02 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 06:48:03 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:6fa1296f44090f6150dfb96d6ae217a58b9d66c56d7a986c35657df6bd1a89f0`  
		Last Modified: Tue, 07 Jun 2022 04:08:13 GMT  
		Size: 28.6 MB (28638482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e980d0c8e278a504f0f8cb00cbb715bc7239eb7e9e13f635db0c77b7e9625c`  
		Last Modified: Tue, 07 Jun 2022 06:53:30 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec96ea557bfa670cf2072437f6b01b817a185da1ef3e1b694d61b29c5da1561e`  
		Last Modified: Tue, 07 Jun 2022 06:53:29 GMT  
		Size: 3.7 MB (3674855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:726015530ec97a71af69b3bda1ced0b4bbdb013fc074478728335d1c714e1ed0`  
		Last Modified: Tue, 07 Jun 2022 06:53:29 GMT  
		Size: 2.0 MB (1954988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b4bef35a73fc4bcfe6311f2e5045128a3861bcd38b075463b870d13c0967b9`  
		Last Modified: Tue, 07 Jun 2022 06:53:29 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe29a6e8adabddd30630efcb94fa1700cbd3c96aa623c45d34e889d00358fc07`  
		Last Modified: Tue, 07 Jun 2022 06:53:29 GMT  
		Size: 2.2 MB (2215965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3784b0c624b488911de05f153cfb7a59247ee32628f054fc1672d59c993907b8`  
		Last Modified: Tue, 07 Jun 2022 06:53:28 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617d10bd27641513a03c157ead3c2d8ea4197b26405ac8fddbbf567c93e87239`  
		Last Modified: Tue, 07 Jun 2022 06:53:28 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2099c5146b88e0e26d5c83a7a4265037c8d96e09287f27f4ffdacd05b55367`  
		Last Modified: Tue, 07 Jun 2022 06:53:37 GMT  
		Size: 68.5 MB (68520411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc255780d5d4f7417bcbf01460b97ff04be077b51fb95afe1f597ddb3edfe703`  
		Last Modified: Tue, 07 Jun 2022 06:53:27 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94abd9929d18abf5725866d9aec57fb93c319aa74a65aa94694e769683204ed5`  
		Last Modified: Tue, 07 Jun 2022 06:53:27 GMT  
		Size: 6.7 KB (6697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.9-rc-jammy`

```console
$ docker pull mariadb@sha256:bb6ba67eed729d1bf0fc5460d8a1fdc32074af00af57db5db49822535df2e668
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mariadb:10.9-rc-jammy` - linux; amd64

```console
$ docker pull mariadb@sha256:dd4cb21a789492015492bd88fcd1b3cb5f01066f2a29394b27693ddadb350a57
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.9 MB (123936501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77fb598a35cd191ab4df137b017094f130450bb1422879aaad55ccceaf3269a4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:25 GMT
ADD file:11157b07dde10107f3f6f2b892c869ea83868475d5825167b5f466a7e410eb05 in / 
# Mon, 06 Jun 2022 22:21:26 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:40:40 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 00:40:56 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:40:56 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 00:41:06 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 00:41:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 00:41:13 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:41:13 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 00:41:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 00:41:14 GMT
ARG MARIADB_VERSION=1:10.9.1+maria~jammy
# Tue, 07 Jun 2022 00:41:14 GMT
ENV MARIADB_VERSION=1:10.9.1+maria~jammy
# Tue, 07 Jun 2022 00:41:15 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.1/repo/ubuntu/ jammy main
# Tue, 07 Jun 2022 00:41:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 00:41:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 00:41:54 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 00:41:54 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 00:41:54 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 07 Jun 2022 00:41:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 00:41:54 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 00:41:55 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:405f018f9d1d0f351c196b841a7c7f226fb8ea448acd6339a9ed8741600275a2`  
		Last Modified: Wed, 01 Jun 2022 03:03:39 GMT  
		Size: 30.4 MB (30423715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a85079b8234f1744aeed618170b84c2f6b970a320e10616ff031d3be24b5cd4`  
		Last Modified: Tue, 07 Jun 2022 00:47:43 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:579c7ff691b1abc2640eb61104ca92a223103daf11214a248cc580163536e70d`  
		Last Modified: Tue, 07 Jun 2022 00:47:42 GMT  
		Size: 3.8 MB (3765124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4976663b5d6daa78634cc56c60cb837f47e79832759e9bdb8f1c592b194411bf`  
		Last Modified: Tue, 07 Jun 2022 00:47:42 GMT  
		Size: 2.0 MB (1991845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:169024b1fb136785c2ed5f758e9707ce456f38d8007d568f863be47b0873afd7`  
		Last Modified: Tue, 07 Jun 2022 00:47:41 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ffe8ce897f6bfdab5ac2fa06b95c2a6187161ced620b3b00e71b31e7b75e47`  
		Last Modified: Tue, 07 Jun 2022 00:47:42 GMT  
		Size: 2.3 MB (2297483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b583c09d23c314a64c34258bda89aaefc6c4b3a488297892863af1dd61bb4113`  
		Last Modified: Tue, 07 Jun 2022 00:47:39 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b087a1c18065759c32e97ec3bdd17826b56e9584329a56f3b2d20ab8107fb12`  
		Last Modified: Tue, 07 Jun 2022 00:47:39 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2228bf46e3619c0bbabb8e69829d07d7d8d1d16b5325308b35ac322045ad9587`  
		Last Modified: Tue, 07 Jun 2022 00:47:51 GMT  
		Size: 85.4 MB (85443427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2bafc0c77fc31ce9c7ce1487965b647df0899aa73e7d98e1ae996edcd18fe6`  
		Last Modified: Tue, 07 Jun 2022 00:47:39 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36c033aae7e5619d18477f364b36b3a4352faf1b358cf8610459ef0d1725b2ed`  
		Last Modified: Tue, 07 Jun 2022 00:47:39 GMT  
		Size: 6.7 KB (6699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.9-rc-jammy` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:9c549fd6b1de0638cd66bb479a66b5e0f8754ff38b56f38847c4feee31c3bf87
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.6 MB (104649846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79226ff3061b39f0ab904ed5aa410a2907783a36f773e484ede8b8fa78e32289`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:52 GMT
ADD file:1e18e22e32f06a7e93275cf3a2eb2a1d3892be27628bdae2de4b2aadb992bd50 in / 
# Fri, 29 Apr 2022 22:49:53 GMT
CMD ["bash"]
# Mon, 23 May 2022 18:40:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Mon, 23 May 2022 18:40:25 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 23 May 2022 18:40:26 GMT
ENV GOSU_VERSION=1.14
# Mon, 23 May 2022 18:40:43 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 23 May 2022 18:40:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 23 May 2022 18:40:53 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 23 May 2022 18:40:53 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Mon, 23 May 2022 18:40:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Mon, 23 May 2022 18:40:56 GMT
ARG MARIADB_VERSION=1:10.9.1+maria~jammy
# Mon, 23 May 2022 18:40:57 GMT
ENV MARIADB_VERSION=1:10.9.1+maria~jammy
# Mon, 23 May 2022 18:40:58 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.1/repo/ubuntu/ jammy main
# Mon, 23 May 2022 18:40:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 23 May 2022 18:41:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 23 May 2022 18:41:19 GMT
VOLUME [/var/lib/mysql]
# Mon, 23 May 2022 18:41:20 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Mon, 23 May 2022 18:41:21 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Mon, 23 May 2022 18:41:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 18:41:22 GMT
EXPOSE 3306
# Mon, 23 May 2022 18:41:23 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:b84950154c181a602d2e93b68e84660f96dc78f94ae36f3df2db8d5701abb6a5`  
		Last Modified: Fri, 29 Apr 2022 22:52:07 GMT  
		Size: 28.4 MB (28376457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ae07faadba444656d4d080edc85dcaba97c3ac8f3ac415b136c2add7ff5393`  
		Last Modified: Mon, 23 May 2022 18:47:26 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46428e702eff2922592a3c96fbe5e3764cbca14a5a770718e36a51ad4c9dc906`  
		Last Modified: Mon, 23 May 2022 18:47:25 GMT  
		Size: 3.6 MB (3592731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e775e0ed5a0037f1c4cce3ef74f7025c80ec7e27e1e60a27c1f39d53e944c75`  
		Last Modified: Mon, 23 May 2022 18:47:25 GMT  
		Size: 4.0 MB (4014468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:031c54d0d9d9d4a999c13ba6733390868914e2c9c66b3ee2feb98e2a93de5d99`  
		Last Modified: Mon, 23 May 2022 18:47:24 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602265dc68e116e160f1e4da3863e9ff8313798a78e0d68554915d7cb1d970b9`  
		Last Modified: Mon, 23 May 2022 18:47:25 GMT  
		Size: 2.2 MB (2210433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d1d131fb6cb45f460fd0eb002edad2f1273dd1d769fff5ad071a2356a239edc`  
		Last Modified: Mon, 23 May 2022 18:47:22 GMT  
		Size: 2.5 KB (2470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a472a231b9bc32ef187c8c40f82604479c8a70ba51f185c27f08ecdacbea74`  
		Last Modified: Mon, 23 May 2022 18:47:22 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b206b9b7f2426f95ff0c1c8ab3e228ab2a6550f12fcab51fae66bce0e073028`  
		Last Modified: Mon, 23 May 2022 18:47:32 GMT  
		Size: 66.4 MB (66440929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83954d0fd1371eec503150a70054b803a3ef6d5cfdbcb6292712ecf1834b5f0a`  
		Last Modified: Mon, 23 May 2022 18:47:22 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c624ab0a5fc6c924c38bd2ec5ab26dd0f83ac9e8d0ec4aeb46590d5920fb81`  
		Last Modified: Mon, 23 May 2022 18:47:22 GMT  
		Size: 6.7 KB (6699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.9-rc-jammy` - linux; s390x

```console
$ docker pull mariadb@sha256:33538e6a86f234d1e45ae0f2c9b3f9dbfb0885fc74ca39eb91273fa2cd7fe142
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (105019606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c1caded8d0213b371f298a00ae52666860fc6794d601e88a0818002d37ce5d4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 07 Jun 2022 04:05:41 GMT
ADD file:5412b0d16961079a78b96411ca23f1838ac09c2fae839829476380b5389e49f8 in / 
# Tue, 07 Jun 2022 04:05:45 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:46:42 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 06:46:54 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:46:55 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 06:47:15 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 06:47:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 06:47:27 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:47:27 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 06:47:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 06:47:30 GMT
ARG MARIADB_VERSION=1:10.9.1+maria~jammy
# Tue, 07 Jun 2022 06:47:30 GMT
ENV MARIADB_VERSION=1:10.9.1+maria~jammy
# Tue, 07 Jun 2022 06:47:31 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.1/repo/ubuntu/ jammy main
# Tue, 07 Jun 2022 06:47:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 06:47:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 06:48:01 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 06:48:01 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 06:48:02 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 07 Jun 2022 06:48:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 06:48:02 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 06:48:03 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:6fa1296f44090f6150dfb96d6ae217a58b9d66c56d7a986c35657df6bd1a89f0`  
		Last Modified: Tue, 07 Jun 2022 04:08:13 GMT  
		Size: 28.6 MB (28638482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e980d0c8e278a504f0f8cb00cbb715bc7239eb7e9e13f635db0c77b7e9625c`  
		Last Modified: Tue, 07 Jun 2022 06:53:30 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec96ea557bfa670cf2072437f6b01b817a185da1ef3e1b694d61b29c5da1561e`  
		Last Modified: Tue, 07 Jun 2022 06:53:29 GMT  
		Size: 3.7 MB (3674855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:726015530ec97a71af69b3bda1ced0b4bbdb013fc074478728335d1c714e1ed0`  
		Last Modified: Tue, 07 Jun 2022 06:53:29 GMT  
		Size: 2.0 MB (1954988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b4bef35a73fc4bcfe6311f2e5045128a3861bcd38b075463b870d13c0967b9`  
		Last Modified: Tue, 07 Jun 2022 06:53:29 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe29a6e8adabddd30630efcb94fa1700cbd3c96aa623c45d34e889d00358fc07`  
		Last Modified: Tue, 07 Jun 2022 06:53:29 GMT  
		Size: 2.2 MB (2215965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3784b0c624b488911de05f153cfb7a59247ee32628f054fc1672d59c993907b8`  
		Last Modified: Tue, 07 Jun 2022 06:53:28 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617d10bd27641513a03c157ead3c2d8ea4197b26405ac8fddbbf567c93e87239`  
		Last Modified: Tue, 07 Jun 2022 06:53:28 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2099c5146b88e0e26d5c83a7a4265037c8d96e09287f27f4ffdacd05b55367`  
		Last Modified: Tue, 07 Jun 2022 06:53:37 GMT  
		Size: 68.5 MB (68520411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc255780d5d4f7417bcbf01460b97ff04be077b51fb95afe1f597ddb3edfe703`  
		Last Modified: Tue, 07 Jun 2022 06:53:27 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94abd9929d18abf5725866d9aec57fb93c319aa74a65aa94694e769683204ed5`  
		Last Modified: Tue, 07 Jun 2022 06:53:27 GMT  
		Size: 6.7 KB (6697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.9.1-rc`

```console
$ docker pull mariadb@sha256:bb6ba67eed729d1bf0fc5460d8a1fdc32074af00af57db5db49822535df2e668
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mariadb:10.9.1-rc` - linux; amd64

```console
$ docker pull mariadb@sha256:dd4cb21a789492015492bd88fcd1b3cb5f01066f2a29394b27693ddadb350a57
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.9 MB (123936501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77fb598a35cd191ab4df137b017094f130450bb1422879aaad55ccceaf3269a4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:25 GMT
ADD file:11157b07dde10107f3f6f2b892c869ea83868475d5825167b5f466a7e410eb05 in / 
# Mon, 06 Jun 2022 22:21:26 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:40:40 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 00:40:56 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:40:56 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 00:41:06 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 00:41:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 00:41:13 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:41:13 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 00:41:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 00:41:14 GMT
ARG MARIADB_VERSION=1:10.9.1+maria~jammy
# Tue, 07 Jun 2022 00:41:14 GMT
ENV MARIADB_VERSION=1:10.9.1+maria~jammy
# Tue, 07 Jun 2022 00:41:15 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.1/repo/ubuntu/ jammy main
# Tue, 07 Jun 2022 00:41:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 00:41:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 00:41:54 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 00:41:54 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 00:41:54 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 07 Jun 2022 00:41:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 00:41:54 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 00:41:55 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:405f018f9d1d0f351c196b841a7c7f226fb8ea448acd6339a9ed8741600275a2`  
		Last Modified: Wed, 01 Jun 2022 03:03:39 GMT  
		Size: 30.4 MB (30423715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a85079b8234f1744aeed618170b84c2f6b970a320e10616ff031d3be24b5cd4`  
		Last Modified: Tue, 07 Jun 2022 00:47:43 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:579c7ff691b1abc2640eb61104ca92a223103daf11214a248cc580163536e70d`  
		Last Modified: Tue, 07 Jun 2022 00:47:42 GMT  
		Size: 3.8 MB (3765124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4976663b5d6daa78634cc56c60cb837f47e79832759e9bdb8f1c592b194411bf`  
		Last Modified: Tue, 07 Jun 2022 00:47:42 GMT  
		Size: 2.0 MB (1991845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:169024b1fb136785c2ed5f758e9707ce456f38d8007d568f863be47b0873afd7`  
		Last Modified: Tue, 07 Jun 2022 00:47:41 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ffe8ce897f6bfdab5ac2fa06b95c2a6187161ced620b3b00e71b31e7b75e47`  
		Last Modified: Tue, 07 Jun 2022 00:47:42 GMT  
		Size: 2.3 MB (2297483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b583c09d23c314a64c34258bda89aaefc6c4b3a488297892863af1dd61bb4113`  
		Last Modified: Tue, 07 Jun 2022 00:47:39 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b087a1c18065759c32e97ec3bdd17826b56e9584329a56f3b2d20ab8107fb12`  
		Last Modified: Tue, 07 Jun 2022 00:47:39 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2228bf46e3619c0bbabb8e69829d07d7d8d1d16b5325308b35ac322045ad9587`  
		Last Modified: Tue, 07 Jun 2022 00:47:51 GMT  
		Size: 85.4 MB (85443427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2bafc0c77fc31ce9c7ce1487965b647df0899aa73e7d98e1ae996edcd18fe6`  
		Last Modified: Tue, 07 Jun 2022 00:47:39 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36c033aae7e5619d18477f364b36b3a4352faf1b358cf8610459ef0d1725b2ed`  
		Last Modified: Tue, 07 Jun 2022 00:47:39 GMT  
		Size: 6.7 KB (6699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.9.1-rc` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:9c549fd6b1de0638cd66bb479a66b5e0f8754ff38b56f38847c4feee31c3bf87
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.6 MB (104649846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79226ff3061b39f0ab904ed5aa410a2907783a36f773e484ede8b8fa78e32289`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:52 GMT
ADD file:1e18e22e32f06a7e93275cf3a2eb2a1d3892be27628bdae2de4b2aadb992bd50 in / 
# Fri, 29 Apr 2022 22:49:53 GMT
CMD ["bash"]
# Mon, 23 May 2022 18:40:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Mon, 23 May 2022 18:40:25 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 23 May 2022 18:40:26 GMT
ENV GOSU_VERSION=1.14
# Mon, 23 May 2022 18:40:43 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 23 May 2022 18:40:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 23 May 2022 18:40:53 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 23 May 2022 18:40:53 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Mon, 23 May 2022 18:40:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Mon, 23 May 2022 18:40:56 GMT
ARG MARIADB_VERSION=1:10.9.1+maria~jammy
# Mon, 23 May 2022 18:40:57 GMT
ENV MARIADB_VERSION=1:10.9.1+maria~jammy
# Mon, 23 May 2022 18:40:58 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.1/repo/ubuntu/ jammy main
# Mon, 23 May 2022 18:40:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 23 May 2022 18:41:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 23 May 2022 18:41:19 GMT
VOLUME [/var/lib/mysql]
# Mon, 23 May 2022 18:41:20 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Mon, 23 May 2022 18:41:21 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Mon, 23 May 2022 18:41:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 18:41:22 GMT
EXPOSE 3306
# Mon, 23 May 2022 18:41:23 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:b84950154c181a602d2e93b68e84660f96dc78f94ae36f3df2db8d5701abb6a5`  
		Last Modified: Fri, 29 Apr 2022 22:52:07 GMT  
		Size: 28.4 MB (28376457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ae07faadba444656d4d080edc85dcaba97c3ac8f3ac415b136c2add7ff5393`  
		Last Modified: Mon, 23 May 2022 18:47:26 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46428e702eff2922592a3c96fbe5e3764cbca14a5a770718e36a51ad4c9dc906`  
		Last Modified: Mon, 23 May 2022 18:47:25 GMT  
		Size: 3.6 MB (3592731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e775e0ed5a0037f1c4cce3ef74f7025c80ec7e27e1e60a27c1f39d53e944c75`  
		Last Modified: Mon, 23 May 2022 18:47:25 GMT  
		Size: 4.0 MB (4014468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:031c54d0d9d9d4a999c13ba6733390868914e2c9c66b3ee2feb98e2a93de5d99`  
		Last Modified: Mon, 23 May 2022 18:47:24 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602265dc68e116e160f1e4da3863e9ff8313798a78e0d68554915d7cb1d970b9`  
		Last Modified: Mon, 23 May 2022 18:47:25 GMT  
		Size: 2.2 MB (2210433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d1d131fb6cb45f460fd0eb002edad2f1273dd1d769fff5ad071a2356a239edc`  
		Last Modified: Mon, 23 May 2022 18:47:22 GMT  
		Size: 2.5 KB (2470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a472a231b9bc32ef187c8c40f82604479c8a70ba51f185c27f08ecdacbea74`  
		Last Modified: Mon, 23 May 2022 18:47:22 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b206b9b7f2426f95ff0c1c8ab3e228ab2a6550f12fcab51fae66bce0e073028`  
		Last Modified: Mon, 23 May 2022 18:47:32 GMT  
		Size: 66.4 MB (66440929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83954d0fd1371eec503150a70054b803a3ef6d5cfdbcb6292712ecf1834b5f0a`  
		Last Modified: Mon, 23 May 2022 18:47:22 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c624ab0a5fc6c924c38bd2ec5ab26dd0f83ac9e8d0ec4aeb46590d5920fb81`  
		Last Modified: Mon, 23 May 2022 18:47:22 GMT  
		Size: 6.7 KB (6699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.9.1-rc` - linux; s390x

```console
$ docker pull mariadb@sha256:33538e6a86f234d1e45ae0f2c9b3f9dbfb0885fc74ca39eb91273fa2cd7fe142
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (105019606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c1caded8d0213b371f298a00ae52666860fc6794d601e88a0818002d37ce5d4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 07 Jun 2022 04:05:41 GMT
ADD file:5412b0d16961079a78b96411ca23f1838ac09c2fae839829476380b5389e49f8 in / 
# Tue, 07 Jun 2022 04:05:45 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:46:42 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 06:46:54 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:46:55 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 06:47:15 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 06:47:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 06:47:27 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:47:27 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 06:47:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 06:47:30 GMT
ARG MARIADB_VERSION=1:10.9.1+maria~jammy
# Tue, 07 Jun 2022 06:47:30 GMT
ENV MARIADB_VERSION=1:10.9.1+maria~jammy
# Tue, 07 Jun 2022 06:47:31 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.1/repo/ubuntu/ jammy main
# Tue, 07 Jun 2022 06:47:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 06:47:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 06:48:01 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 06:48:01 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 06:48:02 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 07 Jun 2022 06:48:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 06:48:02 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 06:48:03 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:6fa1296f44090f6150dfb96d6ae217a58b9d66c56d7a986c35657df6bd1a89f0`  
		Last Modified: Tue, 07 Jun 2022 04:08:13 GMT  
		Size: 28.6 MB (28638482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e980d0c8e278a504f0f8cb00cbb715bc7239eb7e9e13f635db0c77b7e9625c`  
		Last Modified: Tue, 07 Jun 2022 06:53:30 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec96ea557bfa670cf2072437f6b01b817a185da1ef3e1b694d61b29c5da1561e`  
		Last Modified: Tue, 07 Jun 2022 06:53:29 GMT  
		Size: 3.7 MB (3674855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:726015530ec97a71af69b3bda1ced0b4bbdb013fc074478728335d1c714e1ed0`  
		Last Modified: Tue, 07 Jun 2022 06:53:29 GMT  
		Size: 2.0 MB (1954988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b4bef35a73fc4bcfe6311f2e5045128a3861bcd38b075463b870d13c0967b9`  
		Last Modified: Tue, 07 Jun 2022 06:53:29 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe29a6e8adabddd30630efcb94fa1700cbd3c96aa623c45d34e889d00358fc07`  
		Last Modified: Tue, 07 Jun 2022 06:53:29 GMT  
		Size: 2.2 MB (2215965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3784b0c624b488911de05f153cfb7a59247ee32628f054fc1672d59c993907b8`  
		Last Modified: Tue, 07 Jun 2022 06:53:28 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617d10bd27641513a03c157ead3c2d8ea4197b26405ac8fddbbf567c93e87239`  
		Last Modified: Tue, 07 Jun 2022 06:53:28 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2099c5146b88e0e26d5c83a7a4265037c8d96e09287f27f4ffdacd05b55367`  
		Last Modified: Tue, 07 Jun 2022 06:53:37 GMT  
		Size: 68.5 MB (68520411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc255780d5d4f7417bcbf01460b97ff04be077b51fb95afe1f597ddb3edfe703`  
		Last Modified: Tue, 07 Jun 2022 06:53:27 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94abd9929d18abf5725866d9aec57fb93c319aa74a65aa94694e769683204ed5`  
		Last Modified: Tue, 07 Jun 2022 06:53:27 GMT  
		Size: 6.7 KB (6697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.9.1-rc-jammy`

```console
$ docker pull mariadb@sha256:bb6ba67eed729d1bf0fc5460d8a1fdc32074af00af57db5db49822535df2e668
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mariadb:10.9.1-rc-jammy` - linux; amd64

```console
$ docker pull mariadb@sha256:dd4cb21a789492015492bd88fcd1b3cb5f01066f2a29394b27693ddadb350a57
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.9 MB (123936501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77fb598a35cd191ab4df137b017094f130450bb1422879aaad55ccceaf3269a4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:25 GMT
ADD file:11157b07dde10107f3f6f2b892c869ea83868475d5825167b5f466a7e410eb05 in / 
# Mon, 06 Jun 2022 22:21:26 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:40:40 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 00:40:56 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:40:56 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 00:41:06 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 00:41:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 00:41:13 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:41:13 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 00:41:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 00:41:14 GMT
ARG MARIADB_VERSION=1:10.9.1+maria~jammy
# Tue, 07 Jun 2022 00:41:14 GMT
ENV MARIADB_VERSION=1:10.9.1+maria~jammy
# Tue, 07 Jun 2022 00:41:15 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.1/repo/ubuntu/ jammy main
# Tue, 07 Jun 2022 00:41:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 00:41:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 00:41:54 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 00:41:54 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 00:41:54 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 07 Jun 2022 00:41:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 00:41:54 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 00:41:55 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:405f018f9d1d0f351c196b841a7c7f226fb8ea448acd6339a9ed8741600275a2`  
		Last Modified: Wed, 01 Jun 2022 03:03:39 GMT  
		Size: 30.4 MB (30423715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a85079b8234f1744aeed618170b84c2f6b970a320e10616ff031d3be24b5cd4`  
		Last Modified: Tue, 07 Jun 2022 00:47:43 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:579c7ff691b1abc2640eb61104ca92a223103daf11214a248cc580163536e70d`  
		Last Modified: Tue, 07 Jun 2022 00:47:42 GMT  
		Size: 3.8 MB (3765124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4976663b5d6daa78634cc56c60cb837f47e79832759e9bdb8f1c592b194411bf`  
		Last Modified: Tue, 07 Jun 2022 00:47:42 GMT  
		Size: 2.0 MB (1991845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:169024b1fb136785c2ed5f758e9707ce456f38d8007d568f863be47b0873afd7`  
		Last Modified: Tue, 07 Jun 2022 00:47:41 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ffe8ce897f6bfdab5ac2fa06b95c2a6187161ced620b3b00e71b31e7b75e47`  
		Last Modified: Tue, 07 Jun 2022 00:47:42 GMT  
		Size: 2.3 MB (2297483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b583c09d23c314a64c34258bda89aaefc6c4b3a488297892863af1dd61bb4113`  
		Last Modified: Tue, 07 Jun 2022 00:47:39 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b087a1c18065759c32e97ec3bdd17826b56e9584329a56f3b2d20ab8107fb12`  
		Last Modified: Tue, 07 Jun 2022 00:47:39 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2228bf46e3619c0bbabb8e69829d07d7d8d1d16b5325308b35ac322045ad9587`  
		Last Modified: Tue, 07 Jun 2022 00:47:51 GMT  
		Size: 85.4 MB (85443427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2bafc0c77fc31ce9c7ce1487965b647df0899aa73e7d98e1ae996edcd18fe6`  
		Last Modified: Tue, 07 Jun 2022 00:47:39 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36c033aae7e5619d18477f364b36b3a4352faf1b358cf8610459ef0d1725b2ed`  
		Last Modified: Tue, 07 Jun 2022 00:47:39 GMT  
		Size: 6.7 KB (6699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.9.1-rc-jammy` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:9c549fd6b1de0638cd66bb479a66b5e0f8754ff38b56f38847c4feee31c3bf87
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.6 MB (104649846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79226ff3061b39f0ab904ed5aa410a2907783a36f773e484ede8b8fa78e32289`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:52 GMT
ADD file:1e18e22e32f06a7e93275cf3a2eb2a1d3892be27628bdae2de4b2aadb992bd50 in / 
# Fri, 29 Apr 2022 22:49:53 GMT
CMD ["bash"]
# Mon, 23 May 2022 18:40:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Mon, 23 May 2022 18:40:25 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 23 May 2022 18:40:26 GMT
ENV GOSU_VERSION=1.14
# Mon, 23 May 2022 18:40:43 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 23 May 2022 18:40:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 23 May 2022 18:40:53 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 23 May 2022 18:40:53 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Mon, 23 May 2022 18:40:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Mon, 23 May 2022 18:40:56 GMT
ARG MARIADB_VERSION=1:10.9.1+maria~jammy
# Mon, 23 May 2022 18:40:57 GMT
ENV MARIADB_VERSION=1:10.9.1+maria~jammy
# Mon, 23 May 2022 18:40:58 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.1/repo/ubuntu/ jammy main
# Mon, 23 May 2022 18:40:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 23 May 2022 18:41:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 23 May 2022 18:41:19 GMT
VOLUME [/var/lib/mysql]
# Mon, 23 May 2022 18:41:20 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Mon, 23 May 2022 18:41:21 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Mon, 23 May 2022 18:41:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 18:41:22 GMT
EXPOSE 3306
# Mon, 23 May 2022 18:41:23 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:b84950154c181a602d2e93b68e84660f96dc78f94ae36f3df2db8d5701abb6a5`  
		Last Modified: Fri, 29 Apr 2022 22:52:07 GMT  
		Size: 28.4 MB (28376457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ae07faadba444656d4d080edc85dcaba97c3ac8f3ac415b136c2add7ff5393`  
		Last Modified: Mon, 23 May 2022 18:47:26 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46428e702eff2922592a3c96fbe5e3764cbca14a5a770718e36a51ad4c9dc906`  
		Last Modified: Mon, 23 May 2022 18:47:25 GMT  
		Size: 3.6 MB (3592731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e775e0ed5a0037f1c4cce3ef74f7025c80ec7e27e1e60a27c1f39d53e944c75`  
		Last Modified: Mon, 23 May 2022 18:47:25 GMT  
		Size: 4.0 MB (4014468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:031c54d0d9d9d4a999c13ba6733390868914e2c9c66b3ee2feb98e2a93de5d99`  
		Last Modified: Mon, 23 May 2022 18:47:24 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602265dc68e116e160f1e4da3863e9ff8313798a78e0d68554915d7cb1d970b9`  
		Last Modified: Mon, 23 May 2022 18:47:25 GMT  
		Size: 2.2 MB (2210433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d1d131fb6cb45f460fd0eb002edad2f1273dd1d769fff5ad071a2356a239edc`  
		Last Modified: Mon, 23 May 2022 18:47:22 GMT  
		Size: 2.5 KB (2470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a472a231b9bc32ef187c8c40f82604479c8a70ba51f185c27f08ecdacbea74`  
		Last Modified: Mon, 23 May 2022 18:47:22 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b206b9b7f2426f95ff0c1c8ab3e228ab2a6550f12fcab51fae66bce0e073028`  
		Last Modified: Mon, 23 May 2022 18:47:32 GMT  
		Size: 66.4 MB (66440929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83954d0fd1371eec503150a70054b803a3ef6d5cfdbcb6292712ecf1834b5f0a`  
		Last Modified: Mon, 23 May 2022 18:47:22 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c624ab0a5fc6c924c38bd2ec5ab26dd0f83ac9e8d0ec4aeb46590d5920fb81`  
		Last Modified: Mon, 23 May 2022 18:47:22 GMT  
		Size: 6.7 KB (6699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.9.1-rc-jammy` - linux; s390x

```console
$ docker pull mariadb@sha256:33538e6a86f234d1e45ae0f2c9b3f9dbfb0885fc74ca39eb91273fa2cd7fe142
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (105019606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c1caded8d0213b371f298a00ae52666860fc6794d601e88a0818002d37ce5d4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 07 Jun 2022 04:05:41 GMT
ADD file:5412b0d16961079a78b96411ca23f1838ac09c2fae839829476380b5389e49f8 in / 
# Tue, 07 Jun 2022 04:05:45 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:46:42 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 06:46:54 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:46:55 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 06:47:15 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 06:47:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 06:47:27 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:47:27 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 06:47:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 06:47:30 GMT
ARG MARIADB_VERSION=1:10.9.1+maria~jammy
# Tue, 07 Jun 2022 06:47:30 GMT
ENV MARIADB_VERSION=1:10.9.1+maria~jammy
# Tue, 07 Jun 2022 06:47:31 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.1/repo/ubuntu/ jammy main
# Tue, 07 Jun 2022 06:47:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 06:47:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 06:48:01 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 06:48:01 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 06:48:02 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 07 Jun 2022 06:48:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 06:48:02 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 06:48:03 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:6fa1296f44090f6150dfb96d6ae217a58b9d66c56d7a986c35657df6bd1a89f0`  
		Last Modified: Tue, 07 Jun 2022 04:08:13 GMT  
		Size: 28.6 MB (28638482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e980d0c8e278a504f0f8cb00cbb715bc7239eb7e9e13f635db0c77b7e9625c`  
		Last Modified: Tue, 07 Jun 2022 06:53:30 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec96ea557bfa670cf2072437f6b01b817a185da1ef3e1b694d61b29c5da1561e`  
		Last Modified: Tue, 07 Jun 2022 06:53:29 GMT  
		Size: 3.7 MB (3674855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:726015530ec97a71af69b3bda1ced0b4bbdb013fc074478728335d1c714e1ed0`  
		Last Modified: Tue, 07 Jun 2022 06:53:29 GMT  
		Size: 2.0 MB (1954988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b4bef35a73fc4bcfe6311f2e5045128a3861bcd38b075463b870d13c0967b9`  
		Last Modified: Tue, 07 Jun 2022 06:53:29 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe29a6e8adabddd30630efcb94fa1700cbd3c96aa623c45d34e889d00358fc07`  
		Last Modified: Tue, 07 Jun 2022 06:53:29 GMT  
		Size: 2.2 MB (2215965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3784b0c624b488911de05f153cfb7a59247ee32628f054fc1672d59c993907b8`  
		Last Modified: Tue, 07 Jun 2022 06:53:28 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617d10bd27641513a03c157ead3c2d8ea4197b26405ac8fddbbf567c93e87239`  
		Last Modified: Tue, 07 Jun 2022 06:53:28 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2099c5146b88e0e26d5c83a7a4265037c8d96e09287f27f4ffdacd05b55367`  
		Last Modified: Tue, 07 Jun 2022 06:53:37 GMT  
		Size: 68.5 MB (68520411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc255780d5d4f7417bcbf01460b97ff04be077b51fb95afe1f597ddb3edfe703`  
		Last Modified: Tue, 07 Jun 2022 06:53:27 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94abd9929d18abf5725866d9aec57fb93c319aa74a65aa94694e769683204ed5`  
		Last Modified: Tue, 07 Jun 2022 06:53:27 GMT  
		Size: 6.7 KB (6697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:jammy`

```console
$ docker pull mariadb@sha256:8be45db6728d9f755064b1553a20475120a962e49db52dff30f77c487c2da60d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mariadb:jammy` - linux; amd64

```console
$ docker pull mariadb@sha256:483a080b5bcdf0a898ef4574209080f7a42896c7134c60c55b4d4cb5ab3a8d6f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.9 MB (123859860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea81af801379dae14e596b55612f355a63cfca2ed53cf27d047340f4890cf25c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:25 GMT
ADD file:11157b07dde10107f3f6f2b892c869ea83868475d5825167b5f466a7e410eb05 in / 
# Mon, 06 Jun 2022 22:21:26 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:40:40 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 00:40:56 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:40:56 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 00:41:06 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 00:41:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 00:41:13 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:41:13 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 00:41:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 00:42:02 GMT
ARG MARIADB_MAJOR=10.8
# Tue, 07 Jun 2022 00:42:03 GMT
ENV MARIADB_MAJOR=10.8
# Tue, 07 Jun 2022 00:42:03 GMT
ARG MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 07 Jun 2022 00:42:03 GMT
ENV MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 07 Jun 2022 00:42:03 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
# Tue, 07 Jun 2022 00:42:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 00:42:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 00:42:23 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 00:42:23 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 00:42:23 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 07 Jun 2022 00:42:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 00:42:23 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 00:42:23 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:405f018f9d1d0f351c196b841a7c7f226fb8ea448acd6339a9ed8741600275a2`  
		Last Modified: Wed, 01 Jun 2022 03:03:39 GMT  
		Size: 30.4 MB (30423715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a85079b8234f1744aeed618170b84c2f6b970a320e10616ff031d3be24b5cd4`  
		Last Modified: Tue, 07 Jun 2022 00:47:43 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:579c7ff691b1abc2640eb61104ca92a223103daf11214a248cc580163536e70d`  
		Last Modified: Tue, 07 Jun 2022 00:47:42 GMT  
		Size: 3.8 MB (3765124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4976663b5d6daa78634cc56c60cb837f47e79832759e9bdb8f1c592b194411bf`  
		Last Modified: Tue, 07 Jun 2022 00:47:42 GMT  
		Size: 2.0 MB (1991845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:169024b1fb136785c2ed5f758e9707ce456f38d8007d568f863be47b0873afd7`  
		Last Modified: Tue, 07 Jun 2022 00:47:41 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ffe8ce897f6bfdab5ac2fa06b95c2a6187161ced620b3b00e71b31e7b75e47`  
		Last Modified: Tue, 07 Jun 2022 00:47:42 GMT  
		Size: 2.3 MB (2297483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b583c09d23c314a64c34258bda89aaefc6c4b3a488297892863af1dd61bb4113`  
		Last Modified: Tue, 07 Jun 2022 00:47:39 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b9f0c08d08f4ae53297606d8c0aea35c96566d2e544a8a32efb72eebc3749b6`  
		Last Modified: Tue, 07 Jun 2022 00:48:08 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cd51f98458654de3ea7c535ee562e9f9251fd6a0818629346bcadaaa768b71a`  
		Last Modified: Tue, 07 Jun 2022 00:48:20 GMT  
		Size: 85.4 MB (85366786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f506bb8acafbb672f41df13b1d99173b9217140c8137ecc9daec14c4e00f70`  
		Last Modified: Tue, 07 Jun 2022 00:48:08 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d689f79ba4ea066cd24d5c7f7ae294a524fc166bb7f9e8b60d48472f35277a`  
		Last Modified: Tue, 07 Jun 2022 00:48:08 GMT  
		Size: 6.7 KB (6699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:jammy` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:b6764b02b5eb8d6274207dbb827317cafc8694c1505185aa092d5551f8a793f2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.5 MB (104543896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecc004eed0c26ad5c4e0d75baff2cb4e7fdc144f713d053c256f6455b608d280`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:52 GMT
ADD file:1e18e22e32f06a7e93275cf3a2eb2a1d3892be27628bdae2de4b2aadb992bd50 in / 
# Fri, 29 Apr 2022 22:49:53 GMT
CMD ["bash"]
# Mon, 23 May 2022 18:40:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Mon, 23 May 2022 18:40:25 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 23 May 2022 18:40:26 GMT
ENV GOSU_VERSION=1.14
# Mon, 23 May 2022 18:40:43 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 23 May 2022 18:40:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 23 May 2022 18:40:53 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 23 May 2022 18:40:53 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Mon, 23 May 2022 18:40:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Mon, 23 May 2022 18:41:40 GMT
ARG MARIADB_MAJOR=10.8
# Mon, 23 May 2022 18:41:41 GMT
ENV MARIADB_MAJOR=10.8
# Mon, 23 May 2022 18:41:42 GMT
ARG MARIADB_VERSION=1:10.8.3+maria~jammy
# Mon, 23 May 2022 18:41:43 GMT
ENV MARIADB_VERSION=1:10.8.3+maria~jammy
# Mon, 23 May 2022 18:41:44 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
# Mon, 23 May 2022 18:41:45 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 23 May 2022 18:42:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 23 May 2022 18:42:04 GMT
VOLUME [/var/lib/mysql]
# Mon, 23 May 2022 18:42:06 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Mon, 23 May 2022 18:42:07 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Mon, 23 May 2022 18:42:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 18:42:08 GMT
EXPOSE 3306
# Mon, 23 May 2022 18:42:09 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:b84950154c181a602d2e93b68e84660f96dc78f94ae36f3df2db8d5701abb6a5`  
		Last Modified: Fri, 29 Apr 2022 22:52:07 GMT  
		Size: 28.4 MB (28376457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ae07faadba444656d4d080edc85dcaba97c3ac8f3ac415b136c2add7ff5393`  
		Last Modified: Mon, 23 May 2022 18:47:26 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46428e702eff2922592a3c96fbe5e3764cbca14a5a770718e36a51ad4c9dc906`  
		Last Modified: Mon, 23 May 2022 18:47:25 GMT  
		Size: 3.6 MB (3592731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e775e0ed5a0037f1c4cce3ef74f7025c80ec7e27e1e60a27c1f39d53e944c75`  
		Last Modified: Mon, 23 May 2022 18:47:25 GMT  
		Size: 4.0 MB (4014468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:031c54d0d9d9d4a999c13ba6733390868914e2c9c66b3ee2feb98e2a93de5d99`  
		Last Modified: Mon, 23 May 2022 18:47:24 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602265dc68e116e160f1e4da3863e9ff8313798a78e0d68554915d7cb1d970b9`  
		Last Modified: Mon, 23 May 2022 18:47:25 GMT  
		Size: 2.2 MB (2210433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d1d131fb6cb45f460fd0eb002edad2f1273dd1d769fff5ad071a2356a239edc`  
		Last Modified: Mon, 23 May 2022 18:47:22 GMT  
		Size: 2.5 KB (2470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a33ea1b30434b058f9b0ea3af9c9638014b6e11714eaa4888fceb806344fe49`  
		Last Modified: Mon, 23 May 2022 18:47:50 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9539c6148f07eaa2bb03fae3339771575a22824c8b4d9a6ab5cc10210d114a0c`  
		Last Modified: Mon, 23 May 2022 18:48:01 GMT  
		Size: 66.3 MB (66334981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38aa29868643c4f4f19f60129f5a981a1b09518e1621b1ffdcdf6f06c8261231`  
		Last Modified: Mon, 23 May 2022 18:47:50 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3702214dffba8174c27ba1d8d97eebb416c8b984871b3a18b8c497c26b227a77`  
		Last Modified: Mon, 23 May 2022 18:47:50 GMT  
		Size: 6.7 KB (6700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:jammy` - linux; s390x

```console
$ docker pull mariadb@sha256:a9c536d0da138dacf56fd611cd76171a5e7f21b2c254495939f45200a2d2ec7e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (104950766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fad948eb6c3a1c6724e95ac01927251304a6d53ddb9014a73f6964b6092b994`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 07 Jun 2022 04:05:41 GMT
ADD file:5412b0d16961079a78b96411ca23f1838ac09c2fae839829476380b5389e49f8 in / 
# Tue, 07 Jun 2022 04:05:45 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:46:42 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 06:46:54 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:46:55 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 06:47:15 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 06:47:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 06:47:27 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:47:27 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 06:47:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 06:48:14 GMT
ARG MARIADB_MAJOR=10.8
# Tue, 07 Jun 2022 06:48:15 GMT
ENV MARIADB_MAJOR=10.8
# Tue, 07 Jun 2022 06:48:15 GMT
ARG MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 07 Jun 2022 06:48:15 GMT
ENV MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 07 Jun 2022 06:48:15 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
# Tue, 07 Jun 2022 06:48:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 06:48:49 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 06:48:56 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 06:48:56 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 06:48:56 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 07 Jun 2022 06:48:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 06:48:57 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 06:48:57 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:6fa1296f44090f6150dfb96d6ae217a58b9d66c56d7a986c35657df6bd1a89f0`  
		Last Modified: Tue, 07 Jun 2022 04:08:13 GMT  
		Size: 28.6 MB (28638482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e980d0c8e278a504f0f8cb00cbb715bc7239eb7e9e13f635db0c77b7e9625c`  
		Last Modified: Tue, 07 Jun 2022 06:53:30 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec96ea557bfa670cf2072437f6b01b817a185da1ef3e1b694d61b29c5da1561e`  
		Last Modified: Tue, 07 Jun 2022 06:53:29 GMT  
		Size: 3.7 MB (3674855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:726015530ec97a71af69b3bda1ced0b4bbdb013fc074478728335d1c714e1ed0`  
		Last Modified: Tue, 07 Jun 2022 06:53:29 GMT  
		Size: 2.0 MB (1954988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b4bef35a73fc4bcfe6311f2e5045128a3861bcd38b075463b870d13c0967b9`  
		Last Modified: Tue, 07 Jun 2022 06:53:29 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe29a6e8adabddd30630efcb94fa1700cbd3c96aa623c45d34e889d00358fc07`  
		Last Modified: Tue, 07 Jun 2022 06:53:29 GMT  
		Size: 2.2 MB (2215965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3784b0c624b488911de05f153cfb7a59247ee32628f054fc1672d59c993907b8`  
		Last Modified: Tue, 07 Jun 2022 06:53:28 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1811da06c80a8ea4d1138022303a2aee104a2e92377d041edeeea75286fc8df9`  
		Last Modified: Tue, 07 Jun 2022 06:53:50 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b002fb05e958857048b5e3de1eaf8add56ee8be42579108a53beda62649599c`  
		Last Modified: Tue, 07 Jun 2022 06:53:59 GMT  
		Size: 68.5 MB (68451571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12dfba249abcff12b977205f137dffac3b7456bee31377d44e3c935b68ae5e7`  
		Last Modified: Tue, 07 Jun 2022 06:53:50 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fecfeca76a356593a14b01d27c7d0301e7f5b59b14fe638cc7c1b2c0e3dfdeb8`  
		Last Modified: Tue, 07 Jun 2022 06:53:50 GMT  
		Size: 6.7 KB (6694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:latest`

```console
$ docker pull mariadb@sha256:88fcb7d92c7f61cd885c4d309c98461f3607aa6dbd57a2474be86e1956b36d13
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:latest` - linux; amd64

```console
$ docker pull mariadb@sha256:483a080b5bcdf0a898ef4574209080f7a42896c7134c60c55b4d4cb5ab3a8d6f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.9 MB (123859860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea81af801379dae14e596b55612f355a63cfca2ed53cf27d047340f4890cf25c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:25 GMT
ADD file:11157b07dde10107f3f6f2b892c869ea83868475d5825167b5f466a7e410eb05 in / 
# Mon, 06 Jun 2022 22:21:26 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:40:40 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 00:40:56 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:40:56 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 00:41:06 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 00:41:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 00:41:13 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:41:13 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 00:41:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 00:42:02 GMT
ARG MARIADB_MAJOR=10.8
# Tue, 07 Jun 2022 00:42:03 GMT
ENV MARIADB_MAJOR=10.8
# Tue, 07 Jun 2022 00:42:03 GMT
ARG MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 07 Jun 2022 00:42:03 GMT
ENV MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 07 Jun 2022 00:42:03 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
# Tue, 07 Jun 2022 00:42:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 00:42:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 00:42:23 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 00:42:23 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 00:42:23 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 07 Jun 2022 00:42:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 00:42:23 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 00:42:23 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:405f018f9d1d0f351c196b841a7c7f226fb8ea448acd6339a9ed8741600275a2`  
		Last Modified: Wed, 01 Jun 2022 03:03:39 GMT  
		Size: 30.4 MB (30423715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a85079b8234f1744aeed618170b84c2f6b970a320e10616ff031d3be24b5cd4`  
		Last Modified: Tue, 07 Jun 2022 00:47:43 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:579c7ff691b1abc2640eb61104ca92a223103daf11214a248cc580163536e70d`  
		Last Modified: Tue, 07 Jun 2022 00:47:42 GMT  
		Size: 3.8 MB (3765124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4976663b5d6daa78634cc56c60cb837f47e79832759e9bdb8f1c592b194411bf`  
		Last Modified: Tue, 07 Jun 2022 00:47:42 GMT  
		Size: 2.0 MB (1991845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:169024b1fb136785c2ed5f758e9707ce456f38d8007d568f863be47b0873afd7`  
		Last Modified: Tue, 07 Jun 2022 00:47:41 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ffe8ce897f6bfdab5ac2fa06b95c2a6187161ced620b3b00e71b31e7b75e47`  
		Last Modified: Tue, 07 Jun 2022 00:47:42 GMT  
		Size: 2.3 MB (2297483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b583c09d23c314a64c34258bda89aaefc6c4b3a488297892863af1dd61bb4113`  
		Last Modified: Tue, 07 Jun 2022 00:47:39 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b9f0c08d08f4ae53297606d8c0aea35c96566d2e544a8a32efb72eebc3749b6`  
		Last Modified: Tue, 07 Jun 2022 00:48:08 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cd51f98458654de3ea7c535ee562e9f9251fd6a0818629346bcadaaa768b71a`  
		Last Modified: Tue, 07 Jun 2022 00:48:20 GMT  
		Size: 85.4 MB (85366786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f506bb8acafbb672f41df13b1d99173b9217140c8137ecc9daec14c4e00f70`  
		Last Modified: Tue, 07 Jun 2022 00:48:08 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d689f79ba4ea066cd24d5c7f7ae294a524fc166bb7f9e8b60d48472f35277a`  
		Last Modified: Tue, 07 Jun 2022 00:48:08 GMT  
		Size: 6.7 KB (6699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:b6764b02b5eb8d6274207dbb827317cafc8694c1505185aa092d5551f8a793f2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.5 MB (104543896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecc004eed0c26ad5c4e0d75baff2cb4e7fdc144f713d053c256f6455b608d280`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:52 GMT
ADD file:1e18e22e32f06a7e93275cf3a2eb2a1d3892be27628bdae2de4b2aadb992bd50 in / 
# Fri, 29 Apr 2022 22:49:53 GMT
CMD ["bash"]
# Mon, 23 May 2022 18:40:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Mon, 23 May 2022 18:40:25 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 23 May 2022 18:40:26 GMT
ENV GOSU_VERSION=1.14
# Mon, 23 May 2022 18:40:43 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 23 May 2022 18:40:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 23 May 2022 18:40:53 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 23 May 2022 18:40:53 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Mon, 23 May 2022 18:40:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Mon, 23 May 2022 18:41:40 GMT
ARG MARIADB_MAJOR=10.8
# Mon, 23 May 2022 18:41:41 GMT
ENV MARIADB_MAJOR=10.8
# Mon, 23 May 2022 18:41:42 GMT
ARG MARIADB_VERSION=1:10.8.3+maria~jammy
# Mon, 23 May 2022 18:41:43 GMT
ENV MARIADB_VERSION=1:10.8.3+maria~jammy
# Mon, 23 May 2022 18:41:44 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
# Mon, 23 May 2022 18:41:45 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 23 May 2022 18:42:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 23 May 2022 18:42:04 GMT
VOLUME [/var/lib/mysql]
# Mon, 23 May 2022 18:42:06 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Mon, 23 May 2022 18:42:07 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Mon, 23 May 2022 18:42:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 18:42:08 GMT
EXPOSE 3306
# Mon, 23 May 2022 18:42:09 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:b84950154c181a602d2e93b68e84660f96dc78f94ae36f3df2db8d5701abb6a5`  
		Last Modified: Fri, 29 Apr 2022 22:52:07 GMT  
		Size: 28.4 MB (28376457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ae07faadba444656d4d080edc85dcaba97c3ac8f3ac415b136c2add7ff5393`  
		Last Modified: Mon, 23 May 2022 18:47:26 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46428e702eff2922592a3c96fbe5e3764cbca14a5a770718e36a51ad4c9dc906`  
		Last Modified: Mon, 23 May 2022 18:47:25 GMT  
		Size: 3.6 MB (3592731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e775e0ed5a0037f1c4cce3ef74f7025c80ec7e27e1e60a27c1f39d53e944c75`  
		Last Modified: Mon, 23 May 2022 18:47:25 GMT  
		Size: 4.0 MB (4014468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:031c54d0d9d9d4a999c13ba6733390868914e2c9c66b3ee2feb98e2a93de5d99`  
		Last Modified: Mon, 23 May 2022 18:47:24 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602265dc68e116e160f1e4da3863e9ff8313798a78e0d68554915d7cb1d970b9`  
		Last Modified: Mon, 23 May 2022 18:47:25 GMT  
		Size: 2.2 MB (2210433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d1d131fb6cb45f460fd0eb002edad2f1273dd1d769fff5ad071a2356a239edc`  
		Last Modified: Mon, 23 May 2022 18:47:22 GMT  
		Size: 2.5 KB (2470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a33ea1b30434b058f9b0ea3af9c9638014b6e11714eaa4888fceb806344fe49`  
		Last Modified: Mon, 23 May 2022 18:47:50 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9539c6148f07eaa2bb03fae3339771575a22824c8b4d9a6ab5cc10210d114a0c`  
		Last Modified: Mon, 23 May 2022 18:48:01 GMT  
		Size: 66.3 MB (66334981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38aa29868643c4f4f19f60129f5a981a1b09518e1621b1ffdcdf6f06c8261231`  
		Last Modified: Mon, 23 May 2022 18:47:50 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3702214dffba8174c27ba1d8d97eebb416c8b984871b3a18b8c497c26b227a77`  
		Last Modified: Mon, 23 May 2022 18:47:50 GMT  
		Size: 6.7 KB (6700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; ppc64le

```console
$ docker pull mariadb@sha256:9f0a93c25897df9a9b2ca3becf35fccdfd9531009c57b1481d8d027f8722dc49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.5 MB (139538393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b9fdde589bdb89bddd62d2076c08de8ca866b15932b15f44b9809efd0a2c54d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:28 GMT
ADD file:55691ac7d76af0fcfafc39ebd1e5a4f2d7018147d6db6f89812db33fbaffc2f9 in / 
# Fri, 29 Apr 2022 23:22:33 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:50:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:52:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:52:19 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:53:06 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:53:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:53:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:53:51 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:54:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:59:29 GMT
ARG MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 00:59:47 GMT
ENV MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 00:59:55 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Sat, 30 Apr 2022 01:00:09 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Sat, 30 Apr 2022 01:00:25 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 01:00:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:03:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:03:59 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:04:00 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:04:02 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:04:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:04:08 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:04:10 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:e9c0a77cb9f0f7330e3fc62254e4c8ae89ed4bba21209fdc1088195250f950b9`  
		Last Modified: Fri, 29 Apr 2022 23:25:23 GMT  
		Size: 33.3 MB (33290661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933fb2862e2716afd28ee38ed71eb9097a647fd38b4378b802ba4928e819c444`  
		Last Modified: Sat, 30 Apr 2022 01:20:57 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6899bc35ca339b1fbd966c280b0f1a2c3acd469ad358d3b3f48b1e6a1b7bd5`  
		Last Modified: Sat, 30 Apr 2022 01:20:56 GMT  
		Size: 6.7 MB (6667588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185278c53367843a392ed443f9de142076add930e26c0765cd604902e7e0026f`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 3.7 MB (3672592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356d5cab0b98f71595c34fffd4c19a0d48f05279ac84eb9068b1090bafb87d6f`  
		Last Modified: Sat, 30 Apr 2022 01:20:54 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd37e664a57394de1d81b89e36f57a4318e77c9dcbd17a16966cc7924f323fa`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 2.6 MB (2568397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bc301781015b0c1df07f994700ffdfde0f31a2be7b1063ae698b5280f77aa5`  
		Last Modified: Sat, 30 Apr 2022 01:20:51 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c38d1aea9df71e0e7b7a07ebbf73d3df047d6925b8517612731ce14b29d81e6f`  
		Last Modified: Sat, 30 Apr 2022 01:21:32 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219c8b280b85bfcb106c1c23cb4f820d20c27c361c26bc4b7b20b972ae0e550d`  
		Last Modified: Sat, 30 Apr 2022 01:21:50 GMT  
		Size: 93.3 MB (93324167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7ca5c34dd9a2fb0cbcf95168f69c6aa33df79bce1e843d573af62fc0ca0bf60`  
		Last Modified: Sat, 30 Apr 2022 01:21:32 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86ec7c5c6f4af575453b8a299723e99a51c614cf4d411dc507c8c4970ecaf71`  
		Last Modified: Sat, 30 Apr 2022 01:21:32 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; s390x

```console
$ docker pull mariadb@sha256:a9c536d0da138dacf56fd611cd76171a5e7f21b2c254495939f45200a2d2ec7e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (104950766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fad948eb6c3a1c6724e95ac01927251304a6d53ddb9014a73f6964b6092b994`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 07 Jun 2022 04:05:41 GMT
ADD file:5412b0d16961079a78b96411ca23f1838ac09c2fae839829476380b5389e49f8 in / 
# Tue, 07 Jun 2022 04:05:45 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:46:42 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 06:46:54 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:46:55 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 06:47:15 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 06:47:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 06:47:27 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:47:27 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 06:47:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 06:48:14 GMT
ARG MARIADB_MAJOR=10.8
# Tue, 07 Jun 2022 06:48:15 GMT
ENV MARIADB_MAJOR=10.8
# Tue, 07 Jun 2022 06:48:15 GMT
ARG MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 07 Jun 2022 06:48:15 GMT
ENV MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 07 Jun 2022 06:48:15 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
# Tue, 07 Jun 2022 06:48:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 06:48:49 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 06:48:56 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 06:48:56 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 06:48:56 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 07 Jun 2022 06:48:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 06:48:57 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 06:48:57 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:6fa1296f44090f6150dfb96d6ae217a58b9d66c56d7a986c35657df6bd1a89f0`  
		Last Modified: Tue, 07 Jun 2022 04:08:13 GMT  
		Size: 28.6 MB (28638482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e980d0c8e278a504f0f8cb00cbb715bc7239eb7e9e13f635db0c77b7e9625c`  
		Last Modified: Tue, 07 Jun 2022 06:53:30 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec96ea557bfa670cf2072437f6b01b817a185da1ef3e1b694d61b29c5da1561e`  
		Last Modified: Tue, 07 Jun 2022 06:53:29 GMT  
		Size: 3.7 MB (3674855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:726015530ec97a71af69b3bda1ced0b4bbdb013fc074478728335d1c714e1ed0`  
		Last Modified: Tue, 07 Jun 2022 06:53:29 GMT  
		Size: 2.0 MB (1954988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b4bef35a73fc4bcfe6311f2e5045128a3861bcd38b075463b870d13c0967b9`  
		Last Modified: Tue, 07 Jun 2022 06:53:29 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe29a6e8adabddd30630efcb94fa1700cbd3c96aa623c45d34e889d00358fc07`  
		Last Modified: Tue, 07 Jun 2022 06:53:29 GMT  
		Size: 2.2 MB (2215965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3784b0c624b488911de05f153cfb7a59247ee32628f054fc1672d59c993907b8`  
		Last Modified: Tue, 07 Jun 2022 06:53:28 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1811da06c80a8ea4d1138022303a2aee104a2e92377d041edeeea75286fc8df9`  
		Last Modified: Tue, 07 Jun 2022 06:53:50 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b002fb05e958857048b5e3de1eaf8add56ee8be42579108a53beda62649599c`  
		Last Modified: Tue, 07 Jun 2022 06:53:59 GMT  
		Size: 68.5 MB (68451571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12dfba249abcff12b977205f137dffac3b7456bee31377d44e3c935b68ae5e7`  
		Last Modified: Tue, 07 Jun 2022 06:53:50 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fecfeca76a356593a14b01d27c7d0301e7f5b59b14fe638cc7c1b2c0e3dfdeb8`  
		Last Modified: Tue, 07 Jun 2022 06:53:50 GMT  
		Size: 6.7 KB (6694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
