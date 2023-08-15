<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mariadb`

-	[`mariadb:10`](#mariadb10)
-	[`mariadb:10-jammy`](#mariadb10-jammy)
-	[`mariadb:10.10`](#mariadb1010)
-	[`mariadb:10.10-jammy`](#mariadb1010-jammy)
-	[`mariadb:10.10.6`](#mariadb10106)
-	[`mariadb:10.10.6-jammy`](#mariadb10106-jammy)
-	[`mariadb:10.11`](#mariadb1011)
-	[`mariadb:10.11-jammy`](#mariadb1011-jammy)
-	[`mariadb:10.11.5`](#mariadb10115)
-	[`mariadb:10.11.5-jammy`](#mariadb10115-jammy)
-	[`mariadb:10.4`](#mariadb104)
-	[`mariadb:10.4-focal`](#mariadb104-focal)
-	[`mariadb:10.4.31`](#mariadb10431)
-	[`mariadb:10.4.31-focal`](#mariadb10431-focal)
-	[`mariadb:10.5`](#mariadb105)
-	[`mariadb:10.5-focal`](#mariadb105-focal)
-	[`mariadb:10.5.22`](#mariadb10522)
-	[`mariadb:10.5.22-focal`](#mariadb10522-focal)
-	[`mariadb:10.6`](#mariadb106)
-	[`mariadb:10.6-focal`](#mariadb106-focal)
-	[`mariadb:10.6.15`](#mariadb10615)
-	[`mariadb:10.6.15-focal`](#mariadb10615-focal)
-	[`mariadb:10.9`](#mariadb109)
-	[`mariadb:10.9-jammy`](#mariadb109-jammy)
-	[`mariadb:10.9.8`](#mariadb1098)
-	[`mariadb:10.9.8-jammy`](#mariadb1098-jammy)
-	[`mariadb:11`](#mariadb11)
-	[`mariadb:11-jammy`](#mariadb11-jammy)
-	[`mariadb:11.0`](#mariadb110)
-	[`mariadb:11.0-jammy`](#mariadb110-jammy)
-	[`mariadb:11.0.3`](#mariadb1103)
-	[`mariadb:11.0.3-jammy`](#mariadb1103-jammy)
-	[`mariadb:11.1-rc`](#mariadb111-rc)
-	[`mariadb:11.1-rc-jammy`](#mariadb111-rc-jammy)
-	[`mariadb:11.1.1-rc`](#mariadb1111-rc)
-	[`mariadb:11.1.1-rc-jammy`](#mariadb1111-rc-jammy)
-	[`mariadb:jammy`](#mariadbjammy)
-	[`mariadb:latest`](#mariadblatest)
-	[`mariadb:lts`](#mariadblts)
-	[`mariadb:lts-jammy`](#mariadblts-jammy)

## `mariadb:10`

```console
$ docker pull mariadb@sha256:385c0ba6270307511a511ad915350736602c33fafb3f63f663c853920424c365
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10` - linux; amd64

```console
$ docker pull mariadb@sha256:4b6b625ae683588d99507ac01b042863d4311b6e15f81d653be6892762637375
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123105947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8b77d250201f61f86a2a98c7e07d5bd77f96b4a345f40f8ce53593c2ffca84d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 18:27:16 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 18:27:16 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 18:27:16 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 18:27:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 18:27:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 18:27:39 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 18:28:38 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 18:28:38 GMT
ARG MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Tue, 04 Jul 2023 18:28:38 GMT
ENV MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Tue, 04 Jul 2023 18:28:38 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 18:28:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 18:28:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 18:28:57 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 18:28:57 GMT
COPY file:60282e2c078282f09827dfb0926d431a7ad71f6de3495a21fc8a846430fc5fc9 in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 18:28:57 GMT
COPY file:704c6685e9d99f08306a2726e0468f5a764a4040cc2eb6138c1be72ac2529bbc in /usr/local/bin/ 
# Tue, 04 Jul 2023 18:28:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 18:28:57 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 18:28:58 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:718e898a86ffe915c46f60c599bc87928aa5e7e3a9434cbf52066b49651d3a1f`  
		Last Modified: Tue, 04 Jul 2023 18:32:00 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bd7a143a6c5d92cccbae0a38df554277f44cb4dbfcb668436dc5ed3398144a`  
		Last Modified: Tue, 04 Jul 2023 18:32:01 GMT  
		Size: 5.6 MB (5592713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80cdf483b70a4a08d0db0ff26cb8dbdc933588954a3bf91fce2f2544b7be37b8`  
		Last Modified: Tue, 04 Jul 2023 18:31:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9531173fe68dc54682bc25ac9b4c270ed5772c4ba6b47daef52a3d4e70af77`  
		Last Modified: Tue, 04 Jul 2023 18:32:56 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7375440478980efc7a168e77a3f085cd056c5f722e11d17a5ef922de66c95f45`  
		Last Modified: Tue, 04 Jul 2023 18:33:09 GMT  
		Size: 87.1 MB (87068650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8be80cd3b8009d3f30675bf4b5402c953d8dfaae942c2fb610a1fab9f826c3`  
		Last Modified: Tue, 04 Jul 2023 18:32:56 GMT  
		Size: 3.6 KB (3565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2384dd133a6708cc48561cd0773fb9abe3b23eae32323d644c2b8c57c8148f3`  
		Last Modified: Tue, 04 Jul 2023 18:32:56 GMT  
		Size: 7.6 KB (7566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:33e8f9991a22fd6678ef20bf31b2bcecc6fc7c7bea5c62b0144ba4df243ff107
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117618140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fc7fccd2af985a12c6a6c0d2decd2a77618a858164ee12eb905621a5e02e6dc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 15:48:55 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 15:48:55 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 15:48:56 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 15:49:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 15:49:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 15:49:12 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 15:50:06 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 15:50:07 GMT
ARG MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Tue, 04 Jul 2023 15:50:07 GMT
ENV MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Tue, 04 Jul 2023 15:50:07 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 15:50:07 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 15:50:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 15:50:24 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 15:50:24 GMT
COPY file:60282e2c078282f09827dfb0926d431a7ad71f6de3495a21fc8a846430fc5fc9 in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 15:50:24 GMT
COPY file:704c6685e9d99f08306a2726e0468f5a764a4040cc2eb6138c1be72ac2529bbc in /usr/local/bin/ 
# Tue, 04 Jul 2023 15:50:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 15:50:24 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 15:50:24 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f226d4d968a5322b60d61898c78418afeeb62f9a8613d9939d2546229a59ed0`  
		Last Modified: Tue, 04 Jul 2023 15:53:12 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a718d9544847f819e9859244c57b1093e55eb4bbd1d50066804d9ddd24d9c2c`  
		Last Modified: Tue, 04 Jul 2023 15:53:12 GMT  
		Size: 5.4 MB (5406735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad17cece0015293005bd369ad4550b0faa2ef78f55de897f35a48e5b101b83c8`  
		Last Modified: Tue, 04 Jul 2023 15:53:10 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8210aced70ef3e24a46799929c24c1213867224b74ac675905ac218d01442f43`  
		Last Modified: Tue, 04 Jul 2023 15:54:02 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56cb7b8053f2d91dc92f88f643e2865478be6d9ff1a66c023d0c46ac4354ee4b`  
		Last Modified: Tue, 04 Jul 2023 15:54:11 GMT  
		Size: 83.8 MB (83807029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449424199d1167824fde06f204297c2ba55b2095c8bfd15d6a77aa93b09c7e4b`  
		Last Modified: Tue, 04 Jul 2023 15:54:01 GMT  
		Size: 3.6 KB (3565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3ad0253591ba73c469a1fb8a855ae6c9f69b8c1c7c16163e792da830111d9f`  
		Last Modified: Tue, 04 Jul 2023 15:54:02 GMT  
		Size: 7.6 KB (7568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10` - linux; ppc64le

```console
$ docker pull mariadb@sha256:0f837e667037e0f69042accade3ac2b389154167bcff6ea9e8639eb6fe9f0460
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131775039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8822e9bd24ab2483e7f0ae20339330fcf3c800c3fb250d7115a2b071dddd4ec1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:45:53 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:45:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:45:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:45:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:45:56 GMT
ADD file:8c2fc380378944326d602742fde0e30458cd3e82012847b0f7e09c7184bfd135 in / 
# Wed, 28 Jun 2023 08:45:57 GMT
CMD ["/bin/bash"]
# Wed, 05 Jul 2023 01:06:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 05 Jul 2023 01:06:57 GMT
ENV GOSU_VERSION=1.14
# Wed, 05 Jul 2023 01:06:57 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 05 Jul 2023 01:07:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 05 Jul 2023 01:07:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 05 Jul 2023 01:07:36 GMT
ENV LANG=C.UTF-8
# Wed, 05 Jul 2023 01:10:14 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Wed, 05 Jul 2023 01:10:15 GMT
ARG MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Wed, 05 Jul 2023 01:10:15 GMT
ENV MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Wed, 05 Jul 2023 01:10:16 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
# Wed, 05 Jul 2023 01:10:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 05 Jul 2023 01:11:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Wed, 05 Jul 2023 01:11:10 GMT
VOLUME [/var/lib/mysql]
# Wed, 05 Jul 2023 01:11:10 GMT
COPY file:60282e2c078282f09827dfb0926d431a7ad71f6de3495a21fc8a846430fc5fc9 in /usr/local/bin/healthcheck.sh 
# Wed, 05 Jul 2023 01:11:10 GMT
COPY file:704c6685e9d99f08306a2726e0468f5a764a4040cc2eb6138c1be72ac2529bbc in /usr/local/bin/ 
# Wed, 05 Jul 2023 01:11:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Jul 2023 01:11:11 GMT
EXPOSE 3306
# Wed, 05 Jul 2023 01:11:11 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:7faa46ce6b6f5c34485980029504c3995e38149d0bca67d8b976c5dbb3673644`  
		Last Modified: Tue, 04 Jul 2023 04:42:31 GMT  
		Size: 35.7 MB (35711469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af03c7013049bbb43a9d70711423a0aa0933ad63d557a33679e987f9f4552c2`  
		Last Modified: Wed, 05 Jul 2023 01:19:30 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fae131e82b0a7c398eb2a917463894a99192198e537fa4a742953dfdec5d9a5`  
		Last Modified: Wed, 05 Jul 2023 01:19:32 GMT  
		Size: 6.0 MB (6017861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c002ce052617f5efe1f7afc4ec819f1f45b350c5956b79ee09c9bd522fe18736`  
		Last Modified: Wed, 05 Jul 2023 01:19:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:942ea7aeb70e16124a1ff199ecf228e3ab0281f20f179766b0885587643a240d`  
		Last Modified: Wed, 05 Jul 2023 01:21:05 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:115967ee1bae2b450657e120cfba1533a2768c69fe87802e5a90590ba251d1af`  
		Last Modified: Wed, 05 Jul 2023 01:21:29 GMT  
		Size: 90.0 MB (90032344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981e89a22f465c5f29cd8017aceb5dc84553018d607d0a09802db952f21422e6`  
		Last Modified: Wed, 05 Jul 2023 01:21:05 GMT  
		Size: 3.6 KB (3566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e31cc00f3e6a6786d22d5cc34292a0d4e5b50f8ba265c13862ec1ab1e8ddc49`  
		Last Modified: Wed, 05 Jul 2023 01:21:05 GMT  
		Size: 7.6 KB (7568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10` - linux; s390x

```console
$ docker pull mariadb@sha256:2b727f34069c4b59da2e9dae7fa9f907e91d2bce79801c4bdc33012d4cbe038f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.6 MB (121580518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:378fece5fccb2954bad0c49ec6a7ed1c913335d61542c2a7db9cddf4df77e3d5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:53:20 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:53:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:53:22 GMT
ADD file:fa0aef35be7808c8fd6751a52bdec4dd81057e2fcaa075c547a1db53640dae9a in / 
# Wed, 28 Jun 2023 08:53:22 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 16:55:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 16:55:27 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 16:55:27 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 16:55:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 16:55:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 16:55:44 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 16:56:57 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 16:56:57 GMT
ARG MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Tue, 04 Jul 2023 16:56:57 GMT
ENV MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Tue, 04 Jul 2023 16:56:57 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 16:56:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 16:57:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 16:57:18 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 16:57:18 GMT
COPY file:60282e2c078282f09827dfb0926d431a7ad71f6de3495a21fc8a846430fc5fc9 in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 16:57:18 GMT
COPY file:704c6685e9d99f08306a2726e0468f5a764a4040cc2eb6138c1be72ac2529bbc in /usr/local/bin/ 
# Tue, 04 Jul 2023 16:57:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 16:57:18 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 16:57:18 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:ce02ee0330980398d6a84a50abfa1a8c4d1cba27cbd7442b79f4aa1b1a14020d`  
		Last Modified: Tue, 04 Jul 2023 13:08:30 GMT  
		Size: 28.6 MB (28645696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16fb1ab422c0ae864df4333ba064fd3a16ef9b10862dca7b3320a9fb32c7e0bd`  
		Last Modified: Tue, 04 Jul 2023 17:00:17 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be60fdd8cf07af19113cd853d2f0ebedd02fc5cb31582325b43c0d50a323535`  
		Last Modified: Tue, 04 Jul 2023 17:00:18 GMT  
		Size: 5.5 MB (5470782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1374c790d73360e41f53f0d1a2d9cbaef5dd6c371a1ab7c58c7e20e71945704`  
		Last Modified: Tue, 04 Jul 2023 17:00:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27e7e4b86fecdc32e5bd05e78321e6746840e6a0544d4bedbbdf1c2754a5d72`  
		Last Modified: Tue, 04 Jul 2023 17:01:05 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0090bfea6877acf7ee51c046ee6600b616e08ac7ee48d3fdc628a0167e130e3`  
		Last Modified: Tue, 04 Jul 2023 17:01:18 GMT  
		Size: 87.5 MB (87450671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:093cd65cb7e5e05be6911f64a423e13b6109f3d369f8ac17e7e2584cbe74d8a5`  
		Last Modified: Tue, 04 Jul 2023 17:01:05 GMT  
		Size: 3.6 KB (3568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3082833c7ebee98976c11b8826ef88fa09fa5b139d6b6830488e0ed2a7144e3`  
		Last Modified: Tue, 04 Jul 2023 17:01:05 GMT  
		Size: 7.6 KB (7570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10-jammy`

```console
$ docker pull mariadb@sha256:385c0ba6270307511a511ad915350736602c33fafb3f63f663c853920424c365
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10-jammy` - linux; amd64

```console
$ docker pull mariadb@sha256:4b6b625ae683588d99507ac01b042863d4311b6e15f81d653be6892762637375
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123105947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8b77d250201f61f86a2a98c7e07d5bd77f96b4a345f40f8ce53593c2ffca84d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 18:27:16 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 18:27:16 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 18:27:16 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 18:27:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 18:27:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 18:27:39 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 18:28:38 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 18:28:38 GMT
ARG MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Tue, 04 Jul 2023 18:28:38 GMT
ENV MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Tue, 04 Jul 2023 18:28:38 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 18:28:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 18:28:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 18:28:57 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 18:28:57 GMT
COPY file:60282e2c078282f09827dfb0926d431a7ad71f6de3495a21fc8a846430fc5fc9 in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 18:28:57 GMT
COPY file:704c6685e9d99f08306a2726e0468f5a764a4040cc2eb6138c1be72ac2529bbc in /usr/local/bin/ 
# Tue, 04 Jul 2023 18:28:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 18:28:57 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 18:28:58 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:718e898a86ffe915c46f60c599bc87928aa5e7e3a9434cbf52066b49651d3a1f`  
		Last Modified: Tue, 04 Jul 2023 18:32:00 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bd7a143a6c5d92cccbae0a38df554277f44cb4dbfcb668436dc5ed3398144a`  
		Last Modified: Tue, 04 Jul 2023 18:32:01 GMT  
		Size: 5.6 MB (5592713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80cdf483b70a4a08d0db0ff26cb8dbdc933588954a3bf91fce2f2544b7be37b8`  
		Last Modified: Tue, 04 Jul 2023 18:31:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9531173fe68dc54682bc25ac9b4c270ed5772c4ba6b47daef52a3d4e70af77`  
		Last Modified: Tue, 04 Jul 2023 18:32:56 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7375440478980efc7a168e77a3f085cd056c5f722e11d17a5ef922de66c95f45`  
		Last Modified: Tue, 04 Jul 2023 18:33:09 GMT  
		Size: 87.1 MB (87068650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8be80cd3b8009d3f30675bf4b5402c953d8dfaae942c2fb610a1fab9f826c3`  
		Last Modified: Tue, 04 Jul 2023 18:32:56 GMT  
		Size: 3.6 KB (3565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2384dd133a6708cc48561cd0773fb9abe3b23eae32323d644c2b8c57c8148f3`  
		Last Modified: Tue, 04 Jul 2023 18:32:56 GMT  
		Size: 7.6 KB (7566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-jammy` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:33e8f9991a22fd6678ef20bf31b2bcecc6fc7c7bea5c62b0144ba4df243ff107
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117618140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fc7fccd2af985a12c6a6c0d2decd2a77618a858164ee12eb905621a5e02e6dc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 15:48:55 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 15:48:55 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 15:48:56 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 15:49:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 15:49:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 15:49:12 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 15:50:06 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 15:50:07 GMT
ARG MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Tue, 04 Jul 2023 15:50:07 GMT
ENV MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Tue, 04 Jul 2023 15:50:07 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 15:50:07 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 15:50:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 15:50:24 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 15:50:24 GMT
COPY file:60282e2c078282f09827dfb0926d431a7ad71f6de3495a21fc8a846430fc5fc9 in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 15:50:24 GMT
COPY file:704c6685e9d99f08306a2726e0468f5a764a4040cc2eb6138c1be72ac2529bbc in /usr/local/bin/ 
# Tue, 04 Jul 2023 15:50:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 15:50:24 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 15:50:24 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f226d4d968a5322b60d61898c78418afeeb62f9a8613d9939d2546229a59ed0`  
		Last Modified: Tue, 04 Jul 2023 15:53:12 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a718d9544847f819e9859244c57b1093e55eb4bbd1d50066804d9ddd24d9c2c`  
		Last Modified: Tue, 04 Jul 2023 15:53:12 GMT  
		Size: 5.4 MB (5406735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad17cece0015293005bd369ad4550b0faa2ef78f55de897f35a48e5b101b83c8`  
		Last Modified: Tue, 04 Jul 2023 15:53:10 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8210aced70ef3e24a46799929c24c1213867224b74ac675905ac218d01442f43`  
		Last Modified: Tue, 04 Jul 2023 15:54:02 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56cb7b8053f2d91dc92f88f643e2865478be6d9ff1a66c023d0c46ac4354ee4b`  
		Last Modified: Tue, 04 Jul 2023 15:54:11 GMT  
		Size: 83.8 MB (83807029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449424199d1167824fde06f204297c2ba55b2095c8bfd15d6a77aa93b09c7e4b`  
		Last Modified: Tue, 04 Jul 2023 15:54:01 GMT  
		Size: 3.6 KB (3565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3ad0253591ba73c469a1fb8a855ae6c9f69b8c1c7c16163e792da830111d9f`  
		Last Modified: Tue, 04 Jul 2023 15:54:02 GMT  
		Size: 7.6 KB (7568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-jammy` - linux; ppc64le

```console
$ docker pull mariadb@sha256:0f837e667037e0f69042accade3ac2b389154167bcff6ea9e8639eb6fe9f0460
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131775039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8822e9bd24ab2483e7f0ae20339330fcf3c800c3fb250d7115a2b071dddd4ec1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:45:53 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:45:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:45:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:45:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:45:56 GMT
ADD file:8c2fc380378944326d602742fde0e30458cd3e82012847b0f7e09c7184bfd135 in / 
# Wed, 28 Jun 2023 08:45:57 GMT
CMD ["/bin/bash"]
# Wed, 05 Jul 2023 01:06:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 05 Jul 2023 01:06:57 GMT
ENV GOSU_VERSION=1.14
# Wed, 05 Jul 2023 01:06:57 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 05 Jul 2023 01:07:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 05 Jul 2023 01:07:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 05 Jul 2023 01:07:36 GMT
ENV LANG=C.UTF-8
# Wed, 05 Jul 2023 01:10:14 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Wed, 05 Jul 2023 01:10:15 GMT
ARG MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Wed, 05 Jul 2023 01:10:15 GMT
ENV MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Wed, 05 Jul 2023 01:10:16 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
# Wed, 05 Jul 2023 01:10:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 05 Jul 2023 01:11:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Wed, 05 Jul 2023 01:11:10 GMT
VOLUME [/var/lib/mysql]
# Wed, 05 Jul 2023 01:11:10 GMT
COPY file:60282e2c078282f09827dfb0926d431a7ad71f6de3495a21fc8a846430fc5fc9 in /usr/local/bin/healthcheck.sh 
# Wed, 05 Jul 2023 01:11:10 GMT
COPY file:704c6685e9d99f08306a2726e0468f5a764a4040cc2eb6138c1be72ac2529bbc in /usr/local/bin/ 
# Wed, 05 Jul 2023 01:11:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Jul 2023 01:11:11 GMT
EXPOSE 3306
# Wed, 05 Jul 2023 01:11:11 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:7faa46ce6b6f5c34485980029504c3995e38149d0bca67d8b976c5dbb3673644`  
		Last Modified: Tue, 04 Jul 2023 04:42:31 GMT  
		Size: 35.7 MB (35711469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af03c7013049bbb43a9d70711423a0aa0933ad63d557a33679e987f9f4552c2`  
		Last Modified: Wed, 05 Jul 2023 01:19:30 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fae131e82b0a7c398eb2a917463894a99192198e537fa4a742953dfdec5d9a5`  
		Last Modified: Wed, 05 Jul 2023 01:19:32 GMT  
		Size: 6.0 MB (6017861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c002ce052617f5efe1f7afc4ec819f1f45b350c5956b79ee09c9bd522fe18736`  
		Last Modified: Wed, 05 Jul 2023 01:19:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:942ea7aeb70e16124a1ff199ecf228e3ab0281f20f179766b0885587643a240d`  
		Last Modified: Wed, 05 Jul 2023 01:21:05 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:115967ee1bae2b450657e120cfba1533a2768c69fe87802e5a90590ba251d1af`  
		Last Modified: Wed, 05 Jul 2023 01:21:29 GMT  
		Size: 90.0 MB (90032344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981e89a22f465c5f29cd8017aceb5dc84553018d607d0a09802db952f21422e6`  
		Last Modified: Wed, 05 Jul 2023 01:21:05 GMT  
		Size: 3.6 KB (3566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e31cc00f3e6a6786d22d5cc34292a0d4e5b50f8ba265c13862ec1ab1e8ddc49`  
		Last Modified: Wed, 05 Jul 2023 01:21:05 GMT  
		Size: 7.6 KB (7568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-jammy` - linux; s390x

```console
$ docker pull mariadb@sha256:2b727f34069c4b59da2e9dae7fa9f907e91d2bce79801c4bdc33012d4cbe038f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.6 MB (121580518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:378fece5fccb2954bad0c49ec6a7ed1c913335d61542c2a7db9cddf4df77e3d5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:53:20 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:53:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:53:22 GMT
ADD file:fa0aef35be7808c8fd6751a52bdec4dd81057e2fcaa075c547a1db53640dae9a in / 
# Wed, 28 Jun 2023 08:53:22 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 16:55:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 16:55:27 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 16:55:27 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 16:55:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 16:55:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 16:55:44 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 16:56:57 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 16:56:57 GMT
ARG MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Tue, 04 Jul 2023 16:56:57 GMT
ENV MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Tue, 04 Jul 2023 16:56:57 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 16:56:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 16:57:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 16:57:18 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 16:57:18 GMT
COPY file:60282e2c078282f09827dfb0926d431a7ad71f6de3495a21fc8a846430fc5fc9 in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 16:57:18 GMT
COPY file:704c6685e9d99f08306a2726e0468f5a764a4040cc2eb6138c1be72ac2529bbc in /usr/local/bin/ 
# Tue, 04 Jul 2023 16:57:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 16:57:18 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 16:57:18 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:ce02ee0330980398d6a84a50abfa1a8c4d1cba27cbd7442b79f4aa1b1a14020d`  
		Last Modified: Tue, 04 Jul 2023 13:08:30 GMT  
		Size: 28.6 MB (28645696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16fb1ab422c0ae864df4333ba064fd3a16ef9b10862dca7b3320a9fb32c7e0bd`  
		Last Modified: Tue, 04 Jul 2023 17:00:17 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be60fdd8cf07af19113cd853d2f0ebedd02fc5cb31582325b43c0d50a323535`  
		Last Modified: Tue, 04 Jul 2023 17:00:18 GMT  
		Size: 5.5 MB (5470782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1374c790d73360e41f53f0d1a2d9cbaef5dd6c371a1ab7c58c7e20e71945704`  
		Last Modified: Tue, 04 Jul 2023 17:00:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27e7e4b86fecdc32e5bd05e78321e6746840e6a0544d4bedbbdf1c2754a5d72`  
		Last Modified: Tue, 04 Jul 2023 17:01:05 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0090bfea6877acf7ee51c046ee6600b616e08ac7ee48d3fdc628a0167e130e3`  
		Last Modified: Tue, 04 Jul 2023 17:01:18 GMT  
		Size: 87.5 MB (87450671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:093cd65cb7e5e05be6911f64a423e13b6109f3d369f8ac17e7e2584cbe74d8a5`  
		Last Modified: Tue, 04 Jul 2023 17:01:05 GMT  
		Size: 3.6 KB (3568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3082833c7ebee98976c11b8826ef88fa09fa5b139d6b6830488e0ed2a7144e3`  
		Last Modified: Tue, 04 Jul 2023 17:01:05 GMT  
		Size: 7.6 KB (7570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.10`

```console
$ docker pull mariadb@sha256:3c6f07e499298a35fb2087af39e00db4214742c6a05d70ac1614cf504e19ed29
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.10` - linux; amd64

```console
$ docker pull mariadb@sha256:e10c880fb9c36b5055986073a077512e2a6f297ec4fa08bdc5d271d32fb9659f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (123009848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3df0f3d64f437191e1c8f6be2fafac5a8ee5b92020244497c3177547e24a356`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 18:27:16 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 18:27:16 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 18:27:16 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 18:27:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 18:27:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 18:27:39 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 18:29:02 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.10.5 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 18:29:02 GMT
ARG MARIADB_VERSION=1:10.10.5+maria~ubu2204
# Tue, 04 Jul 2023 18:29:02 GMT
ENV MARIADB_VERSION=1:10.10.5+maria~ubu2204
# Tue, 04 Jul 2023 18:29:02 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.5/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 18:29:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.5/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 18:29:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.5/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 18:29:22 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 18:29:22 GMT
COPY file:60282e2c078282f09827dfb0926d431a7ad71f6de3495a21fc8a846430fc5fc9 in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 18:29:22 GMT
COPY file:704c6685e9d99f08306a2726e0468f5a764a4040cc2eb6138c1be72ac2529bbc in /usr/local/bin/ 
# Tue, 04 Jul 2023 18:29:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 18:29:22 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 18:29:22 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:718e898a86ffe915c46f60c599bc87928aa5e7e3a9434cbf52066b49651d3a1f`  
		Last Modified: Tue, 04 Jul 2023 18:32:00 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bd7a143a6c5d92cccbae0a38df554277f44cb4dbfcb668436dc5ed3398144a`  
		Last Modified: Tue, 04 Jul 2023 18:32:01 GMT  
		Size: 5.6 MB (5592713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80cdf483b70a4a08d0db0ff26cb8dbdc933588954a3bf91fce2f2544b7be37b8`  
		Last Modified: Tue, 04 Jul 2023 18:31:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c1119f1a85e0f63e62b5b89d50262467cbed2043fb1e11b67f67a5b8f3a49d`  
		Last Modified: Tue, 04 Jul 2023 18:33:30 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af5d357d87dc3b9c5ded867adf81703d56f9fdf025ba79d719bc6ff195b07f5`  
		Last Modified: Tue, 04 Jul 2023 18:33:42 GMT  
		Size: 87.0 MB (86972545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac6c6bf952818b4e357fed5ba84bf1b25410d472870bd2bc231bf0b1dd945a7`  
		Last Modified: Tue, 04 Jul 2023 18:33:29 GMT  
		Size: 3.6 KB (3567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2428f0f05c3bad59241fb1e208132d997f5b0f9c7c666b07a9b969dcd3638bf7`  
		Last Modified: Tue, 04 Jul 2023 18:33:29 GMT  
		Size: 7.6 KB (7568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.10` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:a8232dbeddfb4b6bc543e767a36b34d3cdd88eb822e64a13b41e3ff0af1c8fb2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117557167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5019b758dcc9cf34c28ca6219e371c592a9e1ec9d1a442d25f58cc6a25a3a5be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 15:48:55 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 15:48:55 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 15:48:56 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 15:49:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 15:49:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 15:49:12 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 15:50:30 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.10.5 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 15:50:30 GMT
ARG MARIADB_VERSION=1:10.10.5+maria~ubu2204
# Tue, 04 Jul 2023 15:50:30 GMT
ENV MARIADB_VERSION=1:10.10.5+maria~ubu2204
# Tue, 04 Jul 2023 15:50:30 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.5/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 15:50:30 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.5/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 15:50:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.5/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 15:50:49 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 15:50:49 GMT
COPY file:60282e2c078282f09827dfb0926d431a7ad71f6de3495a21fc8a846430fc5fc9 in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 15:50:49 GMT
COPY file:704c6685e9d99f08306a2726e0468f5a764a4040cc2eb6138c1be72ac2529bbc in /usr/local/bin/ 
# Tue, 04 Jul 2023 15:50:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 15:50:49 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 15:50:49 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f226d4d968a5322b60d61898c78418afeeb62f9a8613d9939d2546229a59ed0`  
		Last Modified: Tue, 04 Jul 2023 15:53:12 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a718d9544847f819e9859244c57b1093e55eb4bbd1d50066804d9ddd24d9c2c`  
		Last Modified: Tue, 04 Jul 2023 15:53:12 GMT  
		Size: 5.4 MB (5406735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad17cece0015293005bd369ad4550b0faa2ef78f55de897f35a48e5b101b83c8`  
		Last Modified: Tue, 04 Jul 2023 15:53:10 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111d9967141c85bccd6e3616ef88853f1ce3448093c624d53562ecd560fadca3`  
		Last Modified: Tue, 04 Jul 2023 15:54:32 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0064c25d942e4167c2978f86980ee001b495e65e51172ce28d3274512385c881`  
		Last Modified: Tue, 04 Jul 2023 15:54:41 GMT  
		Size: 83.7 MB (83746057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f286fcfa80ee10c181b15b14c293a814a99c59393d188abb7810cb191d5f17`  
		Last Modified: Tue, 04 Jul 2023 15:54:31 GMT  
		Size: 3.6 KB (3564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d7b700188a62c5263a74eb5995fba94005ac056c647b66630a3619bab452643`  
		Last Modified: Tue, 04 Jul 2023 15:54:31 GMT  
		Size: 7.6 KB (7567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.10` - linux; ppc64le

```console
$ docker pull mariadb@sha256:51b43d537b2de725dc7ac4b36d5f8464b801d259f6e8072e8bd4dc6127cc0984
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.7 MB (131692562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d92dcbc11e30c89d8202ef769ed96f5663a89e0d28d2c9644207e52e53960e70`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:45:53 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:45:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:45:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:45:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:45:56 GMT
ADD file:8c2fc380378944326d602742fde0e30458cd3e82012847b0f7e09c7184bfd135 in / 
# Wed, 28 Jun 2023 08:45:57 GMT
CMD ["/bin/bash"]
# Wed, 05 Jul 2023 01:06:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 05 Jul 2023 01:06:57 GMT
ENV GOSU_VERSION=1.14
# Wed, 05 Jul 2023 01:06:57 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 05 Jul 2023 01:07:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 05 Jul 2023 01:07:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 05 Jul 2023 01:07:36 GMT
ENV LANG=C.UTF-8
# Wed, 05 Jul 2023 01:11:24 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.10.5 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Wed, 05 Jul 2023 01:11:25 GMT
ARG MARIADB_VERSION=1:10.10.5+maria~ubu2204
# Wed, 05 Jul 2023 01:11:25 GMT
ENV MARIADB_VERSION=1:10.10.5+maria~ubu2204
# Wed, 05 Jul 2023 01:11:25 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.5/repo/ubuntu/ jammy main
# Wed, 05 Jul 2023 01:11:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.5/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 05 Jul 2023 01:12:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.5/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Wed, 05 Jul 2023 01:12:20 GMT
VOLUME [/var/lib/mysql]
# Wed, 05 Jul 2023 01:12:20 GMT
COPY file:60282e2c078282f09827dfb0926d431a7ad71f6de3495a21fc8a846430fc5fc9 in /usr/local/bin/healthcheck.sh 
# Wed, 05 Jul 2023 01:12:21 GMT
COPY file:704c6685e9d99f08306a2726e0468f5a764a4040cc2eb6138c1be72ac2529bbc in /usr/local/bin/ 
# Wed, 05 Jul 2023 01:12:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Jul 2023 01:12:22 GMT
EXPOSE 3306
# Wed, 05 Jul 2023 01:12:22 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:7faa46ce6b6f5c34485980029504c3995e38149d0bca67d8b976c5dbb3673644`  
		Last Modified: Tue, 04 Jul 2023 04:42:31 GMT  
		Size: 35.7 MB (35711469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af03c7013049bbb43a9d70711423a0aa0933ad63d557a33679e987f9f4552c2`  
		Last Modified: Wed, 05 Jul 2023 01:19:30 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fae131e82b0a7c398eb2a917463894a99192198e537fa4a742953dfdec5d9a5`  
		Last Modified: Wed, 05 Jul 2023 01:19:32 GMT  
		Size: 6.0 MB (6017861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c002ce052617f5efe1f7afc4ec819f1f45b350c5956b79ee09c9bd522fe18736`  
		Last Modified: Wed, 05 Jul 2023 01:19:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70ed38768200acc3f8ffb7aa3716f4e63bfb16d780c019727eff6815968dbf56`  
		Last Modified: Wed, 05 Jul 2023 01:22:01 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4b120544de812cc58b492019f664efac80094f3203969d221a133b4c1df298`  
		Last Modified: Wed, 05 Jul 2023 01:22:26 GMT  
		Size: 89.9 MB (89949876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fc561ff4df70e2ee609b81426cad790a9f2eda69866007852f5bf38ca499bb`  
		Last Modified: Wed, 05 Jul 2023 01:22:01 GMT  
		Size: 3.6 KB (3564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7d226572e2cf0d554f004aa4cdaca337d6b2c2220df69ab72125c4e36529c75`  
		Last Modified: Wed, 05 Jul 2023 01:22:01 GMT  
		Size: 7.6 KB (7564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.10` - linux; s390x

```console
$ docker pull mariadb@sha256:e52b2e1bcac37d8087a7f046cc1dc71e3c25c0f9d377fea2c75e07e50f0ad8f7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.5 MB (121523781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51a3047d3e0689c485772d2ef927d8a8f659fb15905782ea2f0fef3e9d0abc43`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:53:20 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:53:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:53:22 GMT
ADD file:fa0aef35be7808c8fd6751a52bdec4dd81057e2fcaa075c547a1db53640dae9a in / 
# Wed, 28 Jun 2023 08:53:22 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 16:55:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 16:55:27 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 16:55:27 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 16:55:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 16:55:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 16:55:44 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 16:57:25 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.10.5 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 16:57:25 GMT
ARG MARIADB_VERSION=1:10.10.5+maria~ubu2204
# Tue, 04 Jul 2023 16:57:25 GMT
ENV MARIADB_VERSION=1:10.10.5+maria~ubu2204
# Tue, 04 Jul 2023 16:57:25 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.5/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 16:57:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.5/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 16:57:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.5/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 16:57:43 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 16:57:43 GMT
COPY file:60282e2c078282f09827dfb0926d431a7ad71f6de3495a21fc8a846430fc5fc9 in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 16:57:43 GMT
COPY file:704c6685e9d99f08306a2726e0468f5a764a4040cc2eb6138c1be72ac2529bbc in /usr/local/bin/ 
# Tue, 04 Jul 2023 16:57:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 16:57:43 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 16:57:44 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:ce02ee0330980398d6a84a50abfa1a8c4d1cba27cbd7442b79f4aa1b1a14020d`  
		Last Modified: Tue, 04 Jul 2023 13:08:30 GMT  
		Size: 28.6 MB (28645696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16fb1ab422c0ae864df4333ba064fd3a16ef9b10862dca7b3320a9fb32c7e0bd`  
		Last Modified: Tue, 04 Jul 2023 17:00:17 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be60fdd8cf07af19113cd853d2f0ebedd02fc5cb31582325b43c0d50a323535`  
		Last Modified: Tue, 04 Jul 2023 17:00:18 GMT  
		Size: 5.5 MB (5470782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1374c790d73360e41f53f0d1a2d9cbaef5dd6c371a1ab7c58c7e20e71945704`  
		Last Modified: Tue, 04 Jul 2023 17:00:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb43d773f39770eb361e848302b08dc55b09d0c7ae1282f86c5ddb70ec7b54a`  
		Last Modified: Tue, 04 Jul 2023 17:01:31 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6562d699d9175c152e90812a0d3c9be85a76f4b8e5d391982784c376367c1eef`  
		Last Modified: Tue, 04 Jul 2023 17:01:44 GMT  
		Size: 87.4 MB (87393936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34e9ef79549d1de47deef17bf53951da990f44749f81d80948e63d76afb0fbf`  
		Last Modified: Tue, 04 Jul 2023 17:01:31 GMT  
		Size: 3.6 KB (3568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3e7302ecd964dc7340e0cc6e659217e808c6369377865f12785cf1598b15f72`  
		Last Modified: Tue, 04 Jul 2023 17:01:31 GMT  
		Size: 7.6 KB (7570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.10-jammy`

```console
$ docker pull mariadb@sha256:3c6f07e499298a35fb2087af39e00db4214742c6a05d70ac1614cf504e19ed29
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.10-jammy` - linux; amd64

```console
$ docker pull mariadb@sha256:e10c880fb9c36b5055986073a077512e2a6f297ec4fa08bdc5d271d32fb9659f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (123009848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3df0f3d64f437191e1c8f6be2fafac5a8ee5b92020244497c3177547e24a356`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 18:27:16 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 18:27:16 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 18:27:16 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 18:27:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 18:27:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 18:27:39 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 18:29:02 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.10.5 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 18:29:02 GMT
ARG MARIADB_VERSION=1:10.10.5+maria~ubu2204
# Tue, 04 Jul 2023 18:29:02 GMT
ENV MARIADB_VERSION=1:10.10.5+maria~ubu2204
# Tue, 04 Jul 2023 18:29:02 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.5/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 18:29:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.5/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 18:29:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.5/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 18:29:22 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 18:29:22 GMT
COPY file:60282e2c078282f09827dfb0926d431a7ad71f6de3495a21fc8a846430fc5fc9 in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 18:29:22 GMT
COPY file:704c6685e9d99f08306a2726e0468f5a764a4040cc2eb6138c1be72ac2529bbc in /usr/local/bin/ 
# Tue, 04 Jul 2023 18:29:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 18:29:22 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 18:29:22 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:718e898a86ffe915c46f60c599bc87928aa5e7e3a9434cbf52066b49651d3a1f`  
		Last Modified: Tue, 04 Jul 2023 18:32:00 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bd7a143a6c5d92cccbae0a38df554277f44cb4dbfcb668436dc5ed3398144a`  
		Last Modified: Tue, 04 Jul 2023 18:32:01 GMT  
		Size: 5.6 MB (5592713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80cdf483b70a4a08d0db0ff26cb8dbdc933588954a3bf91fce2f2544b7be37b8`  
		Last Modified: Tue, 04 Jul 2023 18:31:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c1119f1a85e0f63e62b5b89d50262467cbed2043fb1e11b67f67a5b8f3a49d`  
		Last Modified: Tue, 04 Jul 2023 18:33:30 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af5d357d87dc3b9c5ded867adf81703d56f9fdf025ba79d719bc6ff195b07f5`  
		Last Modified: Tue, 04 Jul 2023 18:33:42 GMT  
		Size: 87.0 MB (86972545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac6c6bf952818b4e357fed5ba84bf1b25410d472870bd2bc231bf0b1dd945a7`  
		Last Modified: Tue, 04 Jul 2023 18:33:29 GMT  
		Size: 3.6 KB (3567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2428f0f05c3bad59241fb1e208132d997f5b0f9c7c666b07a9b969dcd3638bf7`  
		Last Modified: Tue, 04 Jul 2023 18:33:29 GMT  
		Size: 7.6 KB (7568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.10-jammy` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:a8232dbeddfb4b6bc543e767a36b34d3cdd88eb822e64a13b41e3ff0af1c8fb2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117557167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5019b758dcc9cf34c28ca6219e371c592a9e1ec9d1a442d25f58cc6a25a3a5be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 15:48:55 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 15:48:55 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 15:48:56 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 15:49:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 15:49:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 15:49:12 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 15:50:30 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.10.5 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 15:50:30 GMT
ARG MARIADB_VERSION=1:10.10.5+maria~ubu2204
# Tue, 04 Jul 2023 15:50:30 GMT
ENV MARIADB_VERSION=1:10.10.5+maria~ubu2204
# Tue, 04 Jul 2023 15:50:30 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.5/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 15:50:30 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.5/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 15:50:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.5/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 15:50:49 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 15:50:49 GMT
COPY file:60282e2c078282f09827dfb0926d431a7ad71f6de3495a21fc8a846430fc5fc9 in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 15:50:49 GMT
COPY file:704c6685e9d99f08306a2726e0468f5a764a4040cc2eb6138c1be72ac2529bbc in /usr/local/bin/ 
# Tue, 04 Jul 2023 15:50:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 15:50:49 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 15:50:49 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f226d4d968a5322b60d61898c78418afeeb62f9a8613d9939d2546229a59ed0`  
		Last Modified: Tue, 04 Jul 2023 15:53:12 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a718d9544847f819e9859244c57b1093e55eb4bbd1d50066804d9ddd24d9c2c`  
		Last Modified: Tue, 04 Jul 2023 15:53:12 GMT  
		Size: 5.4 MB (5406735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad17cece0015293005bd369ad4550b0faa2ef78f55de897f35a48e5b101b83c8`  
		Last Modified: Tue, 04 Jul 2023 15:53:10 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111d9967141c85bccd6e3616ef88853f1ce3448093c624d53562ecd560fadca3`  
		Last Modified: Tue, 04 Jul 2023 15:54:32 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0064c25d942e4167c2978f86980ee001b495e65e51172ce28d3274512385c881`  
		Last Modified: Tue, 04 Jul 2023 15:54:41 GMT  
		Size: 83.7 MB (83746057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f286fcfa80ee10c181b15b14c293a814a99c59393d188abb7810cb191d5f17`  
		Last Modified: Tue, 04 Jul 2023 15:54:31 GMT  
		Size: 3.6 KB (3564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d7b700188a62c5263a74eb5995fba94005ac056c647b66630a3619bab452643`  
		Last Modified: Tue, 04 Jul 2023 15:54:31 GMT  
		Size: 7.6 KB (7567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.10-jammy` - linux; ppc64le

```console
$ docker pull mariadb@sha256:51b43d537b2de725dc7ac4b36d5f8464b801d259f6e8072e8bd4dc6127cc0984
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.7 MB (131692562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d92dcbc11e30c89d8202ef769ed96f5663a89e0d28d2c9644207e52e53960e70`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:45:53 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:45:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:45:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:45:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:45:56 GMT
ADD file:8c2fc380378944326d602742fde0e30458cd3e82012847b0f7e09c7184bfd135 in / 
# Wed, 28 Jun 2023 08:45:57 GMT
CMD ["/bin/bash"]
# Wed, 05 Jul 2023 01:06:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 05 Jul 2023 01:06:57 GMT
ENV GOSU_VERSION=1.14
# Wed, 05 Jul 2023 01:06:57 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 05 Jul 2023 01:07:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 05 Jul 2023 01:07:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 05 Jul 2023 01:07:36 GMT
ENV LANG=C.UTF-8
# Wed, 05 Jul 2023 01:11:24 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.10.5 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Wed, 05 Jul 2023 01:11:25 GMT
ARG MARIADB_VERSION=1:10.10.5+maria~ubu2204
# Wed, 05 Jul 2023 01:11:25 GMT
ENV MARIADB_VERSION=1:10.10.5+maria~ubu2204
# Wed, 05 Jul 2023 01:11:25 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.5/repo/ubuntu/ jammy main
# Wed, 05 Jul 2023 01:11:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.5/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 05 Jul 2023 01:12:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.5/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Wed, 05 Jul 2023 01:12:20 GMT
VOLUME [/var/lib/mysql]
# Wed, 05 Jul 2023 01:12:20 GMT
COPY file:60282e2c078282f09827dfb0926d431a7ad71f6de3495a21fc8a846430fc5fc9 in /usr/local/bin/healthcheck.sh 
# Wed, 05 Jul 2023 01:12:21 GMT
COPY file:704c6685e9d99f08306a2726e0468f5a764a4040cc2eb6138c1be72ac2529bbc in /usr/local/bin/ 
# Wed, 05 Jul 2023 01:12:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Jul 2023 01:12:22 GMT
EXPOSE 3306
# Wed, 05 Jul 2023 01:12:22 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:7faa46ce6b6f5c34485980029504c3995e38149d0bca67d8b976c5dbb3673644`  
		Last Modified: Tue, 04 Jul 2023 04:42:31 GMT  
		Size: 35.7 MB (35711469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af03c7013049bbb43a9d70711423a0aa0933ad63d557a33679e987f9f4552c2`  
		Last Modified: Wed, 05 Jul 2023 01:19:30 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fae131e82b0a7c398eb2a917463894a99192198e537fa4a742953dfdec5d9a5`  
		Last Modified: Wed, 05 Jul 2023 01:19:32 GMT  
		Size: 6.0 MB (6017861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c002ce052617f5efe1f7afc4ec819f1f45b350c5956b79ee09c9bd522fe18736`  
		Last Modified: Wed, 05 Jul 2023 01:19:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70ed38768200acc3f8ffb7aa3716f4e63bfb16d780c019727eff6815968dbf56`  
		Last Modified: Wed, 05 Jul 2023 01:22:01 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4b120544de812cc58b492019f664efac80094f3203969d221a133b4c1df298`  
		Last Modified: Wed, 05 Jul 2023 01:22:26 GMT  
		Size: 89.9 MB (89949876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fc561ff4df70e2ee609b81426cad790a9f2eda69866007852f5bf38ca499bb`  
		Last Modified: Wed, 05 Jul 2023 01:22:01 GMT  
		Size: 3.6 KB (3564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7d226572e2cf0d554f004aa4cdaca337d6b2c2220df69ab72125c4e36529c75`  
		Last Modified: Wed, 05 Jul 2023 01:22:01 GMT  
		Size: 7.6 KB (7564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.10-jammy` - linux; s390x

```console
$ docker pull mariadb@sha256:e52b2e1bcac37d8087a7f046cc1dc71e3c25c0f9d377fea2c75e07e50f0ad8f7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.5 MB (121523781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51a3047d3e0689c485772d2ef927d8a8f659fb15905782ea2f0fef3e9d0abc43`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:53:20 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:53:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:53:22 GMT
ADD file:fa0aef35be7808c8fd6751a52bdec4dd81057e2fcaa075c547a1db53640dae9a in / 
# Wed, 28 Jun 2023 08:53:22 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 16:55:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 16:55:27 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 16:55:27 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 16:55:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 16:55:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 16:55:44 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 16:57:25 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.10.5 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 16:57:25 GMT
ARG MARIADB_VERSION=1:10.10.5+maria~ubu2204
# Tue, 04 Jul 2023 16:57:25 GMT
ENV MARIADB_VERSION=1:10.10.5+maria~ubu2204
# Tue, 04 Jul 2023 16:57:25 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.5/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 16:57:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.5/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 16:57:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.5/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 16:57:43 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 16:57:43 GMT
COPY file:60282e2c078282f09827dfb0926d431a7ad71f6de3495a21fc8a846430fc5fc9 in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 16:57:43 GMT
COPY file:704c6685e9d99f08306a2726e0468f5a764a4040cc2eb6138c1be72ac2529bbc in /usr/local/bin/ 
# Tue, 04 Jul 2023 16:57:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 16:57:43 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 16:57:44 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:ce02ee0330980398d6a84a50abfa1a8c4d1cba27cbd7442b79f4aa1b1a14020d`  
		Last Modified: Tue, 04 Jul 2023 13:08:30 GMT  
		Size: 28.6 MB (28645696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16fb1ab422c0ae864df4333ba064fd3a16ef9b10862dca7b3320a9fb32c7e0bd`  
		Last Modified: Tue, 04 Jul 2023 17:00:17 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be60fdd8cf07af19113cd853d2f0ebedd02fc5cb31582325b43c0d50a323535`  
		Last Modified: Tue, 04 Jul 2023 17:00:18 GMT  
		Size: 5.5 MB (5470782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1374c790d73360e41f53f0d1a2d9cbaef5dd6c371a1ab7c58c7e20e71945704`  
		Last Modified: Tue, 04 Jul 2023 17:00:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb43d773f39770eb361e848302b08dc55b09d0c7ae1282f86c5ddb70ec7b54a`  
		Last Modified: Tue, 04 Jul 2023 17:01:31 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6562d699d9175c152e90812a0d3c9be85a76f4b8e5d391982784c376367c1eef`  
		Last Modified: Tue, 04 Jul 2023 17:01:44 GMT  
		Size: 87.4 MB (87393936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34e9ef79549d1de47deef17bf53951da990f44749f81d80948e63d76afb0fbf`  
		Last Modified: Tue, 04 Jul 2023 17:01:31 GMT  
		Size: 3.6 KB (3568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3e7302ecd964dc7340e0cc6e659217e808c6369377865f12785cf1598b15f72`  
		Last Modified: Tue, 04 Jul 2023 17:01:31 GMT  
		Size: 7.6 KB (7570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.10.6`

```console
$ docker pull mariadb@sha256:eb37f58646a901dc7727cf448cae36daaefaba79de33b5058dab79aa4c04aefb
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 0

## `mariadb:10.10.6-jammy`

```console
$ docker pull mariadb@sha256:eb37f58646a901dc7727cf448cae36daaefaba79de33b5058dab79aa4c04aefb
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 0

## `mariadb:10.11`

```console
$ docker pull mariadb@sha256:385c0ba6270307511a511ad915350736602c33fafb3f63f663c853920424c365
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.11` - linux; amd64

```console
$ docker pull mariadb@sha256:4b6b625ae683588d99507ac01b042863d4311b6e15f81d653be6892762637375
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123105947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8b77d250201f61f86a2a98c7e07d5bd77f96b4a345f40f8ce53593c2ffca84d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 18:27:16 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 18:27:16 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 18:27:16 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 18:27:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 18:27:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 18:27:39 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 18:28:38 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 18:28:38 GMT
ARG MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Tue, 04 Jul 2023 18:28:38 GMT
ENV MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Tue, 04 Jul 2023 18:28:38 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 18:28:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 18:28:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 18:28:57 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 18:28:57 GMT
COPY file:60282e2c078282f09827dfb0926d431a7ad71f6de3495a21fc8a846430fc5fc9 in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 18:28:57 GMT
COPY file:704c6685e9d99f08306a2726e0468f5a764a4040cc2eb6138c1be72ac2529bbc in /usr/local/bin/ 
# Tue, 04 Jul 2023 18:28:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 18:28:57 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 18:28:58 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:718e898a86ffe915c46f60c599bc87928aa5e7e3a9434cbf52066b49651d3a1f`  
		Last Modified: Tue, 04 Jul 2023 18:32:00 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bd7a143a6c5d92cccbae0a38df554277f44cb4dbfcb668436dc5ed3398144a`  
		Last Modified: Tue, 04 Jul 2023 18:32:01 GMT  
		Size: 5.6 MB (5592713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80cdf483b70a4a08d0db0ff26cb8dbdc933588954a3bf91fce2f2544b7be37b8`  
		Last Modified: Tue, 04 Jul 2023 18:31:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9531173fe68dc54682bc25ac9b4c270ed5772c4ba6b47daef52a3d4e70af77`  
		Last Modified: Tue, 04 Jul 2023 18:32:56 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7375440478980efc7a168e77a3f085cd056c5f722e11d17a5ef922de66c95f45`  
		Last Modified: Tue, 04 Jul 2023 18:33:09 GMT  
		Size: 87.1 MB (87068650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8be80cd3b8009d3f30675bf4b5402c953d8dfaae942c2fb610a1fab9f826c3`  
		Last Modified: Tue, 04 Jul 2023 18:32:56 GMT  
		Size: 3.6 KB (3565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2384dd133a6708cc48561cd0773fb9abe3b23eae32323d644c2b8c57c8148f3`  
		Last Modified: Tue, 04 Jul 2023 18:32:56 GMT  
		Size: 7.6 KB (7566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.11` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:33e8f9991a22fd6678ef20bf31b2bcecc6fc7c7bea5c62b0144ba4df243ff107
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117618140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fc7fccd2af985a12c6a6c0d2decd2a77618a858164ee12eb905621a5e02e6dc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 15:48:55 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 15:48:55 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 15:48:56 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 15:49:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 15:49:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 15:49:12 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 15:50:06 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 15:50:07 GMT
ARG MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Tue, 04 Jul 2023 15:50:07 GMT
ENV MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Tue, 04 Jul 2023 15:50:07 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 15:50:07 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 15:50:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 15:50:24 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 15:50:24 GMT
COPY file:60282e2c078282f09827dfb0926d431a7ad71f6de3495a21fc8a846430fc5fc9 in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 15:50:24 GMT
COPY file:704c6685e9d99f08306a2726e0468f5a764a4040cc2eb6138c1be72ac2529bbc in /usr/local/bin/ 
# Tue, 04 Jul 2023 15:50:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 15:50:24 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 15:50:24 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f226d4d968a5322b60d61898c78418afeeb62f9a8613d9939d2546229a59ed0`  
		Last Modified: Tue, 04 Jul 2023 15:53:12 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a718d9544847f819e9859244c57b1093e55eb4bbd1d50066804d9ddd24d9c2c`  
		Last Modified: Tue, 04 Jul 2023 15:53:12 GMT  
		Size: 5.4 MB (5406735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad17cece0015293005bd369ad4550b0faa2ef78f55de897f35a48e5b101b83c8`  
		Last Modified: Tue, 04 Jul 2023 15:53:10 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8210aced70ef3e24a46799929c24c1213867224b74ac675905ac218d01442f43`  
		Last Modified: Tue, 04 Jul 2023 15:54:02 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56cb7b8053f2d91dc92f88f643e2865478be6d9ff1a66c023d0c46ac4354ee4b`  
		Last Modified: Tue, 04 Jul 2023 15:54:11 GMT  
		Size: 83.8 MB (83807029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449424199d1167824fde06f204297c2ba55b2095c8bfd15d6a77aa93b09c7e4b`  
		Last Modified: Tue, 04 Jul 2023 15:54:01 GMT  
		Size: 3.6 KB (3565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3ad0253591ba73c469a1fb8a855ae6c9f69b8c1c7c16163e792da830111d9f`  
		Last Modified: Tue, 04 Jul 2023 15:54:02 GMT  
		Size: 7.6 KB (7568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.11` - linux; ppc64le

```console
$ docker pull mariadb@sha256:0f837e667037e0f69042accade3ac2b389154167bcff6ea9e8639eb6fe9f0460
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131775039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8822e9bd24ab2483e7f0ae20339330fcf3c800c3fb250d7115a2b071dddd4ec1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:45:53 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:45:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:45:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:45:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:45:56 GMT
ADD file:8c2fc380378944326d602742fde0e30458cd3e82012847b0f7e09c7184bfd135 in / 
# Wed, 28 Jun 2023 08:45:57 GMT
CMD ["/bin/bash"]
# Wed, 05 Jul 2023 01:06:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 05 Jul 2023 01:06:57 GMT
ENV GOSU_VERSION=1.14
# Wed, 05 Jul 2023 01:06:57 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 05 Jul 2023 01:07:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 05 Jul 2023 01:07:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 05 Jul 2023 01:07:36 GMT
ENV LANG=C.UTF-8
# Wed, 05 Jul 2023 01:10:14 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Wed, 05 Jul 2023 01:10:15 GMT
ARG MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Wed, 05 Jul 2023 01:10:15 GMT
ENV MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Wed, 05 Jul 2023 01:10:16 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
# Wed, 05 Jul 2023 01:10:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 05 Jul 2023 01:11:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Wed, 05 Jul 2023 01:11:10 GMT
VOLUME [/var/lib/mysql]
# Wed, 05 Jul 2023 01:11:10 GMT
COPY file:60282e2c078282f09827dfb0926d431a7ad71f6de3495a21fc8a846430fc5fc9 in /usr/local/bin/healthcheck.sh 
# Wed, 05 Jul 2023 01:11:10 GMT
COPY file:704c6685e9d99f08306a2726e0468f5a764a4040cc2eb6138c1be72ac2529bbc in /usr/local/bin/ 
# Wed, 05 Jul 2023 01:11:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Jul 2023 01:11:11 GMT
EXPOSE 3306
# Wed, 05 Jul 2023 01:11:11 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:7faa46ce6b6f5c34485980029504c3995e38149d0bca67d8b976c5dbb3673644`  
		Last Modified: Tue, 04 Jul 2023 04:42:31 GMT  
		Size: 35.7 MB (35711469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af03c7013049bbb43a9d70711423a0aa0933ad63d557a33679e987f9f4552c2`  
		Last Modified: Wed, 05 Jul 2023 01:19:30 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fae131e82b0a7c398eb2a917463894a99192198e537fa4a742953dfdec5d9a5`  
		Last Modified: Wed, 05 Jul 2023 01:19:32 GMT  
		Size: 6.0 MB (6017861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c002ce052617f5efe1f7afc4ec819f1f45b350c5956b79ee09c9bd522fe18736`  
		Last Modified: Wed, 05 Jul 2023 01:19:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:942ea7aeb70e16124a1ff199ecf228e3ab0281f20f179766b0885587643a240d`  
		Last Modified: Wed, 05 Jul 2023 01:21:05 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:115967ee1bae2b450657e120cfba1533a2768c69fe87802e5a90590ba251d1af`  
		Last Modified: Wed, 05 Jul 2023 01:21:29 GMT  
		Size: 90.0 MB (90032344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981e89a22f465c5f29cd8017aceb5dc84553018d607d0a09802db952f21422e6`  
		Last Modified: Wed, 05 Jul 2023 01:21:05 GMT  
		Size: 3.6 KB (3566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e31cc00f3e6a6786d22d5cc34292a0d4e5b50f8ba265c13862ec1ab1e8ddc49`  
		Last Modified: Wed, 05 Jul 2023 01:21:05 GMT  
		Size: 7.6 KB (7568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.11` - linux; s390x

```console
$ docker pull mariadb@sha256:2b727f34069c4b59da2e9dae7fa9f907e91d2bce79801c4bdc33012d4cbe038f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.6 MB (121580518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:378fece5fccb2954bad0c49ec6a7ed1c913335d61542c2a7db9cddf4df77e3d5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:53:20 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:53:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:53:22 GMT
ADD file:fa0aef35be7808c8fd6751a52bdec4dd81057e2fcaa075c547a1db53640dae9a in / 
# Wed, 28 Jun 2023 08:53:22 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 16:55:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 16:55:27 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 16:55:27 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 16:55:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 16:55:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 16:55:44 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 16:56:57 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 16:56:57 GMT
ARG MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Tue, 04 Jul 2023 16:56:57 GMT
ENV MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Tue, 04 Jul 2023 16:56:57 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 16:56:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 16:57:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 16:57:18 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 16:57:18 GMT
COPY file:60282e2c078282f09827dfb0926d431a7ad71f6de3495a21fc8a846430fc5fc9 in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 16:57:18 GMT
COPY file:704c6685e9d99f08306a2726e0468f5a764a4040cc2eb6138c1be72ac2529bbc in /usr/local/bin/ 
# Tue, 04 Jul 2023 16:57:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 16:57:18 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 16:57:18 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:ce02ee0330980398d6a84a50abfa1a8c4d1cba27cbd7442b79f4aa1b1a14020d`  
		Last Modified: Tue, 04 Jul 2023 13:08:30 GMT  
		Size: 28.6 MB (28645696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16fb1ab422c0ae864df4333ba064fd3a16ef9b10862dca7b3320a9fb32c7e0bd`  
		Last Modified: Tue, 04 Jul 2023 17:00:17 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be60fdd8cf07af19113cd853d2f0ebedd02fc5cb31582325b43c0d50a323535`  
		Last Modified: Tue, 04 Jul 2023 17:00:18 GMT  
		Size: 5.5 MB (5470782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1374c790d73360e41f53f0d1a2d9cbaef5dd6c371a1ab7c58c7e20e71945704`  
		Last Modified: Tue, 04 Jul 2023 17:00:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27e7e4b86fecdc32e5bd05e78321e6746840e6a0544d4bedbbdf1c2754a5d72`  
		Last Modified: Tue, 04 Jul 2023 17:01:05 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0090bfea6877acf7ee51c046ee6600b616e08ac7ee48d3fdc628a0167e130e3`  
		Last Modified: Tue, 04 Jul 2023 17:01:18 GMT  
		Size: 87.5 MB (87450671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:093cd65cb7e5e05be6911f64a423e13b6109f3d369f8ac17e7e2584cbe74d8a5`  
		Last Modified: Tue, 04 Jul 2023 17:01:05 GMT  
		Size: 3.6 KB (3568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3082833c7ebee98976c11b8826ef88fa09fa5b139d6b6830488e0ed2a7144e3`  
		Last Modified: Tue, 04 Jul 2023 17:01:05 GMT  
		Size: 7.6 KB (7570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.11-jammy`

```console
$ docker pull mariadb@sha256:385c0ba6270307511a511ad915350736602c33fafb3f63f663c853920424c365
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.11-jammy` - linux; amd64

```console
$ docker pull mariadb@sha256:4b6b625ae683588d99507ac01b042863d4311b6e15f81d653be6892762637375
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123105947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8b77d250201f61f86a2a98c7e07d5bd77f96b4a345f40f8ce53593c2ffca84d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 18:27:16 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 18:27:16 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 18:27:16 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 18:27:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 18:27:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 18:27:39 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 18:28:38 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 18:28:38 GMT
ARG MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Tue, 04 Jul 2023 18:28:38 GMT
ENV MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Tue, 04 Jul 2023 18:28:38 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 18:28:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 18:28:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 18:28:57 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 18:28:57 GMT
COPY file:60282e2c078282f09827dfb0926d431a7ad71f6de3495a21fc8a846430fc5fc9 in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 18:28:57 GMT
COPY file:704c6685e9d99f08306a2726e0468f5a764a4040cc2eb6138c1be72ac2529bbc in /usr/local/bin/ 
# Tue, 04 Jul 2023 18:28:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 18:28:57 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 18:28:58 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:718e898a86ffe915c46f60c599bc87928aa5e7e3a9434cbf52066b49651d3a1f`  
		Last Modified: Tue, 04 Jul 2023 18:32:00 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bd7a143a6c5d92cccbae0a38df554277f44cb4dbfcb668436dc5ed3398144a`  
		Last Modified: Tue, 04 Jul 2023 18:32:01 GMT  
		Size: 5.6 MB (5592713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80cdf483b70a4a08d0db0ff26cb8dbdc933588954a3bf91fce2f2544b7be37b8`  
		Last Modified: Tue, 04 Jul 2023 18:31:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9531173fe68dc54682bc25ac9b4c270ed5772c4ba6b47daef52a3d4e70af77`  
		Last Modified: Tue, 04 Jul 2023 18:32:56 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7375440478980efc7a168e77a3f085cd056c5f722e11d17a5ef922de66c95f45`  
		Last Modified: Tue, 04 Jul 2023 18:33:09 GMT  
		Size: 87.1 MB (87068650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8be80cd3b8009d3f30675bf4b5402c953d8dfaae942c2fb610a1fab9f826c3`  
		Last Modified: Tue, 04 Jul 2023 18:32:56 GMT  
		Size: 3.6 KB (3565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2384dd133a6708cc48561cd0773fb9abe3b23eae32323d644c2b8c57c8148f3`  
		Last Modified: Tue, 04 Jul 2023 18:32:56 GMT  
		Size: 7.6 KB (7566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.11-jammy` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:33e8f9991a22fd6678ef20bf31b2bcecc6fc7c7bea5c62b0144ba4df243ff107
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117618140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fc7fccd2af985a12c6a6c0d2decd2a77618a858164ee12eb905621a5e02e6dc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 15:48:55 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 15:48:55 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 15:48:56 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 15:49:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 15:49:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 15:49:12 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 15:50:06 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 15:50:07 GMT
ARG MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Tue, 04 Jul 2023 15:50:07 GMT
ENV MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Tue, 04 Jul 2023 15:50:07 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 15:50:07 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 15:50:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 15:50:24 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 15:50:24 GMT
COPY file:60282e2c078282f09827dfb0926d431a7ad71f6de3495a21fc8a846430fc5fc9 in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 15:50:24 GMT
COPY file:704c6685e9d99f08306a2726e0468f5a764a4040cc2eb6138c1be72ac2529bbc in /usr/local/bin/ 
# Tue, 04 Jul 2023 15:50:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 15:50:24 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 15:50:24 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f226d4d968a5322b60d61898c78418afeeb62f9a8613d9939d2546229a59ed0`  
		Last Modified: Tue, 04 Jul 2023 15:53:12 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a718d9544847f819e9859244c57b1093e55eb4bbd1d50066804d9ddd24d9c2c`  
		Last Modified: Tue, 04 Jul 2023 15:53:12 GMT  
		Size: 5.4 MB (5406735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad17cece0015293005bd369ad4550b0faa2ef78f55de897f35a48e5b101b83c8`  
		Last Modified: Tue, 04 Jul 2023 15:53:10 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8210aced70ef3e24a46799929c24c1213867224b74ac675905ac218d01442f43`  
		Last Modified: Tue, 04 Jul 2023 15:54:02 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56cb7b8053f2d91dc92f88f643e2865478be6d9ff1a66c023d0c46ac4354ee4b`  
		Last Modified: Tue, 04 Jul 2023 15:54:11 GMT  
		Size: 83.8 MB (83807029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449424199d1167824fde06f204297c2ba55b2095c8bfd15d6a77aa93b09c7e4b`  
		Last Modified: Tue, 04 Jul 2023 15:54:01 GMT  
		Size: 3.6 KB (3565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3ad0253591ba73c469a1fb8a855ae6c9f69b8c1c7c16163e792da830111d9f`  
		Last Modified: Tue, 04 Jul 2023 15:54:02 GMT  
		Size: 7.6 KB (7568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.11-jammy` - linux; ppc64le

```console
$ docker pull mariadb@sha256:0f837e667037e0f69042accade3ac2b389154167bcff6ea9e8639eb6fe9f0460
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131775039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8822e9bd24ab2483e7f0ae20339330fcf3c800c3fb250d7115a2b071dddd4ec1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:45:53 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:45:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:45:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:45:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:45:56 GMT
ADD file:8c2fc380378944326d602742fde0e30458cd3e82012847b0f7e09c7184bfd135 in / 
# Wed, 28 Jun 2023 08:45:57 GMT
CMD ["/bin/bash"]
# Wed, 05 Jul 2023 01:06:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 05 Jul 2023 01:06:57 GMT
ENV GOSU_VERSION=1.14
# Wed, 05 Jul 2023 01:06:57 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 05 Jul 2023 01:07:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 05 Jul 2023 01:07:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 05 Jul 2023 01:07:36 GMT
ENV LANG=C.UTF-8
# Wed, 05 Jul 2023 01:10:14 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Wed, 05 Jul 2023 01:10:15 GMT
ARG MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Wed, 05 Jul 2023 01:10:15 GMT
ENV MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Wed, 05 Jul 2023 01:10:16 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
# Wed, 05 Jul 2023 01:10:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 05 Jul 2023 01:11:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Wed, 05 Jul 2023 01:11:10 GMT
VOLUME [/var/lib/mysql]
# Wed, 05 Jul 2023 01:11:10 GMT
COPY file:60282e2c078282f09827dfb0926d431a7ad71f6de3495a21fc8a846430fc5fc9 in /usr/local/bin/healthcheck.sh 
# Wed, 05 Jul 2023 01:11:10 GMT
COPY file:704c6685e9d99f08306a2726e0468f5a764a4040cc2eb6138c1be72ac2529bbc in /usr/local/bin/ 
# Wed, 05 Jul 2023 01:11:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Jul 2023 01:11:11 GMT
EXPOSE 3306
# Wed, 05 Jul 2023 01:11:11 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:7faa46ce6b6f5c34485980029504c3995e38149d0bca67d8b976c5dbb3673644`  
		Last Modified: Tue, 04 Jul 2023 04:42:31 GMT  
		Size: 35.7 MB (35711469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af03c7013049bbb43a9d70711423a0aa0933ad63d557a33679e987f9f4552c2`  
		Last Modified: Wed, 05 Jul 2023 01:19:30 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fae131e82b0a7c398eb2a917463894a99192198e537fa4a742953dfdec5d9a5`  
		Last Modified: Wed, 05 Jul 2023 01:19:32 GMT  
		Size: 6.0 MB (6017861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c002ce052617f5efe1f7afc4ec819f1f45b350c5956b79ee09c9bd522fe18736`  
		Last Modified: Wed, 05 Jul 2023 01:19:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:942ea7aeb70e16124a1ff199ecf228e3ab0281f20f179766b0885587643a240d`  
		Last Modified: Wed, 05 Jul 2023 01:21:05 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:115967ee1bae2b450657e120cfba1533a2768c69fe87802e5a90590ba251d1af`  
		Last Modified: Wed, 05 Jul 2023 01:21:29 GMT  
		Size: 90.0 MB (90032344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981e89a22f465c5f29cd8017aceb5dc84553018d607d0a09802db952f21422e6`  
		Last Modified: Wed, 05 Jul 2023 01:21:05 GMT  
		Size: 3.6 KB (3566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e31cc00f3e6a6786d22d5cc34292a0d4e5b50f8ba265c13862ec1ab1e8ddc49`  
		Last Modified: Wed, 05 Jul 2023 01:21:05 GMT  
		Size: 7.6 KB (7568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.11-jammy` - linux; s390x

```console
$ docker pull mariadb@sha256:2b727f34069c4b59da2e9dae7fa9f907e91d2bce79801c4bdc33012d4cbe038f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.6 MB (121580518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:378fece5fccb2954bad0c49ec6a7ed1c913335d61542c2a7db9cddf4df77e3d5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:53:20 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:53:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:53:22 GMT
ADD file:fa0aef35be7808c8fd6751a52bdec4dd81057e2fcaa075c547a1db53640dae9a in / 
# Wed, 28 Jun 2023 08:53:22 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 16:55:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 16:55:27 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 16:55:27 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 16:55:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 16:55:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 16:55:44 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 16:56:57 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 16:56:57 GMT
ARG MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Tue, 04 Jul 2023 16:56:57 GMT
ENV MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Tue, 04 Jul 2023 16:56:57 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 16:56:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 16:57:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 16:57:18 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 16:57:18 GMT
COPY file:60282e2c078282f09827dfb0926d431a7ad71f6de3495a21fc8a846430fc5fc9 in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 16:57:18 GMT
COPY file:704c6685e9d99f08306a2726e0468f5a764a4040cc2eb6138c1be72ac2529bbc in /usr/local/bin/ 
# Tue, 04 Jul 2023 16:57:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 16:57:18 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 16:57:18 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:ce02ee0330980398d6a84a50abfa1a8c4d1cba27cbd7442b79f4aa1b1a14020d`  
		Last Modified: Tue, 04 Jul 2023 13:08:30 GMT  
		Size: 28.6 MB (28645696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16fb1ab422c0ae864df4333ba064fd3a16ef9b10862dca7b3320a9fb32c7e0bd`  
		Last Modified: Tue, 04 Jul 2023 17:00:17 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be60fdd8cf07af19113cd853d2f0ebedd02fc5cb31582325b43c0d50a323535`  
		Last Modified: Tue, 04 Jul 2023 17:00:18 GMT  
		Size: 5.5 MB (5470782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1374c790d73360e41f53f0d1a2d9cbaef5dd6c371a1ab7c58c7e20e71945704`  
		Last Modified: Tue, 04 Jul 2023 17:00:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27e7e4b86fecdc32e5bd05e78321e6746840e6a0544d4bedbbdf1c2754a5d72`  
		Last Modified: Tue, 04 Jul 2023 17:01:05 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0090bfea6877acf7ee51c046ee6600b616e08ac7ee48d3fdc628a0167e130e3`  
		Last Modified: Tue, 04 Jul 2023 17:01:18 GMT  
		Size: 87.5 MB (87450671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:093cd65cb7e5e05be6911f64a423e13b6109f3d369f8ac17e7e2584cbe74d8a5`  
		Last Modified: Tue, 04 Jul 2023 17:01:05 GMT  
		Size: 3.6 KB (3568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3082833c7ebee98976c11b8826ef88fa09fa5b139d6b6830488e0ed2a7144e3`  
		Last Modified: Tue, 04 Jul 2023 17:01:05 GMT  
		Size: 7.6 KB (7570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.11.5`

```console
$ docker pull mariadb@sha256:eb37f58646a901dc7727cf448cae36daaefaba79de33b5058dab79aa4c04aefb
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 0

## `mariadb:10.11.5-jammy`

```console
$ docker pull mariadb@sha256:eb37f58646a901dc7727cf448cae36daaefaba79de33b5058dab79aa4c04aefb
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 0

## `mariadb:10.4`

```console
$ docker pull mariadb@sha256:3ba1ae15411e6505055f07a780c34efdc3c8ff1eab8ee899edfc060afa68effe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4` - linux; amd64

```console
$ docker pull mariadb@sha256:7c7e681f90c8ccc1a89797c3ef1ec19ccadc55fbb769f148a87282118bcd0e9a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.0 MB (119043925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e501f04c12f4cf222fa5d43f655f3b3a7a64a54fe27b0f5cae3d070d854ff98b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:43 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:45 GMT
ADD file:233702cd816c07bc9fed02881b11fb3bdcaee41f3ce3ec1c9f0c4a060b155d5b in / 
# Tue, 01 Aug 2023 06:16:46 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 03:49:46 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 03 Aug 2023 03:49:46 GMT
ENV GOSU_VERSION=1.14
# Thu, 03 Aug 2023 03:49:46 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 03 Aug 2023 03:50:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 03 Aug 2023 03:50:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 03 Aug 2023 03:50:03 GMT
ENV LANG=C.UTF-8
# Thu, 03 Aug 2023 03:50:58 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.4.30 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 03 Aug 2023 03:50:58 GMT
ARG MARIADB_MAJOR=10.4
# Thu, 03 Aug 2023 03:50:58 GMT
ENV MARIADB_MAJOR=10.4
# Thu, 03 Aug 2023 03:50:58 GMT
ARG MARIADB_VERSION=1:10.4.30+maria~ubu2004
# Thu, 03 Aug 2023 03:50:59 GMT
ENV MARIADB_VERSION=1:10.4.30+maria~ubu2004
# Thu, 03 Aug 2023 03:50:59 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.30/repo/ubuntu/ focal main
# Thu, 03 Aug 2023 03:50:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.30/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Aug 2023 03:51:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.30/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 03 Aug 2023 03:51:18 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Aug 2023 03:51:18 GMT
COPY file:d65903e94113c393feb7ef4923c78c7301c6c5d74bc2880bab1896f045005757 in /usr/local/bin/healthcheck.sh 
# Thu, 03 Aug 2023 03:51:19 GMT
COPY file:c949c618eecc4586318fb3f361ab47de11ceab74d2492c4f13f302e2a793ea31 in /usr/local/bin/ 
# Thu, 03 Aug 2023 03:51:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.30/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 03 Aug 2023 03:51:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Aug 2023 03:51:19 GMT
EXPOSE 3306
# Thu, 03 Aug 2023 03:51:19 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d07cf421114a5a250c403ce9a3a93b7298c13ad1c6a57fd1ffdb4e2755868ce`  
		Last Modified: Thu, 03 Aug 2023 03:51:59 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f49892c3e51cdbc8353172618365a3b19a5ef5e2f91ffc7a8ea05aedb7643d0`  
		Last Modified: Thu, 03 Aug 2023 03:52:00 GMT  
		Size: 7.1 MB (7121511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5daef2619c33583cbfa06f371ab8ff5b045c56db124222906abe3996aaa5eb1`  
		Last Modified: Thu, 03 Aug 2023 03:52:00 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4842f413d3788fb86e9822ebfc66bcfa6d33d19ce45676d88a11e61dc71be85a`  
		Last Modified: Thu, 03 Aug 2023 03:52:45 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01533520d8e414fe3dfcc0f3abd1bf98d521a83d3c2eeb5ff0b3664582557927`  
		Last Modified: Thu, 03 Aug 2023 03:52:56 GMT  
		Size: 83.3 MB (83328304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d9dce8ccb475c6348045496f57b1d5adee1efb171b0c8a7caf7e63523095c2`  
		Last Modified: Thu, 03 Aug 2023 03:52:45 GMT  
		Size: 3.6 KB (3567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a6da9eb83839dc8525420038d92eeef1c9d1310b079bb3ec4250660698a4862`  
		Last Modified: Thu, 03 Aug 2023 03:52:45 GMT  
		Size: 7.5 KB (7538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4ad56629547e80f150c9a7bb0f1ece368191f3941e9f41ba668bb9693ff484`  
		Last Modified: Thu, 03 Aug 2023 03:52:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:058196a2852f426c825332b248f9094e4d7b1ce7b84de0ac0aeae4423a2096ed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.6 MB (116592981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c4e87333cf0db58ad016289119639140094490976bfff72b6a5d6a7a0489ccb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 01 Aug 2023 06:20:56 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:20:56 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:20:56 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:20:57 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:21:03 GMT
ADD file:ef6e767091d76c1461d099d5bc7a18c526ec80834cf87280803ab6480192f766 in / 
# Tue, 01 Aug 2023 06:21:03 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 01:26:39 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 03 Aug 2023 01:26:40 GMT
ENV GOSU_VERSION=1.14
# Thu, 03 Aug 2023 01:26:40 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 03 Aug 2023 01:26:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 03 Aug 2023 01:26:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 03 Aug 2023 01:26:55 GMT
ENV LANG=C.UTF-8
# Thu, 03 Aug 2023 01:28:25 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.4.30 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 03 Aug 2023 01:28:25 GMT
ARG MARIADB_MAJOR=10.4
# Thu, 03 Aug 2023 01:28:25 GMT
ENV MARIADB_MAJOR=10.4
# Thu, 03 Aug 2023 01:28:26 GMT
ARG MARIADB_VERSION=1:10.4.30+maria~ubu2004
# Thu, 03 Aug 2023 01:28:26 GMT
ENV MARIADB_VERSION=1:10.4.30+maria~ubu2004
# Thu, 03 Aug 2023 01:28:26 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.30/repo/ubuntu/ focal main
# Thu, 03 Aug 2023 01:28:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.30/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Aug 2023 01:28:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.30/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 03 Aug 2023 01:28:45 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Aug 2023 01:28:45 GMT
COPY file:d65903e94113c393feb7ef4923c78c7301c6c5d74bc2880bab1896f045005757 in /usr/local/bin/healthcheck.sh 
# Thu, 03 Aug 2023 01:28:45 GMT
COPY file:c949c618eecc4586318fb3f361ab47de11ceab74d2492c4f13f302e2a793ea31 in /usr/local/bin/ 
# Thu, 03 Aug 2023 01:28:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.30/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 03 Aug 2023 01:28:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Aug 2023 01:28:46 GMT
EXPOSE 3306
# Thu, 03 Aug 2023 01:28:46 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:edab87ea811e56041127f5e9eb4115fb62cb96d0e6a14056e0d2dbf51a945a22`  
		Last Modified: Wed, 02 Aug 2023 04:28:23 GMT  
		Size: 27.2 MB (27200587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2284a6434f560b2133557b42a6382dceb1dedbb4f91b2e2b8f09c72a90e65901`  
		Last Modified: Thu, 03 Aug 2023 01:29:22 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb060ede2339c044a41658c05b6bd5e977c9b6446d4fe0f02adcd99440ef1f58`  
		Last Modified: Thu, 03 Aug 2023 01:29:23 GMT  
		Size: 6.8 MB (6849661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ed949feb53a8405c2c1a2b71cfb05eb3447b873ffd8c9daa41a13b3ab57552`  
		Last Modified: Thu, 03 Aug 2023 01:29:20 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d27c3f410f888ed2c04b6b43ecbbc515346b649a3fab108f1f794ae499705b`  
		Last Modified: Thu, 03 Aug 2023 01:30:10 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ac8464c9d6f7e39ad14e8e5ca03c2ae68299f922ef2c79f7beadff81bc020a`  
		Last Modified: Thu, 03 Aug 2023 01:30:15 GMT  
		Size: 82.5 MB (82529280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da69c4cc1667dc24beacad3a21a2eafc340fdc6c8c2cc5d3537606193471dcd`  
		Last Modified: Thu, 03 Aug 2023 01:30:06 GMT  
		Size: 3.6 KB (3571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e72f0cf34cfea93e830e1be61722f3c22eb4be683f3f1d397f9406d81496663f`  
		Last Modified: Thu, 03 Aug 2023 01:30:06 GMT  
		Size: 7.5 KB (7541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83cd48be7eb3a5d2eaa955c8da5efaf286cfae7328fcade0cc1af00138b3c89c`  
		Last Modified: Thu, 03 Aug 2023 01:30:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4` - linux; ppc64le

```console
$ docker pull mariadb@sha256:17c6f85c0ca323e288f6742476481a2281bb324a02b77c661e59de16268b6563
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.0 MB (128981828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33c4afe7c7e6504b5f0efdba953b1a15bf79db2c3147efcbb15ecdfa7c7e08a2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 01 Aug 2023 06:20:36 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:20:36 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:20:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:20:37 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:20:40 GMT
ADD file:822df76493d1d533c1a283ab7bb20ce81309f57279422a0eebb2ffb9fab55963 in / 
# Tue, 01 Aug 2023 06:20:40 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 03:10:52 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 03 Aug 2023 03:10:52 GMT
ENV GOSU_VERSION=1.14
# Thu, 03 Aug 2023 03:10:53 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 03 Aug 2023 03:11:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 03 Aug 2023 03:11:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 03 Aug 2023 03:11:46 GMT
ENV LANG=C.UTF-8
# Thu, 03 Aug 2023 03:14:10 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.4.30 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 03 Aug 2023 03:14:11 GMT
ARG MARIADB_MAJOR=10.4
# Thu, 03 Aug 2023 03:14:11 GMT
ENV MARIADB_MAJOR=10.4
# Thu, 03 Aug 2023 03:14:11 GMT
ARG MARIADB_VERSION=1:10.4.30+maria~ubu2004
# Thu, 03 Aug 2023 03:14:12 GMT
ENV MARIADB_VERSION=1:10.4.30+maria~ubu2004
# Thu, 03 Aug 2023 03:14:12 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.30/repo/ubuntu/ focal main
# Thu, 03 Aug 2023 03:14:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.30/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Aug 2023 03:15:01 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.30/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 03 Aug 2023 03:15:06 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Aug 2023 03:15:06 GMT
COPY file:d65903e94113c393feb7ef4923c78c7301c6c5d74bc2880bab1896f045005757 in /usr/local/bin/healthcheck.sh 
# Thu, 03 Aug 2023 03:15:07 GMT
COPY file:c949c618eecc4586318fb3f361ab47de11ceab74d2492c4f13f302e2a793ea31 in /usr/local/bin/ 
# Thu, 03 Aug 2023 03:15:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.30/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 03 Aug 2023 03:15:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Aug 2023 03:15:10 GMT
EXPOSE 3306
# Thu, 03 Aug 2023 03:15:10 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:be0253994e7bea97e6b44cdeec04bf996c8dd3380e70409de3783a1d1971e747`  
		Last Modified: Thu, 03 Aug 2023 02:50:24 GMT  
		Size: 33.3 MB (33306772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48690f21c56aa25403458ebbd3862c5d73e248f8fc2e47199c86fc55cc1f5cb4`  
		Last Modified: Thu, 03 Aug 2023 03:16:24 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0dccff57cc8ee4b6e90243bf698e5cbf73f6255dcf62a2a23e2a797523e267e`  
		Last Modified: Thu, 03 Aug 2023 03:16:26 GMT  
		Size: 7.8 MB (7833713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:922f64b8d88511b05b435916bb5e7f470c4c2390e9f80a153580b6b3b6a3b519`  
		Last Modified: Thu, 03 Aug 2023 03:16:21 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de84f70ebc1d28591e56d2437d3611113132727db457f6336bcfb56f6cdb679`  
		Last Modified: Thu, 03 Aug 2023 03:17:47 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e1d16040c708c19673658665e610169dcd56cc9ed172e4e8438c857c0939e4`  
		Last Modified: Thu, 03 Aug 2023 03:18:09 GMT  
		Size: 87.8 MB (87827891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:add9f7c708278fdd571f50d247fd0ee9d664db1332912e83de3e4334f7444391`  
		Last Modified: Thu, 03 Aug 2023 03:17:47 GMT  
		Size: 3.6 KB (3567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb6dd19ece155f27a0bdc745e8f318fec1a1630c4a47b405aad4d15a7dd05e2`  
		Last Modified: Thu, 03 Aug 2023 03:17:47 GMT  
		Size: 7.5 KB (7537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1770f6abbdbce72a3282a5dd19cf4237b9588d1b2ac0d178cc53ede6abb5681`  
		Last Modified: Thu, 03 Aug 2023 03:17:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4-focal`

```console
$ docker pull mariadb@sha256:3ba1ae15411e6505055f07a780c34efdc3c8ff1eab8ee899edfc060afa68effe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:7c7e681f90c8ccc1a89797c3ef1ec19ccadc55fbb769f148a87282118bcd0e9a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.0 MB (119043925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e501f04c12f4cf222fa5d43f655f3b3a7a64a54fe27b0f5cae3d070d854ff98b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:43 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:45 GMT
ADD file:233702cd816c07bc9fed02881b11fb3bdcaee41f3ce3ec1c9f0c4a060b155d5b in / 
# Tue, 01 Aug 2023 06:16:46 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 03:49:46 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 03 Aug 2023 03:49:46 GMT
ENV GOSU_VERSION=1.14
# Thu, 03 Aug 2023 03:49:46 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 03 Aug 2023 03:50:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 03 Aug 2023 03:50:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 03 Aug 2023 03:50:03 GMT
ENV LANG=C.UTF-8
# Thu, 03 Aug 2023 03:50:58 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.4.30 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 03 Aug 2023 03:50:58 GMT
ARG MARIADB_MAJOR=10.4
# Thu, 03 Aug 2023 03:50:58 GMT
ENV MARIADB_MAJOR=10.4
# Thu, 03 Aug 2023 03:50:58 GMT
ARG MARIADB_VERSION=1:10.4.30+maria~ubu2004
# Thu, 03 Aug 2023 03:50:59 GMT
ENV MARIADB_VERSION=1:10.4.30+maria~ubu2004
# Thu, 03 Aug 2023 03:50:59 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.30/repo/ubuntu/ focal main
# Thu, 03 Aug 2023 03:50:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.30/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Aug 2023 03:51:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.30/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 03 Aug 2023 03:51:18 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Aug 2023 03:51:18 GMT
COPY file:d65903e94113c393feb7ef4923c78c7301c6c5d74bc2880bab1896f045005757 in /usr/local/bin/healthcheck.sh 
# Thu, 03 Aug 2023 03:51:19 GMT
COPY file:c949c618eecc4586318fb3f361ab47de11ceab74d2492c4f13f302e2a793ea31 in /usr/local/bin/ 
# Thu, 03 Aug 2023 03:51:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.30/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 03 Aug 2023 03:51:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Aug 2023 03:51:19 GMT
EXPOSE 3306
# Thu, 03 Aug 2023 03:51:19 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d07cf421114a5a250c403ce9a3a93b7298c13ad1c6a57fd1ffdb4e2755868ce`  
		Last Modified: Thu, 03 Aug 2023 03:51:59 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f49892c3e51cdbc8353172618365a3b19a5ef5e2f91ffc7a8ea05aedb7643d0`  
		Last Modified: Thu, 03 Aug 2023 03:52:00 GMT  
		Size: 7.1 MB (7121511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5daef2619c33583cbfa06f371ab8ff5b045c56db124222906abe3996aaa5eb1`  
		Last Modified: Thu, 03 Aug 2023 03:52:00 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4842f413d3788fb86e9822ebfc66bcfa6d33d19ce45676d88a11e61dc71be85a`  
		Last Modified: Thu, 03 Aug 2023 03:52:45 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01533520d8e414fe3dfcc0f3abd1bf98d521a83d3c2eeb5ff0b3664582557927`  
		Last Modified: Thu, 03 Aug 2023 03:52:56 GMT  
		Size: 83.3 MB (83328304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d9dce8ccb475c6348045496f57b1d5adee1efb171b0c8a7caf7e63523095c2`  
		Last Modified: Thu, 03 Aug 2023 03:52:45 GMT  
		Size: 3.6 KB (3567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a6da9eb83839dc8525420038d92eeef1c9d1310b079bb3ec4250660698a4862`  
		Last Modified: Thu, 03 Aug 2023 03:52:45 GMT  
		Size: 7.5 KB (7538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4ad56629547e80f150c9a7bb0f1ece368191f3941e9f41ba668bb9693ff484`  
		Last Modified: Thu, 03 Aug 2023 03:52:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:058196a2852f426c825332b248f9094e4d7b1ce7b84de0ac0aeae4423a2096ed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.6 MB (116592981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c4e87333cf0db58ad016289119639140094490976bfff72b6a5d6a7a0489ccb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 01 Aug 2023 06:20:56 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:20:56 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:20:56 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:20:57 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:21:03 GMT
ADD file:ef6e767091d76c1461d099d5bc7a18c526ec80834cf87280803ab6480192f766 in / 
# Tue, 01 Aug 2023 06:21:03 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 01:26:39 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 03 Aug 2023 01:26:40 GMT
ENV GOSU_VERSION=1.14
# Thu, 03 Aug 2023 01:26:40 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 03 Aug 2023 01:26:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 03 Aug 2023 01:26:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 03 Aug 2023 01:26:55 GMT
ENV LANG=C.UTF-8
# Thu, 03 Aug 2023 01:28:25 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.4.30 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 03 Aug 2023 01:28:25 GMT
ARG MARIADB_MAJOR=10.4
# Thu, 03 Aug 2023 01:28:25 GMT
ENV MARIADB_MAJOR=10.4
# Thu, 03 Aug 2023 01:28:26 GMT
ARG MARIADB_VERSION=1:10.4.30+maria~ubu2004
# Thu, 03 Aug 2023 01:28:26 GMT
ENV MARIADB_VERSION=1:10.4.30+maria~ubu2004
# Thu, 03 Aug 2023 01:28:26 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.30/repo/ubuntu/ focal main
# Thu, 03 Aug 2023 01:28:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.30/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Aug 2023 01:28:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.30/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 03 Aug 2023 01:28:45 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Aug 2023 01:28:45 GMT
COPY file:d65903e94113c393feb7ef4923c78c7301c6c5d74bc2880bab1896f045005757 in /usr/local/bin/healthcheck.sh 
# Thu, 03 Aug 2023 01:28:45 GMT
COPY file:c949c618eecc4586318fb3f361ab47de11ceab74d2492c4f13f302e2a793ea31 in /usr/local/bin/ 
# Thu, 03 Aug 2023 01:28:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.30/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 03 Aug 2023 01:28:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Aug 2023 01:28:46 GMT
EXPOSE 3306
# Thu, 03 Aug 2023 01:28:46 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:edab87ea811e56041127f5e9eb4115fb62cb96d0e6a14056e0d2dbf51a945a22`  
		Last Modified: Wed, 02 Aug 2023 04:28:23 GMT  
		Size: 27.2 MB (27200587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2284a6434f560b2133557b42a6382dceb1dedbb4f91b2e2b8f09c72a90e65901`  
		Last Modified: Thu, 03 Aug 2023 01:29:22 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb060ede2339c044a41658c05b6bd5e977c9b6446d4fe0f02adcd99440ef1f58`  
		Last Modified: Thu, 03 Aug 2023 01:29:23 GMT  
		Size: 6.8 MB (6849661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ed949feb53a8405c2c1a2b71cfb05eb3447b873ffd8c9daa41a13b3ab57552`  
		Last Modified: Thu, 03 Aug 2023 01:29:20 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d27c3f410f888ed2c04b6b43ecbbc515346b649a3fab108f1f794ae499705b`  
		Last Modified: Thu, 03 Aug 2023 01:30:10 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ac8464c9d6f7e39ad14e8e5ca03c2ae68299f922ef2c79f7beadff81bc020a`  
		Last Modified: Thu, 03 Aug 2023 01:30:15 GMT  
		Size: 82.5 MB (82529280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da69c4cc1667dc24beacad3a21a2eafc340fdc6c8c2cc5d3537606193471dcd`  
		Last Modified: Thu, 03 Aug 2023 01:30:06 GMT  
		Size: 3.6 KB (3571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e72f0cf34cfea93e830e1be61722f3c22eb4be683f3f1d397f9406d81496663f`  
		Last Modified: Thu, 03 Aug 2023 01:30:06 GMT  
		Size: 7.5 KB (7541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83cd48be7eb3a5d2eaa955c8da5efaf286cfae7328fcade0cc1af00138b3c89c`  
		Last Modified: Thu, 03 Aug 2023 01:30:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:17c6f85c0ca323e288f6742476481a2281bb324a02b77c661e59de16268b6563
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.0 MB (128981828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33c4afe7c7e6504b5f0efdba953b1a15bf79db2c3147efcbb15ecdfa7c7e08a2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 01 Aug 2023 06:20:36 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:20:36 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:20:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:20:37 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:20:40 GMT
ADD file:822df76493d1d533c1a283ab7bb20ce81309f57279422a0eebb2ffb9fab55963 in / 
# Tue, 01 Aug 2023 06:20:40 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 03:10:52 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 03 Aug 2023 03:10:52 GMT
ENV GOSU_VERSION=1.14
# Thu, 03 Aug 2023 03:10:53 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 03 Aug 2023 03:11:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 03 Aug 2023 03:11:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 03 Aug 2023 03:11:46 GMT
ENV LANG=C.UTF-8
# Thu, 03 Aug 2023 03:14:10 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.4.30 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 03 Aug 2023 03:14:11 GMT
ARG MARIADB_MAJOR=10.4
# Thu, 03 Aug 2023 03:14:11 GMT
ENV MARIADB_MAJOR=10.4
# Thu, 03 Aug 2023 03:14:11 GMT
ARG MARIADB_VERSION=1:10.4.30+maria~ubu2004
# Thu, 03 Aug 2023 03:14:12 GMT
ENV MARIADB_VERSION=1:10.4.30+maria~ubu2004
# Thu, 03 Aug 2023 03:14:12 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.30/repo/ubuntu/ focal main
# Thu, 03 Aug 2023 03:14:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.30/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Aug 2023 03:15:01 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.30/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 03 Aug 2023 03:15:06 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Aug 2023 03:15:06 GMT
COPY file:d65903e94113c393feb7ef4923c78c7301c6c5d74bc2880bab1896f045005757 in /usr/local/bin/healthcheck.sh 
# Thu, 03 Aug 2023 03:15:07 GMT
COPY file:c949c618eecc4586318fb3f361ab47de11ceab74d2492c4f13f302e2a793ea31 in /usr/local/bin/ 
# Thu, 03 Aug 2023 03:15:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.30/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 03 Aug 2023 03:15:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Aug 2023 03:15:10 GMT
EXPOSE 3306
# Thu, 03 Aug 2023 03:15:10 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:be0253994e7bea97e6b44cdeec04bf996c8dd3380e70409de3783a1d1971e747`  
		Last Modified: Thu, 03 Aug 2023 02:50:24 GMT  
		Size: 33.3 MB (33306772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48690f21c56aa25403458ebbd3862c5d73e248f8fc2e47199c86fc55cc1f5cb4`  
		Last Modified: Thu, 03 Aug 2023 03:16:24 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0dccff57cc8ee4b6e90243bf698e5cbf73f6255dcf62a2a23e2a797523e267e`  
		Last Modified: Thu, 03 Aug 2023 03:16:26 GMT  
		Size: 7.8 MB (7833713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:922f64b8d88511b05b435916bb5e7f470c4c2390e9f80a153580b6b3b6a3b519`  
		Last Modified: Thu, 03 Aug 2023 03:16:21 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de84f70ebc1d28591e56d2437d3611113132727db457f6336bcfb56f6cdb679`  
		Last Modified: Thu, 03 Aug 2023 03:17:47 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e1d16040c708c19673658665e610169dcd56cc9ed172e4e8438c857c0939e4`  
		Last Modified: Thu, 03 Aug 2023 03:18:09 GMT  
		Size: 87.8 MB (87827891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:add9f7c708278fdd571f50d247fd0ee9d664db1332912e83de3e4334f7444391`  
		Last Modified: Thu, 03 Aug 2023 03:17:47 GMT  
		Size: 3.6 KB (3567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb6dd19ece155f27a0bdc745e8f318fec1a1630c4a47b405aad4d15a7dd05e2`  
		Last Modified: Thu, 03 Aug 2023 03:17:47 GMT  
		Size: 7.5 KB (7537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1770f6abbdbce72a3282a5dd19cf4237b9588d1b2ac0d178cc53ede6abb5681`  
		Last Modified: Thu, 03 Aug 2023 03:17:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4.31`

```console
$ docker pull mariadb@sha256:eb37f58646a901dc7727cf448cae36daaefaba79de33b5058dab79aa4c04aefb
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 0

## `mariadb:10.4.31-focal`

```console
$ docker pull mariadb@sha256:eb37f58646a901dc7727cf448cae36daaefaba79de33b5058dab79aa4c04aefb
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 0

## `mariadb:10.5`

```console
$ docker pull mariadb@sha256:f3ec8c1d1cd3d62a21e7c6e3dee4cb33227c7df6dab5644bf2c077e21dfbc63d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.5` - linux; amd64

```console
$ docker pull mariadb@sha256:d956e42fa8eb913150b56bf2d9978dd537d611384bc9c911d84eab51ddeb6c21
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.3 MB (121322823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91c5d89f2dfa3143ada7441f3f0848cc0e93e0bb166085b80888ee49321173ba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:43 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:45 GMT
ADD file:233702cd816c07bc9fed02881b11fb3bdcaee41f3ce3ec1c9f0c4a060b155d5b in / 
# Tue, 01 Aug 2023 06:16:46 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 03:49:46 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 03 Aug 2023 03:49:46 GMT
ENV GOSU_VERSION=1.14
# Thu, 03 Aug 2023 03:49:46 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 03 Aug 2023 03:50:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 03 Aug 2023 03:50:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 03 Aug 2023 03:50:03 GMT
ENV LANG=C.UTF-8
# Thu, 03 Aug 2023 03:50:34 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.5.21 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 03 Aug 2023 03:50:34 GMT
ARG MARIADB_MAJOR=10.5
# Thu, 03 Aug 2023 03:50:34 GMT
ENV MARIADB_MAJOR=10.5
# Thu, 03 Aug 2023 03:50:34 GMT
ARG MARIADB_VERSION=1:10.5.21+maria~ubu2004
# Thu, 03 Aug 2023 03:50:34 GMT
ENV MARIADB_VERSION=1:10.5.21+maria~ubu2004
# Thu, 03 Aug 2023 03:50:34 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.21/repo/ubuntu/ focal main
# Thu, 03 Aug 2023 03:50:35 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.21/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Aug 2023 03:50:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.21/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 03 Aug 2023 03:50:54 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Aug 2023 03:50:54 GMT
COPY file:c534033a3ab62fadd9805cf9184c056c4e093e40393ab02a2d4200993557f120 in /usr/local/bin/healthcheck.sh 
# Thu, 03 Aug 2023 03:50:54 GMT
COPY file:84de1d17cf262b8374dbb86e2371b6d0b6f46c2b7dc9d6dda45d43f280afb75f in /usr/local/bin/ 
# Thu, 03 Aug 2023 03:50:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Aug 2023 03:50:54 GMT
EXPOSE 3306
# Thu, 03 Aug 2023 03:50:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d07cf421114a5a250c403ce9a3a93b7298c13ad1c6a57fd1ffdb4e2755868ce`  
		Last Modified: Thu, 03 Aug 2023 03:51:59 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f49892c3e51cdbc8353172618365a3b19a5ef5e2f91ffc7a8ea05aedb7643d0`  
		Last Modified: Thu, 03 Aug 2023 03:52:00 GMT  
		Size: 7.1 MB (7121511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5daef2619c33583cbfa06f371ab8ff5b045c56db124222906abe3996aaa5eb1`  
		Last Modified: Thu, 03 Aug 2023 03:52:00 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27c7a5445b56824f73fb11544c8ae76939de32facbbd97d8674afeba17ea2455`  
		Last Modified: Thu, 03 Aug 2023 03:52:21 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19767b3c363d97569031ea39564e5e52ce70b70889e967153cdd5d7e0e889c60`  
		Last Modified: Thu, 03 Aug 2023 03:52:33 GMT  
		Size: 85.6 MB (85607323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9071817754e7a4aafb2f8cb92d003af0c29561d78cc6988f5daa225fa40294aa`  
		Last Modified: Thu, 03 Aug 2023 03:52:21 GMT  
		Size: 3.6 KB (3564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e96f8813bbec922e59142d3565d23da3c35b844495c9177dd8f57a4f9f49ab0`  
		Last Modified: Thu, 03 Aug 2023 03:52:21 GMT  
		Size: 7.5 KB (7537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:9fde42fec11a59c459b941b02be7248aa388225d959677a74b9cca9f62e94dce
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.8 MB (118778931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ae9672dfd7d32e095e674021abce2d232d16f688e394c73633d28ab9ac6c922`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 01 Aug 2023 06:20:56 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:20:56 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:20:56 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:20:57 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:21:03 GMT
ADD file:ef6e767091d76c1461d099d5bc7a18c526ec80834cf87280803ab6480192f766 in / 
# Tue, 01 Aug 2023 06:21:03 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 01:26:39 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 03 Aug 2023 01:26:40 GMT
ENV GOSU_VERSION=1.14
# Thu, 03 Aug 2023 01:26:40 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 03 Aug 2023 01:26:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 03 Aug 2023 01:26:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 03 Aug 2023 01:26:55 GMT
ENV LANG=C.UTF-8
# Thu, 03 Aug 2023 01:28:02 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.5.21 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 03 Aug 2023 01:28:02 GMT
ARG MARIADB_MAJOR=10.5
# Thu, 03 Aug 2023 01:28:02 GMT
ENV MARIADB_MAJOR=10.5
# Thu, 03 Aug 2023 01:28:02 GMT
ARG MARIADB_VERSION=1:10.5.21+maria~ubu2004
# Thu, 03 Aug 2023 01:28:02 GMT
ENV MARIADB_VERSION=1:10.5.21+maria~ubu2004
# Thu, 03 Aug 2023 01:28:02 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.21/repo/ubuntu/ focal main
# Thu, 03 Aug 2023 01:28:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.21/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Aug 2023 01:28:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.21/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 03 Aug 2023 01:28:21 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Aug 2023 01:28:21 GMT
COPY file:c534033a3ab62fadd9805cf9184c056c4e093e40393ab02a2d4200993557f120 in /usr/local/bin/healthcheck.sh 
# Thu, 03 Aug 2023 01:28:21 GMT
COPY file:84de1d17cf262b8374dbb86e2371b6d0b6f46c2b7dc9d6dda45d43f280afb75f in /usr/local/bin/ 
# Thu, 03 Aug 2023 01:28:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Aug 2023 01:28:21 GMT
EXPOSE 3306
# Thu, 03 Aug 2023 01:28:21 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:edab87ea811e56041127f5e9eb4115fb62cb96d0e6a14056e0d2dbf51a945a22`  
		Last Modified: Wed, 02 Aug 2023 04:28:23 GMT  
		Size: 27.2 MB (27200587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2284a6434f560b2133557b42a6382dceb1dedbb4f91b2e2b8f09c72a90e65901`  
		Last Modified: Thu, 03 Aug 2023 01:29:22 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb060ede2339c044a41658c05b6bd5e977c9b6446d4fe0f02adcd99440ef1f58`  
		Last Modified: Thu, 03 Aug 2023 01:29:23 GMT  
		Size: 6.8 MB (6849661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ed949feb53a8405c2c1a2b71cfb05eb3447b873ffd8c9daa41a13b3ab57552`  
		Last Modified: Thu, 03 Aug 2023 01:29:20 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7702cb430171b44eabcd1a4bfaeabcb1051dbfe2a1aa884cd7af821fac8273e5`  
		Last Modified: Thu, 03 Aug 2023 01:29:42 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:686f38724a7823d0b26a6b2fb6f7c94b2c0e163a5bb33817431ac095310cc326`  
		Last Modified: Thu, 03 Aug 2023 01:29:52 GMT  
		Size: 84.7 MB (84715361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:042d06030a3b604ee62eada0efcb783a2cc416c076127f45a76d0fa87f5ea46d`  
		Last Modified: Thu, 03 Aug 2023 01:29:42 GMT  
		Size: 3.6 KB (3565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:180147d6aed50312e0d76656d839c7ac77c278be6c94c23cdd27b43df28cbf2b`  
		Last Modified: Thu, 03 Aug 2023 01:29:42 GMT  
		Size: 7.5 KB (7538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; ppc64le

```console
$ docker pull mariadb@sha256:ab99391cd386be32ec9d268a64aca9ab1082de440c8d5fb49c45880ef42de6be
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.2 MB (131245386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b06f2efbfe41809796e7a9ebdd0f6e706749894c2c4fcaecee4d99537b0e3bf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 01 Aug 2023 06:20:36 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:20:36 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:20:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:20:37 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:20:40 GMT
ADD file:822df76493d1d533c1a283ab7bb20ce81309f57279422a0eebb2ffb9fab55963 in / 
# Tue, 01 Aug 2023 06:20:40 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 03:10:52 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 03 Aug 2023 03:10:52 GMT
ENV GOSU_VERSION=1.14
# Thu, 03 Aug 2023 03:10:53 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 03 Aug 2023 03:11:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 03 Aug 2023 03:11:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 03 Aug 2023 03:11:46 GMT
ENV LANG=C.UTF-8
# Thu, 03 Aug 2023 03:13:00 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.5.21 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 03 Aug 2023 03:13:01 GMT
ARG MARIADB_MAJOR=10.5
# Thu, 03 Aug 2023 03:13:01 GMT
ENV MARIADB_MAJOR=10.5
# Thu, 03 Aug 2023 03:13:02 GMT
ARG MARIADB_VERSION=1:10.5.21+maria~ubu2004
# Thu, 03 Aug 2023 03:13:03 GMT
ENV MARIADB_VERSION=1:10.5.21+maria~ubu2004
# Thu, 03 Aug 2023 03:13:03 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.21/repo/ubuntu/ focal main
# Thu, 03 Aug 2023 03:13:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.21/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Aug 2023 03:13:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.21/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 03 Aug 2023 03:14:01 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Aug 2023 03:14:01 GMT
COPY file:c534033a3ab62fadd9805cf9184c056c4e093e40393ab02a2d4200993557f120 in /usr/local/bin/healthcheck.sh 
# Thu, 03 Aug 2023 03:14:01 GMT
COPY file:84de1d17cf262b8374dbb86e2371b6d0b6f46c2b7dc9d6dda45d43f280afb75f in /usr/local/bin/ 
# Thu, 03 Aug 2023 03:14:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Aug 2023 03:14:02 GMT
EXPOSE 3306
# Thu, 03 Aug 2023 03:14:03 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:be0253994e7bea97e6b44cdeec04bf996c8dd3380e70409de3783a1d1971e747`  
		Last Modified: Thu, 03 Aug 2023 02:50:24 GMT  
		Size: 33.3 MB (33306772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48690f21c56aa25403458ebbd3862c5d73e248f8fc2e47199c86fc55cc1f5cb4`  
		Last Modified: Thu, 03 Aug 2023 03:16:24 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0dccff57cc8ee4b6e90243bf698e5cbf73f6255dcf62a2a23e2a797523e267e`  
		Last Modified: Thu, 03 Aug 2023 03:16:26 GMT  
		Size: 7.8 MB (7833713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:922f64b8d88511b05b435916bb5e7f470c4c2390e9f80a153580b6b3b6a3b519`  
		Last Modified: Thu, 03 Aug 2023 03:16:21 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4516815ecec47cdffaaf74d7b1bf15c29bca64410945379b45a71bdc5a4bb99`  
		Last Modified: Thu, 03 Aug 2023 03:17:04 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac682a43e72257262715395465d76bcc3a0482c2100c9339b8c1081ee003ef2`  
		Last Modified: Thu, 03 Aug 2023 03:17:28 GMT  
		Size: 90.1 MB (90091569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb1c1cd684d6a1e76444656f0385142d88b5b270beb55ad092ee868f9d05f5e`  
		Last Modified: Thu, 03 Aug 2023 03:17:04 GMT  
		Size: 3.6 KB (3566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da384fda59d5fbc7ff7fa5c48edb93f10565906b1a521327b4ae1e07572e011c`  
		Last Modified: Thu, 03 Aug 2023 03:17:04 GMT  
		Size: 7.5 KB (7539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; s390x

```console
$ docker pull mariadb@sha256:4ca9e4ece1636bcda9afbaadb94d0475959f7acdd3d9c630931612523046d134
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.5 MB (120538676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3e1770f0f9def0385683b564c390f3e9eb47d40a940f991e60e2aea3c57f428`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 01 Aug 2023 06:17:39 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:17:39 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:17:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:17:39 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:17:41 GMT
ADD file:36efc3ec29bb54e0987fe91be1aa7cc849909b3cd2534af3de2d3d07a03804cf in / 
# Tue, 01 Aug 2023 06:17:41 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 00:00:50 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 03 Aug 2023 00:00:50 GMT
ENV GOSU_VERSION=1.14
# Thu, 03 Aug 2023 00:00:50 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 03 Aug 2023 00:01:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 03 Aug 2023 00:01:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 03 Aug 2023 00:01:22 GMT
ENV LANG=C.UTF-8
# Thu, 03 Aug 2023 00:02:09 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.5.21 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 03 Aug 2023 00:02:09 GMT
ARG MARIADB_MAJOR=10.5
# Thu, 03 Aug 2023 00:02:09 GMT
ENV MARIADB_MAJOR=10.5
# Thu, 03 Aug 2023 00:02:09 GMT
ARG MARIADB_VERSION=1:10.5.21+maria~ubu2004
# Thu, 03 Aug 2023 00:02:09 GMT
ENV MARIADB_VERSION=1:10.5.21+maria~ubu2004
# Thu, 03 Aug 2023 00:02:09 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.21/repo/ubuntu/ focal main
# Thu, 03 Aug 2023 00:02:10 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.21/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Aug 2023 00:02:31 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.21/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 03 Aug 2023 00:02:35 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Aug 2023 00:02:35 GMT
COPY file:c534033a3ab62fadd9805cf9184c056c4e093e40393ab02a2d4200993557f120 in /usr/local/bin/healthcheck.sh 
# Thu, 03 Aug 2023 00:02:35 GMT
COPY file:84de1d17cf262b8374dbb86e2371b6d0b6f46c2b7dc9d6dda45d43f280afb75f in /usr/local/bin/ 
# Thu, 03 Aug 2023 00:02:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Aug 2023 00:02:36 GMT
EXPOSE 3306
# Thu, 03 Aug 2023 00:02:36 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:365fa2124eb5f6f369204f3fe0210d9965952628707dfacd4194a8e15caf0420`  
		Last Modified: Thu, 03 Aug 2023 00:03:37 GMT  
		Size: 27.0 MB (27014233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0adb725e694cf559e6a39a507c55bd0249efdb6249fe800a853d6ff58f42e65b`  
		Last Modified: Thu, 03 Aug 2023 00:03:33 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a570866ba929cce3eb9fb0d52a61756244ac3f17c4e5825e2d036d500b17c6f`  
		Last Modified: Thu, 03 Aug 2023 00:03:33 GMT  
		Size: 6.7 MB (6672025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e4a7ce2693e5abd7571288813bf6e7e1c2ef88aa663172fb337b178235a940`  
		Last Modified: Thu, 03 Aug 2023 00:03:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f95940b2e7809ea742ab6b0ae3b56abd5c551286eb0dca19cd8690a9eed446`  
		Last Modified: Thu, 03 Aug 2023 00:03:54 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c58fa69c942bce9238ba89f6fa1345b73e29e505599d557c44fa96df5d30f8e`  
		Last Modified: Thu, 03 Aug 2023 00:04:08 GMT  
		Size: 86.8 MB (86839097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d38f09e6172e7e96a004fb65031a521a3c6d2914a5ee26a1a1f0b1b092545d4e`  
		Last Modified: Thu, 03 Aug 2023 00:03:54 GMT  
		Size: 3.6 KB (3564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5404d852124df867e7ff71828ecbe57a7a4756fc138072768138b1c417e3e05`  
		Last Modified: Thu, 03 Aug 2023 00:03:54 GMT  
		Size: 7.5 KB (7534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5-focal`

```console
$ docker pull mariadb@sha256:f3ec8c1d1cd3d62a21e7c6e3dee4cb33227c7df6dab5644bf2c077e21dfbc63d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.5-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:d956e42fa8eb913150b56bf2d9978dd537d611384bc9c911d84eab51ddeb6c21
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.3 MB (121322823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91c5d89f2dfa3143ada7441f3f0848cc0e93e0bb166085b80888ee49321173ba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:43 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:45 GMT
ADD file:233702cd816c07bc9fed02881b11fb3bdcaee41f3ce3ec1c9f0c4a060b155d5b in / 
# Tue, 01 Aug 2023 06:16:46 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 03:49:46 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 03 Aug 2023 03:49:46 GMT
ENV GOSU_VERSION=1.14
# Thu, 03 Aug 2023 03:49:46 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 03 Aug 2023 03:50:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 03 Aug 2023 03:50:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 03 Aug 2023 03:50:03 GMT
ENV LANG=C.UTF-8
# Thu, 03 Aug 2023 03:50:34 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.5.21 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 03 Aug 2023 03:50:34 GMT
ARG MARIADB_MAJOR=10.5
# Thu, 03 Aug 2023 03:50:34 GMT
ENV MARIADB_MAJOR=10.5
# Thu, 03 Aug 2023 03:50:34 GMT
ARG MARIADB_VERSION=1:10.5.21+maria~ubu2004
# Thu, 03 Aug 2023 03:50:34 GMT
ENV MARIADB_VERSION=1:10.5.21+maria~ubu2004
# Thu, 03 Aug 2023 03:50:34 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.21/repo/ubuntu/ focal main
# Thu, 03 Aug 2023 03:50:35 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.21/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Aug 2023 03:50:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.21/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 03 Aug 2023 03:50:54 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Aug 2023 03:50:54 GMT
COPY file:c534033a3ab62fadd9805cf9184c056c4e093e40393ab02a2d4200993557f120 in /usr/local/bin/healthcheck.sh 
# Thu, 03 Aug 2023 03:50:54 GMT
COPY file:84de1d17cf262b8374dbb86e2371b6d0b6f46c2b7dc9d6dda45d43f280afb75f in /usr/local/bin/ 
# Thu, 03 Aug 2023 03:50:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Aug 2023 03:50:54 GMT
EXPOSE 3306
# Thu, 03 Aug 2023 03:50:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d07cf421114a5a250c403ce9a3a93b7298c13ad1c6a57fd1ffdb4e2755868ce`  
		Last Modified: Thu, 03 Aug 2023 03:51:59 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f49892c3e51cdbc8353172618365a3b19a5ef5e2f91ffc7a8ea05aedb7643d0`  
		Last Modified: Thu, 03 Aug 2023 03:52:00 GMT  
		Size: 7.1 MB (7121511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5daef2619c33583cbfa06f371ab8ff5b045c56db124222906abe3996aaa5eb1`  
		Last Modified: Thu, 03 Aug 2023 03:52:00 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27c7a5445b56824f73fb11544c8ae76939de32facbbd97d8674afeba17ea2455`  
		Last Modified: Thu, 03 Aug 2023 03:52:21 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19767b3c363d97569031ea39564e5e52ce70b70889e967153cdd5d7e0e889c60`  
		Last Modified: Thu, 03 Aug 2023 03:52:33 GMT  
		Size: 85.6 MB (85607323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9071817754e7a4aafb2f8cb92d003af0c29561d78cc6988f5daa225fa40294aa`  
		Last Modified: Thu, 03 Aug 2023 03:52:21 GMT  
		Size: 3.6 KB (3564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e96f8813bbec922e59142d3565d23da3c35b844495c9177dd8f57a4f9f49ab0`  
		Last Modified: Thu, 03 Aug 2023 03:52:21 GMT  
		Size: 7.5 KB (7537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:9fde42fec11a59c459b941b02be7248aa388225d959677a74b9cca9f62e94dce
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.8 MB (118778931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ae9672dfd7d32e095e674021abce2d232d16f688e394c73633d28ab9ac6c922`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 01 Aug 2023 06:20:56 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:20:56 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:20:56 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:20:57 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:21:03 GMT
ADD file:ef6e767091d76c1461d099d5bc7a18c526ec80834cf87280803ab6480192f766 in / 
# Tue, 01 Aug 2023 06:21:03 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 01:26:39 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 03 Aug 2023 01:26:40 GMT
ENV GOSU_VERSION=1.14
# Thu, 03 Aug 2023 01:26:40 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 03 Aug 2023 01:26:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 03 Aug 2023 01:26:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 03 Aug 2023 01:26:55 GMT
ENV LANG=C.UTF-8
# Thu, 03 Aug 2023 01:28:02 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.5.21 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 03 Aug 2023 01:28:02 GMT
ARG MARIADB_MAJOR=10.5
# Thu, 03 Aug 2023 01:28:02 GMT
ENV MARIADB_MAJOR=10.5
# Thu, 03 Aug 2023 01:28:02 GMT
ARG MARIADB_VERSION=1:10.5.21+maria~ubu2004
# Thu, 03 Aug 2023 01:28:02 GMT
ENV MARIADB_VERSION=1:10.5.21+maria~ubu2004
# Thu, 03 Aug 2023 01:28:02 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.21/repo/ubuntu/ focal main
# Thu, 03 Aug 2023 01:28:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.21/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Aug 2023 01:28:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.21/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 03 Aug 2023 01:28:21 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Aug 2023 01:28:21 GMT
COPY file:c534033a3ab62fadd9805cf9184c056c4e093e40393ab02a2d4200993557f120 in /usr/local/bin/healthcheck.sh 
# Thu, 03 Aug 2023 01:28:21 GMT
COPY file:84de1d17cf262b8374dbb86e2371b6d0b6f46c2b7dc9d6dda45d43f280afb75f in /usr/local/bin/ 
# Thu, 03 Aug 2023 01:28:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Aug 2023 01:28:21 GMT
EXPOSE 3306
# Thu, 03 Aug 2023 01:28:21 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:edab87ea811e56041127f5e9eb4115fb62cb96d0e6a14056e0d2dbf51a945a22`  
		Last Modified: Wed, 02 Aug 2023 04:28:23 GMT  
		Size: 27.2 MB (27200587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2284a6434f560b2133557b42a6382dceb1dedbb4f91b2e2b8f09c72a90e65901`  
		Last Modified: Thu, 03 Aug 2023 01:29:22 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb060ede2339c044a41658c05b6bd5e977c9b6446d4fe0f02adcd99440ef1f58`  
		Last Modified: Thu, 03 Aug 2023 01:29:23 GMT  
		Size: 6.8 MB (6849661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ed949feb53a8405c2c1a2b71cfb05eb3447b873ffd8c9daa41a13b3ab57552`  
		Last Modified: Thu, 03 Aug 2023 01:29:20 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7702cb430171b44eabcd1a4bfaeabcb1051dbfe2a1aa884cd7af821fac8273e5`  
		Last Modified: Thu, 03 Aug 2023 01:29:42 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:686f38724a7823d0b26a6b2fb6f7c94b2c0e163a5bb33817431ac095310cc326`  
		Last Modified: Thu, 03 Aug 2023 01:29:52 GMT  
		Size: 84.7 MB (84715361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:042d06030a3b604ee62eada0efcb783a2cc416c076127f45a76d0fa87f5ea46d`  
		Last Modified: Thu, 03 Aug 2023 01:29:42 GMT  
		Size: 3.6 KB (3565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:180147d6aed50312e0d76656d839c7ac77c278be6c94c23cdd27b43df28cbf2b`  
		Last Modified: Thu, 03 Aug 2023 01:29:42 GMT  
		Size: 7.5 KB (7538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:ab99391cd386be32ec9d268a64aca9ab1082de440c8d5fb49c45880ef42de6be
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.2 MB (131245386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b06f2efbfe41809796e7a9ebdd0f6e706749894c2c4fcaecee4d99537b0e3bf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 01 Aug 2023 06:20:36 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:20:36 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:20:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:20:37 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:20:40 GMT
ADD file:822df76493d1d533c1a283ab7bb20ce81309f57279422a0eebb2ffb9fab55963 in / 
# Tue, 01 Aug 2023 06:20:40 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 03:10:52 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 03 Aug 2023 03:10:52 GMT
ENV GOSU_VERSION=1.14
# Thu, 03 Aug 2023 03:10:53 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 03 Aug 2023 03:11:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 03 Aug 2023 03:11:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 03 Aug 2023 03:11:46 GMT
ENV LANG=C.UTF-8
# Thu, 03 Aug 2023 03:13:00 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.5.21 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 03 Aug 2023 03:13:01 GMT
ARG MARIADB_MAJOR=10.5
# Thu, 03 Aug 2023 03:13:01 GMT
ENV MARIADB_MAJOR=10.5
# Thu, 03 Aug 2023 03:13:02 GMT
ARG MARIADB_VERSION=1:10.5.21+maria~ubu2004
# Thu, 03 Aug 2023 03:13:03 GMT
ENV MARIADB_VERSION=1:10.5.21+maria~ubu2004
# Thu, 03 Aug 2023 03:13:03 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.21/repo/ubuntu/ focal main
# Thu, 03 Aug 2023 03:13:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.21/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Aug 2023 03:13:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.21/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 03 Aug 2023 03:14:01 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Aug 2023 03:14:01 GMT
COPY file:c534033a3ab62fadd9805cf9184c056c4e093e40393ab02a2d4200993557f120 in /usr/local/bin/healthcheck.sh 
# Thu, 03 Aug 2023 03:14:01 GMT
COPY file:84de1d17cf262b8374dbb86e2371b6d0b6f46c2b7dc9d6dda45d43f280afb75f in /usr/local/bin/ 
# Thu, 03 Aug 2023 03:14:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Aug 2023 03:14:02 GMT
EXPOSE 3306
# Thu, 03 Aug 2023 03:14:03 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:be0253994e7bea97e6b44cdeec04bf996c8dd3380e70409de3783a1d1971e747`  
		Last Modified: Thu, 03 Aug 2023 02:50:24 GMT  
		Size: 33.3 MB (33306772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48690f21c56aa25403458ebbd3862c5d73e248f8fc2e47199c86fc55cc1f5cb4`  
		Last Modified: Thu, 03 Aug 2023 03:16:24 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0dccff57cc8ee4b6e90243bf698e5cbf73f6255dcf62a2a23e2a797523e267e`  
		Last Modified: Thu, 03 Aug 2023 03:16:26 GMT  
		Size: 7.8 MB (7833713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:922f64b8d88511b05b435916bb5e7f470c4c2390e9f80a153580b6b3b6a3b519`  
		Last Modified: Thu, 03 Aug 2023 03:16:21 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4516815ecec47cdffaaf74d7b1bf15c29bca64410945379b45a71bdc5a4bb99`  
		Last Modified: Thu, 03 Aug 2023 03:17:04 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac682a43e72257262715395465d76bcc3a0482c2100c9339b8c1081ee003ef2`  
		Last Modified: Thu, 03 Aug 2023 03:17:28 GMT  
		Size: 90.1 MB (90091569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb1c1cd684d6a1e76444656f0385142d88b5b270beb55ad092ee868f9d05f5e`  
		Last Modified: Thu, 03 Aug 2023 03:17:04 GMT  
		Size: 3.6 KB (3566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da384fda59d5fbc7ff7fa5c48edb93f10565906b1a521327b4ae1e07572e011c`  
		Last Modified: Thu, 03 Aug 2023 03:17:04 GMT  
		Size: 7.5 KB (7539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:4ca9e4ece1636bcda9afbaadb94d0475959f7acdd3d9c630931612523046d134
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.5 MB (120538676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3e1770f0f9def0385683b564c390f3e9eb47d40a940f991e60e2aea3c57f428`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 01 Aug 2023 06:17:39 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:17:39 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:17:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:17:39 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:17:41 GMT
ADD file:36efc3ec29bb54e0987fe91be1aa7cc849909b3cd2534af3de2d3d07a03804cf in / 
# Tue, 01 Aug 2023 06:17:41 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 00:00:50 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 03 Aug 2023 00:00:50 GMT
ENV GOSU_VERSION=1.14
# Thu, 03 Aug 2023 00:00:50 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 03 Aug 2023 00:01:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 03 Aug 2023 00:01:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 03 Aug 2023 00:01:22 GMT
ENV LANG=C.UTF-8
# Thu, 03 Aug 2023 00:02:09 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.5.21 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 03 Aug 2023 00:02:09 GMT
ARG MARIADB_MAJOR=10.5
# Thu, 03 Aug 2023 00:02:09 GMT
ENV MARIADB_MAJOR=10.5
# Thu, 03 Aug 2023 00:02:09 GMT
ARG MARIADB_VERSION=1:10.5.21+maria~ubu2004
# Thu, 03 Aug 2023 00:02:09 GMT
ENV MARIADB_VERSION=1:10.5.21+maria~ubu2004
# Thu, 03 Aug 2023 00:02:09 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.21/repo/ubuntu/ focal main
# Thu, 03 Aug 2023 00:02:10 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.21/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Aug 2023 00:02:31 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.21/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 03 Aug 2023 00:02:35 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Aug 2023 00:02:35 GMT
COPY file:c534033a3ab62fadd9805cf9184c056c4e093e40393ab02a2d4200993557f120 in /usr/local/bin/healthcheck.sh 
# Thu, 03 Aug 2023 00:02:35 GMT
COPY file:84de1d17cf262b8374dbb86e2371b6d0b6f46c2b7dc9d6dda45d43f280afb75f in /usr/local/bin/ 
# Thu, 03 Aug 2023 00:02:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Aug 2023 00:02:36 GMT
EXPOSE 3306
# Thu, 03 Aug 2023 00:02:36 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:365fa2124eb5f6f369204f3fe0210d9965952628707dfacd4194a8e15caf0420`  
		Last Modified: Thu, 03 Aug 2023 00:03:37 GMT  
		Size: 27.0 MB (27014233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0adb725e694cf559e6a39a507c55bd0249efdb6249fe800a853d6ff58f42e65b`  
		Last Modified: Thu, 03 Aug 2023 00:03:33 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a570866ba929cce3eb9fb0d52a61756244ac3f17c4e5825e2d036d500b17c6f`  
		Last Modified: Thu, 03 Aug 2023 00:03:33 GMT  
		Size: 6.7 MB (6672025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e4a7ce2693e5abd7571288813bf6e7e1c2ef88aa663172fb337b178235a940`  
		Last Modified: Thu, 03 Aug 2023 00:03:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f95940b2e7809ea742ab6b0ae3b56abd5c551286eb0dca19cd8690a9eed446`  
		Last Modified: Thu, 03 Aug 2023 00:03:54 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c58fa69c942bce9238ba89f6fa1345b73e29e505599d557c44fa96df5d30f8e`  
		Last Modified: Thu, 03 Aug 2023 00:04:08 GMT  
		Size: 86.8 MB (86839097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d38f09e6172e7e96a004fb65031a521a3c6d2914a5ee26a1a1f0b1b092545d4e`  
		Last Modified: Thu, 03 Aug 2023 00:03:54 GMT  
		Size: 3.6 KB (3564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5404d852124df867e7ff71828ecbe57a7a4756fc138072768138b1c417e3e05`  
		Last Modified: Thu, 03 Aug 2023 00:03:54 GMT  
		Size: 7.5 KB (7534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5.22`

```console
$ docker pull mariadb@sha256:eb37f58646a901dc7727cf448cae36daaefaba79de33b5058dab79aa4c04aefb
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 0

## `mariadb:10.5.22-focal`

```console
$ docker pull mariadb@sha256:eb37f58646a901dc7727cf448cae36daaefaba79de33b5058dab79aa4c04aefb
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 0

## `mariadb:10.6`

```console
$ docker pull mariadb@sha256:9156c6c088e554b19bdcad795f5b536d5796766806935da63d1268bc647f05b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.6` - linux; amd64

```console
$ docker pull mariadb@sha256:0ecd837a038b6c64a4a046cec70618e306ecbb2d7c044c746912297dae1e3a93
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.6 MB (121632866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf6aa23aa4ff3d40153afcd1cae6e311a4530f54041f25a909a1c9b7339fa5b3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:43 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:45 GMT
ADD file:233702cd816c07bc9fed02881b11fb3bdcaee41f3ce3ec1c9f0c4a060b155d5b in / 
# Tue, 01 Aug 2023 06:16:46 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 03:49:46 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 03 Aug 2023 03:49:46 GMT
ENV GOSU_VERSION=1.14
# Thu, 03 Aug 2023 03:49:46 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 03 Aug 2023 03:50:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 03 Aug 2023 03:50:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 03 Aug 2023 03:50:03 GMT
ENV LANG=C.UTF-8
# Thu, 03 Aug 2023 03:50:03 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.6.14 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 03 Aug 2023 03:50:04 GMT
ARG MARIADB_MAJOR=10.6
# Thu, 03 Aug 2023 03:50:04 GMT
ENV MARIADB_MAJOR=10.6
# Thu, 03 Aug 2023 03:50:04 GMT
ARG MARIADB_VERSION=1:10.6.14+maria~ubu2004
# Thu, 03 Aug 2023 03:50:04 GMT
ENV MARIADB_VERSION=1:10.6.14+maria~ubu2004
# Thu, 03 Aug 2023 03:50:04 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.14/repo/ubuntu/ focal main
# Thu, 03 Aug 2023 03:50:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.14/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Aug 2023 03:50:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.14/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 03 Aug 2023 03:50:27 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Aug 2023 03:50:27 GMT
COPY file:60282e2c078282f09827dfb0926d431a7ad71f6de3495a21fc8a846430fc5fc9 in /usr/local/bin/healthcheck.sh 
# Thu, 03 Aug 2023 03:50:27 GMT
COPY file:704c6685e9d99f08306a2726e0468f5a764a4040cc2eb6138c1be72ac2529bbc in /usr/local/bin/ 
# Thu, 03 Aug 2023 03:50:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Aug 2023 03:50:27 GMT
EXPOSE 3306
# Thu, 03 Aug 2023 03:50:27 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d07cf421114a5a250c403ce9a3a93b7298c13ad1c6a57fd1ffdb4e2755868ce`  
		Last Modified: Thu, 03 Aug 2023 03:51:59 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f49892c3e51cdbc8353172618365a3b19a5ef5e2f91ffc7a8ea05aedb7643d0`  
		Last Modified: Thu, 03 Aug 2023 03:52:00 GMT  
		Size: 7.1 MB (7121511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5daef2619c33583cbfa06f371ab8ff5b045c56db124222906abe3996aaa5eb1`  
		Last Modified: Thu, 03 Aug 2023 03:52:00 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59c36b808a2839fb44ca1b6c4ca60b409c00345ee3567dce18bfb97b8b6c7c0`  
		Last Modified: Thu, 03 Aug 2023 03:51:57 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d12450bcf979a36f64c4019a5e4a6b3bd8b7a00c86b142863fcc15130b141516`  
		Last Modified: Thu, 03 Aug 2023 03:52:09 GMT  
		Size: 85.9 MB (85917337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11011cbf6a2acf48a7b6646cec4b8df7d275284a50dbcab99acda9240ed06f47`  
		Last Modified: Thu, 03 Aug 2023 03:51:57 GMT  
		Size: 3.6 KB (3566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc6463f1b65f394ee1e47b0eaf189c705f9f31b5aa8910e8ec1848d1b364ced9`  
		Last Modified: Thu, 03 Aug 2023 03:51:57 GMT  
		Size: 7.6 KB (7568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:805190f08efde33e24fded93fe7c61fccd47b9a21a402ba083a48f826e005ec5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.9 MB (118945985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53898260b9e47ef8b10962ee6acda2df4ce788131cfbc8ca99a63da9a19c4cef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 01 Aug 2023 06:20:56 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:20:56 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:20:56 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:20:57 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:21:03 GMT
ADD file:ef6e767091d76c1461d099d5bc7a18c526ec80834cf87280803ab6480192f766 in / 
# Tue, 01 Aug 2023 06:21:03 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 01:26:39 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 03 Aug 2023 01:26:40 GMT
ENV GOSU_VERSION=1.14
# Thu, 03 Aug 2023 01:26:40 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 03 Aug 2023 01:26:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 03 Aug 2023 01:26:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 03 Aug 2023 01:26:55 GMT
ENV LANG=C.UTF-8
# Thu, 03 Aug 2023 01:26:55 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.6.14 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 03 Aug 2023 01:26:55 GMT
ARG MARIADB_MAJOR=10.6
# Thu, 03 Aug 2023 01:26:55 GMT
ENV MARIADB_MAJOR=10.6
# Thu, 03 Aug 2023 01:26:55 GMT
ARG MARIADB_VERSION=1:10.6.14+maria~ubu2004
# Thu, 03 Aug 2023 01:26:55 GMT
ENV MARIADB_VERSION=1:10.6.14+maria~ubu2004
# Thu, 03 Aug 2023 01:26:56 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.14/repo/ubuntu/ focal main
# Thu, 03 Aug 2023 01:26:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.14/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Aug 2023 01:27:45 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.14/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 03 Aug 2023 01:27:47 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Aug 2023 01:27:47 GMT
COPY file:60282e2c078282f09827dfb0926d431a7ad71f6de3495a21fc8a846430fc5fc9 in /usr/local/bin/healthcheck.sh 
# Thu, 03 Aug 2023 01:27:47 GMT
COPY file:704c6685e9d99f08306a2726e0468f5a764a4040cc2eb6138c1be72ac2529bbc in /usr/local/bin/ 
# Thu, 03 Aug 2023 01:27:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Aug 2023 01:27:47 GMT
EXPOSE 3306
# Thu, 03 Aug 2023 01:27:47 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:edab87ea811e56041127f5e9eb4115fb62cb96d0e6a14056e0d2dbf51a945a22`  
		Last Modified: Wed, 02 Aug 2023 04:28:23 GMT  
		Size: 27.2 MB (27200587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2284a6434f560b2133557b42a6382dceb1dedbb4f91b2e2b8f09c72a90e65901`  
		Last Modified: Thu, 03 Aug 2023 01:29:22 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb060ede2339c044a41658c05b6bd5e977c9b6446d4fe0f02adcd99440ef1f58`  
		Last Modified: Thu, 03 Aug 2023 01:29:23 GMT  
		Size: 6.8 MB (6849661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ed949feb53a8405c2c1a2b71cfb05eb3447b873ffd8c9daa41a13b3ab57552`  
		Last Modified: Thu, 03 Aug 2023 01:29:20 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:941ce653181fe64a4f78ee03f4fc2d1c7b002bd0f48b5f81d82e68aff61f2c05`  
		Last Modified: Thu, 03 Aug 2023 01:29:20 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69476c9fead1edf07b7d57489b3c63d2a475e710f6e2736a8fa3f6891d2d5cc9`  
		Last Modified: Thu, 03 Aug 2023 01:29:29 GMT  
		Size: 84.9 MB (84882391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603324c9e8fddec9c036ec9c7336dcddf48fc9fb6024743221ee208866e7449e`  
		Last Modified: Thu, 03 Aug 2023 01:29:20 GMT  
		Size: 3.6 KB (3563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:909af65085d3de7c3b0949c642c8d4e58edddfdd82486e7e6d39bd0f506bccce`  
		Last Modified: Thu, 03 Aug 2023 01:29:20 GMT  
		Size: 7.6 KB (7565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6` - linux; ppc64le

```console
$ docker pull mariadb@sha256:61e9212a0219222516e7af781d5cb1ec6305a17a01c9116a5d87be27f9b099b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.4 MB (131387157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0513668ad3f60025ee363c56ae3a3890ea5f753bae96967d31b1894439d3b644`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 01 Aug 2023 06:20:36 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:20:36 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:20:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:20:37 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:20:40 GMT
ADD file:822df76493d1d533c1a283ab7bb20ce81309f57279422a0eebb2ffb9fab55963 in / 
# Tue, 01 Aug 2023 06:20:40 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 03:10:52 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 03 Aug 2023 03:10:52 GMT
ENV GOSU_VERSION=1.14
# Thu, 03 Aug 2023 03:10:53 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 03 Aug 2023 03:11:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 03 Aug 2023 03:11:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 03 Aug 2023 03:11:46 GMT
ENV LANG=C.UTF-8
# Thu, 03 Aug 2023 03:11:47 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.6.14 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 03 Aug 2023 03:11:48 GMT
ARG MARIADB_MAJOR=10.6
# Thu, 03 Aug 2023 03:11:48 GMT
ENV MARIADB_MAJOR=10.6
# Thu, 03 Aug 2023 03:11:48 GMT
ARG MARIADB_VERSION=1:10.6.14+maria~ubu2004
# Thu, 03 Aug 2023 03:11:49 GMT
ENV MARIADB_VERSION=1:10.6.14+maria~ubu2004
# Thu, 03 Aug 2023 03:11:49 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.14/repo/ubuntu/ focal main
# Thu, 03 Aug 2023 03:11:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.14/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Aug 2023 03:12:49 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.14/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 03 Aug 2023 03:12:53 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Aug 2023 03:12:53 GMT
COPY file:60282e2c078282f09827dfb0926d431a7ad71f6de3495a21fc8a846430fc5fc9 in /usr/local/bin/healthcheck.sh 
# Thu, 03 Aug 2023 03:12:54 GMT
COPY file:704c6685e9d99f08306a2726e0468f5a764a4040cc2eb6138c1be72ac2529bbc in /usr/local/bin/ 
# Thu, 03 Aug 2023 03:12:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Aug 2023 03:12:55 GMT
EXPOSE 3306
# Thu, 03 Aug 2023 03:12:56 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:be0253994e7bea97e6b44cdeec04bf996c8dd3380e70409de3783a1d1971e747`  
		Last Modified: Thu, 03 Aug 2023 02:50:24 GMT  
		Size: 33.3 MB (33306772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48690f21c56aa25403458ebbd3862c5d73e248f8fc2e47199c86fc55cc1f5cb4`  
		Last Modified: Thu, 03 Aug 2023 03:16:24 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0dccff57cc8ee4b6e90243bf698e5cbf73f6255dcf62a2a23e2a797523e267e`  
		Last Modified: Thu, 03 Aug 2023 03:16:26 GMT  
		Size: 7.8 MB (7833713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:922f64b8d88511b05b435916bb5e7f470c4c2390e9f80a153580b6b3b6a3b519`  
		Last Modified: Thu, 03 Aug 2023 03:16:21 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5e19e7b12a515b11347b3fdb783a239dc532cd9544ba4cb7ba2b015811a24be`  
		Last Modified: Thu, 03 Aug 2023 03:16:21 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8104b5e25b2c0b67695a64e8e8adf73f9968f092b3e83e4ce3cadb7fff1f31f`  
		Last Modified: Thu, 03 Aug 2023 03:16:44 GMT  
		Size: 90.2 MB (90233319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0dbbfeccfb3340b5417d545d8a55a5867366bc888f9153b7e948ea2b12f775c`  
		Last Modified: Thu, 03 Aug 2023 03:16:21 GMT  
		Size: 3.6 KB (3564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c510ce96f283592d7f50e061def6e7252484828d9dcd620da0301c19e4e87a`  
		Last Modified: Thu, 03 Aug 2023 03:16:21 GMT  
		Size: 7.6 KB (7565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6` - linux; s390x

```console
$ docker pull mariadb@sha256:41c428545b6b3d8eedcaa0e6806a60a94aee38aad6c13ae497c8010bb36eb30b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.6 MB (120637780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:807b8e7b49dd3d511474cf39f79c481c731937deff43e66bc337628de310d26d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 01 Aug 2023 06:17:39 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:17:39 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:17:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:17:39 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:17:41 GMT
ADD file:36efc3ec29bb54e0987fe91be1aa7cc849909b3cd2534af3de2d3d07a03804cf in / 
# Tue, 01 Aug 2023 06:17:41 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 00:00:50 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 03 Aug 2023 00:00:50 GMT
ENV GOSU_VERSION=1.14
# Thu, 03 Aug 2023 00:00:50 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 03 Aug 2023 00:01:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 03 Aug 2023 00:01:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 03 Aug 2023 00:01:22 GMT
ENV LANG=C.UTF-8
# Thu, 03 Aug 2023 00:01:22 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.6.14 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 03 Aug 2023 00:01:23 GMT
ARG MARIADB_MAJOR=10.6
# Thu, 03 Aug 2023 00:01:23 GMT
ENV MARIADB_MAJOR=10.6
# Thu, 03 Aug 2023 00:01:23 GMT
ARG MARIADB_VERSION=1:10.6.14+maria~ubu2004
# Thu, 03 Aug 2023 00:01:23 GMT
ENV MARIADB_VERSION=1:10.6.14+maria~ubu2004
# Thu, 03 Aug 2023 00:01:23 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.14/repo/ubuntu/ focal main
# Thu, 03 Aug 2023 00:01:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.14/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Aug 2023 00:01:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.14/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 03 Aug 2023 00:01:59 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Aug 2023 00:02:00 GMT
COPY file:60282e2c078282f09827dfb0926d431a7ad71f6de3495a21fc8a846430fc5fc9 in /usr/local/bin/healthcheck.sh 
# Thu, 03 Aug 2023 00:02:00 GMT
COPY file:704c6685e9d99f08306a2726e0468f5a764a4040cc2eb6138c1be72ac2529bbc in /usr/local/bin/ 
# Thu, 03 Aug 2023 00:02:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Aug 2023 00:02:00 GMT
EXPOSE 3306
# Thu, 03 Aug 2023 00:02:00 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:365fa2124eb5f6f369204f3fe0210d9965952628707dfacd4194a8e15caf0420`  
		Last Modified: Thu, 03 Aug 2023 00:03:37 GMT  
		Size: 27.0 MB (27014233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0adb725e694cf559e6a39a507c55bd0249efdb6249fe800a853d6ff58f42e65b`  
		Last Modified: Thu, 03 Aug 2023 00:03:33 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a570866ba929cce3eb9fb0d52a61756244ac3f17c4e5825e2d036d500b17c6f`  
		Last Modified: Thu, 03 Aug 2023 00:03:33 GMT  
		Size: 6.7 MB (6672025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e4a7ce2693e5abd7571288813bf6e7e1c2ef88aa663172fb337b178235a940`  
		Last Modified: Thu, 03 Aug 2023 00:03:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f8ad913c4a752baebd2f15143677d1be43cbda92dbec0925d6feeebb7660185`  
		Last Modified: Thu, 03 Aug 2023 00:03:31 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5518560e8a567f317e56f5a43dc461e5927b088e25b6042dae7f1715cf233afe`  
		Last Modified: Thu, 03 Aug 2023 00:03:45 GMT  
		Size: 86.9 MB (86938172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f32a1a46fc68dd7b37077d9beedd9d6cd6e8b677645c3008848f0749520ba78d`  
		Last Modified: Thu, 03 Aug 2023 00:03:31 GMT  
		Size: 3.6 KB (3563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d423b092e21bfd317ececa13c3e577b4fd239d9472794be1a736395637e365e0`  
		Last Modified: Thu, 03 Aug 2023 00:03:31 GMT  
		Size: 7.6 KB (7565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.6-focal`

```console
$ docker pull mariadb@sha256:9156c6c088e554b19bdcad795f5b536d5796766806935da63d1268bc647f05b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.6-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:0ecd837a038b6c64a4a046cec70618e306ecbb2d7c044c746912297dae1e3a93
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.6 MB (121632866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf6aa23aa4ff3d40153afcd1cae6e311a4530f54041f25a909a1c9b7339fa5b3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:43 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:45 GMT
ADD file:233702cd816c07bc9fed02881b11fb3bdcaee41f3ce3ec1c9f0c4a060b155d5b in / 
# Tue, 01 Aug 2023 06:16:46 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 03:49:46 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 03 Aug 2023 03:49:46 GMT
ENV GOSU_VERSION=1.14
# Thu, 03 Aug 2023 03:49:46 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 03 Aug 2023 03:50:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 03 Aug 2023 03:50:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 03 Aug 2023 03:50:03 GMT
ENV LANG=C.UTF-8
# Thu, 03 Aug 2023 03:50:03 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.6.14 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 03 Aug 2023 03:50:04 GMT
ARG MARIADB_MAJOR=10.6
# Thu, 03 Aug 2023 03:50:04 GMT
ENV MARIADB_MAJOR=10.6
# Thu, 03 Aug 2023 03:50:04 GMT
ARG MARIADB_VERSION=1:10.6.14+maria~ubu2004
# Thu, 03 Aug 2023 03:50:04 GMT
ENV MARIADB_VERSION=1:10.6.14+maria~ubu2004
# Thu, 03 Aug 2023 03:50:04 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.14/repo/ubuntu/ focal main
# Thu, 03 Aug 2023 03:50:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.14/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Aug 2023 03:50:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.14/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 03 Aug 2023 03:50:27 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Aug 2023 03:50:27 GMT
COPY file:60282e2c078282f09827dfb0926d431a7ad71f6de3495a21fc8a846430fc5fc9 in /usr/local/bin/healthcheck.sh 
# Thu, 03 Aug 2023 03:50:27 GMT
COPY file:704c6685e9d99f08306a2726e0468f5a764a4040cc2eb6138c1be72ac2529bbc in /usr/local/bin/ 
# Thu, 03 Aug 2023 03:50:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Aug 2023 03:50:27 GMT
EXPOSE 3306
# Thu, 03 Aug 2023 03:50:27 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d07cf421114a5a250c403ce9a3a93b7298c13ad1c6a57fd1ffdb4e2755868ce`  
		Last Modified: Thu, 03 Aug 2023 03:51:59 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f49892c3e51cdbc8353172618365a3b19a5ef5e2f91ffc7a8ea05aedb7643d0`  
		Last Modified: Thu, 03 Aug 2023 03:52:00 GMT  
		Size: 7.1 MB (7121511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5daef2619c33583cbfa06f371ab8ff5b045c56db124222906abe3996aaa5eb1`  
		Last Modified: Thu, 03 Aug 2023 03:52:00 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59c36b808a2839fb44ca1b6c4ca60b409c00345ee3567dce18bfb97b8b6c7c0`  
		Last Modified: Thu, 03 Aug 2023 03:51:57 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d12450bcf979a36f64c4019a5e4a6b3bd8b7a00c86b142863fcc15130b141516`  
		Last Modified: Thu, 03 Aug 2023 03:52:09 GMT  
		Size: 85.9 MB (85917337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11011cbf6a2acf48a7b6646cec4b8df7d275284a50dbcab99acda9240ed06f47`  
		Last Modified: Thu, 03 Aug 2023 03:51:57 GMT  
		Size: 3.6 KB (3566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc6463f1b65f394ee1e47b0eaf189c705f9f31b5aa8910e8ec1848d1b364ced9`  
		Last Modified: Thu, 03 Aug 2023 03:51:57 GMT  
		Size: 7.6 KB (7568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:805190f08efde33e24fded93fe7c61fccd47b9a21a402ba083a48f826e005ec5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.9 MB (118945985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53898260b9e47ef8b10962ee6acda2df4ce788131cfbc8ca99a63da9a19c4cef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 01 Aug 2023 06:20:56 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:20:56 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:20:56 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:20:57 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:21:03 GMT
ADD file:ef6e767091d76c1461d099d5bc7a18c526ec80834cf87280803ab6480192f766 in / 
# Tue, 01 Aug 2023 06:21:03 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 01:26:39 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 03 Aug 2023 01:26:40 GMT
ENV GOSU_VERSION=1.14
# Thu, 03 Aug 2023 01:26:40 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 03 Aug 2023 01:26:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 03 Aug 2023 01:26:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 03 Aug 2023 01:26:55 GMT
ENV LANG=C.UTF-8
# Thu, 03 Aug 2023 01:26:55 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.6.14 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 03 Aug 2023 01:26:55 GMT
ARG MARIADB_MAJOR=10.6
# Thu, 03 Aug 2023 01:26:55 GMT
ENV MARIADB_MAJOR=10.6
# Thu, 03 Aug 2023 01:26:55 GMT
ARG MARIADB_VERSION=1:10.6.14+maria~ubu2004
# Thu, 03 Aug 2023 01:26:55 GMT
ENV MARIADB_VERSION=1:10.6.14+maria~ubu2004
# Thu, 03 Aug 2023 01:26:56 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.14/repo/ubuntu/ focal main
# Thu, 03 Aug 2023 01:26:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.14/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Aug 2023 01:27:45 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.14/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 03 Aug 2023 01:27:47 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Aug 2023 01:27:47 GMT
COPY file:60282e2c078282f09827dfb0926d431a7ad71f6de3495a21fc8a846430fc5fc9 in /usr/local/bin/healthcheck.sh 
# Thu, 03 Aug 2023 01:27:47 GMT
COPY file:704c6685e9d99f08306a2726e0468f5a764a4040cc2eb6138c1be72ac2529bbc in /usr/local/bin/ 
# Thu, 03 Aug 2023 01:27:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Aug 2023 01:27:47 GMT
EXPOSE 3306
# Thu, 03 Aug 2023 01:27:47 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:edab87ea811e56041127f5e9eb4115fb62cb96d0e6a14056e0d2dbf51a945a22`  
		Last Modified: Wed, 02 Aug 2023 04:28:23 GMT  
		Size: 27.2 MB (27200587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2284a6434f560b2133557b42a6382dceb1dedbb4f91b2e2b8f09c72a90e65901`  
		Last Modified: Thu, 03 Aug 2023 01:29:22 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb060ede2339c044a41658c05b6bd5e977c9b6446d4fe0f02adcd99440ef1f58`  
		Last Modified: Thu, 03 Aug 2023 01:29:23 GMT  
		Size: 6.8 MB (6849661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ed949feb53a8405c2c1a2b71cfb05eb3447b873ffd8c9daa41a13b3ab57552`  
		Last Modified: Thu, 03 Aug 2023 01:29:20 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:941ce653181fe64a4f78ee03f4fc2d1c7b002bd0f48b5f81d82e68aff61f2c05`  
		Last Modified: Thu, 03 Aug 2023 01:29:20 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69476c9fead1edf07b7d57489b3c63d2a475e710f6e2736a8fa3f6891d2d5cc9`  
		Last Modified: Thu, 03 Aug 2023 01:29:29 GMT  
		Size: 84.9 MB (84882391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603324c9e8fddec9c036ec9c7336dcddf48fc9fb6024743221ee208866e7449e`  
		Last Modified: Thu, 03 Aug 2023 01:29:20 GMT  
		Size: 3.6 KB (3563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:909af65085d3de7c3b0949c642c8d4e58edddfdd82486e7e6d39bd0f506bccce`  
		Last Modified: Thu, 03 Aug 2023 01:29:20 GMT  
		Size: 7.6 KB (7565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:61e9212a0219222516e7af781d5cb1ec6305a17a01c9116a5d87be27f9b099b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.4 MB (131387157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0513668ad3f60025ee363c56ae3a3890ea5f753bae96967d31b1894439d3b644`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 01 Aug 2023 06:20:36 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:20:36 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:20:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:20:37 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:20:40 GMT
ADD file:822df76493d1d533c1a283ab7bb20ce81309f57279422a0eebb2ffb9fab55963 in / 
# Tue, 01 Aug 2023 06:20:40 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 03:10:52 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 03 Aug 2023 03:10:52 GMT
ENV GOSU_VERSION=1.14
# Thu, 03 Aug 2023 03:10:53 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 03 Aug 2023 03:11:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 03 Aug 2023 03:11:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 03 Aug 2023 03:11:46 GMT
ENV LANG=C.UTF-8
# Thu, 03 Aug 2023 03:11:47 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.6.14 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 03 Aug 2023 03:11:48 GMT
ARG MARIADB_MAJOR=10.6
# Thu, 03 Aug 2023 03:11:48 GMT
ENV MARIADB_MAJOR=10.6
# Thu, 03 Aug 2023 03:11:48 GMT
ARG MARIADB_VERSION=1:10.6.14+maria~ubu2004
# Thu, 03 Aug 2023 03:11:49 GMT
ENV MARIADB_VERSION=1:10.6.14+maria~ubu2004
# Thu, 03 Aug 2023 03:11:49 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.14/repo/ubuntu/ focal main
# Thu, 03 Aug 2023 03:11:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.14/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Aug 2023 03:12:49 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.14/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 03 Aug 2023 03:12:53 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Aug 2023 03:12:53 GMT
COPY file:60282e2c078282f09827dfb0926d431a7ad71f6de3495a21fc8a846430fc5fc9 in /usr/local/bin/healthcheck.sh 
# Thu, 03 Aug 2023 03:12:54 GMT
COPY file:704c6685e9d99f08306a2726e0468f5a764a4040cc2eb6138c1be72ac2529bbc in /usr/local/bin/ 
# Thu, 03 Aug 2023 03:12:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Aug 2023 03:12:55 GMT
EXPOSE 3306
# Thu, 03 Aug 2023 03:12:56 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:be0253994e7bea97e6b44cdeec04bf996c8dd3380e70409de3783a1d1971e747`  
		Last Modified: Thu, 03 Aug 2023 02:50:24 GMT  
		Size: 33.3 MB (33306772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48690f21c56aa25403458ebbd3862c5d73e248f8fc2e47199c86fc55cc1f5cb4`  
		Last Modified: Thu, 03 Aug 2023 03:16:24 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0dccff57cc8ee4b6e90243bf698e5cbf73f6255dcf62a2a23e2a797523e267e`  
		Last Modified: Thu, 03 Aug 2023 03:16:26 GMT  
		Size: 7.8 MB (7833713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:922f64b8d88511b05b435916bb5e7f470c4c2390e9f80a153580b6b3b6a3b519`  
		Last Modified: Thu, 03 Aug 2023 03:16:21 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5e19e7b12a515b11347b3fdb783a239dc532cd9544ba4cb7ba2b015811a24be`  
		Last Modified: Thu, 03 Aug 2023 03:16:21 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8104b5e25b2c0b67695a64e8e8adf73f9968f092b3e83e4ce3cadb7fff1f31f`  
		Last Modified: Thu, 03 Aug 2023 03:16:44 GMT  
		Size: 90.2 MB (90233319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0dbbfeccfb3340b5417d545d8a55a5867366bc888f9153b7e948ea2b12f775c`  
		Last Modified: Thu, 03 Aug 2023 03:16:21 GMT  
		Size: 3.6 KB (3564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c510ce96f283592d7f50e061def6e7252484828d9dcd620da0301c19e4e87a`  
		Last Modified: Thu, 03 Aug 2023 03:16:21 GMT  
		Size: 7.6 KB (7565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:41c428545b6b3d8eedcaa0e6806a60a94aee38aad6c13ae497c8010bb36eb30b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.6 MB (120637780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:807b8e7b49dd3d511474cf39f79c481c731937deff43e66bc337628de310d26d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 01 Aug 2023 06:17:39 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:17:39 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:17:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:17:39 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:17:41 GMT
ADD file:36efc3ec29bb54e0987fe91be1aa7cc849909b3cd2534af3de2d3d07a03804cf in / 
# Tue, 01 Aug 2023 06:17:41 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 00:00:50 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 03 Aug 2023 00:00:50 GMT
ENV GOSU_VERSION=1.14
# Thu, 03 Aug 2023 00:00:50 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 03 Aug 2023 00:01:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 03 Aug 2023 00:01:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 03 Aug 2023 00:01:22 GMT
ENV LANG=C.UTF-8
# Thu, 03 Aug 2023 00:01:22 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.6.14 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 03 Aug 2023 00:01:23 GMT
ARG MARIADB_MAJOR=10.6
# Thu, 03 Aug 2023 00:01:23 GMT
ENV MARIADB_MAJOR=10.6
# Thu, 03 Aug 2023 00:01:23 GMT
ARG MARIADB_VERSION=1:10.6.14+maria~ubu2004
# Thu, 03 Aug 2023 00:01:23 GMT
ENV MARIADB_VERSION=1:10.6.14+maria~ubu2004
# Thu, 03 Aug 2023 00:01:23 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.14/repo/ubuntu/ focal main
# Thu, 03 Aug 2023 00:01:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.14/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Aug 2023 00:01:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.14/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 03 Aug 2023 00:01:59 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Aug 2023 00:02:00 GMT
COPY file:60282e2c078282f09827dfb0926d431a7ad71f6de3495a21fc8a846430fc5fc9 in /usr/local/bin/healthcheck.sh 
# Thu, 03 Aug 2023 00:02:00 GMT
COPY file:704c6685e9d99f08306a2726e0468f5a764a4040cc2eb6138c1be72ac2529bbc in /usr/local/bin/ 
# Thu, 03 Aug 2023 00:02:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Aug 2023 00:02:00 GMT
EXPOSE 3306
# Thu, 03 Aug 2023 00:02:00 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:365fa2124eb5f6f369204f3fe0210d9965952628707dfacd4194a8e15caf0420`  
		Last Modified: Thu, 03 Aug 2023 00:03:37 GMT  
		Size: 27.0 MB (27014233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0adb725e694cf559e6a39a507c55bd0249efdb6249fe800a853d6ff58f42e65b`  
		Last Modified: Thu, 03 Aug 2023 00:03:33 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a570866ba929cce3eb9fb0d52a61756244ac3f17c4e5825e2d036d500b17c6f`  
		Last Modified: Thu, 03 Aug 2023 00:03:33 GMT  
		Size: 6.7 MB (6672025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e4a7ce2693e5abd7571288813bf6e7e1c2ef88aa663172fb337b178235a940`  
		Last Modified: Thu, 03 Aug 2023 00:03:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f8ad913c4a752baebd2f15143677d1be43cbda92dbec0925d6feeebb7660185`  
		Last Modified: Thu, 03 Aug 2023 00:03:31 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5518560e8a567f317e56f5a43dc461e5927b088e25b6042dae7f1715cf233afe`  
		Last Modified: Thu, 03 Aug 2023 00:03:45 GMT  
		Size: 86.9 MB (86938172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f32a1a46fc68dd7b37077d9beedd9d6cd6e8b677645c3008848f0749520ba78d`  
		Last Modified: Thu, 03 Aug 2023 00:03:31 GMT  
		Size: 3.6 KB (3563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d423b092e21bfd317ececa13c3e577b4fd239d9472794be1a736395637e365e0`  
		Last Modified: Thu, 03 Aug 2023 00:03:31 GMT  
		Size: 7.6 KB (7565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.6.15`

```console
$ docker pull mariadb@sha256:eb37f58646a901dc7727cf448cae36daaefaba79de33b5058dab79aa4c04aefb
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 0

## `mariadb:10.6.15-focal`

```console
$ docker pull mariadb@sha256:eb37f58646a901dc7727cf448cae36daaefaba79de33b5058dab79aa4c04aefb
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 0

## `mariadb:10.9`

```console
$ docker pull mariadb@sha256:198c7a5fea3d7285762042a628fe8f83f0a7ccef559605b4cc9502e65210880b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.9` - linux; amd64

```console
$ docker pull mariadb@sha256:e1987703abda3340edd61aea1b0847002041c33eb9dfd149f2188f900faf988a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.4 MB (119396592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf484902e4425e551800bd3f5b74354ea047aa4c75b30a1d07885208d88e1212`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 18:27:16 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 18:27:16 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 18:27:16 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 18:27:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 18:27:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 18:27:39 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 18:29:26 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.9.7 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 18:29:26 GMT
ARG MARIADB_VERSION=1:10.9.7+maria~ubu2204
# Tue, 04 Jul 2023 18:29:26 GMT
ENV MARIADB_VERSION=1:10.9.7+maria~ubu2204
# Tue, 04 Jul 2023 18:29:26 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.7/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 18:29:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.7/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 18:29:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.7/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 18:29:43 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 18:29:44 GMT
COPY file:60282e2c078282f09827dfb0926d431a7ad71f6de3495a21fc8a846430fc5fc9 in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 18:29:44 GMT
COPY file:704c6685e9d99f08306a2726e0468f5a764a4040cc2eb6138c1be72ac2529bbc in /usr/local/bin/ 
# Tue, 04 Jul 2023 18:29:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 18:29:44 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 18:29:44 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:718e898a86ffe915c46f60c599bc87928aa5e7e3a9434cbf52066b49651d3a1f`  
		Last Modified: Tue, 04 Jul 2023 18:32:00 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bd7a143a6c5d92cccbae0a38df554277f44cb4dbfcb668436dc5ed3398144a`  
		Last Modified: Tue, 04 Jul 2023 18:32:01 GMT  
		Size: 5.6 MB (5592713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80cdf483b70a4a08d0db0ff26cb8dbdc933588954a3bf91fce2f2544b7be37b8`  
		Last Modified: Tue, 04 Jul 2023 18:31:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8a08318bab8e1a9437115c87f13b6935a5c1b424af982eb11a7af33f5c3ef6`  
		Last Modified: Tue, 04 Jul 2023 18:33:55 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11cbda562e63b4d81ad8fa1a767c075da3a95d5b10d4c8d35da950b3156ca969`  
		Last Modified: Tue, 04 Jul 2023 18:34:06 GMT  
		Size: 83.4 MB (83359294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b08c01f12c66810e485eb49344ec3322d687578dd7ef0f9a37834d9a2e25e6a`  
		Last Modified: Tue, 04 Jul 2023 18:33:54 GMT  
		Size: 3.6 KB (3564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2706b46a144d9f6f3b8df440cd9b7a4965df549b72fea4779d7c734771e8da`  
		Last Modified: Tue, 04 Jul 2023 18:33:54 GMT  
		Size: 7.6 KB (7566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.9` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:18c72e298609ecf8aa949e7c60467c54e3c6405e39eea4a8c300b4fc16c1f69e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (113976612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e65f2f69d71abb401013ba32225b68ac9d73e6883d0ffcd8848e98a1c6ae932`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 15:48:55 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 15:48:55 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 15:48:56 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 15:49:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 15:49:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 15:49:12 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 15:50:53 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.9.7 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 15:50:53 GMT
ARG MARIADB_VERSION=1:10.9.7+maria~ubu2204
# Tue, 04 Jul 2023 15:50:53 GMT
ENV MARIADB_VERSION=1:10.9.7+maria~ubu2204
# Tue, 04 Jul 2023 15:50:53 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.7/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 15:50:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.7/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 15:51:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.7/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 15:51:10 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 15:51:10 GMT
COPY file:60282e2c078282f09827dfb0926d431a7ad71f6de3495a21fc8a846430fc5fc9 in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 15:51:10 GMT
COPY file:704c6685e9d99f08306a2726e0468f5a764a4040cc2eb6138c1be72ac2529bbc in /usr/local/bin/ 
# Tue, 04 Jul 2023 15:51:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 15:51:10 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 15:51:11 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f226d4d968a5322b60d61898c78418afeeb62f9a8613d9939d2546229a59ed0`  
		Last Modified: Tue, 04 Jul 2023 15:53:12 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a718d9544847f819e9859244c57b1093e55eb4bbd1d50066804d9ddd24d9c2c`  
		Last Modified: Tue, 04 Jul 2023 15:53:12 GMT  
		Size: 5.4 MB (5406735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad17cece0015293005bd369ad4550b0faa2ef78f55de897f35a48e5b101b83c8`  
		Last Modified: Tue, 04 Jul 2023 15:53:10 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e27e59297db3e95226ec8d49d91a7b40ccaca85992be2fa1d0ee22b76e0776`  
		Last Modified: Tue, 04 Jul 2023 15:54:53 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:071d3aa54b0dad3b9f11dec652cc671c93c6439ceb3d5a882fd1cadac83ff6ad`  
		Last Modified: Tue, 04 Jul 2023 15:55:02 GMT  
		Size: 80.2 MB (80165501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53cab7a25e192fc18dd77cc36443a1612db445521ba8d40d275089d40c628252`  
		Last Modified: Tue, 04 Jul 2023 15:54:53 GMT  
		Size: 3.6 KB (3564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:385df4b80e86ea79b6e0a5c2e1bd8cf5bf6011c045eccd155d4d051ad6dc2bcc`  
		Last Modified: Tue, 04 Jul 2023 15:54:53 GMT  
		Size: 7.6 KB (7568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.9` - linux; ppc64le

```console
$ docker pull mariadb@sha256:c3d35bcd9f8140c8a348efd5d7c2855d290db5735d4e9624ccd3f488cc71b265
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.0 MB (128009640 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:320f99002093a07778cc3326faa7967f79f38e0a8a7e2a2ba8703d8d60a3c292`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:45:53 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:45:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:45:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:45:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:45:56 GMT
ADD file:8c2fc380378944326d602742fde0e30458cd3e82012847b0f7e09c7184bfd135 in / 
# Wed, 28 Jun 2023 08:45:57 GMT
CMD ["/bin/bash"]
# Wed, 05 Jul 2023 01:06:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 05 Jul 2023 01:06:57 GMT
ENV GOSU_VERSION=1.14
# Wed, 05 Jul 2023 01:06:57 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 05 Jul 2023 01:07:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 05 Jul 2023 01:07:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 05 Jul 2023 01:07:36 GMT
ENV LANG=C.UTF-8
# Wed, 05 Jul 2023 01:12:35 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.9.7 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Wed, 05 Jul 2023 01:12:36 GMT
ARG MARIADB_VERSION=1:10.9.7+maria~ubu2204
# Wed, 05 Jul 2023 01:12:36 GMT
ENV MARIADB_VERSION=1:10.9.7+maria~ubu2204
# Wed, 05 Jul 2023 01:12:36 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.7/repo/ubuntu/ jammy main
# Wed, 05 Jul 2023 01:12:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.7/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 05 Jul 2023 01:13:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.7/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Wed, 05 Jul 2023 01:13:38 GMT
VOLUME [/var/lib/mysql]
# Wed, 05 Jul 2023 01:13:38 GMT
COPY file:60282e2c078282f09827dfb0926d431a7ad71f6de3495a21fc8a846430fc5fc9 in /usr/local/bin/healthcheck.sh 
# Wed, 05 Jul 2023 01:13:38 GMT
COPY file:704c6685e9d99f08306a2726e0468f5a764a4040cc2eb6138c1be72ac2529bbc in /usr/local/bin/ 
# Wed, 05 Jul 2023 01:13:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Jul 2023 01:13:40 GMT
EXPOSE 3306
# Wed, 05 Jul 2023 01:13:40 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:7faa46ce6b6f5c34485980029504c3995e38149d0bca67d8b976c5dbb3673644`  
		Last Modified: Tue, 04 Jul 2023 04:42:31 GMT  
		Size: 35.7 MB (35711469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af03c7013049bbb43a9d70711423a0aa0933ad63d557a33679e987f9f4552c2`  
		Last Modified: Wed, 05 Jul 2023 01:19:30 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fae131e82b0a7c398eb2a917463894a99192198e537fa4a742953dfdec5d9a5`  
		Last Modified: Wed, 05 Jul 2023 01:19:32 GMT  
		Size: 6.0 MB (6017861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c002ce052617f5efe1f7afc4ec819f1f45b350c5956b79ee09c9bd522fe18736`  
		Last Modified: Wed, 05 Jul 2023 01:19:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b8d63d9276e132465e5c830926ecd1e53ac966802898c9f1af11f9b6569e164`  
		Last Modified: Wed, 05 Jul 2023 01:22:44 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614b7d9cb45b5c9f42057b6dc29409ca9a93e37e6cc110eaf2870d4a0ce6c80a`  
		Last Modified: Wed, 05 Jul 2023 01:23:06 GMT  
		Size: 86.3 MB (86266955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32beb7549b9392e3a03b21726174138afc1e3f3734f77d3e96260d513a8af7f`  
		Last Modified: Wed, 05 Jul 2023 01:22:44 GMT  
		Size: 3.6 KB (3563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9ae778c1e44b29fa37d0c22717fec569c039d58dafafaaf05b764a25625617f`  
		Last Modified: Wed, 05 Jul 2023 01:22:44 GMT  
		Size: 7.6 KB (7565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.9` - linux; s390x

```console
$ docker pull mariadb@sha256:c83da50930e2b724837443a2679a443f522c62294ad51193af755d3880b68635
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.0 MB (117015168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55e82153b96c7795033dd02f51b8af68e75f5c99a60e1b5a2a9ce47c5acdd8aa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:53:20 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:53:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:53:22 GMT
ADD file:fa0aef35be7808c8fd6751a52bdec4dd81057e2fcaa075c547a1db53640dae9a in / 
# Wed, 28 Jun 2023 08:53:22 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 16:55:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 16:55:27 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 16:55:27 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 16:55:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 16:55:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 16:55:44 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 16:57:49 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.9.7 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 16:57:49 GMT
ARG MARIADB_VERSION=1:10.9.7+maria~ubu2204
# Tue, 04 Jul 2023 16:57:49 GMT
ENV MARIADB_VERSION=1:10.9.7+maria~ubu2204
# Tue, 04 Jul 2023 16:57:50 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.7/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 16:57:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.7/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 16:58:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.7/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 16:58:06 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 16:58:06 GMT
COPY file:60282e2c078282f09827dfb0926d431a7ad71f6de3495a21fc8a846430fc5fc9 in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 16:58:06 GMT
COPY file:704c6685e9d99f08306a2726e0468f5a764a4040cc2eb6138c1be72ac2529bbc in /usr/local/bin/ 
# Tue, 04 Jul 2023 16:58:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 16:58:06 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 16:58:07 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:ce02ee0330980398d6a84a50abfa1a8c4d1cba27cbd7442b79f4aa1b1a14020d`  
		Last Modified: Tue, 04 Jul 2023 13:08:30 GMT  
		Size: 28.6 MB (28645696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16fb1ab422c0ae864df4333ba064fd3a16ef9b10862dca7b3320a9fb32c7e0bd`  
		Last Modified: Tue, 04 Jul 2023 17:00:17 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be60fdd8cf07af19113cd853d2f0ebedd02fc5cb31582325b43c0d50a323535`  
		Last Modified: Tue, 04 Jul 2023 17:00:18 GMT  
		Size: 5.5 MB (5470782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1374c790d73360e41f53f0d1a2d9cbaef5dd6c371a1ab7c58c7e20e71945704`  
		Last Modified: Tue, 04 Jul 2023 17:00:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edebe53511ca3858a69e2d21dcd8b889be6d1b2e6f057478f144039dca526635`  
		Last Modified: Tue, 04 Jul 2023 17:01:52 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3b6380a5977bca4c9b01582bf30faa0ff95dbead17d9ba496f4623fc09bfa2`  
		Last Modified: Tue, 04 Jul 2023 17:02:04 GMT  
		Size: 82.9 MB (82885324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d0dc0ccafaa1d6b05d7e76903b51fa1b13f66fc7a58dc6ed2957b215b61f50`  
		Last Modified: Tue, 04 Jul 2023 17:01:52 GMT  
		Size: 3.6 KB (3566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440388d4fedd5fe8ddb99c39ec783be344a31487e587af90034ba73c4638cea4`  
		Last Modified: Tue, 04 Jul 2023 17:01:52 GMT  
		Size: 7.6 KB (7570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.9-jammy`

```console
$ docker pull mariadb@sha256:198c7a5fea3d7285762042a628fe8f83f0a7ccef559605b4cc9502e65210880b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.9-jammy` - linux; amd64

```console
$ docker pull mariadb@sha256:e1987703abda3340edd61aea1b0847002041c33eb9dfd149f2188f900faf988a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.4 MB (119396592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf484902e4425e551800bd3f5b74354ea047aa4c75b30a1d07885208d88e1212`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 18:27:16 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 18:27:16 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 18:27:16 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 18:27:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 18:27:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 18:27:39 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 18:29:26 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.9.7 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 18:29:26 GMT
ARG MARIADB_VERSION=1:10.9.7+maria~ubu2204
# Tue, 04 Jul 2023 18:29:26 GMT
ENV MARIADB_VERSION=1:10.9.7+maria~ubu2204
# Tue, 04 Jul 2023 18:29:26 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.7/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 18:29:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.7/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 18:29:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.7/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 18:29:43 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 18:29:44 GMT
COPY file:60282e2c078282f09827dfb0926d431a7ad71f6de3495a21fc8a846430fc5fc9 in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 18:29:44 GMT
COPY file:704c6685e9d99f08306a2726e0468f5a764a4040cc2eb6138c1be72ac2529bbc in /usr/local/bin/ 
# Tue, 04 Jul 2023 18:29:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 18:29:44 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 18:29:44 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:718e898a86ffe915c46f60c599bc87928aa5e7e3a9434cbf52066b49651d3a1f`  
		Last Modified: Tue, 04 Jul 2023 18:32:00 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bd7a143a6c5d92cccbae0a38df554277f44cb4dbfcb668436dc5ed3398144a`  
		Last Modified: Tue, 04 Jul 2023 18:32:01 GMT  
		Size: 5.6 MB (5592713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80cdf483b70a4a08d0db0ff26cb8dbdc933588954a3bf91fce2f2544b7be37b8`  
		Last Modified: Tue, 04 Jul 2023 18:31:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8a08318bab8e1a9437115c87f13b6935a5c1b424af982eb11a7af33f5c3ef6`  
		Last Modified: Tue, 04 Jul 2023 18:33:55 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11cbda562e63b4d81ad8fa1a767c075da3a95d5b10d4c8d35da950b3156ca969`  
		Last Modified: Tue, 04 Jul 2023 18:34:06 GMT  
		Size: 83.4 MB (83359294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b08c01f12c66810e485eb49344ec3322d687578dd7ef0f9a37834d9a2e25e6a`  
		Last Modified: Tue, 04 Jul 2023 18:33:54 GMT  
		Size: 3.6 KB (3564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2706b46a144d9f6f3b8df440cd9b7a4965df549b72fea4779d7c734771e8da`  
		Last Modified: Tue, 04 Jul 2023 18:33:54 GMT  
		Size: 7.6 KB (7566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.9-jammy` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:18c72e298609ecf8aa949e7c60467c54e3c6405e39eea4a8c300b4fc16c1f69e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (113976612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e65f2f69d71abb401013ba32225b68ac9d73e6883d0ffcd8848e98a1c6ae932`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 15:48:55 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 15:48:55 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 15:48:56 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 15:49:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 15:49:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 15:49:12 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 15:50:53 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.9.7 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 15:50:53 GMT
ARG MARIADB_VERSION=1:10.9.7+maria~ubu2204
# Tue, 04 Jul 2023 15:50:53 GMT
ENV MARIADB_VERSION=1:10.9.7+maria~ubu2204
# Tue, 04 Jul 2023 15:50:53 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.7/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 15:50:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.7/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 15:51:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.7/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 15:51:10 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 15:51:10 GMT
COPY file:60282e2c078282f09827dfb0926d431a7ad71f6de3495a21fc8a846430fc5fc9 in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 15:51:10 GMT
COPY file:704c6685e9d99f08306a2726e0468f5a764a4040cc2eb6138c1be72ac2529bbc in /usr/local/bin/ 
# Tue, 04 Jul 2023 15:51:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 15:51:10 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 15:51:11 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f226d4d968a5322b60d61898c78418afeeb62f9a8613d9939d2546229a59ed0`  
		Last Modified: Tue, 04 Jul 2023 15:53:12 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a718d9544847f819e9859244c57b1093e55eb4bbd1d50066804d9ddd24d9c2c`  
		Last Modified: Tue, 04 Jul 2023 15:53:12 GMT  
		Size: 5.4 MB (5406735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad17cece0015293005bd369ad4550b0faa2ef78f55de897f35a48e5b101b83c8`  
		Last Modified: Tue, 04 Jul 2023 15:53:10 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e27e59297db3e95226ec8d49d91a7b40ccaca85992be2fa1d0ee22b76e0776`  
		Last Modified: Tue, 04 Jul 2023 15:54:53 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:071d3aa54b0dad3b9f11dec652cc671c93c6439ceb3d5a882fd1cadac83ff6ad`  
		Last Modified: Tue, 04 Jul 2023 15:55:02 GMT  
		Size: 80.2 MB (80165501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53cab7a25e192fc18dd77cc36443a1612db445521ba8d40d275089d40c628252`  
		Last Modified: Tue, 04 Jul 2023 15:54:53 GMT  
		Size: 3.6 KB (3564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:385df4b80e86ea79b6e0a5c2e1bd8cf5bf6011c045eccd155d4d051ad6dc2bcc`  
		Last Modified: Tue, 04 Jul 2023 15:54:53 GMT  
		Size: 7.6 KB (7568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.9-jammy` - linux; ppc64le

```console
$ docker pull mariadb@sha256:c3d35bcd9f8140c8a348efd5d7c2855d290db5735d4e9624ccd3f488cc71b265
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.0 MB (128009640 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:320f99002093a07778cc3326faa7967f79f38e0a8a7e2a2ba8703d8d60a3c292`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:45:53 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:45:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:45:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:45:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:45:56 GMT
ADD file:8c2fc380378944326d602742fde0e30458cd3e82012847b0f7e09c7184bfd135 in / 
# Wed, 28 Jun 2023 08:45:57 GMT
CMD ["/bin/bash"]
# Wed, 05 Jul 2023 01:06:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 05 Jul 2023 01:06:57 GMT
ENV GOSU_VERSION=1.14
# Wed, 05 Jul 2023 01:06:57 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 05 Jul 2023 01:07:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 05 Jul 2023 01:07:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 05 Jul 2023 01:07:36 GMT
ENV LANG=C.UTF-8
# Wed, 05 Jul 2023 01:12:35 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.9.7 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Wed, 05 Jul 2023 01:12:36 GMT
ARG MARIADB_VERSION=1:10.9.7+maria~ubu2204
# Wed, 05 Jul 2023 01:12:36 GMT
ENV MARIADB_VERSION=1:10.9.7+maria~ubu2204
# Wed, 05 Jul 2023 01:12:36 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.7/repo/ubuntu/ jammy main
# Wed, 05 Jul 2023 01:12:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.7/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 05 Jul 2023 01:13:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.7/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Wed, 05 Jul 2023 01:13:38 GMT
VOLUME [/var/lib/mysql]
# Wed, 05 Jul 2023 01:13:38 GMT
COPY file:60282e2c078282f09827dfb0926d431a7ad71f6de3495a21fc8a846430fc5fc9 in /usr/local/bin/healthcheck.sh 
# Wed, 05 Jul 2023 01:13:38 GMT
COPY file:704c6685e9d99f08306a2726e0468f5a764a4040cc2eb6138c1be72ac2529bbc in /usr/local/bin/ 
# Wed, 05 Jul 2023 01:13:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Jul 2023 01:13:40 GMT
EXPOSE 3306
# Wed, 05 Jul 2023 01:13:40 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:7faa46ce6b6f5c34485980029504c3995e38149d0bca67d8b976c5dbb3673644`  
		Last Modified: Tue, 04 Jul 2023 04:42:31 GMT  
		Size: 35.7 MB (35711469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af03c7013049bbb43a9d70711423a0aa0933ad63d557a33679e987f9f4552c2`  
		Last Modified: Wed, 05 Jul 2023 01:19:30 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fae131e82b0a7c398eb2a917463894a99192198e537fa4a742953dfdec5d9a5`  
		Last Modified: Wed, 05 Jul 2023 01:19:32 GMT  
		Size: 6.0 MB (6017861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c002ce052617f5efe1f7afc4ec819f1f45b350c5956b79ee09c9bd522fe18736`  
		Last Modified: Wed, 05 Jul 2023 01:19:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b8d63d9276e132465e5c830926ecd1e53ac966802898c9f1af11f9b6569e164`  
		Last Modified: Wed, 05 Jul 2023 01:22:44 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614b7d9cb45b5c9f42057b6dc29409ca9a93e37e6cc110eaf2870d4a0ce6c80a`  
		Last Modified: Wed, 05 Jul 2023 01:23:06 GMT  
		Size: 86.3 MB (86266955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32beb7549b9392e3a03b21726174138afc1e3f3734f77d3e96260d513a8af7f`  
		Last Modified: Wed, 05 Jul 2023 01:22:44 GMT  
		Size: 3.6 KB (3563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9ae778c1e44b29fa37d0c22717fec569c039d58dafafaaf05b764a25625617f`  
		Last Modified: Wed, 05 Jul 2023 01:22:44 GMT  
		Size: 7.6 KB (7565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.9-jammy` - linux; s390x

```console
$ docker pull mariadb@sha256:c83da50930e2b724837443a2679a443f522c62294ad51193af755d3880b68635
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.0 MB (117015168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55e82153b96c7795033dd02f51b8af68e75f5c99a60e1b5a2a9ce47c5acdd8aa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:53:20 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:53:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:53:22 GMT
ADD file:fa0aef35be7808c8fd6751a52bdec4dd81057e2fcaa075c547a1db53640dae9a in / 
# Wed, 28 Jun 2023 08:53:22 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 16:55:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 16:55:27 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 16:55:27 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 16:55:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 16:55:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 16:55:44 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 16:57:49 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.9.7 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 16:57:49 GMT
ARG MARIADB_VERSION=1:10.9.7+maria~ubu2204
# Tue, 04 Jul 2023 16:57:49 GMT
ENV MARIADB_VERSION=1:10.9.7+maria~ubu2204
# Tue, 04 Jul 2023 16:57:50 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.7/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 16:57:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.7/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 16:58:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.7/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 16:58:06 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 16:58:06 GMT
COPY file:60282e2c078282f09827dfb0926d431a7ad71f6de3495a21fc8a846430fc5fc9 in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 16:58:06 GMT
COPY file:704c6685e9d99f08306a2726e0468f5a764a4040cc2eb6138c1be72ac2529bbc in /usr/local/bin/ 
# Tue, 04 Jul 2023 16:58:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 16:58:06 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 16:58:07 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:ce02ee0330980398d6a84a50abfa1a8c4d1cba27cbd7442b79f4aa1b1a14020d`  
		Last Modified: Tue, 04 Jul 2023 13:08:30 GMT  
		Size: 28.6 MB (28645696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16fb1ab422c0ae864df4333ba064fd3a16ef9b10862dca7b3320a9fb32c7e0bd`  
		Last Modified: Tue, 04 Jul 2023 17:00:17 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be60fdd8cf07af19113cd853d2f0ebedd02fc5cb31582325b43c0d50a323535`  
		Last Modified: Tue, 04 Jul 2023 17:00:18 GMT  
		Size: 5.5 MB (5470782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1374c790d73360e41f53f0d1a2d9cbaef5dd6c371a1ab7c58c7e20e71945704`  
		Last Modified: Tue, 04 Jul 2023 17:00:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edebe53511ca3858a69e2d21dcd8b889be6d1b2e6f057478f144039dca526635`  
		Last Modified: Tue, 04 Jul 2023 17:01:52 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3b6380a5977bca4c9b01582bf30faa0ff95dbead17d9ba496f4623fc09bfa2`  
		Last Modified: Tue, 04 Jul 2023 17:02:04 GMT  
		Size: 82.9 MB (82885324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d0dc0ccafaa1d6b05d7e76903b51fa1b13f66fc7a58dc6ed2957b215b61f50`  
		Last Modified: Tue, 04 Jul 2023 17:01:52 GMT  
		Size: 3.6 KB (3566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440388d4fedd5fe8ddb99c39ec783be344a31487e587af90034ba73c4638cea4`  
		Last Modified: Tue, 04 Jul 2023 17:01:52 GMT  
		Size: 7.6 KB (7570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.9.8`

```console
$ docker pull mariadb@sha256:eb37f58646a901dc7727cf448cae36daaefaba79de33b5058dab79aa4c04aefb
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 0

## `mariadb:10.9.8-jammy`

```console
$ docker pull mariadb@sha256:eb37f58646a901dc7727cf448cae36daaefaba79de33b5058dab79aa4c04aefb
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 0

## `mariadb:11`

```console
$ docker pull mariadb@sha256:f94bb4868d953fed5220c9d3cdc8449f4c314efb07d3a18eefa6010b383f2ab8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:11` - linux; amd64

```console
$ docker pull mariadb@sha256:c57215c3aabbdb96353ce8b89a7bd6be089f49a4d6bb37f199288a1bf0438a02
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123083360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:011343cf3ec310ee1d70da41536b2ae61e93633dafdba600d865beeb93db6ff8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 18:27:16 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 18:27:16 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 18:27:16 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 18:27:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 18:27:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 18:27:39 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 18:28:14 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.0.2 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 18:28:14 GMT
ARG MARIADB_VERSION=1:11.0.2+maria~ubu2204
# Tue, 04 Jul 2023 18:28:14 GMT
ENV MARIADB_VERSION=1:11.0.2+maria~ubu2204
# Tue, 04 Jul 2023 18:28:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 18:28:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 18:28:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 18:28:33 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 18:28:33 GMT
COPY file:1980cab2a8b7fba7431710370aad263c40d659a4885e66510adf2002b57ddf4c in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 18:28:33 GMT
COPY file:41cd6c305128c82d238b47cc775ecf2262c7b95806428fa87026c43a3d858b56 in /usr/local/bin/ 
# Tue, 04 Jul 2023 18:28:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 18:28:33 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 18:28:33 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:718e898a86ffe915c46f60c599bc87928aa5e7e3a9434cbf52066b49651d3a1f`  
		Last Modified: Tue, 04 Jul 2023 18:32:00 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bd7a143a6c5d92cccbae0a38df554277f44cb4dbfcb668436dc5ed3398144a`  
		Last Modified: Tue, 04 Jul 2023 18:32:01 GMT  
		Size: 5.6 MB (5592713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80cdf483b70a4a08d0db0ff26cb8dbdc933588954a3bf91fce2f2544b7be37b8`  
		Last Modified: Tue, 04 Jul 2023 18:31:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c13b197eea76a7fddd36bbf730423197e52a2298e33993c2189bbe5b3d791d8`  
		Last Modified: Tue, 04 Jul 2023 18:32:23 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe76c18bf258b3649fe944d0678c684ed03c8c96ae60ba50b1d470968adb9c9e`  
		Last Modified: Tue, 04 Jul 2023 18:32:35 GMT  
		Size: 87.0 MB (87046060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67fa5c829e7fb09dbd973997e9219701b99fa6e16d0d5e5a4708ec4f1c60b426`  
		Last Modified: Tue, 04 Jul 2023 18:32:23 GMT  
		Size: 3.6 KB (3566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5cb79f31ff672547bc4a5931db38f52f8900f2b1db24c5179e3da9177b3fc49`  
		Last Modified: Tue, 04 Jul 2023 18:32:23 GMT  
		Size: 7.6 KB (7568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:11` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:35f86cd13f6b6368ad65a3422d572019aaba33daaadd8f312c42dc5dff0d0562
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117620280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4935389ac6b4f1f7ac98fe3b47b5411e8e30630073672e0f21a2117f04e3e160`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 15:48:55 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 15:48:55 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 15:48:56 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 15:49:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 15:49:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 15:49:12 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 15:49:43 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.0.2 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 15:49:43 GMT
ARG MARIADB_VERSION=1:11.0.2+maria~ubu2204
# Tue, 04 Jul 2023 15:49:43 GMT
ENV MARIADB_VERSION=1:11.0.2+maria~ubu2204
# Tue, 04 Jul 2023 15:49:43 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 15:49:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 15:49:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 15:50:01 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 15:50:01 GMT
COPY file:1980cab2a8b7fba7431710370aad263c40d659a4885e66510adf2002b57ddf4c in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 15:50:01 GMT
COPY file:41cd6c305128c82d238b47cc775ecf2262c7b95806428fa87026c43a3d858b56 in /usr/local/bin/ 
# Tue, 04 Jul 2023 15:50:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 15:50:01 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 15:50:01 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f226d4d968a5322b60d61898c78418afeeb62f9a8613d9939d2546229a59ed0`  
		Last Modified: Tue, 04 Jul 2023 15:53:12 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a718d9544847f819e9859244c57b1093e55eb4bbd1d50066804d9ddd24d9c2c`  
		Last Modified: Tue, 04 Jul 2023 15:53:12 GMT  
		Size: 5.4 MB (5406735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad17cece0015293005bd369ad4550b0faa2ef78f55de897f35a48e5b101b83c8`  
		Last Modified: Tue, 04 Jul 2023 15:53:10 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d645dfb141364d7dba62264383035be88d4b865ee99fde0634f178451ceb0f`  
		Last Modified: Tue, 04 Jul 2023 15:53:32 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad716fe25d457aa9fbaa4da59699c447a5e6bad763f5581966bfe4e9756f44ea`  
		Last Modified: Tue, 04 Jul 2023 15:53:42 GMT  
		Size: 83.8 MB (83809168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be4f5d63350215e844e2f9a8409682ffcea79777da31fd1235cb15d19ac85c0`  
		Last Modified: Tue, 04 Jul 2023 15:53:32 GMT  
		Size: 3.6 KB (3565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d127bd39936fe36a0d7b70697a79791a2d2e733708dde4f91a6b31b949e07e6b`  
		Last Modified: Tue, 04 Jul 2023 15:53:32 GMT  
		Size: 7.6 KB (7568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:11` - linux; ppc64le

```console
$ docker pull mariadb@sha256:2b2ed944def75ab4f8dd292d7682dd4d508d2d834b24a1811cfaccfe8f9fd20e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.7 MB (131748397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ec1500d07e746be7f4e6631e0714883d1aadffd88d60f0d280abbf1420a07aa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:45:53 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:45:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:45:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:45:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:45:56 GMT
ADD file:8c2fc380378944326d602742fde0e30458cd3e82012847b0f7e09c7184bfd135 in / 
# Wed, 28 Jun 2023 08:45:57 GMT
CMD ["/bin/bash"]
# Wed, 05 Jul 2023 01:06:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 05 Jul 2023 01:06:57 GMT
ENV GOSU_VERSION=1.14
# Wed, 05 Jul 2023 01:06:57 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 05 Jul 2023 01:07:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 05 Jul 2023 01:07:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 05 Jul 2023 01:07:36 GMT
ENV LANG=C.UTF-8
# Wed, 05 Jul 2023 01:08:51 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.0.2 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Wed, 05 Jul 2023 01:08:52 GMT
ARG MARIADB_VERSION=1:11.0.2+maria~ubu2204
# Wed, 05 Jul 2023 01:08:54 GMT
ENV MARIADB_VERSION=1:11.0.2+maria~ubu2204
# Wed, 05 Jul 2023 01:08:56 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
# Wed, 05 Jul 2023 01:09:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 05 Jul 2023 01:09:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Wed, 05 Jul 2023 01:10:00 GMT
VOLUME [/var/lib/mysql]
# Wed, 05 Jul 2023 01:10:00 GMT
COPY file:1980cab2a8b7fba7431710370aad263c40d659a4885e66510adf2002b57ddf4c in /usr/local/bin/healthcheck.sh 
# Wed, 05 Jul 2023 01:10:00 GMT
COPY file:41cd6c305128c82d238b47cc775ecf2262c7b95806428fa87026c43a3d858b56 in /usr/local/bin/ 
# Wed, 05 Jul 2023 01:10:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Jul 2023 01:10:02 GMT
EXPOSE 3306
# Wed, 05 Jul 2023 01:10:03 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:7faa46ce6b6f5c34485980029504c3995e38149d0bca67d8b976c5dbb3673644`  
		Last Modified: Tue, 04 Jul 2023 04:42:31 GMT  
		Size: 35.7 MB (35711469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af03c7013049bbb43a9d70711423a0aa0933ad63d557a33679e987f9f4552c2`  
		Last Modified: Wed, 05 Jul 2023 01:19:30 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fae131e82b0a7c398eb2a917463894a99192198e537fa4a742953dfdec5d9a5`  
		Last Modified: Wed, 05 Jul 2023 01:19:32 GMT  
		Size: 6.0 MB (6017861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c002ce052617f5efe1f7afc4ec819f1f45b350c5956b79ee09c9bd522fe18736`  
		Last Modified: Wed, 05 Jul 2023 01:19:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8036bf31dcde2e2ac8325b42c737558cf33a8cb4d01e5cedda956b06b87e05b1`  
		Last Modified: Wed, 05 Jul 2023 01:20:09 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d3a3242885374320250cbe4559b4118f1a835c6434f7905bb2ecf1f0135e49`  
		Last Modified: Wed, 05 Jul 2023 01:20:34 GMT  
		Size: 90.0 MB (90005706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb4f4475038f4dcfbb395f132f635565400316ed33037211135421a08449cb55`  
		Last Modified: Wed, 05 Jul 2023 01:20:09 GMT  
		Size: 3.6 KB (3564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3156cef64baa3f1944fde330137217b9cab7a8724be1ce677aed5b374711228`  
		Last Modified: Wed, 05 Jul 2023 01:20:09 GMT  
		Size: 7.6 KB (7567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:11` - linux; s390x

```console
$ docker pull mariadb@sha256:fec237d61ee4f020ee1942a5ce7ba77851271df7760c330791d49d21e38fd76d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.6 MB (121591761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd61cf2f3f72cf840df9a6079260a2004a1aaedaef78506d8c73ba968e19edfe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:53:20 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:53:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:53:22 GMT
ADD file:fa0aef35be7808c8fd6751a52bdec4dd81057e2fcaa075c547a1db53640dae9a in / 
# Wed, 28 Jun 2023 08:53:22 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 16:55:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 16:55:27 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 16:55:27 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 16:55:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 16:55:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 16:55:44 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 16:56:25 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.0.2 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 16:56:25 GMT
ARG MARIADB_VERSION=1:11.0.2+maria~ubu2204
# Tue, 04 Jul 2023 16:56:25 GMT
ENV MARIADB_VERSION=1:11.0.2+maria~ubu2204
# Tue, 04 Jul 2023 16:56:25 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 16:56:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 16:56:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 16:56:47 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 16:56:47 GMT
COPY file:1980cab2a8b7fba7431710370aad263c40d659a4885e66510adf2002b57ddf4c in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 16:56:47 GMT
COPY file:41cd6c305128c82d238b47cc775ecf2262c7b95806428fa87026c43a3d858b56 in /usr/local/bin/ 
# Tue, 04 Jul 2023 16:56:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 16:56:48 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 16:56:48 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:ce02ee0330980398d6a84a50abfa1a8c4d1cba27cbd7442b79f4aa1b1a14020d`  
		Last Modified: Tue, 04 Jul 2023 13:08:30 GMT  
		Size: 28.6 MB (28645696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16fb1ab422c0ae864df4333ba064fd3a16ef9b10862dca7b3320a9fb32c7e0bd`  
		Last Modified: Tue, 04 Jul 2023 17:00:17 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be60fdd8cf07af19113cd853d2f0ebedd02fc5cb31582325b43c0d50a323535`  
		Last Modified: Tue, 04 Jul 2023 17:00:18 GMT  
		Size: 5.5 MB (5470782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1374c790d73360e41f53f0d1a2d9cbaef5dd6c371a1ab7c58c7e20e71945704`  
		Last Modified: Tue, 04 Jul 2023 17:00:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dab15d1c6f25f9d41f7cca3c3dbef72f78adfd2c93e1b5118c2540ab35c9ff5`  
		Last Modified: Tue, 04 Jul 2023 17:00:39 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45f1884ccf2c53f7935d0379452a5e07b67da5146f499569abca9707a426a333`  
		Last Modified: Tue, 04 Jul 2023 17:00:52 GMT  
		Size: 87.5 MB (87461916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895d0bb1d3eef4bc781bd9a29370b15b508f63542867d4e350ba9d0414e35543`  
		Last Modified: Tue, 04 Jul 2023 17:00:39 GMT  
		Size: 3.6 KB (3567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:450856d007683a11eed69967457b4ed8325a4811cae92db3e313920af6019084`  
		Last Modified: Tue, 04 Jul 2023 17:00:39 GMT  
		Size: 7.6 KB (7570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:11-jammy`

```console
$ docker pull mariadb@sha256:f94bb4868d953fed5220c9d3cdc8449f4c314efb07d3a18eefa6010b383f2ab8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:11-jammy` - linux; amd64

```console
$ docker pull mariadb@sha256:c57215c3aabbdb96353ce8b89a7bd6be089f49a4d6bb37f199288a1bf0438a02
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123083360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:011343cf3ec310ee1d70da41536b2ae61e93633dafdba600d865beeb93db6ff8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 18:27:16 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 18:27:16 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 18:27:16 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 18:27:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 18:27:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 18:27:39 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 18:28:14 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.0.2 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 18:28:14 GMT
ARG MARIADB_VERSION=1:11.0.2+maria~ubu2204
# Tue, 04 Jul 2023 18:28:14 GMT
ENV MARIADB_VERSION=1:11.0.2+maria~ubu2204
# Tue, 04 Jul 2023 18:28:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 18:28:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 18:28:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 18:28:33 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 18:28:33 GMT
COPY file:1980cab2a8b7fba7431710370aad263c40d659a4885e66510adf2002b57ddf4c in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 18:28:33 GMT
COPY file:41cd6c305128c82d238b47cc775ecf2262c7b95806428fa87026c43a3d858b56 in /usr/local/bin/ 
# Tue, 04 Jul 2023 18:28:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 18:28:33 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 18:28:33 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:718e898a86ffe915c46f60c599bc87928aa5e7e3a9434cbf52066b49651d3a1f`  
		Last Modified: Tue, 04 Jul 2023 18:32:00 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bd7a143a6c5d92cccbae0a38df554277f44cb4dbfcb668436dc5ed3398144a`  
		Last Modified: Tue, 04 Jul 2023 18:32:01 GMT  
		Size: 5.6 MB (5592713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80cdf483b70a4a08d0db0ff26cb8dbdc933588954a3bf91fce2f2544b7be37b8`  
		Last Modified: Tue, 04 Jul 2023 18:31:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c13b197eea76a7fddd36bbf730423197e52a2298e33993c2189bbe5b3d791d8`  
		Last Modified: Tue, 04 Jul 2023 18:32:23 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe76c18bf258b3649fe944d0678c684ed03c8c96ae60ba50b1d470968adb9c9e`  
		Last Modified: Tue, 04 Jul 2023 18:32:35 GMT  
		Size: 87.0 MB (87046060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67fa5c829e7fb09dbd973997e9219701b99fa6e16d0d5e5a4708ec4f1c60b426`  
		Last Modified: Tue, 04 Jul 2023 18:32:23 GMT  
		Size: 3.6 KB (3566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5cb79f31ff672547bc4a5931db38f52f8900f2b1db24c5179e3da9177b3fc49`  
		Last Modified: Tue, 04 Jul 2023 18:32:23 GMT  
		Size: 7.6 KB (7568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:11-jammy` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:35f86cd13f6b6368ad65a3422d572019aaba33daaadd8f312c42dc5dff0d0562
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117620280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4935389ac6b4f1f7ac98fe3b47b5411e8e30630073672e0f21a2117f04e3e160`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 15:48:55 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 15:48:55 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 15:48:56 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 15:49:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 15:49:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 15:49:12 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 15:49:43 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.0.2 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 15:49:43 GMT
ARG MARIADB_VERSION=1:11.0.2+maria~ubu2204
# Tue, 04 Jul 2023 15:49:43 GMT
ENV MARIADB_VERSION=1:11.0.2+maria~ubu2204
# Tue, 04 Jul 2023 15:49:43 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 15:49:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 15:49:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 15:50:01 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 15:50:01 GMT
COPY file:1980cab2a8b7fba7431710370aad263c40d659a4885e66510adf2002b57ddf4c in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 15:50:01 GMT
COPY file:41cd6c305128c82d238b47cc775ecf2262c7b95806428fa87026c43a3d858b56 in /usr/local/bin/ 
# Tue, 04 Jul 2023 15:50:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 15:50:01 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 15:50:01 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f226d4d968a5322b60d61898c78418afeeb62f9a8613d9939d2546229a59ed0`  
		Last Modified: Tue, 04 Jul 2023 15:53:12 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a718d9544847f819e9859244c57b1093e55eb4bbd1d50066804d9ddd24d9c2c`  
		Last Modified: Tue, 04 Jul 2023 15:53:12 GMT  
		Size: 5.4 MB (5406735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad17cece0015293005bd369ad4550b0faa2ef78f55de897f35a48e5b101b83c8`  
		Last Modified: Tue, 04 Jul 2023 15:53:10 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d645dfb141364d7dba62264383035be88d4b865ee99fde0634f178451ceb0f`  
		Last Modified: Tue, 04 Jul 2023 15:53:32 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad716fe25d457aa9fbaa4da59699c447a5e6bad763f5581966bfe4e9756f44ea`  
		Last Modified: Tue, 04 Jul 2023 15:53:42 GMT  
		Size: 83.8 MB (83809168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be4f5d63350215e844e2f9a8409682ffcea79777da31fd1235cb15d19ac85c0`  
		Last Modified: Tue, 04 Jul 2023 15:53:32 GMT  
		Size: 3.6 KB (3565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d127bd39936fe36a0d7b70697a79791a2d2e733708dde4f91a6b31b949e07e6b`  
		Last Modified: Tue, 04 Jul 2023 15:53:32 GMT  
		Size: 7.6 KB (7568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:11-jammy` - linux; ppc64le

```console
$ docker pull mariadb@sha256:2b2ed944def75ab4f8dd292d7682dd4d508d2d834b24a1811cfaccfe8f9fd20e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.7 MB (131748397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ec1500d07e746be7f4e6631e0714883d1aadffd88d60f0d280abbf1420a07aa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:45:53 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:45:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:45:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:45:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:45:56 GMT
ADD file:8c2fc380378944326d602742fde0e30458cd3e82012847b0f7e09c7184bfd135 in / 
# Wed, 28 Jun 2023 08:45:57 GMT
CMD ["/bin/bash"]
# Wed, 05 Jul 2023 01:06:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 05 Jul 2023 01:06:57 GMT
ENV GOSU_VERSION=1.14
# Wed, 05 Jul 2023 01:06:57 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 05 Jul 2023 01:07:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 05 Jul 2023 01:07:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 05 Jul 2023 01:07:36 GMT
ENV LANG=C.UTF-8
# Wed, 05 Jul 2023 01:08:51 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.0.2 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Wed, 05 Jul 2023 01:08:52 GMT
ARG MARIADB_VERSION=1:11.0.2+maria~ubu2204
# Wed, 05 Jul 2023 01:08:54 GMT
ENV MARIADB_VERSION=1:11.0.2+maria~ubu2204
# Wed, 05 Jul 2023 01:08:56 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
# Wed, 05 Jul 2023 01:09:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 05 Jul 2023 01:09:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Wed, 05 Jul 2023 01:10:00 GMT
VOLUME [/var/lib/mysql]
# Wed, 05 Jul 2023 01:10:00 GMT
COPY file:1980cab2a8b7fba7431710370aad263c40d659a4885e66510adf2002b57ddf4c in /usr/local/bin/healthcheck.sh 
# Wed, 05 Jul 2023 01:10:00 GMT
COPY file:41cd6c305128c82d238b47cc775ecf2262c7b95806428fa87026c43a3d858b56 in /usr/local/bin/ 
# Wed, 05 Jul 2023 01:10:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Jul 2023 01:10:02 GMT
EXPOSE 3306
# Wed, 05 Jul 2023 01:10:03 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:7faa46ce6b6f5c34485980029504c3995e38149d0bca67d8b976c5dbb3673644`  
		Last Modified: Tue, 04 Jul 2023 04:42:31 GMT  
		Size: 35.7 MB (35711469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af03c7013049bbb43a9d70711423a0aa0933ad63d557a33679e987f9f4552c2`  
		Last Modified: Wed, 05 Jul 2023 01:19:30 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fae131e82b0a7c398eb2a917463894a99192198e537fa4a742953dfdec5d9a5`  
		Last Modified: Wed, 05 Jul 2023 01:19:32 GMT  
		Size: 6.0 MB (6017861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c002ce052617f5efe1f7afc4ec819f1f45b350c5956b79ee09c9bd522fe18736`  
		Last Modified: Wed, 05 Jul 2023 01:19:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8036bf31dcde2e2ac8325b42c737558cf33a8cb4d01e5cedda956b06b87e05b1`  
		Last Modified: Wed, 05 Jul 2023 01:20:09 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d3a3242885374320250cbe4559b4118f1a835c6434f7905bb2ecf1f0135e49`  
		Last Modified: Wed, 05 Jul 2023 01:20:34 GMT  
		Size: 90.0 MB (90005706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb4f4475038f4dcfbb395f132f635565400316ed33037211135421a08449cb55`  
		Last Modified: Wed, 05 Jul 2023 01:20:09 GMT  
		Size: 3.6 KB (3564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3156cef64baa3f1944fde330137217b9cab7a8724be1ce677aed5b374711228`  
		Last Modified: Wed, 05 Jul 2023 01:20:09 GMT  
		Size: 7.6 KB (7567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:11-jammy` - linux; s390x

```console
$ docker pull mariadb@sha256:fec237d61ee4f020ee1942a5ce7ba77851271df7760c330791d49d21e38fd76d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.6 MB (121591761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd61cf2f3f72cf840df9a6079260a2004a1aaedaef78506d8c73ba968e19edfe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:53:20 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:53:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:53:22 GMT
ADD file:fa0aef35be7808c8fd6751a52bdec4dd81057e2fcaa075c547a1db53640dae9a in / 
# Wed, 28 Jun 2023 08:53:22 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 16:55:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 16:55:27 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 16:55:27 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 16:55:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 16:55:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 16:55:44 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 16:56:25 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.0.2 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 16:56:25 GMT
ARG MARIADB_VERSION=1:11.0.2+maria~ubu2204
# Tue, 04 Jul 2023 16:56:25 GMT
ENV MARIADB_VERSION=1:11.0.2+maria~ubu2204
# Tue, 04 Jul 2023 16:56:25 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 16:56:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 16:56:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 16:56:47 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 16:56:47 GMT
COPY file:1980cab2a8b7fba7431710370aad263c40d659a4885e66510adf2002b57ddf4c in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 16:56:47 GMT
COPY file:41cd6c305128c82d238b47cc775ecf2262c7b95806428fa87026c43a3d858b56 in /usr/local/bin/ 
# Tue, 04 Jul 2023 16:56:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 16:56:48 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 16:56:48 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:ce02ee0330980398d6a84a50abfa1a8c4d1cba27cbd7442b79f4aa1b1a14020d`  
		Last Modified: Tue, 04 Jul 2023 13:08:30 GMT  
		Size: 28.6 MB (28645696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16fb1ab422c0ae864df4333ba064fd3a16ef9b10862dca7b3320a9fb32c7e0bd`  
		Last Modified: Tue, 04 Jul 2023 17:00:17 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be60fdd8cf07af19113cd853d2f0ebedd02fc5cb31582325b43c0d50a323535`  
		Last Modified: Tue, 04 Jul 2023 17:00:18 GMT  
		Size: 5.5 MB (5470782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1374c790d73360e41f53f0d1a2d9cbaef5dd6c371a1ab7c58c7e20e71945704`  
		Last Modified: Tue, 04 Jul 2023 17:00:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dab15d1c6f25f9d41f7cca3c3dbef72f78adfd2c93e1b5118c2540ab35c9ff5`  
		Last Modified: Tue, 04 Jul 2023 17:00:39 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45f1884ccf2c53f7935d0379452a5e07b67da5146f499569abca9707a426a333`  
		Last Modified: Tue, 04 Jul 2023 17:00:52 GMT  
		Size: 87.5 MB (87461916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895d0bb1d3eef4bc781bd9a29370b15b508f63542867d4e350ba9d0414e35543`  
		Last Modified: Tue, 04 Jul 2023 17:00:39 GMT  
		Size: 3.6 KB (3567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:450856d007683a11eed69967457b4ed8325a4811cae92db3e313920af6019084`  
		Last Modified: Tue, 04 Jul 2023 17:00:39 GMT  
		Size: 7.6 KB (7570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:11.0`

```console
$ docker pull mariadb@sha256:f94bb4868d953fed5220c9d3cdc8449f4c314efb07d3a18eefa6010b383f2ab8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:11.0` - linux; amd64

```console
$ docker pull mariadb@sha256:c57215c3aabbdb96353ce8b89a7bd6be089f49a4d6bb37f199288a1bf0438a02
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123083360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:011343cf3ec310ee1d70da41536b2ae61e93633dafdba600d865beeb93db6ff8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 18:27:16 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 18:27:16 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 18:27:16 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 18:27:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 18:27:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 18:27:39 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 18:28:14 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.0.2 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 18:28:14 GMT
ARG MARIADB_VERSION=1:11.0.2+maria~ubu2204
# Tue, 04 Jul 2023 18:28:14 GMT
ENV MARIADB_VERSION=1:11.0.2+maria~ubu2204
# Tue, 04 Jul 2023 18:28:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 18:28:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 18:28:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 18:28:33 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 18:28:33 GMT
COPY file:1980cab2a8b7fba7431710370aad263c40d659a4885e66510adf2002b57ddf4c in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 18:28:33 GMT
COPY file:41cd6c305128c82d238b47cc775ecf2262c7b95806428fa87026c43a3d858b56 in /usr/local/bin/ 
# Tue, 04 Jul 2023 18:28:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 18:28:33 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 18:28:33 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:718e898a86ffe915c46f60c599bc87928aa5e7e3a9434cbf52066b49651d3a1f`  
		Last Modified: Tue, 04 Jul 2023 18:32:00 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bd7a143a6c5d92cccbae0a38df554277f44cb4dbfcb668436dc5ed3398144a`  
		Last Modified: Tue, 04 Jul 2023 18:32:01 GMT  
		Size: 5.6 MB (5592713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80cdf483b70a4a08d0db0ff26cb8dbdc933588954a3bf91fce2f2544b7be37b8`  
		Last Modified: Tue, 04 Jul 2023 18:31:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c13b197eea76a7fddd36bbf730423197e52a2298e33993c2189bbe5b3d791d8`  
		Last Modified: Tue, 04 Jul 2023 18:32:23 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe76c18bf258b3649fe944d0678c684ed03c8c96ae60ba50b1d470968adb9c9e`  
		Last Modified: Tue, 04 Jul 2023 18:32:35 GMT  
		Size: 87.0 MB (87046060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67fa5c829e7fb09dbd973997e9219701b99fa6e16d0d5e5a4708ec4f1c60b426`  
		Last Modified: Tue, 04 Jul 2023 18:32:23 GMT  
		Size: 3.6 KB (3566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5cb79f31ff672547bc4a5931db38f52f8900f2b1db24c5179e3da9177b3fc49`  
		Last Modified: Tue, 04 Jul 2023 18:32:23 GMT  
		Size: 7.6 KB (7568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:11.0` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:35f86cd13f6b6368ad65a3422d572019aaba33daaadd8f312c42dc5dff0d0562
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117620280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4935389ac6b4f1f7ac98fe3b47b5411e8e30630073672e0f21a2117f04e3e160`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 15:48:55 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 15:48:55 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 15:48:56 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 15:49:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 15:49:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 15:49:12 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 15:49:43 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.0.2 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 15:49:43 GMT
ARG MARIADB_VERSION=1:11.0.2+maria~ubu2204
# Tue, 04 Jul 2023 15:49:43 GMT
ENV MARIADB_VERSION=1:11.0.2+maria~ubu2204
# Tue, 04 Jul 2023 15:49:43 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 15:49:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 15:49:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 15:50:01 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 15:50:01 GMT
COPY file:1980cab2a8b7fba7431710370aad263c40d659a4885e66510adf2002b57ddf4c in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 15:50:01 GMT
COPY file:41cd6c305128c82d238b47cc775ecf2262c7b95806428fa87026c43a3d858b56 in /usr/local/bin/ 
# Tue, 04 Jul 2023 15:50:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 15:50:01 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 15:50:01 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f226d4d968a5322b60d61898c78418afeeb62f9a8613d9939d2546229a59ed0`  
		Last Modified: Tue, 04 Jul 2023 15:53:12 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a718d9544847f819e9859244c57b1093e55eb4bbd1d50066804d9ddd24d9c2c`  
		Last Modified: Tue, 04 Jul 2023 15:53:12 GMT  
		Size: 5.4 MB (5406735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad17cece0015293005bd369ad4550b0faa2ef78f55de897f35a48e5b101b83c8`  
		Last Modified: Tue, 04 Jul 2023 15:53:10 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d645dfb141364d7dba62264383035be88d4b865ee99fde0634f178451ceb0f`  
		Last Modified: Tue, 04 Jul 2023 15:53:32 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad716fe25d457aa9fbaa4da59699c447a5e6bad763f5581966bfe4e9756f44ea`  
		Last Modified: Tue, 04 Jul 2023 15:53:42 GMT  
		Size: 83.8 MB (83809168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be4f5d63350215e844e2f9a8409682ffcea79777da31fd1235cb15d19ac85c0`  
		Last Modified: Tue, 04 Jul 2023 15:53:32 GMT  
		Size: 3.6 KB (3565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d127bd39936fe36a0d7b70697a79791a2d2e733708dde4f91a6b31b949e07e6b`  
		Last Modified: Tue, 04 Jul 2023 15:53:32 GMT  
		Size: 7.6 KB (7568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:11.0` - linux; ppc64le

```console
$ docker pull mariadb@sha256:2b2ed944def75ab4f8dd292d7682dd4d508d2d834b24a1811cfaccfe8f9fd20e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.7 MB (131748397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ec1500d07e746be7f4e6631e0714883d1aadffd88d60f0d280abbf1420a07aa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:45:53 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:45:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:45:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:45:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:45:56 GMT
ADD file:8c2fc380378944326d602742fde0e30458cd3e82012847b0f7e09c7184bfd135 in / 
# Wed, 28 Jun 2023 08:45:57 GMT
CMD ["/bin/bash"]
# Wed, 05 Jul 2023 01:06:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 05 Jul 2023 01:06:57 GMT
ENV GOSU_VERSION=1.14
# Wed, 05 Jul 2023 01:06:57 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 05 Jul 2023 01:07:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 05 Jul 2023 01:07:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 05 Jul 2023 01:07:36 GMT
ENV LANG=C.UTF-8
# Wed, 05 Jul 2023 01:08:51 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.0.2 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Wed, 05 Jul 2023 01:08:52 GMT
ARG MARIADB_VERSION=1:11.0.2+maria~ubu2204
# Wed, 05 Jul 2023 01:08:54 GMT
ENV MARIADB_VERSION=1:11.0.2+maria~ubu2204
# Wed, 05 Jul 2023 01:08:56 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
# Wed, 05 Jul 2023 01:09:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 05 Jul 2023 01:09:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Wed, 05 Jul 2023 01:10:00 GMT
VOLUME [/var/lib/mysql]
# Wed, 05 Jul 2023 01:10:00 GMT
COPY file:1980cab2a8b7fba7431710370aad263c40d659a4885e66510adf2002b57ddf4c in /usr/local/bin/healthcheck.sh 
# Wed, 05 Jul 2023 01:10:00 GMT
COPY file:41cd6c305128c82d238b47cc775ecf2262c7b95806428fa87026c43a3d858b56 in /usr/local/bin/ 
# Wed, 05 Jul 2023 01:10:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Jul 2023 01:10:02 GMT
EXPOSE 3306
# Wed, 05 Jul 2023 01:10:03 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:7faa46ce6b6f5c34485980029504c3995e38149d0bca67d8b976c5dbb3673644`  
		Last Modified: Tue, 04 Jul 2023 04:42:31 GMT  
		Size: 35.7 MB (35711469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af03c7013049bbb43a9d70711423a0aa0933ad63d557a33679e987f9f4552c2`  
		Last Modified: Wed, 05 Jul 2023 01:19:30 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fae131e82b0a7c398eb2a917463894a99192198e537fa4a742953dfdec5d9a5`  
		Last Modified: Wed, 05 Jul 2023 01:19:32 GMT  
		Size: 6.0 MB (6017861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c002ce052617f5efe1f7afc4ec819f1f45b350c5956b79ee09c9bd522fe18736`  
		Last Modified: Wed, 05 Jul 2023 01:19:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8036bf31dcde2e2ac8325b42c737558cf33a8cb4d01e5cedda956b06b87e05b1`  
		Last Modified: Wed, 05 Jul 2023 01:20:09 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d3a3242885374320250cbe4559b4118f1a835c6434f7905bb2ecf1f0135e49`  
		Last Modified: Wed, 05 Jul 2023 01:20:34 GMT  
		Size: 90.0 MB (90005706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb4f4475038f4dcfbb395f132f635565400316ed33037211135421a08449cb55`  
		Last Modified: Wed, 05 Jul 2023 01:20:09 GMT  
		Size: 3.6 KB (3564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3156cef64baa3f1944fde330137217b9cab7a8724be1ce677aed5b374711228`  
		Last Modified: Wed, 05 Jul 2023 01:20:09 GMT  
		Size: 7.6 KB (7567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:11.0` - linux; s390x

```console
$ docker pull mariadb@sha256:fec237d61ee4f020ee1942a5ce7ba77851271df7760c330791d49d21e38fd76d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.6 MB (121591761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd61cf2f3f72cf840df9a6079260a2004a1aaedaef78506d8c73ba968e19edfe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:53:20 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:53:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:53:22 GMT
ADD file:fa0aef35be7808c8fd6751a52bdec4dd81057e2fcaa075c547a1db53640dae9a in / 
# Wed, 28 Jun 2023 08:53:22 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 16:55:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 16:55:27 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 16:55:27 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 16:55:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 16:55:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 16:55:44 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 16:56:25 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.0.2 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 16:56:25 GMT
ARG MARIADB_VERSION=1:11.0.2+maria~ubu2204
# Tue, 04 Jul 2023 16:56:25 GMT
ENV MARIADB_VERSION=1:11.0.2+maria~ubu2204
# Tue, 04 Jul 2023 16:56:25 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 16:56:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 16:56:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 16:56:47 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 16:56:47 GMT
COPY file:1980cab2a8b7fba7431710370aad263c40d659a4885e66510adf2002b57ddf4c in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 16:56:47 GMT
COPY file:41cd6c305128c82d238b47cc775ecf2262c7b95806428fa87026c43a3d858b56 in /usr/local/bin/ 
# Tue, 04 Jul 2023 16:56:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 16:56:48 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 16:56:48 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:ce02ee0330980398d6a84a50abfa1a8c4d1cba27cbd7442b79f4aa1b1a14020d`  
		Last Modified: Tue, 04 Jul 2023 13:08:30 GMT  
		Size: 28.6 MB (28645696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16fb1ab422c0ae864df4333ba064fd3a16ef9b10862dca7b3320a9fb32c7e0bd`  
		Last Modified: Tue, 04 Jul 2023 17:00:17 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be60fdd8cf07af19113cd853d2f0ebedd02fc5cb31582325b43c0d50a323535`  
		Last Modified: Tue, 04 Jul 2023 17:00:18 GMT  
		Size: 5.5 MB (5470782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1374c790d73360e41f53f0d1a2d9cbaef5dd6c371a1ab7c58c7e20e71945704`  
		Last Modified: Tue, 04 Jul 2023 17:00:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dab15d1c6f25f9d41f7cca3c3dbef72f78adfd2c93e1b5118c2540ab35c9ff5`  
		Last Modified: Tue, 04 Jul 2023 17:00:39 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45f1884ccf2c53f7935d0379452a5e07b67da5146f499569abca9707a426a333`  
		Last Modified: Tue, 04 Jul 2023 17:00:52 GMT  
		Size: 87.5 MB (87461916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895d0bb1d3eef4bc781bd9a29370b15b508f63542867d4e350ba9d0414e35543`  
		Last Modified: Tue, 04 Jul 2023 17:00:39 GMT  
		Size: 3.6 KB (3567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:450856d007683a11eed69967457b4ed8325a4811cae92db3e313920af6019084`  
		Last Modified: Tue, 04 Jul 2023 17:00:39 GMT  
		Size: 7.6 KB (7570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:11.0-jammy`

```console
$ docker pull mariadb@sha256:f94bb4868d953fed5220c9d3cdc8449f4c314efb07d3a18eefa6010b383f2ab8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:11.0-jammy` - linux; amd64

```console
$ docker pull mariadb@sha256:c57215c3aabbdb96353ce8b89a7bd6be089f49a4d6bb37f199288a1bf0438a02
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123083360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:011343cf3ec310ee1d70da41536b2ae61e93633dafdba600d865beeb93db6ff8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 18:27:16 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 18:27:16 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 18:27:16 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 18:27:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 18:27:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 18:27:39 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 18:28:14 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.0.2 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 18:28:14 GMT
ARG MARIADB_VERSION=1:11.0.2+maria~ubu2204
# Tue, 04 Jul 2023 18:28:14 GMT
ENV MARIADB_VERSION=1:11.0.2+maria~ubu2204
# Tue, 04 Jul 2023 18:28:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 18:28:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 18:28:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 18:28:33 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 18:28:33 GMT
COPY file:1980cab2a8b7fba7431710370aad263c40d659a4885e66510adf2002b57ddf4c in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 18:28:33 GMT
COPY file:41cd6c305128c82d238b47cc775ecf2262c7b95806428fa87026c43a3d858b56 in /usr/local/bin/ 
# Tue, 04 Jul 2023 18:28:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 18:28:33 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 18:28:33 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:718e898a86ffe915c46f60c599bc87928aa5e7e3a9434cbf52066b49651d3a1f`  
		Last Modified: Tue, 04 Jul 2023 18:32:00 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bd7a143a6c5d92cccbae0a38df554277f44cb4dbfcb668436dc5ed3398144a`  
		Last Modified: Tue, 04 Jul 2023 18:32:01 GMT  
		Size: 5.6 MB (5592713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80cdf483b70a4a08d0db0ff26cb8dbdc933588954a3bf91fce2f2544b7be37b8`  
		Last Modified: Tue, 04 Jul 2023 18:31:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c13b197eea76a7fddd36bbf730423197e52a2298e33993c2189bbe5b3d791d8`  
		Last Modified: Tue, 04 Jul 2023 18:32:23 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe76c18bf258b3649fe944d0678c684ed03c8c96ae60ba50b1d470968adb9c9e`  
		Last Modified: Tue, 04 Jul 2023 18:32:35 GMT  
		Size: 87.0 MB (87046060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67fa5c829e7fb09dbd973997e9219701b99fa6e16d0d5e5a4708ec4f1c60b426`  
		Last Modified: Tue, 04 Jul 2023 18:32:23 GMT  
		Size: 3.6 KB (3566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5cb79f31ff672547bc4a5931db38f52f8900f2b1db24c5179e3da9177b3fc49`  
		Last Modified: Tue, 04 Jul 2023 18:32:23 GMT  
		Size: 7.6 KB (7568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:11.0-jammy` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:35f86cd13f6b6368ad65a3422d572019aaba33daaadd8f312c42dc5dff0d0562
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117620280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4935389ac6b4f1f7ac98fe3b47b5411e8e30630073672e0f21a2117f04e3e160`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 15:48:55 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 15:48:55 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 15:48:56 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 15:49:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 15:49:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 15:49:12 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 15:49:43 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.0.2 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 15:49:43 GMT
ARG MARIADB_VERSION=1:11.0.2+maria~ubu2204
# Tue, 04 Jul 2023 15:49:43 GMT
ENV MARIADB_VERSION=1:11.0.2+maria~ubu2204
# Tue, 04 Jul 2023 15:49:43 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 15:49:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 15:49:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 15:50:01 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 15:50:01 GMT
COPY file:1980cab2a8b7fba7431710370aad263c40d659a4885e66510adf2002b57ddf4c in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 15:50:01 GMT
COPY file:41cd6c305128c82d238b47cc775ecf2262c7b95806428fa87026c43a3d858b56 in /usr/local/bin/ 
# Tue, 04 Jul 2023 15:50:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 15:50:01 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 15:50:01 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f226d4d968a5322b60d61898c78418afeeb62f9a8613d9939d2546229a59ed0`  
		Last Modified: Tue, 04 Jul 2023 15:53:12 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a718d9544847f819e9859244c57b1093e55eb4bbd1d50066804d9ddd24d9c2c`  
		Last Modified: Tue, 04 Jul 2023 15:53:12 GMT  
		Size: 5.4 MB (5406735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad17cece0015293005bd369ad4550b0faa2ef78f55de897f35a48e5b101b83c8`  
		Last Modified: Tue, 04 Jul 2023 15:53:10 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d645dfb141364d7dba62264383035be88d4b865ee99fde0634f178451ceb0f`  
		Last Modified: Tue, 04 Jul 2023 15:53:32 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad716fe25d457aa9fbaa4da59699c447a5e6bad763f5581966bfe4e9756f44ea`  
		Last Modified: Tue, 04 Jul 2023 15:53:42 GMT  
		Size: 83.8 MB (83809168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be4f5d63350215e844e2f9a8409682ffcea79777da31fd1235cb15d19ac85c0`  
		Last Modified: Tue, 04 Jul 2023 15:53:32 GMT  
		Size: 3.6 KB (3565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d127bd39936fe36a0d7b70697a79791a2d2e733708dde4f91a6b31b949e07e6b`  
		Last Modified: Tue, 04 Jul 2023 15:53:32 GMT  
		Size: 7.6 KB (7568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:11.0-jammy` - linux; ppc64le

```console
$ docker pull mariadb@sha256:2b2ed944def75ab4f8dd292d7682dd4d508d2d834b24a1811cfaccfe8f9fd20e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.7 MB (131748397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ec1500d07e746be7f4e6631e0714883d1aadffd88d60f0d280abbf1420a07aa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:45:53 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:45:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:45:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:45:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:45:56 GMT
ADD file:8c2fc380378944326d602742fde0e30458cd3e82012847b0f7e09c7184bfd135 in / 
# Wed, 28 Jun 2023 08:45:57 GMT
CMD ["/bin/bash"]
# Wed, 05 Jul 2023 01:06:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 05 Jul 2023 01:06:57 GMT
ENV GOSU_VERSION=1.14
# Wed, 05 Jul 2023 01:06:57 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 05 Jul 2023 01:07:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 05 Jul 2023 01:07:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 05 Jul 2023 01:07:36 GMT
ENV LANG=C.UTF-8
# Wed, 05 Jul 2023 01:08:51 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.0.2 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Wed, 05 Jul 2023 01:08:52 GMT
ARG MARIADB_VERSION=1:11.0.2+maria~ubu2204
# Wed, 05 Jul 2023 01:08:54 GMT
ENV MARIADB_VERSION=1:11.0.2+maria~ubu2204
# Wed, 05 Jul 2023 01:08:56 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
# Wed, 05 Jul 2023 01:09:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 05 Jul 2023 01:09:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Wed, 05 Jul 2023 01:10:00 GMT
VOLUME [/var/lib/mysql]
# Wed, 05 Jul 2023 01:10:00 GMT
COPY file:1980cab2a8b7fba7431710370aad263c40d659a4885e66510adf2002b57ddf4c in /usr/local/bin/healthcheck.sh 
# Wed, 05 Jul 2023 01:10:00 GMT
COPY file:41cd6c305128c82d238b47cc775ecf2262c7b95806428fa87026c43a3d858b56 in /usr/local/bin/ 
# Wed, 05 Jul 2023 01:10:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Jul 2023 01:10:02 GMT
EXPOSE 3306
# Wed, 05 Jul 2023 01:10:03 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:7faa46ce6b6f5c34485980029504c3995e38149d0bca67d8b976c5dbb3673644`  
		Last Modified: Tue, 04 Jul 2023 04:42:31 GMT  
		Size: 35.7 MB (35711469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af03c7013049bbb43a9d70711423a0aa0933ad63d557a33679e987f9f4552c2`  
		Last Modified: Wed, 05 Jul 2023 01:19:30 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fae131e82b0a7c398eb2a917463894a99192198e537fa4a742953dfdec5d9a5`  
		Last Modified: Wed, 05 Jul 2023 01:19:32 GMT  
		Size: 6.0 MB (6017861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c002ce052617f5efe1f7afc4ec819f1f45b350c5956b79ee09c9bd522fe18736`  
		Last Modified: Wed, 05 Jul 2023 01:19:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8036bf31dcde2e2ac8325b42c737558cf33a8cb4d01e5cedda956b06b87e05b1`  
		Last Modified: Wed, 05 Jul 2023 01:20:09 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d3a3242885374320250cbe4559b4118f1a835c6434f7905bb2ecf1f0135e49`  
		Last Modified: Wed, 05 Jul 2023 01:20:34 GMT  
		Size: 90.0 MB (90005706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb4f4475038f4dcfbb395f132f635565400316ed33037211135421a08449cb55`  
		Last Modified: Wed, 05 Jul 2023 01:20:09 GMT  
		Size: 3.6 KB (3564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3156cef64baa3f1944fde330137217b9cab7a8724be1ce677aed5b374711228`  
		Last Modified: Wed, 05 Jul 2023 01:20:09 GMT  
		Size: 7.6 KB (7567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:11.0-jammy` - linux; s390x

```console
$ docker pull mariadb@sha256:fec237d61ee4f020ee1942a5ce7ba77851271df7760c330791d49d21e38fd76d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.6 MB (121591761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd61cf2f3f72cf840df9a6079260a2004a1aaedaef78506d8c73ba968e19edfe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:53:20 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:53:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:53:22 GMT
ADD file:fa0aef35be7808c8fd6751a52bdec4dd81057e2fcaa075c547a1db53640dae9a in / 
# Wed, 28 Jun 2023 08:53:22 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 16:55:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 16:55:27 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 16:55:27 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 16:55:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 16:55:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 16:55:44 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 16:56:25 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.0.2 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 16:56:25 GMT
ARG MARIADB_VERSION=1:11.0.2+maria~ubu2204
# Tue, 04 Jul 2023 16:56:25 GMT
ENV MARIADB_VERSION=1:11.0.2+maria~ubu2204
# Tue, 04 Jul 2023 16:56:25 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 16:56:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 16:56:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 16:56:47 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 16:56:47 GMT
COPY file:1980cab2a8b7fba7431710370aad263c40d659a4885e66510adf2002b57ddf4c in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 16:56:47 GMT
COPY file:41cd6c305128c82d238b47cc775ecf2262c7b95806428fa87026c43a3d858b56 in /usr/local/bin/ 
# Tue, 04 Jul 2023 16:56:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 16:56:48 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 16:56:48 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:ce02ee0330980398d6a84a50abfa1a8c4d1cba27cbd7442b79f4aa1b1a14020d`  
		Last Modified: Tue, 04 Jul 2023 13:08:30 GMT  
		Size: 28.6 MB (28645696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16fb1ab422c0ae864df4333ba064fd3a16ef9b10862dca7b3320a9fb32c7e0bd`  
		Last Modified: Tue, 04 Jul 2023 17:00:17 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be60fdd8cf07af19113cd853d2f0ebedd02fc5cb31582325b43c0d50a323535`  
		Last Modified: Tue, 04 Jul 2023 17:00:18 GMT  
		Size: 5.5 MB (5470782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1374c790d73360e41f53f0d1a2d9cbaef5dd6c371a1ab7c58c7e20e71945704`  
		Last Modified: Tue, 04 Jul 2023 17:00:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dab15d1c6f25f9d41f7cca3c3dbef72f78adfd2c93e1b5118c2540ab35c9ff5`  
		Last Modified: Tue, 04 Jul 2023 17:00:39 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45f1884ccf2c53f7935d0379452a5e07b67da5146f499569abca9707a426a333`  
		Last Modified: Tue, 04 Jul 2023 17:00:52 GMT  
		Size: 87.5 MB (87461916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895d0bb1d3eef4bc781bd9a29370b15b508f63542867d4e350ba9d0414e35543`  
		Last Modified: Tue, 04 Jul 2023 17:00:39 GMT  
		Size: 3.6 KB (3567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:450856d007683a11eed69967457b4ed8325a4811cae92db3e313920af6019084`  
		Last Modified: Tue, 04 Jul 2023 17:00:39 GMT  
		Size: 7.6 KB (7570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:11.0.3`

```console
$ docker pull mariadb@sha256:eb37f58646a901dc7727cf448cae36daaefaba79de33b5058dab79aa4c04aefb
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 0

## `mariadb:11.0.3-jammy`

```console
$ docker pull mariadb@sha256:eb37f58646a901dc7727cf448cae36daaefaba79de33b5058dab79aa4c04aefb
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 0

## `mariadb:11.1-rc`

```console
$ docker pull mariadb@sha256:cded8337bc683dff87d051a67a5db644816e28987f14e6f2ce0ccaf630f0c4b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:11.1-rc` - linux; amd64

```console
$ docker pull mariadb@sha256:8774e3d7ee291b6f1a5a3915aab8bf46f9ed5053185a3717561bfa82222416a0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123150513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5a9439794dd4358658805a3d955ab59d73e2c4bd562a3931fae4f43b9ebf19d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 18:27:16 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 18:27:16 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 18:27:16 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 18:27:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 18:27:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 18:27:39 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 18:27:39 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.1.1 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 18:27:39 GMT
ARG MARIADB_VERSION=1:11.1.1+maria~ubu2204
# Tue, 04 Jul 2023 18:27:39 GMT
ENV MARIADB_VERSION=1:11.1.1+maria~ubu2204
# Tue, 04 Jul 2023 18:27:39 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.1.1/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 18:27:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.1.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 18:28:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.1.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 18:28:02 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 18:28:03 GMT
COPY file:1980cab2a8b7fba7431710370aad263c40d659a4885e66510adf2002b57ddf4c in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 18:28:03 GMT
COPY file:41cd6c305128c82d238b47cc775ecf2262c7b95806428fa87026c43a3d858b56 in /usr/local/bin/ 
# Tue, 04 Jul 2023 18:28:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 18:28:03 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 18:28:03 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:718e898a86ffe915c46f60c599bc87928aa5e7e3a9434cbf52066b49651d3a1f`  
		Last Modified: Tue, 04 Jul 2023 18:32:00 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bd7a143a6c5d92cccbae0a38df554277f44cb4dbfcb668436dc5ed3398144a`  
		Last Modified: Tue, 04 Jul 2023 18:32:01 GMT  
		Size: 5.6 MB (5592713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80cdf483b70a4a08d0db0ff26cb8dbdc933588954a3bf91fce2f2544b7be37b8`  
		Last Modified: Tue, 04 Jul 2023 18:31:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b82ab599a4fbd4785060b9af603f7890d3622eba02eb23d31d7c87f8075ca232`  
		Last Modified: Tue, 04 Jul 2023 18:31:58 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d6556a37154c2a0a7d56b77704afbf59ca5558e9a7ea1b4fc79cefca660ce9`  
		Last Modified: Tue, 04 Jul 2023 18:32:10 GMT  
		Size: 87.1 MB (87113219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aab1772f362f5a1932cea6bd4d693afe3111afc1a4edb880b073fe242b8503f`  
		Last Modified: Tue, 04 Jul 2023 18:31:58 GMT  
		Size: 3.6 KB (3563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d246961b13fab9b449fc8a804e2e915bd77386f61520b0f90d90fbcd0d7484`  
		Last Modified: Tue, 04 Jul 2023 18:31:58 GMT  
		Size: 7.6 KB (7565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:11.1-rc` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:956fe12689977baf73a944dbb89baf5b147ed695c1a43d28e5d98ed7d643c08f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117696296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:deea06397718d08697721e70352f05dbb9ccde45f8e17340645b5e456c4bb61b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 15:48:55 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 15:48:55 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 15:48:56 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 15:49:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 15:49:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 15:49:12 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 15:49:12 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.1.1 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 15:49:12 GMT
ARG MARIADB_VERSION=1:11.1.1+maria~ubu2204
# Tue, 04 Jul 2023 15:49:12 GMT
ENV MARIADB_VERSION=1:11.1.1+maria~ubu2204
# Tue, 04 Jul 2023 15:49:12 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.1.1/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 15:49:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.1.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 15:49:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.1.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 15:49:38 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 15:49:38 GMT
COPY file:1980cab2a8b7fba7431710370aad263c40d659a4885e66510adf2002b57ddf4c in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 15:49:38 GMT
COPY file:41cd6c305128c82d238b47cc775ecf2262c7b95806428fa87026c43a3d858b56 in /usr/local/bin/ 
# Tue, 04 Jul 2023 15:49:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 15:49:38 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 15:49:38 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f226d4d968a5322b60d61898c78418afeeb62f9a8613d9939d2546229a59ed0`  
		Last Modified: Tue, 04 Jul 2023 15:53:12 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a718d9544847f819e9859244c57b1093e55eb4bbd1d50066804d9ddd24d9c2c`  
		Last Modified: Tue, 04 Jul 2023 15:53:12 GMT  
		Size: 5.4 MB (5406735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad17cece0015293005bd369ad4550b0faa2ef78f55de897f35a48e5b101b83c8`  
		Last Modified: Tue, 04 Jul 2023 15:53:10 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f4ea6b6ff6af99737a45901ace343d55f7eb4bf7362b1ebb27f9eafa03b443`  
		Last Modified: Tue, 04 Jul 2023 15:53:10 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f75dd35d51c665f406c4b0adcfd54225cb50668af2637a07303a2b084b2d6d30`  
		Last Modified: Tue, 04 Jul 2023 15:53:19 GMT  
		Size: 83.9 MB (83885183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c44d01c3a37c48f7c25ccd5463879b8d71850453c8019fc47b36a200ef127f5c`  
		Last Modified: Tue, 04 Jul 2023 15:53:10 GMT  
		Size: 3.6 KB (3565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed030bc9c3e422d3437fc0df493e2e27fb79385e60437c13bcf306eaa57a5a2f`  
		Last Modified: Tue, 04 Jul 2023 15:53:10 GMT  
		Size: 7.6 KB (7569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:11.1-rc` - linux; ppc64le

```console
$ docker pull mariadb@sha256:ea6c63b76a55d3bddd2da50df1f9411140d7b019fde5596cee40ada67cf13c2b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131840846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd21e7c9fae803d685d8cc7aa1f03936fae99b57211a8f2a8c927e51eabc5792`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:45:53 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:45:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:45:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:45:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:45:56 GMT
ADD file:8c2fc380378944326d602742fde0e30458cd3e82012847b0f7e09c7184bfd135 in / 
# Wed, 28 Jun 2023 08:45:57 GMT
CMD ["/bin/bash"]
# Wed, 05 Jul 2023 01:06:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 05 Jul 2023 01:06:57 GMT
ENV GOSU_VERSION=1.14
# Wed, 05 Jul 2023 01:06:57 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 05 Jul 2023 01:07:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 05 Jul 2023 01:07:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 05 Jul 2023 01:07:36 GMT
ENV LANG=C.UTF-8
# Wed, 05 Jul 2023 01:07:37 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.1.1 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Wed, 05 Jul 2023 01:07:37 GMT
ARG MARIADB_VERSION=1:11.1.1+maria~ubu2204
# Wed, 05 Jul 2023 01:07:38 GMT
ENV MARIADB_VERSION=1:11.1.1+maria~ubu2204
# Wed, 05 Jul 2023 01:07:38 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.1.1/repo/ubuntu/ jammy main
# Wed, 05 Jul 2023 01:07:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.1.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 05 Jul 2023 01:08:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.1.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Wed, 05 Jul 2023 01:08:38 GMT
VOLUME [/var/lib/mysql]
# Wed, 05 Jul 2023 01:08:38 GMT
COPY file:1980cab2a8b7fba7431710370aad263c40d659a4885e66510adf2002b57ddf4c in /usr/local/bin/healthcheck.sh 
# Wed, 05 Jul 2023 01:08:38 GMT
COPY file:41cd6c305128c82d238b47cc775ecf2262c7b95806428fa87026c43a3d858b56 in /usr/local/bin/ 
# Wed, 05 Jul 2023 01:08:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Jul 2023 01:08:41 GMT
EXPOSE 3306
# Wed, 05 Jul 2023 01:08:41 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:7faa46ce6b6f5c34485980029504c3995e38149d0bca67d8b976c5dbb3673644`  
		Last Modified: Tue, 04 Jul 2023 04:42:31 GMT  
		Size: 35.7 MB (35711469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af03c7013049bbb43a9d70711423a0aa0933ad63d557a33679e987f9f4552c2`  
		Last Modified: Wed, 05 Jul 2023 01:19:30 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fae131e82b0a7c398eb2a917463894a99192198e537fa4a742953dfdec5d9a5`  
		Last Modified: Wed, 05 Jul 2023 01:19:32 GMT  
		Size: 6.0 MB (6017861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c002ce052617f5efe1f7afc4ec819f1f45b350c5956b79ee09c9bd522fe18736`  
		Last Modified: Wed, 05 Jul 2023 01:19:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9908f50a74c2038253ae01cd286fab767cb167f8b2a3319de974220c8ad6399f`  
		Last Modified: Wed, 05 Jul 2023 01:19:27 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:525aea57a5666be44f5b4fdd987bbd0b801ea69581f5cf3108bf2203562db240`  
		Last Modified: Wed, 05 Jul 2023 01:19:51 GMT  
		Size: 90.1 MB (90098153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0870103cf5b2145a783cc0b30426bbc20317367c29a2b93701604729d8dc8d56`  
		Last Modified: Wed, 05 Jul 2023 01:19:27 GMT  
		Size: 3.6 KB (3565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e274499441f4679a905cca66fa38b1a50b80f6f4638c33ec768ad7a2c52fa53`  
		Last Modified: Wed, 05 Jul 2023 01:19:27 GMT  
		Size: 7.6 KB (7568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:11.1-rc` - linux; s390x

```console
$ docker pull mariadb@sha256:a67040f8a27a0e43ba3ba29ddbd8985f9fc7269f69a170b2e32b14dce28e012e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.6 MB (121637236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a597ef9813bcf18b03749441d80d3d2b35a7d31eeab2031c7dbdcab994feaa98`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:53:20 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:53:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:53:22 GMT
ADD file:fa0aef35be7808c8fd6751a52bdec4dd81057e2fcaa075c547a1db53640dae9a in / 
# Wed, 28 Jun 2023 08:53:22 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 16:55:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 16:55:27 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 16:55:27 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 16:55:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 16:55:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 16:55:44 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 16:55:44 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.1.1 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 16:55:45 GMT
ARG MARIADB_VERSION=1:11.1.1+maria~ubu2204
# Tue, 04 Jul 2023 16:55:45 GMT
ENV MARIADB_VERSION=1:11.1.1+maria~ubu2204
# Tue, 04 Jul 2023 16:55:45 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.1.1/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 16:55:45 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.1.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 16:56:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.1.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 16:56:10 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 16:56:10 GMT
COPY file:1980cab2a8b7fba7431710370aad263c40d659a4885e66510adf2002b57ddf4c in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 16:56:11 GMT
COPY file:41cd6c305128c82d238b47cc775ecf2262c7b95806428fa87026c43a3d858b56 in /usr/local/bin/ 
# Tue, 04 Jul 2023 16:56:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 16:56:11 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 16:56:11 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:ce02ee0330980398d6a84a50abfa1a8c4d1cba27cbd7442b79f4aa1b1a14020d`  
		Last Modified: Tue, 04 Jul 2023 13:08:30 GMT  
		Size: 28.6 MB (28645696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16fb1ab422c0ae864df4333ba064fd3a16ef9b10862dca7b3320a9fb32c7e0bd`  
		Last Modified: Tue, 04 Jul 2023 17:00:17 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be60fdd8cf07af19113cd853d2f0ebedd02fc5cb31582325b43c0d50a323535`  
		Last Modified: Tue, 04 Jul 2023 17:00:18 GMT  
		Size: 5.5 MB (5470782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1374c790d73360e41f53f0d1a2d9cbaef5dd6c371a1ab7c58c7e20e71945704`  
		Last Modified: Tue, 04 Jul 2023 17:00:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e239c05ca62f91445dc7fe0aba563e7bdbeee9f786bfce63d94a946c30d7ac4`  
		Last Modified: Tue, 04 Jul 2023 17:00:16 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbc9bd9f18343edad61efded52e30f678cec5663673b228cca5dedc651cfb2a`  
		Last Modified: Tue, 04 Jul 2023 17:00:29 GMT  
		Size: 87.5 MB (87507393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93527107ba58b4a5ce0c8c2d1a5cf08fb561f881116c9e45240c78eb52600786`  
		Last Modified: Tue, 04 Jul 2023 17:00:16 GMT  
		Size: 3.6 KB (3566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb522e9ad670521288354d322ba484764f992de8bf4484d0595c2d53b2e322e`  
		Last Modified: Tue, 04 Jul 2023 17:00:16 GMT  
		Size: 7.6 KB (7570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:11.1-rc-jammy`

```console
$ docker pull mariadb@sha256:cded8337bc683dff87d051a67a5db644816e28987f14e6f2ce0ccaf630f0c4b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:11.1-rc-jammy` - linux; amd64

```console
$ docker pull mariadb@sha256:8774e3d7ee291b6f1a5a3915aab8bf46f9ed5053185a3717561bfa82222416a0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123150513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5a9439794dd4358658805a3d955ab59d73e2c4bd562a3931fae4f43b9ebf19d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 18:27:16 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 18:27:16 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 18:27:16 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 18:27:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 18:27:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 18:27:39 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 18:27:39 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.1.1 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 18:27:39 GMT
ARG MARIADB_VERSION=1:11.1.1+maria~ubu2204
# Tue, 04 Jul 2023 18:27:39 GMT
ENV MARIADB_VERSION=1:11.1.1+maria~ubu2204
# Tue, 04 Jul 2023 18:27:39 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.1.1/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 18:27:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.1.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 18:28:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.1.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 18:28:02 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 18:28:03 GMT
COPY file:1980cab2a8b7fba7431710370aad263c40d659a4885e66510adf2002b57ddf4c in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 18:28:03 GMT
COPY file:41cd6c305128c82d238b47cc775ecf2262c7b95806428fa87026c43a3d858b56 in /usr/local/bin/ 
# Tue, 04 Jul 2023 18:28:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 18:28:03 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 18:28:03 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:718e898a86ffe915c46f60c599bc87928aa5e7e3a9434cbf52066b49651d3a1f`  
		Last Modified: Tue, 04 Jul 2023 18:32:00 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bd7a143a6c5d92cccbae0a38df554277f44cb4dbfcb668436dc5ed3398144a`  
		Last Modified: Tue, 04 Jul 2023 18:32:01 GMT  
		Size: 5.6 MB (5592713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80cdf483b70a4a08d0db0ff26cb8dbdc933588954a3bf91fce2f2544b7be37b8`  
		Last Modified: Tue, 04 Jul 2023 18:31:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b82ab599a4fbd4785060b9af603f7890d3622eba02eb23d31d7c87f8075ca232`  
		Last Modified: Tue, 04 Jul 2023 18:31:58 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d6556a37154c2a0a7d56b77704afbf59ca5558e9a7ea1b4fc79cefca660ce9`  
		Last Modified: Tue, 04 Jul 2023 18:32:10 GMT  
		Size: 87.1 MB (87113219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aab1772f362f5a1932cea6bd4d693afe3111afc1a4edb880b073fe242b8503f`  
		Last Modified: Tue, 04 Jul 2023 18:31:58 GMT  
		Size: 3.6 KB (3563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d246961b13fab9b449fc8a804e2e915bd77386f61520b0f90d90fbcd0d7484`  
		Last Modified: Tue, 04 Jul 2023 18:31:58 GMT  
		Size: 7.6 KB (7565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:11.1-rc-jammy` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:956fe12689977baf73a944dbb89baf5b147ed695c1a43d28e5d98ed7d643c08f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117696296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:deea06397718d08697721e70352f05dbb9ccde45f8e17340645b5e456c4bb61b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 15:48:55 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 15:48:55 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 15:48:56 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 15:49:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 15:49:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 15:49:12 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 15:49:12 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.1.1 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 15:49:12 GMT
ARG MARIADB_VERSION=1:11.1.1+maria~ubu2204
# Tue, 04 Jul 2023 15:49:12 GMT
ENV MARIADB_VERSION=1:11.1.1+maria~ubu2204
# Tue, 04 Jul 2023 15:49:12 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.1.1/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 15:49:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.1.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 15:49:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.1.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 15:49:38 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 15:49:38 GMT
COPY file:1980cab2a8b7fba7431710370aad263c40d659a4885e66510adf2002b57ddf4c in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 15:49:38 GMT
COPY file:41cd6c305128c82d238b47cc775ecf2262c7b95806428fa87026c43a3d858b56 in /usr/local/bin/ 
# Tue, 04 Jul 2023 15:49:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 15:49:38 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 15:49:38 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f226d4d968a5322b60d61898c78418afeeb62f9a8613d9939d2546229a59ed0`  
		Last Modified: Tue, 04 Jul 2023 15:53:12 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a718d9544847f819e9859244c57b1093e55eb4bbd1d50066804d9ddd24d9c2c`  
		Last Modified: Tue, 04 Jul 2023 15:53:12 GMT  
		Size: 5.4 MB (5406735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad17cece0015293005bd369ad4550b0faa2ef78f55de897f35a48e5b101b83c8`  
		Last Modified: Tue, 04 Jul 2023 15:53:10 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f4ea6b6ff6af99737a45901ace343d55f7eb4bf7362b1ebb27f9eafa03b443`  
		Last Modified: Tue, 04 Jul 2023 15:53:10 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f75dd35d51c665f406c4b0adcfd54225cb50668af2637a07303a2b084b2d6d30`  
		Last Modified: Tue, 04 Jul 2023 15:53:19 GMT  
		Size: 83.9 MB (83885183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c44d01c3a37c48f7c25ccd5463879b8d71850453c8019fc47b36a200ef127f5c`  
		Last Modified: Tue, 04 Jul 2023 15:53:10 GMT  
		Size: 3.6 KB (3565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed030bc9c3e422d3437fc0df493e2e27fb79385e60437c13bcf306eaa57a5a2f`  
		Last Modified: Tue, 04 Jul 2023 15:53:10 GMT  
		Size: 7.6 KB (7569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:11.1-rc-jammy` - linux; ppc64le

```console
$ docker pull mariadb@sha256:ea6c63b76a55d3bddd2da50df1f9411140d7b019fde5596cee40ada67cf13c2b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131840846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd21e7c9fae803d685d8cc7aa1f03936fae99b57211a8f2a8c927e51eabc5792`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:45:53 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:45:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:45:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:45:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:45:56 GMT
ADD file:8c2fc380378944326d602742fde0e30458cd3e82012847b0f7e09c7184bfd135 in / 
# Wed, 28 Jun 2023 08:45:57 GMT
CMD ["/bin/bash"]
# Wed, 05 Jul 2023 01:06:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 05 Jul 2023 01:06:57 GMT
ENV GOSU_VERSION=1.14
# Wed, 05 Jul 2023 01:06:57 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 05 Jul 2023 01:07:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 05 Jul 2023 01:07:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 05 Jul 2023 01:07:36 GMT
ENV LANG=C.UTF-8
# Wed, 05 Jul 2023 01:07:37 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.1.1 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Wed, 05 Jul 2023 01:07:37 GMT
ARG MARIADB_VERSION=1:11.1.1+maria~ubu2204
# Wed, 05 Jul 2023 01:07:38 GMT
ENV MARIADB_VERSION=1:11.1.1+maria~ubu2204
# Wed, 05 Jul 2023 01:07:38 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.1.1/repo/ubuntu/ jammy main
# Wed, 05 Jul 2023 01:07:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.1.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 05 Jul 2023 01:08:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.1.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Wed, 05 Jul 2023 01:08:38 GMT
VOLUME [/var/lib/mysql]
# Wed, 05 Jul 2023 01:08:38 GMT
COPY file:1980cab2a8b7fba7431710370aad263c40d659a4885e66510adf2002b57ddf4c in /usr/local/bin/healthcheck.sh 
# Wed, 05 Jul 2023 01:08:38 GMT
COPY file:41cd6c305128c82d238b47cc775ecf2262c7b95806428fa87026c43a3d858b56 in /usr/local/bin/ 
# Wed, 05 Jul 2023 01:08:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Jul 2023 01:08:41 GMT
EXPOSE 3306
# Wed, 05 Jul 2023 01:08:41 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:7faa46ce6b6f5c34485980029504c3995e38149d0bca67d8b976c5dbb3673644`  
		Last Modified: Tue, 04 Jul 2023 04:42:31 GMT  
		Size: 35.7 MB (35711469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af03c7013049bbb43a9d70711423a0aa0933ad63d557a33679e987f9f4552c2`  
		Last Modified: Wed, 05 Jul 2023 01:19:30 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fae131e82b0a7c398eb2a917463894a99192198e537fa4a742953dfdec5d9a5`  
		Last Modified: Wed, 05 Jul 2023 01:19:32 GMT  
		Size: 6.0 MB (6017861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c002ce052617f5efe1f7afc4ec819f1f45b350c5956b79ee09c9bd522fe18736`  
		Last Modified: Wed, 05 Jul 2023 01:19:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9908f50a74c2038253ae01cd286fab767cb167f8b2a3319de974220c8ad6399f`  
		Last Modified: Wed, 05 Jul 2023 01:19:27 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:525aea57a5666be44f5b4fdd987bbd0b801ea69581f5cf3108bf2203562db240`  
		Last Modified: Wed, 05 Jul 2023 01:19:51 GMT  
		Size: 90.1 MB (90098153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0870103cf5b2145a783cc0b30426bbc20317367c29a2b93701604729d8dc8d56`  
		Last Modified: Wed, 05 Jul 2023 01:19:27 GMT  
		Size: 3.6 KB (3565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e274499441f4679a905cca66fa38b1a50b80f6f4638c33ec768ad7a2c52fa53`  
		Last Modified: Wed, 05 Jul 2023 01:19:27 GMT  
		Size: 7.6 KB (7568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:11.1-rc-jammy` - linux; s390x

```console
$ docker pull mariadb@sha256:a67040f8a27a0e43ba3ba29ddbd8985f9fc7269f69a170b2e32b14dce28e012e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.6 MB (121637236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a597ef9813bcf18b03749441d80d3d2b35a7d31eeab2031c7dbdcab994feaa98`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:53:20 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:53:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:53:22 GMT
ADD file:fa0aef35be7808c8fd6751a52bdec4dd81057e2fcaa075c547a1db53640dae9a in / 
# Wed, 28 Jun 2023 08:53:22 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 16:55:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 16:55:27 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 16:55:27 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 16:55:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 16:55:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 16:55:44 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 16:55:44 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.1.1 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 16:55:45 GMT
ARG MARIADB_VERSION=1:11.1.1+maria~ubu2204
# Tue, 04 Jul 2023 16:55:45 GMT
ENV MARIADB_VERSION=1:11.1.1+maria~ubu2204
# Tue, 04 Jul 2023 16:55:45 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.1.1/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 16:55:45 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.1.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 16:56:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.1.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 16:56:10 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 16:56:10 GMT
COPY file:1980cab2a8b7fba7431710370aad263c40d659a4885e66510adf2002b57ddf4c in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 16:56:11 GMT
COPY file:41cd6c305128c82d238b47cc775ecf2262c7b95806428fa87026c43a3d858b56 in /usr/local/bin/ 
# Tue, 04 Jul 2023 16:56:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 16:56:11 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 16:56:11 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:ce02ee0330980398d6a84a50abfa1a8c4d1cba27cbd7442b79f4aa1b1a14020d`  
		Last Modified: Tue, 04 Jul 2023 13:08:30 GMT  
		Size: 28.6 MB (28645696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16fb1ab422c0ae864df4333ba064fd3a16ef9b10862dca7b3320a9fb32c7e0bd`  
		Last Modified: Tue, 04 Jul 2023 17:00:17 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be60fdd8cf07af19113cd853d2f0ebedd02fc5cb31582325b43c0d50a323535`  
		Last Modified: Tue, 04 Jul 2023 17:00:18 GMT  
		Size: 5.5 MB (5470782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1374c790d73360e41f53f0d1a2d9cbaef5dd6c371a1ab7c58c7e20e71945704`  
		Last Modified: Tue, 04 Jul 2023 17:00:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e239c05ca62f91445dc7fe0aba563e7bdbeee9f786bfce63d94a946c30d7ac4`  
		Last Modified: Tue, 04 Jul 2023 17:00:16 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbc9bd9f18343edad61efded52e30f678cec5663673b228cca5dedc651cfb2a`  
		Last Modified: Tue, 04 Jul 2023 17:00:29 GMT  
		Size: 87.5 MB (87507393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93527107ba58b4a5ce0c8c2d1a5cf08fb561f881116c9e45240c78eb52600786`  
		Last Modified: Tue, 04 Jul 2023 17:00:16 GMT  
		Size: 3.6 KB (3566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb522e9ad670521288354d322ba484764f992de8bf4484d0595c2d53b2e322e`  
		Last Modified: Tue, 04 Jul 2023 17:00:16 GMT  
		Size: 7.6 KB (7570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:11.1.1-rc`

```console
$ docker pull mariadb@sha256:cded8337bc683dff87d051a67a5db644816e28987f14e6f2ce0ccaf630f0c4b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:11.1.1-rc` - linux; amd64

```console
$ docker pull mariadb@sha256:8774e3d7ee291b6f1a5a3915aab8bf46f9ed5053185a3717561bfa82222416a0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123150513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5a9439794dd4358658805a3d955ab59d73e2c4bd562a3931fae4f43b9ebf19d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 18:27:16 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 18:27:16 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 18:27:16 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 18:27:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 18:27:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 18:27:39 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 18:27:39 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.1.1 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 18:27:39 GMT
ARG MARIADB_VERSION=1:11.1.1+maria~ubu2204
# Tue, 04 Jul 2023 18:27:39 GMT
ENV MARIADB_VERSION=1:11.1.1+maria~ubu2204
# Tue, 04 Jul 2023 18:27:39 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.1.1/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 18:27:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.1.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 18:28:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.1.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 18:28:02 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 18:28:03 GMT
COPY file:1980cab2a8b7fba7431710370aad263c40d659a4885e66510adf2002b57ddf4c in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 18:28:03 GMT
COPY file:41cd6c305128c82d238b47cc775ecf2262c7b95806428fa87026c43a3d858b56 in /usr/local/bin/ 
# Tue, 04 Jul 2023 18:28:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 18:28:03 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 18:28:03 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:718e898a86ffe915c46f60c599bc87928aa5e7e3a9434cbf52066b49651d3a1f`  
		Last Modified: Tue, 04 Jul 2023 18:32:00 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bd7a143a6c5d92cccbae0a38df554277f44cb4dbfcb668436dc5ed3398144a`  
		Last Modified: Tue, 04 Jul 2023 18:32:01 GMT  
		Size: 5.6 MB (5592713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80cdf483b70a4a08d0db0ff26cb8dbdc933588954a3bf91fce2f2544b7be37b8`  
		Last Modified: Tue, 04 Jul 2023 18:31:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b82ab599a4fbd4785060b9af603f7890d3622eba02eb23d31d7c87f8075ca232`  
		Last Modified: Tue, 04 Jul 2023 18:31:58 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d6556a37154c2a0a7d56b77704afbf59ca5558e9a7ea1b4fc79cefca660ce9`  
		Last Modified: Tue, 04 Jul 2023 18:32:10 GMT  
		Size: 87.1 MB (87113219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aab1772f362f5a1932cea6bd4d693afe3111afc1a4edb880b073fe242b8503f`  
		Last Modified: Tue, 04 Jul 2023 18:31:58 GMT  
		Size: 3.6 KB (3563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d246961b13fab9b449fc8a804e2e915bd77386f61520b0f90d90fbcd0d7484`  
		Last Modified: Tue, 04 Jul 2023 18:31:58 GMT  
		Size: 7.6 KB (7565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:11.1.1-rc` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:956fe12689977baf73a944dbb89baf5b147ed695c1a43d28e5d98ed7d643c08f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117696296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:deea06397718d08697721e70352f05dbb9ccde45f8e17340645b5e456c4bb61b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 15:48:55 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 15:48:55 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 15:48:56 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 15:49:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 15:49:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 15:49:12 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 15:49:12 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.1.1 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 15:49:12 GMT
ARG MARIADB_VERSION=1:11.1.1+maria~ubu2204
# Tue, 04 Jul 2023 15:49:12 GMT
ENV MARIADB_VERSION=1:11.1.1+maria~ubu2204
# Tue, 04 Jul 2023 15:49:12 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.1.1/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 15:49:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.1.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 15:49:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.1.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 15:49:38 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 15:49:38 GMT
COPY file:1980cab2a8b7fba7431710370aad263c40d659a4885e66510adf2002b57ddf4c in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 15:49:38 GMT
COPY file:41cd6c305128c82d238b47cc775ecf2262c7b95806428fa87026c43a3d858b56 in /usr/local/bin/ 
# Tue, 04 Jul 2023 15:49:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 15:49:38 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 15:49:38 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f226d4d968a5322b60d61898c78418afeeb62f9a8613d9939d2546229a59ed0`  
		Last Modified: Tue, 04 Jul 2023 15:53:12 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a718d9544847f819e9859244c57b1093e55eb4bbd1d50066804d9ddd24d9c2c`  
		Last Modified: Tue, 04 Jul 2023 15:53:12 GMT  
		Size: 5.4 MB (5406735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad17cece0015293005bd369ad4550b0faa2ef78f55de897f35a48e5b101b83c8`  
		Last Modified: Tue, 04 Jul 2023 15:53:10 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f4ea6b6ff6af99737a45901ace343d55f7eb4bf7362b1ebb27f9eafa03b443`  
		Last Modified: Tue, 04 Jul 2023 15:53:10 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f75dd35d51c665f406c4b0adcfd54225cb50668af2637a07303a2b084b2d6d30`  
		Last Modified: Tue, 04 Jul 2023 15:53:19 GMT  
		Size: 83.9 MB (83885183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c44d01c3a37c48f7c25ccd5463879b8d71850453c8019fc47b36a200ef127f5c`  
		Last Modified: Tue, 04 Jul 2023 15:53:10 GMT  
		Size: 3.6 KB (3565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed030bc9c3e422d3437fc0df493e2e27fb79385e60437c13bcf306eaa57a5a2f`  
		Last Modified: Tue, 04 Jul 2023 15:53:10 GMT  
		Size: 7.6 KB (7569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:11.1.1-rc` - linux; ppc64le

```console
$ docker pull mariadb@sha256:ea6c63b76a55d3bddd2da50df1f9411140d7b019fde5596cee40ada67cf13c2b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131840846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd21e7c9fae803d685d8cc7aa1f03936fae99b57211a8f2a8c927e51eabc5792`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:45:53 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:45:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:45:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:45:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:45:56 GMT
ADD file:8c2fc380378944326d602742fde0e30458cd3e82012847b0f7e09c7184bfd135 in / 
# Wed, 28 Jun 2023 08:45:57 GMT
CMD ["/bin/bash"]
# Wed, 05 Jul 2023 01:06:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 05 Jul 2023 01:06:57 GMT
ENV GOSU_VERSION=1.14
# Wed, 05 Jul 2023 01:06:57 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 05 Jul 2023 01:07:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 05 Jul 2023 01:07:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 05 Jul 2023 01:07:36 GMT
ENV LANG=C.UTF-8
# Wed, 05 Jul 2023 01:07:37 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.1.1 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Wed, 05 Jul 2023 01:07:37 GMT
ARG MARIADB_VERSION=1:11.1.1+maria~ubu2204
# Wed, 05 Jul 2023 01:07:38 GMT
ENV MARIADB_VERSION=1:11.1.1+maria~ubu2204
# Wed, 05 Jul 2023 01:07:38 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.1.1/repo/ubuntu/ jammy main
# Wed, 05 Jul 2023 01:07:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.1.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 05 Jul 2023 01:08:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.1.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Wed, 05 Jul 2023 01:08:38 GMT
VOLUME [/var/lib/mysql]
# Wed, 05 Jul 2023 01:08:38 GMT
COPY file:1980cab2a8b7fba7431710370aad263c40d659a4885e66510adf2002b57ddf4c in /usr/local/bin/healthcheck.sh 
# Wed, 05 Jul 2023 01:08:38 GMT
COPY file:41cd6c305128c82d238b47cc775ecf2262c7b95806428fa87026c43a3d858b56 in /usr/local/bin/ 
# Wed, 05 Jul 2023 01:08:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Jul 2023 01:08:41 GMT
EXPOSE 3306
# Wed, 05 Jul 2023 01:08:41 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:7faa46ce6b6f5c34485980029504c3995e38149d0bca67d8b976c5dbb3673644`  
		Last Modified: Tue, 04 Jul 2023 04:42:31 GMT  
		Size: 35.7 MB (35711469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af03c7013049bbb43a9d70711423a0aa0933ad63d557a33679e987f9f4552c2`  
		Last Modified: Wed, 05 Jul 2023 01:19:30 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fae131e82b0a7c398eb2a917463894a99192198e537fa4a742953dfdec5d9a5`  
		Last Modified: Wed, 05 Jul 2023 01:19:32 GMT  
		Size: 6.0 MB (6017861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c002ce052617f5efe1f7afc4ec819f1f45b350c5956b79ee09c9bd522fe18736`  
		Last Modified: Wed, 05 Jul 2023 01:19:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9908f50a74c2038253ae01cd286fab767cb167f8b2a3319de974220c8ad6399f`  
		Last Modified: Wed, 05 Jul 2023 01:19:27 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:525aea57a5666be44f5b4fdd987bbd0b801ea69581f5cf3108bf2203562db240`  
		Last Modified: Wed, 05 Jul 2023 01:19:51 GMT  
		Size: 90.1 MB (90098153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0870103cf5b2145a783cc0b30426bbc20317367c29a2b93701604729d8dc8d56`  
		Last Modified: Wed, 05 Jul 2023 01:19:27 GMT  
		Size: 3.6 KB (3565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e274499441f4679a905cca66fa38b1a50b80f6f4638c33ec768ad7a2c52fa53`  
		Last Modified: Wed, 05 Jul 2023 01:19:27 GMT  
		Size: 7.6 KB (7568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:11.1.1-rc` - linux; s390x

```console
$ docker pull mariadb@sha256:a67040f8a27a0e43ba3ba29ddbd8985f9fc7269f69a170b2e32b14dce28e012e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.6 MB (121637236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a597ef9813bcf18b03749441d80d3d2b35a7d31eeab2031c7dbdcab994feaa98`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:53:20 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:53:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:53:22 GMT
ADD file:fa0aef35be7808c8fd6751a52bdec4dd81057e2fcaa075c547a1db53640dae9a in / 
# Wed, 28 Jun 2023 08:53:22 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 16:55:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 16:55:27 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 16:55:27 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 16:55:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 16:55:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 16:55:44 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 16:55:44 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.1.1 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 16:55:45 GMT
ARG MARIADB_VERSION=1:11.1.1+maria~ubu2204
# Tue, 04 Jul 2023 16:55:45 GMT
ENV MARIADB_VERSION=1:11.1.1+maria~ubu2204
# Tue, 04 Jul 2023 16:55:45 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.1.1/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 16:55:45 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.1.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 16:56:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.1.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 16:56:10 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 16:56:10 GMT
COPY file:1980cab2a8b7fba7431710370aad263c40d659a4885e66510adf2002b57ddf4c in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 16:56:11 GMT
COPY file:41cd6c305128c82d238b47cc775ecf2262c7b95806428fa87026c43a3d858b56 in /usr/local/bin/ 
# Tue, 04 Jul 2023 16:56:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 16:56:11 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 16:56:11 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:ce02ee0330980398d6a84a50abfa1a8c4d1cba27cbd7442b79f4aa1b1a14020d`  
		Last Modified: Tue, 04 Jul 2023 13:08:30 GMT  
		Size: 28.6 MB (28645696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16fb1ab422c0ae864df4333ba064fd3a16ef9b10862dca7b3320a9fb32c7e0bd`  
		Last Modified: Tue, 04 Jul 2023 17:00:17 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be60fdd8cf07af19113cd853d2f0ebedd02fc5cb31582325b43c0d50a323535`  
		Last Modified: Tue, 04 Jul 2023 17:00:18 GMT  
		Size: 5.5 MB (5470782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1374c790d73360e41f53f0d1a2d9cbaef5dd6c371a1ab7c58c7e20e71945704`  
		Last Modified: Tue, 04 Jul 2023 17:00:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e239c05ca62f91445dc7fe0aba563e7bdbeee9f786bfce63d94a946c30d7ac4`  
		Last Modified: Tue, 04 Jul 2023 17:00:16 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbc9bd9f18343edad61efded52e30f678cec5663673b228cca5dedc651cfb2a`  
		Last Modified: Tue, 04 Jul 2023 17:00:29 GMT  
		Size: 87.5 MB (87507393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93527107ba58b4a5ce0c8c2d1a5cf08fb561f881116c9e45240c78eb52600786`  
		Last Modified: Tue, 04 Jul 2023 17:00:16 GMT  
		Size: 3.6 KB (3566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb522e9ad670521288354d322ba484764f992de8bf4484d0595c2d53b2e322e`  
		Last Modified: Tue, 04 Jul 2023 17:00:16 GMT  
		Size: 7.6 KB (7570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:11.1.1-rc-jammy`

```console
$ docker pull mariadb@sha256:cded8337bc683dff87d051a67a5db644816e28987f14e6f2ce0ccaf630f0c4b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:11.1.1-rc-jammy` - linux; amd64

```console
$ docker pull mariadb@sha256:8774e3d7ee291b6f1a5a3915aab8bf46f9ed5053185a3717561bfa82222416a0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123150513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5a9439794dd4358658805a3d955ab59d73e2c4bd562a3931fae4f43b9ebf19d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 18:27:16 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 18:27:16 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 18:27:16 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 18:27:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 18:27:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 18:27:39 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 18:27:39 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.1.1 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 18:27:39 GMT
ARG MARIADB_VERSION=1:11.1.1+maria~ubu2204
# Tue, 04 Jul 2023 18:27:39 GMT
ENV MARIADB_VERSION=1:11.1.1+maria~ubu2204
# Tue, 04 Jul 2023 18:27:39 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.1.1/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 18:27:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.1.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 18:28:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.1.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 18:28:02 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 18:28:03 GMT
COPY file:1980cab2a8b7fba7431710370aad263c40d659a4885e66510adf2002b57ddf4c in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 18:28:03 GMT
COPY file:41cd6c305128c82d238b47cc775ecf2262c7b95806428fa87026c43a3d858b56 in /usr/local/bin/ 
# Tue, 04 Jul 2023 18:28:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 18:28:03 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 18:28:03 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:718e898a86ffe915c46f60c599bc87928aa5e7e3a9434cbf52066b49651d3a1f`  
		Last Modified: Tue, 04 Jul 2023 18:32:00 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bd7a143a6c5d92cccbae0a38df554277f44cb4dbfcb668436dc5ed3398144a`  
		Last Modified: Tue, 04 Jul 2023 18:32:01 GMT  
		Size: 5.6 MB (5592713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80cdf483b70a4a08d0db0ff26cb8dbdc933588954a3bf91fce2f2544b7be37b8`  
		Last Modified: Tue, 04 Jul 2023 18:31:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b82ab599a4fbd4785060b9af603f7890d3622eba02eb23d31d7c87f8075ca232`  
		Last Modified: Tue, 04 Jul 2023 18:31:58 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d6556a37154c2a0a7d56b77704afbf59ca5558e9a7ea1b4fc79cefca660ce9`  
		Last Modified: Tue, 04 Jul 2023 18:32:10 GMT  
		Size: 87.1 MB (87113219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aab1772f362f5a1932cea6bd4d693afe3111afc1a4edb880b073fe242b8503f`  
		Last Modified: Tue, 04 Jul 2023 18:31:58 GMT  
		Size: 3.6 KB (3563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d246961b13fab9b449fc8a804e2e915bd77386f61520b0f90d90fbcd0d7484`  
		Last Modified: Tue, 04 Jul 2023 18:31:58 GMT  
		Size: 7.6 KB (7565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:11.1.1-rc-jammy` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:956fe12689977baf73a944dbb89baf5b147ed695c1a43d28e5d98ed7d643c08f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117696296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:deea06397718d08697721e70352f05dbb9ccde45f8e17340645b5e456c4bb61b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 15:48:55 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 15:48:55 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 15:48:56 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 15:49:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 15:49:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 15:49:12 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 15:49:12 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.1.1 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 15:49:12 GMT
ARG MARIADB_VERSION=1:11.1.1+maria~ubu2204
# Tue, 04 Jul 2023 15:49:12 GMT
ENV MARIADB_VERSION=1:11.1.1+maria~ubu2204
# Tue, 04 Jul 2023 15:49:12 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.1.1/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 15:49:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.1.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 15:49:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.1.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 15:49:38 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 15:49:38 GMT
COPY file:1980cab2a8b7fba7431710370aad263c40d659a4885e66510adf2002b57ddf4c in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 15:49:38 GMT
COPY file:41cd6c305128c82d238b47cc775ecf2262c7b95806428fa87026c43a3d858b56 in /usr/local/bin/ 
# Tue, 04 Jul 2023 15:49:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 15:49:38 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 15:49:38 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f226d4d968a5322b60d61898c78418afeeb62f9a8613d9939d2546229a59ed0`  
		Last Modified: Tue, 04 Jul 2023 15:53:12 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a718d9544847f819e9859244c57b1093e55eb4bbd1d50066804d9ddd24d9c2c`  
		Last Modified: Tue, 04 Jul 2023 15:53:12 GMT  
		Size: 5.4 MB (5406735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad17cece0015293005bd369ad4550b0faa2ef78f55de897f35a48e5b101b83c8`  
		Last Modified: Tue, 04 Jul 2023 15:53:10 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f4ea6b6ff6af99737a45901ace343d55f7eb4bf7362b1ebb27f9eafa03b443`  
		Last Modified: Tue, 04 Jul 2023 15:53:10 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f75dd35d51c665f406c4b0adcfd54225cb50668af2637a07303a2b084b2d6d30`  
		Last Modified: Tue, 04 Jul 2023 15:53:19 GMT  
		Size: 83.9 MB (83885183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c44d01c3a37c48f7c25ccd5463879b8d71850453c8019fc47b36a200ef127f5c`  
		Last Modified: Tue, 04 Jul 2023 15:53:10 GMT  
		Size: 3.6 KB (3565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed030bc9c3e422d3437fc0df493e2e27fb79385e60437c13bcf306eaa57a5a2f`  
		Last Modified: Tue, 04 Jul 2023 15:53:10 GMT  
		Size: 7.6 KB (7569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:11.1.1-rc-jammy` - linux; ppc64le

```console
$ docker pull mariadb@sha256:ea6c63b76a55d3bddd2da50df1f9411140d7b019fde5596cee40ada67cf13c2b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131840846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd21e7c9fae803d685d8cc7aa1f03936fae99b57211a8f2a8c927e51eabc5792`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:45:53 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:45:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:45:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:45:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:45:56 GMT
ADD file:8c2fc380378944326d602742fde0e30458cd3e82012847b0f7e09c7184bfd135 in / 
# Wed, 28 Jun 2023 08:45:57 GMT
CMD ["/bin/bash"]
# Wed, 05 Jul 2023 01:06:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 05 Jul 2023 01:06:57 GMT
ENV GOSU_VERSION=1.14
# Wed, 05 Jul 2023 01:06:57 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 05 Jul 2023 01:07:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 05 Jul 2023 01:07:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 05 Jul 2023 01:07:36 GMT
ENV LANG=C.UTF-8
# Wed, 05 Jul 2023 01:07:37 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.1.1 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Wed, 05 Jul 2023 01:07:37 GMT
ARG MARIADB_VERSION=1:11.1.1+maria~ubu2204
# Wed, 05 Jul 2023 01:07:38 GMT
ENV MARIADB_VERSION=1:11.1.1+maria~ubu2204
# Wed, 05 Jul 2023 01:07:38 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.1.1/repo/ubuntu/ jammy main
# Wed, 05 Jul 2023 01:07:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.1.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 05 Jul 2023 01:08:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.1.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Wed, 05 Jul 2023 01:08:38 GMT
VOLUME [/var/lib/mysql]
# Wed, 05 Jul 2023 01:08:38 GMT
COPY file:1980cab2a8b7fba7431710370aad263c40d659a4885e66510adf2002b57ddf4c in /usr/local/bin/healthcheck.sh 
# Wed, 05 Jul 2023 01:08:38 GMT
COPY file:41cd6c305128c82d238b47cc775ecf2262c7b95806428fa87026c43a3d858b56 in /usr/local/bin/ 
# Wed, 05 Jul 2023 01:08:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Jul 2023 01:08:41 GMT
EXPOSE 3306
# Wed, 05 Jul 2023 01:08:41 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:7faa46ce6b6f5c34485980029504c3995e38149d0bca67d8b976c5dbb3673644`  
		Last Modified: Tue, 04 Jul 2023 04:42:31 GMT  
		Size: 35.7 MB (35711469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af03c7013049bbb43a9d70711423a0aa0933ad63d557a33679e987f9f4552c2`  
		Last Modified: Wed, 05 Jul 2023 01:19:30 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fae131e82b0a7c398eb2a917463894a99192198e537fa4a742953dfdec5d9a5`  
		Last Modified: Wed, 05 Jul 2023 01:19:32 GMT  
		Size: 6.0 MB (6017861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c002ce052617f5efe1f7afc4ec819f1f45b350c5956b79ee09c9bd522fe18736`  
		Last Modified: Wed, 05 Jul 2023 01:19:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9908f50a74c2038253ae01cd286fab767cb167f8b2a3319de974220c8ad6399f`  
		Last Modified: Wed, 05 Jul 2023 01:19:27 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:525aea57a5666be44f5b4fdd987bbd0b801ea69581f5cf3108bf2203562db240`  
		Last Modified: Wed, 05 Jul 2023 01:19:51 GMT  
		Size: 90.1 MB (90098153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0870103cf5b2145a783cc0b30426bbc20317367c29a2b93701604729d8dc8d56`  
		Last Modified: Wed, 05 Jul 2023 01:19:27 GMT  
		Size: 3.6 KB (3565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e274499441f4679a905cca66fa38b1a50b80f6f4638c33ec768ad7a2c52fa53`  
		Last Modified: Wed, 05 Jul 2023 01:19:27 GMT  
		Size: 7.6 KB (7568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:11.1.1-rc-jammy` - linux; s390x

```console
$ docker pull mariadb@sha256:a67040f8a27a0e43ba3ba29ddbd8985f9fc7269f69a170b2e32b14dce28e012e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.6 MB (121637236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a597ef9813bcf18b03749441d80d3d2b35a7d31eeab2031c7dbdcab994feaa98`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:53:20 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:53:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:53:22 GMT
ADD file:fa0aef35be7808c8fd6751a52bdec4dd81057e2fcaa075c547a1db53640dae9a in / 
# Wed, 28 Jun 2023 08:53:22 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 16:55:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 16:55:27 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 16:55:27 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 16:55:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 16:55:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 16:55:44 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 16:55:44 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.1.1 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 16:55:45 GMT
ARG MARIADB_VERSION=1:11.1.1+maria~ubu2204
# Tue, 04 Jul 2023 16:55:45 GMT
ENV MARIADB_VERSION=1:11.1.1+maria~ubu2204
# Tue, 04 Jul 2023 16:55:45 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.1.1/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 16:55:45 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.1.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 16:56:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.1.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 16:56:10 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 16:56:10 GMT
COPY file:1980cab2a8b7fba7431710370aad263c40d659a4885e66510adf2002b57ddf4c in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 16:56:11 GMT
COPY file:41cd6c305128c82d238b47cc775ecf2262c7b95806428fa87026c43a3d858b56 in /usr/local/bin/ 
# Tue, 04 Jul 2023 16:56:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 16:56:11 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 16:56:11 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:ce02ee0330980398d6a84a50abfa1a8c4d1cba27cbd7442b79f4aa1b1a14020d`  
		Last Modified: Tue, 04 Jul 2023 13:08:30 GMT  
		Size: 28.6 MB (28645696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16fb1ab422c0ae864df4333ba064fd3a16ef9b10862dca7b3320a9fb32c7e0bd`  
		Last Modified: Tue, 04 Jul 2023 17:00:17 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be60fdd8cf07af19113cd853d2f0ebedd02fc5cb31582325b43c0d50a323535`  
		Last Modified: Tue, 04 Jul 2023 17:00:18 GMT  
		Size: 5.5 MB (5470782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1374c790d73360e41f53f0d1a2d9cbaef5dd6c371a1ab7c58c7e20e71945704`  
		Last Modified: Tue, 04 Jul 2023 17:00:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e239c05ca62f91445dc7fe0aba563e7bdbeee9f786bfce63d94a946c30d7ac4`  
		Last Modified: Tue, 04 Jul 2023 17:00:16 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbc9bd9f18343edad61efded52e30f678cec5663673b228cca5dedc651cfb2a`  
		Last Modified: Tue, 04 Jul 2023 17:00:29 GMT  
		Size: 87.5 MB (87507393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93527107ba58b4a5ce0c8c2d1a5cf08fb561f881116c9e45240c78eb52600786`  
		Last Modified: Tue, 04 Jul 2023 17:00:16 GMT  
		Size: 3.6 KB (3566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb522e9ad670521288354d322ba484764f992de8bf4484d0595c2d53b2e322e`  
		Last Modified: Tue, 04 Jul 2023 17:00:16 GMT  
		Size: 7.6 KB (7570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:jammy`

```console
$ docker pull mariadb@sha256:f94bb4868d953fed5220c9d3cdc8449f4c314efb07d3a18eefa6010b383f2ab8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:jammy` - linux; amd64

```console
$ docker pull mariadb@sha256:c57215c3aabbdb96353ce8b89a7bd6be089f49a4d6bb37f199288a1bf0438a02
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123083360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:011343cf3ec310ee1d70da41536b2ae61e93633dafdba600d865beeb93db6ff8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 18:27:16 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 18:27:16 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 18:27:16 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 18:27:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 18:27:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 18:27:39 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 18:28:14 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.0.2 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 18:28:14 GMT
ARG MARIADB_VERSION=1:11.0.2+maria~ubu2204
# Tue, 04 Jul 2023 18:28:14 GMT
ENV MARIADB_VERSION=1:11.0.2+maria~ubu2204
# Tue, 04 Jul 2023 18:28:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 18:28:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 18:28:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 18:28:33 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 18:28:33 GMT
COPY file:1980cab2a8b7fba7431710370aad263c40d659a4885e66510adf2002b57ddf4c in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 18:28:33 GMT
COPY file:41cd6c305128c82d238b47cc775ecf2262c7b95806428fa87026c43a3d858b56 in /usr/local/bin/ 
# Tue, 04 Jul 2023 18:28:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 18:28:33 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 18:28:33 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:718e898a86ffe915c46f60c599bc87928aa5e7e3a9434cbf52066b49651d3a1f`  
		Last Modified: Tue, 04 Jul 2023 18:32:00 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bd7a143a6c5d92cccbae0a38df554277f44cb4dbfcb668436dc5ed3398144a`  
		Last Modified: Tue, 04 Jul 2023 18:32:01 GMT  
		Size: 5.6 MB (5592713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80cdf483b70a4a08d0db0ff26cb8dbdc933588954a3bf91fce2f2544b7be37b8`  
		Last Modified: Tue, 04 Jul 2023 18:31:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c13b197eea76a7fddd36bbf730423197e52a2298e33993c2189bbe5b3d791d8`  
		Last Modified: Tue, 04 Jul 2023 18:32:23 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe76c18bf258b3649fe944d0678c684ed03c8c96ae60ba50b1d470968adb9c9e`  
		Last Modified: Tue, 04 Jul 2023 18:32:35 GMT  
		Size: 87.0 MB (87046060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67fa5c829e7fb09dbd973997e9219701b99fa6e16d0d5e5a4708ec4f1c60b426`  
		Last Modified: Tue, 04 Jul 2023 18:32:23 GMT  
		Size: 3.6 KB (3566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5cb79f31ff672547bc4a5931db38f52f8900f2b1db24c5179e3da9177b3fc49`  
		Last Modified: Tue, 04 Jul 2023 18:32:23 GMT  
		Size: 7.6 KB (7568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:jammy` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:35f86cd13f6b6368ad65a3422d572019aaba33daaadd8f312c42dc5dff0d0562
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117620280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4935389ac6b4f1f7ac98fe3b47b5411e8e30630073672e0f21a2117f04e3e160`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 15:48:55 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 15:48:55 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 15:48:56 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 15:49:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 15:49:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 15:49:12 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 15:49:43 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.0.2 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 15:49:43 GMT
ARG MARIADB_VERSION=1:11.0.2+maria~ubu2204
# Tue, 04 Jul 2023 15:49:43 GMT
ENV MARIADB_VERSION=1:11.0.2+maria~ubu2204
# Tue, 04 Jul 2023 15:49:43 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 15:49:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 15:49:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 15:50:01 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 15:50:01 GMT
COPY file:1980cab2a8b7fba7431710370aad263c40d659a4885e66510adf2002b57ddf4c in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 15:50:01 GMT
COPY file:41cd6c305128c82d238b47cc775ecf2262c7b95806428fa87026c43a3d858b56 in /usr/local/bin/ 
# Tue, 04 Jul 2023 15:50:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 15:50:01 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 15:50:01 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f226d4d968a5322b60d61898c78418afeeb62f9a8613d9939d2546229a59ed0`  
		Last Modified: Tue, 04 Jul 2023 15:53:12 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a718d9544847f819e9859244c57b1093e55eb4bbd1d50066804d9ddd24d9c2c`  
		Last Modified: Tue, 04 Jul 2023 15:53:12 GMT  
		Size: 5.4 MB (5406735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad17cece0015293005bd369ad4550b0faa2ef78f55de897f35a48e5b101b83c8`  
		Last Modified: Tue, 04 Jul 2023 15:53:10 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d645dfb141364d7dba62264383035be88d4b865ee99fde0634f178451ceb0f`  
		Last Modified: Tue, 04 Jul 2023 15:53:32 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad716fe25d457aa9fbaa4da59699c447a5e6bad763f5581966bfe4e9756f44ea`  
		Last Modified: Tue, 04 Jul 2023 15:53:42 GMT  
		Size: 83.8 MB (83809168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be4f5d63350215e844e2f9a8409682ffcea79777da31fd1235cb15d19ac85c0`  
		Last Modified: Tue, 04 Jul 2023 15:53:32 GMT  
		Size: 3.6 KB (3565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d127bd39936fe36a0d7b70697a79791a2d2e733708dde4f91a6b31b949e07e6b`  
		Last Modified: Tue, 04 Jul 2023 15:53:32 GMT  
		Size: 7.6 KB (7568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:jammy` - linux; ppc64le

```console
$ docker pull mariadb@sha256:2b2ed944def75ab4f8dd292d7682dd4d508d2d834b24a1811cfaccfe8f9fd20e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.7 MB (131748397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ec1500d07e746be7f4e6631e0714883d1aadffd88d60f0d280abbf1420a07aa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:45:53 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:45:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:45:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:45:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:45:56 GMT
ADD file:8c2fc380378944326d602742fde0e30458cd3e82012847b0f7e09c7184bfd135 in / 
# Wed, 28 Jun 2023 08:45:57 GMT
CMD ["/bin/bash"]
# Wed, 05 Jul 2023 01:06:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 05 Jul 2023 01:06:57 GMT
ENV GOSU_VERSION=1.14
# Wed, 05 Jul 2023 01:06:57 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 05 Jul 2023 01:07:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 05 Jul 2023 01:07:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 05 Jul 2023 01:07:36 GMT
ENV LANG=C.UTF-8
# Wed, 05 Jul 2023 01:08:51 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.0.2 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Wed, 05 Jul 2023 01:08:52 GMT
ARG MARIADB_VERSION=1:11.0.2+maria~ubu2204
# Wed, 05 Jul 2023 01:08:54 GMT
ENV MARIADB_VERSION=1:11.0.2+maria~ubu2204
# Wed, 05 Jul 2023 01:08:56 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
# Wed, 05 Jul 2023 01:09:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 05 Jul 2023 01:09:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Wed, 05 Jul 2023 01:10:00 GMT
VOLUME [/var/lib/mysql]
# Wed, 05 Jul 2023 01:10:00 GMT
COPY file:1980cab2a8b7fba7431710370aad263c40d659a4885e66510adf2002b57ddf4c in /usr/local/bin/healthcheck.sh 
# Wed, 05 Jul 2023 01:10:00 GMT
COPY file:41cd6c305128c82d238b47cc775ecf2262c7b95806428fa87026c43a3d858b56 in /usr/local/bin/ 
# Wed, 05 Jul 2023 01:10:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Jul 2023 01:10:02 GMT
EXPOSE 3306
# Wed, 05 Jul 2023 01:10:03 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:7faa46ce6b6f5c34485980029504c3995e38149d0bca67d8b976c5dbb3673644`  
		Last Modified: Tue, 04 Jul 2023 04:42:31 GMT  
		Size: 35.7 MB (35711469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af03c7013049bbb43a9d70711423a0aa0933ad63d557a33679e987f9f4552c2`  
		Last Modified: Wed, 05 Jul 2023 01:19:30 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fae131e82b0a7c398eb2a917463894a99192198e537fa4a742953dfdec5d9a5`  
		Last Modified: Wed, 05 Jul 2023 01:19:32 GMT  
		Size: 6.0 MB (6017861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c002ce052617f5efe1f7afc4ec819f1f45b350c5956b79ee09c9bd522fe18736`  
		Last Modified: Wed, 05 Jul 2023 01:19:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8036bf31dcde2e2ac8325b42c737558cf33a8cb4d01e5cedda956b06b87e05b1`  
		Last Modified: Wed, 05 Jul 2023 01:20:09 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d3a3242885374320250cbe4559b4118f1a835c6434f7905bb2ecf1f0135e49`  
		Last Modified: Wed, 05 Jul 2023 01:20:34 GMT  
		Size: 90.0 MB (90005706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb4f4475038f4dcfbb395f132f635565400316ed33037211135421a08449cb55`  
		Last Modified: Wed, 05 Jul 2023 01:20:09 GMT  
		Size: 3.6 KB (3564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3156cef64baa3f1944fde330137217b9cab7a8724be1ce677aed5b374711228`  
		Last Modified: Wed, 05 Jul 2023 01:20:09 GMT  
		Size: 7.6 KB (7567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:jammy` - linux; s390x

```console
$ docker pull mariadb@sha256:fec237d61ee4f020ee1942a5ce7ba77851271df7760c330791d49d21e38fd76d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.6 MB (121591761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd61cf2f3f72cf840df9a6079260a2004a1aaedaef78506d8c73ba968e19edfe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:53:20 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:53:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:53:22 GMT
ADD file:fa0aef35be7808c8fd6751a52bdec4dd81057e2fcaa075c547a1db53640dae9a in / 
# Wed, 28 Jun 2023 08:53:22 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 16:55:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 16:55:27 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 16:55:27 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 16:55:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 16:55:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 16:55:44 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 16:56:25 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.0.2 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 16:56:25 GMT
ARG MARIADB_VERSION=1:11.0.2+maria~ubu2204
# Tue, 04 Jul 2023 16:56:25 GMT
ENV MARIADB_VERSION=1:11.0.2+maria~ubu2204
# Tue, 04 Jul 2023 16:56:25 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 16:56:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 16:56:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 16:56:47 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 16:56:47 GMT
COPY file:1980cab2a8b7fba7431710370aad263c40d659a4885e66510adf2002b57ddf4c in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 16:56:47 GMT
COPY file:41cd6c305128c82d238b47cc775ecf2262c7b95806428fa87026c43a3d858b56 in /usr/local/bin/ 
# Tue, 04 Jul 2023 16:56:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 16:56:48 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 16:56:48 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:ce02ee0330980398d6a84a50abfa1a8c4d1cba27cbd7442b79f4aa1b1a14020d`  
		Last Modified: Tue, 04 Jul 2023 13:08:30 GMT  
		Size: 28.6 MB (28645696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16fb1ab422c0ae864df4333ba064fd3a16ef9b10862dca7b3320a9fb32c7e0bd`  
		Last Modified: Tue, 04 Jul 2023 17:00:17 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be60fdd8cf07af19113cd853d2f0ebedd02fc5cb31582325b43c0d50a323535`  
		Last Modified: Tue, 04 Jul 2023 17:00:18 GMT  
		Size: 5.5 MB (5470782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1374c790d73360e41f53f0d1a2d9cbaef5dd6c371a1ab7c58c7e20e71945704`  
		Last Modified: Tue, 04 Jul 2023 17:00:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dab15d1c6f25f9d41f7cca3c3dbef72f78adfd2c93e1b5118c2540ab35c9ff5`  
		Last Modified: Tue, 04 Jul 2023 17:00:39 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45f1884ccf2c53f7935d0379452a5e07b67da5146f499569abca9707a426a333`  
		Last Modified: Tue, 04 Jul 2023 17:00:52 GMT  
		Size: 87.5 MB (87461916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895d0bb1d3eef4bc781bd9a29370b15b508f63542867d4e350ba9d0414e35543`  
		Last Modified: Tue, 04 Jul 2023 17:00:39 GMT  
		Size: 3.6 KB (3567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:450856d007683a11eed69967457b4ed8325a4811cae92db3e313920af6019084`  
		Last Modified: Tue, 04 Jul 2023 17:00:39 GMT  
		Size: 7.6 KB (7570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:latest`

```console
$ docker pull mariadb@sha256:f94bb4868d953fed5220c9d3cdc8449f4c314efb07d3a18eefa6010b383f2ab8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:latest` - linux; amd64

```console
$ docker pull mariadb@sha256:c57215c3aabbdb96353ce8b89a7bd6be089f49a4d6bb37f199288a1bf0438a02
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123083360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:011343cf3ec310ee1d70da41536b2ae61e93633dafdba600d865beeb93db6ff8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 18:27:16 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 18:27:16 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 18:27:16 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 18:27:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 18:27:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 18:27:39 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 18:28:14 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.0.2 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 18:28:14 GMT
ARG MARIADB_VERSION=1:11.0.2+maria~ubu2204
# Tue, 04 Jul 2023 18:28:14 GMT
ENV MARIADB_VERSION=1:11.0.2+maria~ubu2204
# Tue, 04 Jul 2023 18:28:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 18:28:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 18:28:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 18:28:33 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 18:28:33 GMT
COPY file:1980cab2a8b7fba7431710370aad263c40d659a4885e66510adf2002b57ddf4c in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 18:28:33 GMT
COPY file:41cd6c305128c82d238b47cc775ecf2262c7b95806428fa87026c43a3d858b56 in /usr/local/bin/ 
# Tue, 04 Jul 2023 18:28:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 18:28:33 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 18:28:33 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:718e898a86ffe915c46f60c599bc87928aa5e7e3a9434cbf52066b49651d3a1f`  
		Last Modified: Tue, 04 Jul 2023 18:32:00 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bd7a143a6c5d92cccbae0a38df554277f44cb4dbfcb668436dc5ed3398144a`  
		Last Modified: Tue, 04 Jul 2023 18:32:01 GMT  
		Size: 5.6 MB (5592713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80cdf483b70a4a08d0db0ff26cb8dbdc933588954a3bf91fce2f2544b7be37b8`  
		Last Modified: Tue, 04 Jul 2023 18:31:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c13b197eea76a7fddd36bbf730423197e52a2298e33993c2189bbe5b3d791d8`  
		Last Modified: Tue, 04 Jul 2023 18:32:23 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe76c18bf258b3649fe944d0678c684ed03c8c96ae60ba50b1d470968adb9c9e`  
		Last Modified: Tue, 04 Jul 2023 18:32:35 GMT  
		Size: 87.0 MB (87046060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67fa5c829e7fb09dbd973997e9219701b99fa6e16d0d5e5a4708ec4f1c60b426`  
		Last Modified: Tue, 04 Jul 2023 18:32:23 GMT  
		Size: 3.6 KB (3566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5cb79f31ff672547bc4a5931db38f52f8900f2b1db24c5179e3da9177b3fc49`  
		Last Modified: Tue, 04 Jul 2023 18:32:23 GMT  
		Size: 7.6 KB (7568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:35f86cd13f6b6368ad65a3422d572019aaba33daaadd8f312c42dc5dff0d0562
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117620280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4935389ac6b4f1f7ac98fe3b47b5411e8e30630073672e0f21a2117f04e3e160`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 15:48:55 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 15:48:55 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 15:48:56 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 15:49:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 15:49:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 15:49:12 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 15:49:43 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.0.2 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 15:49:43 GMT
ARG MARIADB_VERSION=1:11.0.2+maria~ubu2204
# Tue, 04 Jul 2023 15:49:43 GMT
ENV MARIADB_VERSION=1:11.0.2+maria~ubu2204
# Tue, 04 Jul 2023 15:49:43 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 15:49:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 15:49:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 15:50:01 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 15:50:01 GMT
COPY file:1980cab2a8b7fba7431710370aad263c40d659a4885e66510adf2002b57ddf4c in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 15:50:01 GMT
COPY file:41cd6c305128c82d238b47cc775ecf2262c7b95806428fa87026c43a3d858b56 in /usr/local/bin/ 
# Tue, 04 Jul 2023 15:50:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 15:50:01 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 15:50:01 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f226d4d968a5322b60d61898c78418afeeb62f9a8613d9939d2546229a59ed0`  
		Last Modified: Tue, 04 Jul 2023 15:53:12 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a718d9544847f819e9859244c57b1093e55eb4bbd1d50066804d9ddd24d9c2c`  
		Last Modified: Tue, 04 Jul 2023 15:53:12 GMT  
		Size: 5.4 MB (5406735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad17cece0015293005bd369ad4550b0faa2ef78f55de897f35a48e5b101b83c8`  
		Last Modified: Tue, 04 Jul 2023 15:53:10 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d645dfb141364d7dba62264383035be88d4b865ee99fde0634f178451ceb0f`  
		Last Modified: Tue, 04 Jul 2023 15:53:32 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad716fe25d457aa9fbaa4da59699c447a5e6bad763f5581966bfe4e9756f44ea`  
		Last Modified: Tue, 04 Jul 2023 15:53:42 GMT  
		Size: 83.8 MB (83809168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be4f5d63350215e844e2f9a8409682ffcea79777da31fd1235cb15d19ac85c0`  
		Last Modified: Tue, 04 Jul 2023 15:53:32 GMT  
		Size: 3.6 KB (3565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d127bd39936fe36a0d7b70697a79791a2d2e733708dde4f91a6b31b949e07e6b`  
		Last Modified: Tue, 04 Jul 2023 15:53:32 GMT  
		Size: 7.6 KB (7568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; ppc64le

```console
$ docker pull mariadb@sha256:2b2ed944def75ab4f8dd292d7682dd4d508d2d834b24a1811cfaccfe8f9fd20e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.7 MB (131748397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ec1500d07e746be7f4e6631e0714883d1aadffd88d60f0d280abbf1420a07aa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:45:53 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:45:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:45:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:45:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:45:56 GMT
ADD file:8c2fc380378944326d602742fde0e30458cd3e82012847b0f7e09c7184bfd135 in / 
# Wed, 28 Jun 2023 08:45:57 GMT
CMD ["/bin/bash"]
# Wed, 05 Jul 2023 01:06:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 05 Jul 2023 01:06:57 GMT
ENV GOSU_VERSION=1.14
# Wed, 05 Jul 2023 01:06:57 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 05 Jul 2023 01:07:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 05 Jul 2023 01:07:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 05 Jul 2023 01:07:36 GMT
ENV LANG=C.UTF-8
# Wed, 05 Jul 2023 01:08:51 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.0.2 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Wed, 05 Jul 2023 01:08:52 GMT
ARG MARIADB_VERSION=1:11.0.2+maria~ubu2204
# Wed, 05 Jul 2023 01:08:54 GMT
ENV MARIADB_VERSION=1:11.0.2+maria~ubu2204
# Wed, 05 Jul 2023 01:08:56 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
# Wed, 05 Jul 2023 01:09:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 05 Jul 2023 01:09:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Wed, 05 Jul 2023 01:10:00 GMT
VOLUME [/var/lib/mysql]
# Wed, 05 Jul 2023 01:10:00 GMT
COPY file:1980cab2a8b7fba7431710370aad263c40d659a4885e66510adf2002b57ddf4c in /usr/local/bin/healthcheck.sh 
# Wed, 05 Jul 2023 01:10:00 GMT
COPY file:41cd6c305128c82d238b47cc775ecf2262c7b95806428fa87026c43a3d858b56 in /usr/local/bin/ 
# Wed, 05 Jul 2023 01:10:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Jul 2023 01:10:02 GMT
EXPOSE 3306
# Wed, 05 Jul 2023 01:10:03 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:7faa46ce6b6f5c34485980029504c3995e38149d0bca67d8b976c5dbb3673644`  
		Last Modified: Tue, 04 Jul 2023 04:42:31 GMT  
		Size: 35.7 MB (35711469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af03c7013049bbb43a9d70711423a0aa0933ad63d557a33679e987f9f4552c2`  
		Last Modified: Wed, 05 Jul 2023 01:19:30 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fae131e82b0a7c398eb2a917463894a99192198e537fa4a742953dfdec5d9a5`  
		Last Modified: Wed, 05 Jul 2023 01:19:32 GMT  
		Size: 6.0 MB (6017861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c002ce052617f5efe1f7afc4ec819f1f45b350c5956b79ee09c9bd522fe18736`  
		Last Modified: Wed, 05 Jul 2023 01:19:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8036bf31dcde2e2ac8325b42c737558cf33a8cb4d01e5cedda956b06b87e05b1`  
		Last Modified: Wed, 05 Jul 2023 01:20:09 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d3a3242885374320250cbe4559b4118f1a835c6434f7905bb2ecf1f0135e49`  
		Last Modified: Wed, 05 Jul 2023 01:20:34 GMT  
		Size: 90.0 MB (90005706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb4f4475038f4dcfbb395f132f635565400316ed33037211135421a08449cb55`  
		Last Modified: Wed, 05 Jul 2023 01:20:09 GMT  
		Size: 3.6 KB (3564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3156cef64baa3f1944fde330137217b9cab7a8724be1ce677aed5b374711228`  
		Last Modified: Wed, 05 Jul 2023 01:20:09 GMT  
		Size: 7.6 KB (7567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; s390x

```console
$ docker pull mariadb@sha256:fec237d61ee4f020ee1942a5ce7ba77851271df7760c330791d49d21e38fd76d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.6 MB (121591761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd61cf2f3f72cf840df9a6079260a2004a1aaedaef78506d8c73ba968e19edfe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:53:20 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:53:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:53:22 GMT
ADD file:fa0aef35be7808c8fd6751a52bdec4dd81057e2fcaa075c547a1db53640dae9a in / 
# Wed, 28 Jun 2023 08:53:22 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 16:55:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 16:55:27 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 16:55:27 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 16:55:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 16:55:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 16:55:44 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 16:56:25 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.0.2 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 16:56:25 GMT
ARG MARIADB_VERSION=1:11.0.2+maria~ubu2204
# Tue, 04 Jul 2023 16:56:25 GMT
ENV MARIADB_VERSION=1:11.0.2+maria~ubu2204
# Tue, 04 Jul 2023 16:56:25 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 16:56:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 16:56:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 16:56:47 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 16:56:47 GMT
COPY file:1980cab2a8b7fba7431710370aad263c40d659a4885e66510adf2002b57ddf4c in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 16:56:47 GMT
COPY file:41cd6c305128c82d238b47cc775ecf2262c7b95806428fa87026c43a3d858b56 in /usr/local/bin/ 
# Tue, 04 Jul 2023 16:56:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 16:56:48 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 16:56:48 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:ce02ee0330980398d6a84a50abfa1a8c4d1cba27cbd7442b79f4aa1b1a14020d`  
		Last Modified: Tue, 04 Jul 2023 13:08:30 GMT  
		Size: 28.6 MB (28645696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16fb1ab422c0ae864df4333ba064fd3a16ef9b10862dca7b3320a9fb32c7e0bd`  
		Last Modified: Tue, 04 Jul 2023 17:00:17 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be60fdd8cf07af19113cd853d2f0ebedd02fc5cb31582325b43c0d50a323535`  
		Last Modified: Tue, 04 Jul 2023 17:00:18 GMT  
		Size: 5.5 MB (5470782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1374c790d73360e41f53f0d1a2d9cbaef5dd6c371a1ab7c58c7e20e71945704`  
		Last Modified: Tue, 04 Jul 2023 17:00:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dab15d1c6f25f9d41f7cca3c3dbef72f78adfd2c93e1b5118c2540ab35c9ff5`  
		Last Modified: Tue, 04 Jul 2023 17:00:39 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45f1884ccf2c53f7935d0379452a5e07b67da5146f499569abca9707a426a333`  
		Last Modified: Tue, 04 Jul 2023 17:00:52 GMT  
		Size: 87.5 MB (87461916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895d0bb1d3eef4bc781bd9a29370b15b508f63542867d4e350ba9d0414e35543`  
		Last Modified: Tue, 04 Jul 2023 17:00:39 GMT  
		Size: 3.6 KB (3567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:450856d007683a11eed69967457b4ed8325a4811cae92db3e313920af6019084`  
		Last Modified: Tue, 04 Jul 2023 17:00:39 GMT  
		Size: 7.6 KB (7570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:lts`

```console
$ docker pull mariadb@sha256:385c0ba6270307511a511ad915350736602c33fafb3f63f663c853920424c365
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:lts` - linux; amd64

```console
$ docker pull mariadb@sha256:4b6b625ae683588d99507ac01b042863d4311b6e15f81d653be6892762637375
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123105947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8b77d250201f61f86a2a98c7e07d5bd77f96b4a345f40f8ce53593c2ffca84d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 18:27:16 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 18:27:16 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 18:27:16 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 18:27:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 18:27:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 18:27:39 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 18:28:38 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 18:28:38 GMT
ARG MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Tue, 04 Jul 2023 18:28:38 GMT
ENV MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Tue, 04 Jul 2023 18:28:38 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 18:28:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 18:28:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 18:28:57 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 18:28:57 GMT
COPY file:60282e2c078282f09827dfb0926d431a7ad71f6de3495a21fc8a846430fc5fc9 in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 18:28:57 GMT
COPY file:704c6685e9d99f08306a2726e0468f5a764a4040cc2eb6138c1be72ac2529bbc in /usr/local/bin/ 
# Tue, 04 Jul 2023 18:28:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 18:28:57 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 18:28:58 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:718e898a86ffe915c46f60c599bc87928aa5e7e3a9434cbf52066b49651d3a1f`  
		Last Modified: Tue, 04 Jul 2023 18:32:00 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bd7a143a6c5d92cccbae0a38df554277f44cb4dbfcb668436dc5ed3398144a`  
		Last Modified: Tue, 04 Jul 2023 18:32:01 GMT  
		Size: 5.6 MB (5592713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80cdf483b70a4a08d0db0ff26cb8dbdc933588954a3bf91fce2f2544b7be37b8`  
		Last Modified: Tue, 04 Jul 2023 18:31:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9531173fe68dc54682bc25ac9b4c270ed5772c4ba6b47daef52a3d4e70af77`  
		Last Modified: Tue, 04 Jul 2023 18:32:56 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7375440478980efc7a168e77a3f085cd056c5f722e11d17a5ef922de66c95f45`  
		Last Modified: Tue, 04 Jul 2023 18:33:09 GMT  
		Size: 87.1 MB (87068650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8be80cd3b8009d3f30675bf4b5402c953d8dfaae942c2fb610a1fab9f826c3`  
		Last Modified: Tue, 04 Jul 2023 18:32:56 GMT  
		Size: 3.6 KB (3565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2384dd133a6708cc48561cd0773fb9abe3b23eae32323d644c2b8c57c8148f3`  
		Last Modified: Tue, 04 Jul 2023 18:32:56 GMT  
		Size: 7.6 KB (7566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:lts` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:33e8f9991a22fd6678ef20bf31b2bcecc6fc7c7bea5c62b0144ba4df243ff107
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117618140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fc7fccd2af985a12c6a6c0d2decd2a77618a858164ee12eb905621a5e02e6dc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 15:48:55 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 15:48:55 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 15:48:56 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 15:49:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 15:49:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 15:49:12 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 15:50:06 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 15:50:07 GMT
ARG MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Tue, 04 Jul 2023 15:50:07 GMT
ENV MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Tue, 04 Jul 2023 15:50:07 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 15:50:07 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 15:50:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 15:50:24 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 15:50:24 GMT
COPY file:60282e2c078282f09827dfb0926d431a7ad71f6de3495a21fc8a846430fc5fc9 in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 15:50:24 GMT
COPY file:704c6685e9d99f08306a2726e0468f5a764a4040cc2eb6138c1be72ac2529bbc in /usr/local/bin/ 
# Tue, 04 Jul 2023 15:50:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 15:50:24 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 15:50:24 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f226d4d968a5322b60d61898c78418afeeb62f9a8613d9939d2546229a59ed0`  
		Last Modified: Tue, 04 Jul 2023 15:53:12 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a718d9544847f819e9859244c57b1093e55eb4bbd1d50066804d9ddd24d9c2c`  
		Last Modified: Tue, 04 Jul 2023 15:53:12 GMT  
		Size: 5.4 MB (5406735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad17cece0015293005bd369ad4550b0faa2ef78f55de897f35a48e5b101b83c8`  
		Last Modified: Tue, 04 Jul 2023 15:53:10 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8210aced70ef3e24a46799929c24c1213867224b74ac675905ac218d01442f43`  
		Last Modified: Tue, 04 Jul 2023 15:54:02 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56cb7b8053f2d91dc92f88f643e2865478be6d9ff1a66c023d0c46ac4354ee4b`  
		Last Modified: Tue, 04 Jul 2023 15:54:11 GMT  
		Size: 83.8 MB (83807029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449424199d1167824fde06f204297c2ba55b2095c8bfd15d6a77aa93b09c7e4b`  
		Last Modified: Tue, 04 Jul 2023 15:54:01 GMT  
		Size: 3.6 KB (3565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3ad0253591ba73c469a1fb8a855ae6c9f69b8c1c7c16163e792da830111d9f`  
		Last Modified: Tue, 04 Jul 2023 15:54:02 GMT  
		Size: 7.6 KB (7568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:lts` - linux; ppc64le

```console
$ docker pull mariadb@sha256:0f837e667037e0f69042accade3ac2b389154167bcff6ea9e8639eb6fe9f0460
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131775039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8822e9bd24ab2483e7f0ae20339330fcf3c800c3fb250d7115a2b071dddd4ec1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:45:53 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:45:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:45:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:45:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:45:56 GMT
ADD file:8c2fc380378944326d602742fde0e30458cd3e82012847b0f7e09c7184bfd135 in / 
# Wed, 28 Jun 2023 08:45:57 GMT
CMD ["/bin/bash"]
# Wed, 05 Jul 2023 01:06:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 05 Jul 2023 01:06:57 GMT
ENV GOSU_VERSION=1.14
# Wed, 05 Jul 2023 01:06:57 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 05 Jul 2023 01:07:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 05 Jul 2023 01:07:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 05 Jul 2023 01:07:36 GMT
ENV LANG=C.UTF-8
# Wed, 05 Jul 2023 01:10:14 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Wed, 05 Jul 2023 01:10:15 GMT
ARG MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Wed, 05 Jul 2023 01:10:15 GMT
ENV MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Wed, 05 Jul 2023 01:10:16 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
# Wed, 05 Jul 2023 01:10:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 05 Jul 2023 01:11:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Wed, 05 Jul 2023 01:11:10 GMT
VOLUME [/var/lib/mysql]
# Wed, 05 Jul 2023 01:11:10 GMT
COPY file:60282e2c078282f09827dfb0926d431a7ad71f6de3495a21fc8a846430fc5fc9 in /usr/local/bin/healthcheck.sh 
# Wed, 05 Jul 2023 01:11:10 GMT
COPY file:704c6685e9d99f08306a2726e0468f5a764a4040cc2eb6138c1be72ac2529bbc in /usr/local/bin/ 
# Wed, 05 Jul 2023 01:11:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Jul 2023 01:11:11 GMT
EXPOSE 3306
# Wed, 05 Jul 2023 01:11:11 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:7faa46ce6b6f5c34485980029504c3995e38149d0bca67d8b976c5dbb3673644`  
		Last Modified: Tue, 04 Jul 2023 04:42:31 GMT  
		Size: 35.7 MB (35711469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af03c7013049bbb43a9d70711423a0aa0933ad63d557a33679e987f9f4552c2`  
		Last Modified: Wed, 05 Jul 2023 01:19:30 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fae131e82b0a7c398eb2a917463894a99192198e537fa4a742953dfdec5d9a5`  
		Last Modified: Wed, 05 Jul 2023 01:19:32 GMT  
		Size: 6.0 MB (6017861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c002ce052617f5efe1f7afc4ec819f1f45b350c5956b79ee09c9bd522fe18736`  
		Last Modified: Wed, 05 Jul 2023 01:19:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:942ea7aeb70e16124a1ff199ecf228e3ab0281f20f179766b0885587643a240d`  
		Last Modified: Wed, 05 Jul 2023 01:21:05 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:115967ee1bae2b450657e120cfba1533a2768c69fe87802e5a90590ba251d1af`  
		Last Modified: Wed, 05 Jul 2023 01:21:29 GMT  
		Size: 90.0 MB (90032344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981e89a22f465c5f29cd8017aceb5dc84553018d607d0a09802db952f21422e6`  
		Last Modified: Wed, 05 Jul 2023 01:21:05 GMT  
		Size: 3.6 KB (3566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e31cc00f3e6a6786d22d5cc34292a0d4e5b50f8ba265c13862ec1ab1e8ddc49`  
		Last Modified: Wed, 05 Jul 2023 01:21:05 GMT  
		Size: 7.6 KB (7568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:lts` - linux; s390x

```console
$ docker pull mariadb@sha256:2b727f34069c4b59da2e9dae7fa9f907e91d2bce79801c4bdc33012d4cbe038f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.6 MB (121580518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:378fece5fccb2954bad0c49ec6a7ed1c913335d61542c2a7db9cddf4df77e3d5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:53:20 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:53:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:53:22 GMT
ADD file:fa0aef35be7808c8fd6751a52bdec4dd81057e2fcaa075c547a1db53640dae9a in / 
# Wed, 28 Jun 2023 08:53:22 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 16:55:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 16:55:27 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 16:55:27 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 16:55:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 16:55:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 16:55:44 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 16:56:57 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 16:56:57 GMT
ARG MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Tue, 04 Jul 2023 16:56:57 GMT
ENV MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Tue, 04 Jul 2023 16:56:57 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 16:56:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 16:57:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 16:57:18 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 16:57:18 GMT
COPY file:60282e2c078282f09827dfb0926d431a7ad71f6de3495a21fc8a846430fc5fc9 in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 16:57:18 GMT
COPY file:704c6685e9d99f08306a2726e0468f5a764a4040cc2eb6138c1be72ac2529bbc in /usr/local/bin/ 
# Tue, 04 Jul 2023 16:57:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 16:57:18 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 16:57:18 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:ce02ee0330980398d6a84a50abfa1a8c4d1cba27cbd7442b79f4aa1b1a14020d`  
		Last Modified: Tue, 04 Jul 2023 13:08:30 GMT  
		Size: 28.6 MB (28645696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16fb1ab422c0ae864df4333ba064fd3a16ef9b10862dca7b3320a9fb32c7e0bd`  
		Last Modified: Tue, 04 Jul 2023 17:00:17 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be60fdd8cf07af19113cd853d2f0ebedd02fc5cb31582325b43c0d50a323535`  
		Last Modified: Tue, 04 Jul 2023 17:00:18 GMT  
		Size: 5.5 MB (5470782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1374c790d73360e41f53f0d1a2d9cbaef5dd6c371a1ab7c58c7e20e71945704`  
		Last Modified: Tue, 04 Jul 2023 17:00:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27e7e4b86fecdc32e5bd05e78321e6746840e6a0544d4bedbbdf1c2754a5d72`  
		Last Modified: Tue, 04 Jul 2023 17:01:05 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0090bfea6877acf7ee51c046ee6600b616e08ac7ee48d3fdc628a0167e130e3`  
		Last Modified: Tue, 04 Jul 2023 17:01:18 GMT  
		Size: 87.5 MB (87450671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:093cd65cb7e5e05be6911f64a423e13b6109f3d369f8ac17e7e2584cbe74d8a5`  
		Last Modified: Tue, 04 Jul 2023 17:01:05 GMT  
		Size: 3.6 KB (3568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3082833c7ebee98976c11b8826ef88fa09fa5b139d6b6830488e0ed2a7144e3`  
		Last Modified: Tue, 04 Jul 2023 17:01:05 GMT  
		Size: 7.6 KB (7570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:lts-jammy`

```console
$ docker pull mariadb@sha256:385c0ba6270307511a511ad915350736602c33fafb3f63f663c853920424c365
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:lts-jammy` - linux; amd64

```console
$ docker pull mariadb@sha256:4b6b625ae683588d99507ac01b042863d4311b6e15f81d653be6892762637375
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123105947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8b77d250201f61f86a2a98c7e07d5bd77f96b4a345f40f8ce53593c2ffca84d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 18:27:16 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 18:27:16 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 18:27:16 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 18:27:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 18:27:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 18:27:39 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 18:28:38 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 18:28:38 GMT
ARG MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Tue, 04 Jul 2023 18:28:38 GMT
ENV MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Tue, 04 Jul 2023 18:28:38 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 18:28:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 18:28:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 18:28:57 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 18:28:57 GMT
COPY file:60282e2c078282f09827dfb0926d431a7ad71f6de3495a21fc8a846430fc5fc9 in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 18:28:57 GMT
COPY file:704c6685e9d99f08306a2726e0468f5a764a4040cc2eb6138c1be72ac2529bbc in /usr/local/bin/ 
# Tue, 04 Jul 2023 18:28:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 18:28:57 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 18:28:58 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:718e898a86ffe915c46f60c599bc87928aa5e7e3a9434cbf52066b49651d3a1f`  
		Last Modified: Tue, 04 Jul 2023 18:32:00 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bd7a143a6c5d92cccbae0a38df554277f44cb4dbfcb668436dc5ed3398144a`  
		Last Modified: Tue, 04 Jul 2023 18:32:01 GMT  
		Size: 5.6 MB (5592713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80cdf483b70a4a08d0db0ff26cb8dbdc933588954a3bf91fce2f2544b7be37b8`  
		Last Modified: Tue, 04 Jul 2023 18:31:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9531173fe68dc54682bc25ac9b4c270ed5772c4ba6b47daef52a3d4e70af77`  
		Last Modified: Tue, 04 Jul 2023 18:32:56 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7375440478980efc7a168e77a3f085cd056c5f722e11d17a5ef922de66c95f45`  
		Last Modified: Tue, 04 Jul 2023 18:33:09 GMT  
		Size: 87.1 MB (87068650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8be80cd3b8009d3f30675bf4b5402c953d8dfaae942c2fb610a1fab9f826c3`  
		Last Modified: Tue, 04 Jul 2023 18:32:56 GMT  
		Size: 3.6 KB (3565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2384dd133a6708cc48561cd0773fb9abe3b23eae32323d644c2b8c57c8148f3`  
		Last Modified: Tue, 04 Jul 2023 18:32:56 GMT  
		Size: 7.6 KB (7566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:lts-jammy` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:33e8f9991a22fd6678ef20bf31b2bcecc6fc7c7bea5c62b0144ba4df243ff107
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117618140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fc7fccd2af985a12c6a6c0d2decd2a77618a858164ee12eb905621a5e02e6dc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 15:48:55 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 15:48:55 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 15:48:56 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 15:49:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 15:49:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 15:49:12 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 15:50:06 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 15:50:07 GMT
ARG MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Tue, 04 Jul 2023 15:50:07 GMT
ENV MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Tue, 04 Jul 2023 15:50:07 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 15:50:07 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 15:50:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 15:50:24 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 15:50:24 GMT
COPY file:60282e2c078282f09827dfb0926d431a7ad71f6de3495a21fc8a846430fc5fc9 in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 15:50:24 GMT
COPY file:704c6685e9d99f08306a2726e0468f5a764a4040cc2eb6138c1be72ac2529bbc in /usr/local/bin/ 
# Tue, 04 Jul 2023 15:50:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 15:50:24 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 15:50:24 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f226d4d968a5322b60d61898c78418afeeb62f9a8613d9939d2546229a59ed0`  
		Last Modified: Tue, 04 Jul 2023 15:53:12 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a718d9544847f819e9859244c57b1093e55eb4bbd1d50066804d9ddd24d9c2c`  
		Last Modified: Tue, 04 Jul 2023 15:53:12 GMT  
		Size: 5.4 MB (5406735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad17cece0015293005bd369ad4550b0faa2ef78f55de897f35a48e5b101b83c8`  
		Last Modified: Tue, 04 Jul 2023 15:53:10 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8210aced70ef3e24a46799929c24c1213867224b74ac675905ac218d01442f43`  
		Last Modified: Tue, 04 Jul 2023 15:54:02 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56cb7b8053f2d91dc92f88f643e2865478be6d9ff1a66c023d0c46ac4354ee4b`  
		Last Modified: Tue, 04 Jul 2023 15:54:11 GMT  
		Size: 83.8 MB (83807029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449424199d1167824fde06f204297c2ba55b2095c8bfd15d6a77aa93b09c7e4b`  
		Last Modified: Tue, 04 Jul 2023 15:54:01 GMT  
		Size: 3.6 KB (3565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3ad0253591ba73c469a1fb8a855ae6c9f69b8c1c7c16163e792da830111d9f`  
		Last Modified: Tue, 04 Jul 2023 15:54:02 GMT  
		Size: 7.6 KB (7568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:lts-jammy` - linux; ppc64le

```console
$ docker pull mariadb@sha256:0f837e667037e0f69042accade3ac2b389154167bcff6ea9e8639eb6fe9f0460
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131775039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8822e9bd24ab2483e7f0ae20339330fcf3c800c3fb250d7115a2b071dddd4ec1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:45:53 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:45:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:45:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:45:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:45:56 GMT
ADD file:8c2fc380378944326d602742fde0e30458cd3e82012847b0f7e09c7184bfd135 in / 
# Wed, 28 Jun 2023 08:45:57 GMT
CMD ["/bin/bash"]
# Wed, 05 Jul 2023 01:06:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 05 Jul 2023 01:06:57 GMT
ENV GOSU_VERSION=1.14
# Wed, 05 Jul 2023 01:06:57 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 05 Jul 2023 01:07:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 05 Jul 2023 01:07:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 05 Jul 2023 01:07:36 GMT
ENV LANG=C.UTF-8
# Wed, 05 Jul 2023 01:10:14 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Wed, 05 Jul 2023 01:10:15 GMT
ARG MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Wed, 05 Jul 2023 01:10:15 GMT
ENV MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Wed, 05 Jul 2023 01:10:16 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
# Wed, 05 Jul 2023 01:10:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 05 Jul 2023 01:11:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Wed, 05 Jul 2023 01:11:10 GMT
VOLUME [/var/lib/mysql]
# Wed, 05 Jul 2023 01:11:10 GMT
COPY file:60282e2c078282f09827dfb0926d431a7ad71f6de3495a21fc8a846430fc5fc9 in /usr/local/bin/healthcheck.sh 
# Wed, 05 Jul 2023 01:11:10 GMT
COPY file:704c6685e9d99f08306a2726e0468f5a764a4040cc2eb6138c1be72ac2529bbc in /usr/local/bin/ 
# Wed, 05 Jul 2023 01:11:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Jul 2023 01:11:11 GMT
EXPOSE 3306
# Wed, 05 Jul 2023 01:11:11 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:7faa46ce6b6f5c34485980029504c3995e38149d0bca67d8b976c5dbb3673644`  
		Last Modified: Tue, 04 Jul 2023 04:42:31 GMT  
		Size: 35.7 MB (35711469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af03c7013049bbb43a9d70711423a0aa0933ad63d557a33679e987f9f4552c2`  
		Last Modified: Wed, 05 Jul 2023 01:19:30 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fae131e82b0a7c398eb2a917463894a99192198e537fa4a742953dfdec5d9a5`  
		Last Modified: Wed, 05 Jul 2023 01:19:32 GMT  
		Size: 6.0 MB (6017861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c002ce052617f5efe1f7afc4ec819f1f45b350c5956b79ee09c9bd522fe18736`  
		Last Modified: Wed, 05 Jul 2023 01:19:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:942ea7aeb70e16124a1ff199ecf228e3ab0281f20f179766b0885587643a240d`  
		Last Modified: Wed, 05 Jul 2023 01:21:05 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:115967ee1bae2b450657e120cfba1533a2768c69fe87802e5a90590ba251d1af`  
		Last Modified: Wed, 05 Jul 2023 01:21:29 GMT  
		Size: 90.0 MB (90032344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981e89a22f465c5f29cd8017aceb5dc84553018d607d0a09802db952f21422e6`  
		Last Modified: Wed, 05 Jul 2023 01:21:05 GMT  
		Size: 3.6 KB (3566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e31cc00f3e6a6786d22d5cc34292a0d4e5b50f8ba265c13862ec1ab1e8ddc49`  
		Last Modified: Wed, 05 Jul 2023 01:21:05 GMT  
		Size: 7.6 KB (7568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:lts-jammy` - linux; s390x

```console
$ docker pull mariadb@sha256:2b727f34069c4b59da2e9dae7fa9f907e91d2bce79801c4bdc33012d4cbe038f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.6 MB (121580518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:378fece5fccb2954bad0c49ec6a7ed1c913335d61542c2a7db9cddf4df77e3d5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 28 Jun 2023 08:53:20 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:53:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:53:22 GMT
ADD file:fa0aef35be7808c8fd6751a52bdec4dd81057e2fcaa075c547a1db53640dae9a in / 
# Wed, 28 Jun 2023 08:53:22 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 16:55:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 16:55:27 GMT
ENV GOSU_VERSION=1.14
# Tue, 04 Jul 2023 16:55:27 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 04 Jul 2023 16:55:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 16:55:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 16:55:44 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 16:56:57 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 04 Jul 2023 16:56:57 GMT
ARG MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Tue, 04 Jul 2023 16:56:57 GMT
ENV MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Tue, 04 Jul 2023 16:56:57 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
# Tue, 04 Jul 2023 16:56:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 04 Jul 2023 16:57:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 04 Jul 2023 16:57:18 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 16:57:18 GMT
COPY file:60282e2c078282f09827dfb0926d431a7ad71f6de3495a21fc8a846430fc5fc9 in /usr/local/bin/healthcheck.sh 
# Tue, 04 Jul 2023 16:57:18 GMT
COPY file:704c6685e9d99f08306a2726e0468f5a764a4040cc2eb6138c1be72ac2529bbc in /usr/local/bin/ 
# Tue, 04 Jul 2023 16:57:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 16:57:18 GMT
EXPOSE 3306
# Tue, 04 Jul 2023 16:57:18 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:ce02ee0330980398d6a84a50abfa1a8c4d1cba27cbd7442b79f4aa1b1a14020d`  
		Last Modified: Tue, 04 Jul 2023 13:08:30 GMT  
		Size: 28.6 MB (28645696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16fb1ab422c0ae864df4333ba064fd3a16ef9b10862dca7b3320a9fb32c7e0bd`  
		Last Modified: Tue, 04 Jul 2023 17:00:17 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be60fdd8cf07af19113cd853d2f0ebedd02fc5cb31582325b43c0d50a323535`  
		Last Modified: Tue, 04 Jul 2023 17:00:18 GMT  
		Size: 5.5 MB (5470782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1374c790d73360e41f53f0d1a2d9cbaef5dd6c371a1ab7c58c7e20e71945704`  
		Last Modified: Tue, 04 Jul 2023 17:00:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27e7e4b86fecdc32e5bd05e78321e6746840e6a0544d4bedbbdf1c2754a5d72`  
		Last Modified: Tue, 04 Jul 2023 17:01:05 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0090bfea6877acf7ee51c046ee6600b616e08ac7ee48d3fdc628a0167e130e3`  
		Last Modified: Tue, 04 Jul 2023 17:01:18 GMT  
		Size: 87.5 MB (87450671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:093cd65cb7e5e05be6911f64a423e13b6109f3d369f8ac17e7e2584cbe74d8a5`  
		Last Modified: Tue, 04 Jul 2023 17:01:05 GMT  
		Size: 3.6 KB (3568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3082833c7ebee98976c11b8826ef88fa09fa5b139d6b6830488e0ed2a7144e3`  
		Last Modified: Tue, 04 Jul 2023 17:01:05 GMT  
		Size: 7.6 KB (7570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
