<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mariadb`

-	[`mariadb:10`](#mariadb10)
-	[`mariadb:10-jammy`](#mariadb10-jammy)
-	[`mariadb:10.10`](#mariadb1010)
-	[`mariadb:10.10-jammy`](#mariadb1010-jammy)
-	[`mariadb:10.10.4`](#mariadb10104)
-	[`mariadb:10.10.4-jammy`](#mariadb10104-jammy)
-	[`mariadb:10.11`](#mariadb1011)
-	[`mariadb:10.11-jammy`](#mariadb1011-jammy)
-	[`mariadb:10.11.3`](#mariadb10113)
-	[`mariadb:10.11.3-jammy`](#mariadb10113-jammy)
-	[`mariadb:10.3`](#mariadb103)
-	[`mariadb:10.3-focal`](#mariadb103-focal)
-	[`mariadb:10.3.39`](#mariadb10339)
-	[`mariadb:10.3.39-focal`](#mariadb10339-focal)
-	[`mariadb:10.4`](#mariadb104)
-	[`mariadb:10.4-focal`](#mariadb104-focal)
-	[`mariadb:10.4.29`](#mariadb10429)
-	[`mariadb:10.4.29-focal`](#mariadb10429-focal)
-	[`mariadb:10.5`](#mariadb105)
-	[`mariadb:10.5-focal`](#mariadb105-focal)
-	[`mariadb:10.5.20`](#mariadb10520)
-	[`mariadb:10.5.20-focal`](#mariadb10520-focal)
-	[`mariadb:10.6`](#mariadb106)
-	[`mariadb:10.6-focal`](#mariadb106-focal)
-	[`mariadb:10.6.13`](#mariadb10613)
-	[`mariadb:10.6.13-focal`](#mariadb10613-focal)
-	[`mariadb:10.8`](#mariadb108)
-	[`mariadb:10.8-jammy`](#mariadb108-jammy)
-	[`mariadb:10.8.8`](#mariadb1088)
-	[`mariadb:10.8.8-jammy`](#mariadb1088-jammy)
-	[`mariadb:10.9`](#mariadb109)
-	[`mariadb:10.9-jammy`](#mariadb109-jammy)
-	[`mariadb:10.9.6`](#mariadb1096)
-	[`mariadb:10.9.6-jammy`](#mariadb1096-jammy)
-	[`mariadb:11.0-rc`](#mariadb110-rc)
-	[`mariadb:11.0-rc-jammy`](#mariadb110-rc-jammy)
-	[`mariadb:11.0.1-rc`](#mariadb1101-rc)
-	[`mariadb:11.0.1-rc-jammy`](#mariadb1101-rc-jammy)
-	[`mariadb:jammy`](#mariadbjammy)
-	[`mariadb:latest`](#mariadblatest)
-	[`mariadb:lts`](#mariadblts)
-	[`mariadb:lts-jammy`](#mariadblts-jammy)

## `mariadb:10`

```console
$ docker pull mariadb@sha256:5701c619e8f355f7d4d601f0007f1138f35d02882e206106e5d4a747a6805ed8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10` - linux; amd64

```console
$ docker pull mariadb@sha256:f77c69a548d1a948f59d6b5eacf25903410cc156f84f33102cc4c662435dea72
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123112287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4af0c16be4b1af0799fd6f831b4fe63eab4ebe5e47d45bedac69b31d23c298e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 07:52:03 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 07:52:03 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 07:52:03 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 07:52:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 07:52:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 07:52:19 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:53:38 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.3 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:53:39 GMT
ARG MARIADB_VERSION=1:10.11.3+maria~ubu2204
# Thu, 11 May 2023 22:53:39 GMT
ENV MARIADB_VERSION=1:10.11.3+maria~ubu2204
# Thu, 11 May 2023 22:53:39 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
# Thu, 11 May 2023 22:53:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:54:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:54:06 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:54:06 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:54:06 GMT
COPY file:94a071210c811522ac7cb9cd9b6d33b1df5eb056971fbdeefa8e9bc2e8a2d629 in /usr/local/bin/ 
# Thu, 11 May 2023 22:54:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:54:06 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:54:07 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:1bc677758ad7fa4503417ae5be18809c5a8679b5b36fcd1464d5a8e41cb13305`  
		Last Modified: Tue, 25 Apr 2023 22:54:44 GMT  
		Size: 30.4 MB (30430220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196e1740aea41b9915498de02cc132de54583dad1a212d06c9f6eb4690e1e0cb`  
		Last Modified: Thu, 04 May 2023 07:54:52 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4df0997938e5fd755403145484e1253115d3739285c704f562cf3bd6d89ec8`  
		Last Modified: Thu, 04 May 2023 07:54:53 GMT  
		Size: 5.6 MB (5595975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa4e41848249471f699386db900347fa61b39622dfba140344d9c51b264e7db`  
		Last Modified: Thu, 04 May 2023 07:54:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a134c78ed13cbf2e6ac7f37c3ef851e65671664763a229e5460065d76e2ed7fa`  
		Last Modified: Thu, 11 May 2023 22:57:57 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7cd475067d8253d1d2cd28269770d3abf6eb40757983f4c92ae62f7a89b5535`  
		Last Modified: Thu, 11 May 2023 22:58:09 GMT  
		Size: 87.1 MB (87072824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348ae7ff2d74996bdc3e5da86e199b871eac8e2f86e7e15f7d03cbccc7231fa5`  
		Last Modified: Thu, 11 May 2023 22:57:57 GMT  
		Size: 3.5 KB (3528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e83ab58cb77ae0bded1f1bbd34ccc3c633547646227392d393af71e8b24a893`  
		Last Modified: Thu, 11 May 2023 22:57:57 GMT  
		Size: 7.5 KB (7516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:b180bb51094778a95fb835b429cfc2583d0f4e8e666cab652c221f3f03b6708b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117608447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ba3efd0815f87edbc030f0f8d50f783c1c9aa0c47ffec82ab94c6bad5822d7d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 03:46:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 03:46:08 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 03:46:08 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 03:46:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 03:46:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 03:46:28 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:37:14 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.3 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:37:14 GMT
ARG MARIADB_VERSION=1:10.11.3+maria~ubu2204
# Thu, 11 May 2023 22:37:14 GMT
ENV MARIADB_VERSION=1:10.11.3+maria~ubu2204
# Thu, 11 May 2023 22:37:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
# Thu, 11 May 2023 22:37:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:37:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:37:46 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:37:46 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:37:46 GMT
COPY file:94a071210c811522ac7cb9cd9b6d33b1df5eb056971fbdeefa8e9bc2e8a2d629 in /usr/local/bin/ 
# Thu, 11 May 2023 22:37:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:37:46 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:37:46 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:f3f60f415e9a03eed88bd5dd5268c841cde08dacf16911a3ef1e4e0fcdd76568`  
		Last Modified: Wed, 26 Apr 2023 02:08:37 GMT  
		Size: 28.4 MB (28389440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bfb87016de46ece16208cd39b5fa89740b8e8db147c2da2f6483551b3e8d521`  
		Last Modified: Thu, 04 May 2023 03:49:02 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8bd3f48f8f1fc94a1a143132ba91e005df50ee4327d0e209553cc89145a91f`  
		Last Modified: Thu, 04 May 2023 03:49:03 GMT  
		Size: 5.4 MB (5409831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ebb0502bf43d03d32f27b6cfa9ea349e89bccb62bd1ef3cf96a9a769e6c1fa`  
		Last Modified: Thu, 04 May 2023 03:49:00 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c39b9daac872cd7020c71e2bcfb8c097a1ea4c92c6e75f0fa1c5457a9793fabd`  
		Last Modified: Thu, 11 May 2023 22:41:30 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d0e97236e823170f83bde496cd664d5a354bdc0e3812e70d9e9dc434a067506`  
		Last Modified: Thu, 11 May 2023 22:41:40 GMT  
		Size: 83.8 MB (83795910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b5a4e92f3071fd8c0fcaba769b1d01c887847907025859069a695bebdfd2ca`  
		Last Modified: Thu, 11 May 2023 22:41:30 GMT  
		Size: 3.5 KB (3527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e100a9688501846d85a74ce52c2427d070849317340c48bdb06946ff8f89178`  
		Last Modified: Thu, 11 May 2023 22:41:30 GMT  
		Size: 7.5 KB (7515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10` - linux; ppc64le

```console
$ docker pull mariadb@sha256:4d240e05dd2101a66ba61dd58ddc69e210df50aeefa05a74cbf242c6662dd584
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.9 MB (131883188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f8168152d1fd9b321f68df36d3f926ad414075ce59cb8a0b139cc40dc3a652c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:17 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:18 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:21 GMT
ADD file:e75f08a67f0576b5441bb2fe454cad4b5b31a9d4efea23be791af62e1e0c712f in / 
# Tue, 25 Apr 2023 17:30:21 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 14:29:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 14:29:33 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 14:29:33 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 14:30:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 14:30:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 14:30:21 GMT
ENV LANG=C.UTF-8
# Thu, 04 May 2023 14:31:55 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.2 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 04 May 2023 14:31:55 GMT
ARG MARIADB_VERSION=1:10.11.2+maria~ubu2204
# Thu, 04 May 2023 14:31:56 GMT
ENV MARIADB_VERSION=1:10.11.2+maria~ubu2204
# Thu, 04 May 2023 14:31:56 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.2/repo/ubuntu/ jammy main
# Thu, 04 May 2023 14:31:58 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 04 May 2023 14:32:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 04 May 2023 14:33:04 GMT
VOLUME [/var/lib/mysql]
# Thu, 04 May 2023 14:33:05 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 04 May 2023 14:33:05 GMT
COPY file:ebdfbcbc74dda1874f1c75d86e1c32733edb402d13440b2b7140a952010bc21f in /usr/local/bin/ 
# Thu, 04 May 2023 14:33:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 May 2023 14:33:07 GMT
EXPOSE 3306
# Thu, 04 May 2023 14:33:07 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:f6a63d8cd043e76933823b18cbb7057a55bb4d66d64639c81e15a4700c101582`  
		Last Modified: Wed, 03 May 2023 17:09:07 GMT  
		Size: 35.7 MB (35712706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df46cdfc9a45a40dd254c1a0f2ccb2b0020e6852a5fb101d44d79250da5ddc69`  
		Last Modified: Thu, 04 May 2023 14:38:11 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11d1aa00f5a23d7276d6c701876911c79820fef6401156510e68eecb03012091`  
		Last Modified: Thu, 04 May 2023 14:38:12 GMT  
		Size: 6.0 MB (6021655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ec0fb2f57daffaea6b67a61d9012d55d4fcef64766481235d00d0438513793b`  
		Last Modified: Thu, 04 May 2023 14:38:08 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5222456a7c2bfe3bf5175c63ee69047694ca04828ae27b736d3e365bb098e6`  
		Last Modified: Thu, 04 May 2023 14:38:49 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c483e4bc0a4a66eedb7d32ac48ebb035053d2581b308082f7f73aae65b5695`  
		Last Modified: Thu, 04 May 2023 14:39:13 GMT  
		Size: 90.1 MB (90136103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c20716d8d6a4a6fffb6a1a4433d2c519498b3245749451035f81128a7d9d6f5a`  
		Last Modified: Thu, 04 May 2023 14:38:49 GMT  
		Size: 3.5 KB (3526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92aecaeb58f118d19cc858ade38f52e5cc3f8fbd518c7cd5d71caecd07b49db`  
		Last Modified: Thu, 04 May 2023 14:38:49 GMT  
		Size: 7.0 KB (6970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10` - linux; s390x

```console
$ docker pull mariadb@sha256:6776cef0f480be971c0746153bfc7d3c6a6ba04acb53448303d2ee7fd50b10d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121445424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5c39fb429a2411a98cc5e9ce78feeefc35cd3d0d3f948609f9d0d7162e091bf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 26 Jan 2023 05:08:35 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:08:35 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:08:36 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:08:36 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:08:37 GMT
ADD file:a9794efc1a102ab6a7160e660a63f4b267797b8b7e0b0bfd9c04ed62846cfb36 in / 
# Thu, 26 Jan 2023 05:08:38 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:42:50 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 31 Jan 2023 18:42:50 GMT
ENV GOSU_VERSION=1.14
# Tue, 31 Jan 2023 18:42:50 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 31 Jan 2023 18:43:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 31 Jan 2023 18:43:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 31 Jan 2023 18:43:06 GMT
ENV LANG=C.UTF-8
# Sat, 18 Feb 2023 00:39:43 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.2 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Sat, 18 Feb 2023 00:39:43 GMT
ARG MARIADB_VERSION=1:10.11.2+maria~ubu2204
# Sat, 18 Feb 2023 00:39:43 GMT
ENV MARIADB_VERSION=1:10.11.2+maria~ubu2204
# Sat, 18 Feb 2023 00:39:44 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.2/repo/ubuntu/ jammy main
# Sat, 18 Feb 2023 00:39:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 18 Feb 2023 00:40:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Sat, 18 Feb 2023 00:40:18 GMT
VOLUME [/var/lib/mysql]
# Sat, 25 Feb 2023 04:00:33 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Sat, 25 Feb 2023 04:00:33 GMT
COPY file:ebdfbcbc74dda1874f1c75d86e1c32733edb402d13440b2b7140a952010bc21f in /usr/local/bin/ 
# Sat, 25 Feb 2023 04:00:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 25 Feb 2023 04:00:33 GMT
EXPOSE 3306
# Sat, 25 Feb 2023 04:00:33 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:dd969ed9de43018fe5442c859bf66eabf23145b966b9338392ea707aed18b26f`  
		Last Modified: Tue, 31 Jan 2023 17:55:34 GMT  
		Size: 28.6 MB (28641926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b702438b56d7a6aaaad49e2be85e1bb2f3beb85406f6b9db1a232f798c558b3`  
		Last Modified: Tue, 31 Jan 2023 18:48:25 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60737998d0295bde808ca8856933482817ca605937f714f3cfca1ab0b4ca99ed`  
		Last Modified: Tue, 31 Jan 2023 18:48:26 GMT  
		Size: 5.4 MB (5401827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6e12a0288bb0803aeb23e581ca842e1fdf826fa28b4a730dd83585ea125ff8`  
		Last Modified: Tue, 31 Jan 2023 18:48:24 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36528da402899a29c65aec506cc3573ecd9edf046e710740371ea56b98466ce`  
		Last Modified: Sat, 18 Feb 2023 00:42:04 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c45532e045d6549e8a41f2b8cce4c9cc336de9d1dac3d929d2a7ea3fee6fcf`  
		Last Modified: Sat, 18 Feb 2023 00:42:16 GMT  
		Size: 87.4 MB (87388947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf76dfdfa839489a3b54c3eb3679f8718726a96a30cc2049089b7ac593b41ae`  
		Last Modified: Sat, 25 Feb 2023 04:02:18 GMT  
		Size: 3.5 KB (3526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f477561fbd237479df484d7fc122750ffa7b64e394c3ca9d2cc6e5072810967d`  
		Last Modified: Sat, 25 Feb 2023 04:02:18 GMT  
		Size: 7.0 KB (6971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10-jammy`

```console
$ docker pull mariadb@sha256:5701c619e8f355f7d4d601f0007f1138f35d02882e206106e5d4a747a6805ed8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10-jammy` - linux; amd64

```console
$ docker pull mariadb@sha256:f77c69a548d1a948f59d6b5eacf25903410cc156f84f33102cc4c662435dea72
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123112287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4af0c16be4b1af0799fd6f831b4fe63eab4ebe5e47d45bedac69b31d23c298e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 07:52:03 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 07:52:03 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 07:52:03 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 07:52:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 07:52:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 07:52:19 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:53:38 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.3 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:53:39 GMT
ARG MARIADB_VERSION=1:10.11.3+maria~ubu2204
# Thu, 11 May 2023 22:53:39 GMT
ENV MARIADB_VERSION=1:10.11.3+maria~ubu2204
# Thu, 11 May 2023 22:53:39 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
# Thu, 11 May 2023 22:53:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:54:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:54:06 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:54:06 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:54:06 GMT
COPY file:94a071210c811522ac7cb9cd9b6d33b1df5eb056971fbdeefa8e9bc2e8a2d629 in /usr/local/bin/ 
# Thu, 11 May 2023 22:54:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:54:06 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:54:07 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:1bc677758ad7fa4503417ae5be18809c5a8679b5b36fcd1464d5a8e41cb13305`  
		Last Modified: Tue, 25 Apr 2023 22:54:44 GMT  
		Size: 30.4 MB (30430220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196e1740aea41b9915498de02cc132de54583dad1a212d06c9f6eb4690e1e0cb`  
		Last Modified: Thu, 04 May 2023 07:54:52 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4df0997938e5fd755403145484e1253115d3739285c704f562cf3bd6d89ec8`  
		Last Modified: Thu, 04 May 2023 07:54:53 GMT  
		Size: 5.6 MB (5595975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa4e41848249471f699386db900347fa61b39622dfba140344d9c51b264e7db`  
		Last Modified: Thu, 04 May 2023 07:54:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a134c78ed13cbf2e6ac7f37c3ef851e65671664763a229e5460065d76e2ed7fa`  
		Last Modified: Thu, 11 May 2023 22:57:57 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7cd475067d8253d1d2cd28269770d3abf6eb40757983f4c92ae62f7a89b5535`  
		Last Modified: Thu, 11 May 2023 22:58:09 GMT  
		Size: 87.1 MB (87072824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348ae7ff2d74996bdc3e5da86e199b871eac8e2f86e7e15f7d03cbccc7231fa5`  
		Last Modified: Thu, 11 May 2023 22:57:57 GMT  
		Size: 3.5 KB (3528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e83ab58cb77ae0bded1f1bbd34ccc3c633547646227392d393af71e8b24a893`  
		Last Modified: Thu, 11 May 2023 22:57:57 GMT  
		Size: 7.5 KB (7516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-jammy` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:b180bb51094778a95fb835b429cfc2583d0f4e8e666cab652c221f3f03b6708b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117608447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ba3efd0815f87edbc030f0f8d50f783c1c9aa0c47ffec82ab94c6bad5822d7d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 03:46:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 03:46:08 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 03:46:08 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 03:46:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 03:46:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 03:46:28 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:37:14 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.3 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:37:14 GMT
ARG MARIADB_VERSION=1:10.11.3+maria~ubu2204
# Thu, 11 May 2023 22:37:14 GMT
ENV MARIADB_VERSION=1:10.11.3+maria~ubu2204
# Thu, 11 May 2023 22:37:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
# Thu, 11 May 2023 22:37:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:37:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:37:46 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:37:46 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:37:46 GMT
COPY file:94a071210c811522ac7cb9cd9b6d33b1df5eb056971fbdeefa8e9bc2e8a2d629 in /usr/local/bin/ 
# Thu, 11 May 2023 22:37:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:37:46 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:37:46 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:f3f60f415e9a03eed88bd5dd5268c841cde08dacf16911a3ef1e4e0fcdd76568`  
		Last Modified: Wed, 26 Apr 2023 02:08:37 GMT  
		Size: 28.4 MB (28389440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bfb87016de46ece16208cd39b5fa89740b8e8db147c2da2f6483551b3e8d521`  
		Last Modified: Thu, 04 May 2023 03:49:02 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8bd3f48f8f1fc94a1a143132ba91e005df50ee4327d0e209553cc89145a91f`  
		Last Modified: Thu, 04 May 2023 03:49:03 GMT  
		Size: 5.4 MB (5409831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ebb0502bf43d03d32f27b6cfa9ea349e89bccb62bd1ef3cf96a9a769e6c1fa`  
		Last Modified: Thu, 04 May 2023 03:49:00 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c39b9daac872cd7020c71e2bcfb8c097a1ea4c92c6e75f0fa1c5457a9793fabd`  
		Last Modified: Thu, 11 May 2023 22:41:30 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d0e97236e823170f83bde496cd664d5a354bdc0e3812e70d9e9dc434a067506`  
		Last Modified: Thu, 11 May 2023 22:41:40 GMT  
		Size: 83.8 MB (83795910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b5a4e92f3071fd8c0fcaba769b1d01c887847907025859069a695bebdfd2ca`  
		Last Modified: Thu, 11 May 2023 22:41:30 GMT  
		Size: 3.5 KB (3527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e100a9688501846d85a74ce52c2427d070849317340c48bdb06946ff8f89178`  
		Last Modified: Thu, 11 May 2023 22:41:30 GMT  
		Size: 7.5 KB (7515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-jammy` - linux; ppc64le

```console
$ docker pull mariadb@sha256:4d240e05dd2101a66ba61dd58ddc69e210df50aeefa05a74cbf242c6662dd584
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.9 MB (131883188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f8168152d1fd9b321f68df36d3f926ad414075ce59cb8a0b139cc40dc3a652c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:17 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:18 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:21 GMT
ADD file:e75f08a67f0576b5441bb2fe454cad4b5b31a9d4efea23be791af62e1e0c712f in / 
# Tue, 25 Apr 2023 17:30:21 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 14:29:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 14:29:33 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 14:29:33 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 14:30:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 14:30:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 14:30:21 GMT
ENV LANG=C.UTF-8
# Thu, 04 May 2023 14:31:55 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.2 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 04 May 2023 14:31:55 GMT
ARG MARIADB_VERSION=1:10.11.2+maria~ubu2204
# Thu, 04 May 2023 14:31:56 GMT
ENV MARIADB_VERSION=1:10.11.2+maria~ubu2204
# Thu, 04 May 2023 14:31:56 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.2/repo/ubuntu/ jammy main
# Thu, 04 May 2023 14:31:58 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 04 May 2023 14:32:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 04 May 2023 14:33:04 GMT
VOLUME [/var/lib/mysql]
# Thu, 04 May 2023 14:33:05 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 04 May 2023 14:33:05 GMT
COPY file:ebdfbcbc74dda1874f1c75d86e1c32733edb402d13440b2b7140a952010bc21f in /usr/local/bin/ 
# Thu, 04 May 2023 14:33:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 May 2023 14:33:07 GMT
EXPOSE 3306
# Thu, 04 May 2023 14:33:07 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:f6a63d8cd043e76933823b18cbb7057a55bb4d66d64639c81e15a4700c101582`  
		Last Modified: Wed, 03 May 2023 17:09:07 GMT  
		Size: 35.7 MB (35712706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df46cdfc9a45a40dd254c1a0f2ccb2b0020e6852a5fb101d44d79250da5ddc69`  
		Last Modified: Thu, 04 May 2023 14:38:11 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11d1aa00f5a23d7276d6c701876911c79820fef6401156510e68eecb03012091`  
		Last Modified: Thu, 04 May 2023 14:38:12 GMT  
		Size: 6.0 MB (6021655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ec0fb2f57daffaea6b67a61d9012d55d4fcef64766481235d00d0438513793b`  
		Last Modified: Thu, 04 May 2023 14:38:08 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5222456a7c2bfe3bf5175c63ee69047694ca04828ae27b736d3e365bb098e6`  
		Last Modified: Thu, 04 May 2023 14:38:49 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c483e4bc0a4a66eedb7d32ac48ebb035053d2581b308082f7f73aae65b5695`  
		Last Modified: Thu, 04 May 2023 14:39:13 GMT  
		Size: 90.1 MB (90136103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c20716d8d6a4a6fffb6a1a4433d2c519498b3245749451035f81128a7d9d6f5a`  
		Last Modified: Thu, 04 May 2023 14:38:49 GMT  
		Size: 3.5 KB (3526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92aecaeb58f118d19cc858ade38f52e5cc3f8fbd518c7cd5d71caecd07b49db`  
		Last Modified: Thu, 04 May 2023 14:38:49 GMT  
		Size: 7.0 KB (6970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-jammy` - linux; s390x

```console
$ docker pull mariadb@sha256:6776cef0f480be971c0746153bfc7d3c6a6ba04acb53448303d2ee7fd50b10d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121445424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5c39fb429a2411a98cc5e9ce78feeefc35cd3d0d3f948609f9d0d7162e091bf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 26 Jan 2023 05:08:35 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:08:35 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:08:36 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:08:36 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:08:37 GMT
ADD file:a9794efc1a102ab6a7160e660a63f4b267797b8b7e0b0bfd9c04ed62846cfb36 in / 
# Thu, 26 Jan 2023 05:08:38 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:42:50 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 31 Jan 2023 18:42:50 GMT
ENV GOSU_VERSION=1.14
# Tue, 31 Jan 2023 18:42:50 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 31 Jan 2023 18:43:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 31 Jan 2023 18:43:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 31 Jan 2023 18:43:06 GMT
ENV LANG=C.UTF-8
# Sat, 18 Feb 2023 00:39:43 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.2 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Sat, 18 Feb 2023 00:39:43 GMT
ARG MARIADB_VERSION=1:10.11.2+maria~ubu2204
# Sat, 18 Feb 2023 00:39:43 GMT
ENV MARIADB_VERSION=1:10.11.2+maria~ubu2204
# Sat, 18 Feb 2023 00:39:44 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.2/repo/ubuntu/ jammy main
# Sat, 18 Feb 2023 00:39:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 18 Feb 2023 00:40:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Sat, 18 Feb 2023 00:40:18 GMT
VOLUME [/var/lib/mysql]
# Sat, 25 Feb 2023 04:00:33 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Sat, 25 Feb 2023 04:00:33 GMT
COPY file:ebdfbcbc74dda1874f1c75d86e1c32733edb402d13440b2b7140a952010bc21f in /usr/local/bin/ 
# Sat, 25 Feb 2023 04:00:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 25 Feb 2023 04:00:33 GMT
EXPOSE 3306
# Sat, 25 Feb 2023 04:00:33 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:dd969ed9de43018fe5442c859bf66eabf23145b966b9338392ea707aed18b26f`  
		Last Modified: Tue, 31 Jan 2023 17:55:34 GMT  
		Size: 28.6 MB (28641926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b702438b56d7a6aaaad49e2be85e1bb2f3beb85406f6b9db1a232f798c558b3`  
		Last Modified: Tue, 31 Jan 2023 18:48:25 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60737998d0295bde808ca8856933482817ca605937f714f3cfca1ab0b4ca99ed`  
		Last Modified: Tue, 31 Jan 2023 18:48:26 GMT  
		Size: 5.4 MB (5401827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6e12a0288bb0803aeb23e581ca842e1fdf826fa28b4a730dd83585ea125ff8`  
		Last Modified: Tue, 31 Jan 2023 18:48:24 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36528da402899a29c65aec506cc3573ecd9edf046e710740371ea56b98466ce`  
		Last Modified: Sat, 18 Feb 2023 00:42:04 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c45532e045d6549e8a41f2b8cce4c9cc336de9d1dac3d929d2a7ea3fee6fcf`  
		Last Modified: Sat, 18 Feb 2023 00:42:16 GMT  
		Size: 87.4 MB (87388947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf76dfdfa839489a3b54c3eb3679f8718726a96a30cc2049089b7ac593b41ae`  
		Last Modified: Sat, 25 Feb 2023 04:02:18 GMT  
		Size: 3.5 KB (3526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f477561fbd237479df484d7fc122750ffa7b64e394c3ca9d2cc6e5072810967d`  
		Last Modified: Sat, 25 Feb 2023 04:02:18 GMT  
		Size: 7.0 KB (6971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.10`

```console
$ docker pull mariadb@sha256:4757ffc13119ddab0be0c56f9b96429884f111d26cc7a16a42b8bd2cf16b12d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.10` - linux; amd64

```console
$ docker pull mariadb@sha256:5c8108be2a1fee4e67b0c457b0d270fe2952808b72a67b99e46288bb7642bcf5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (123005292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22f577dc07cda75b8814ba97db4f5d740d7d80c859a3887b67d0311551cc1c18`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 07:52:03 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 07:52:03 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 07:52:03 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 07:52:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 07:52:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 07:52:19 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:54:12 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.10.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:54:12 GMT
ARG MARIADB_VERSION=1:10.10.4+maria~ubu2204
# Thu, 11 May 2023 22:54:12 GMT
ENV MARIADB_VERSION=1:10.10.4+maria~ubu2204
# Thu, 11 May 2023 22:54:12 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.4/repo/ubuntu/ jammy main
# Thu, 11 May 2023 22:54:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:54:31 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:54:31 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:54:31 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:54:31 GMT
COPY file:94a071210c811522ac7cb9cd9b6d33b1df5eb056971fbdeefa8e9bc2e8a2d629 in /usr/local/bin/ 
# Thu, 11 May 2023 22:54:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:54:32 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:54:32 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:1bc677758ad7fa4503417ae5be18809c5a8679b5b36fcd1464d5a8e41cb13305`  
		Last Modified: Tue, 25 Apr 2023 22:54:44 GMT  
		Size: 30.4 MB (30430220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196e1740aea41b9915498de02cc132de54583dad1a212d06c9f6eb4690e1e0cb`  
		Last Modified: Thu, 04 May 2023 07:54:52 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4df0997938e5fd755403145484e1253115d3739285c704f562cf3bd6d89ec8`  
		Last Modified: Thu, 04 May 2023 07:54:53 GMT  
		Size: 5.6 MB (5595975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa4e41848249471f699386db900347fa61b39622dfba140344d9c51b264e7db`  
		Last Modified: Thu, 04 May 2023 07:54:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca0f9117e04f38fb2ca9e302a6c40b1f4364fce2a057901ef29cdbddf5008647`  
		Last Modified: Thu, 11 May 2023 22:58:34 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64be93be0d00fccf0a5c024dc96532effc8c2764df0ec2afabaa9db3d0f7e716`  
		Last Modified: Thu, 11 May 2023 22:58:46 GMT  
		Size: 87.0 MB (86965834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e2a65579dc5b4c25a213ea1725a0a9d5f6e773b3d400d590b9498c2925d70e`  
		Last Modified: Thu, 11 May 2023 22:58:34 GMT  
		Size: 3.5 KB (3524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5616973b9970f93a5c1f077e9829b21f7bd1d772703020f3c37993bb7a4b1c`  
		Last Modified: Thu, 11 May 2023 22:58:34 GMT  
		Size: 7.5 KB (7513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.10` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:bb0deb17cbfc05502af1b7f21f8b57da00fc4546697931f415deff2cc8cc11ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117553164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1462cc7b3f97cf672d7ecdca1e996dab61c3bb0763d716b91d48754ab08d3137`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 03:46:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 03:46:08 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 03:46:08 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 03:46:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 03:46:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 03:46:28 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:37:53 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.10.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:37:53 GMT
ARG MARIADB_VERSION=1:10.10.4+maria~ubu2204
# Thu, 11 May 2023 22:37:53 GMT
ENV MARIADB_VERSION=1:10.10.4+maria~ubu2204
# Thu, 11 May 2023 22:37:54 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.4/repo/ubuntu/ jammy main
# Thu, 11 May 2023 22:37:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:38:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:38:12 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:38:13 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:38:13 GMT
COPY file:94a071210c811522ac7cb9cd9b6d33b1df5eb056971fbdeefa8e9bc2e8a2d629 in /usr/local/bin/ 
# Thu, 11 May 2023 22:38:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:38:13 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:38:13 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:f3f60f415e9a03eed88bd5dd5268c841cde08dacf16911a3ef1e4e0fcdd76568`  
		Last Modified: Wed, 26 Apr 2023 02:08:37 GMT  
		Size: 28.4 MB (28389440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bfb87016de46ece16208cd39b5fa89740b8e8db147c2da2f6483551b3e8d521`  
		Last Modified: Thu, 04 May 2023 03:49:02 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8bd3f48f8f1fc94a1a143132ba91e005df50ee4327d0e209553cc89145a91f`  
		Last Modified: Thu, 04 May 2023 03:49:03 GMT  
		Size: 5.4 MB (5409831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ebb0502bf43d03d32f27b6cfa9ea349e89bccb62bd1ef3cf96a9a769e6c1fa`  
		Last Modified: Thu, 04 May 2023 03:49:00 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:828adc034bf64362d646efa73f61fa80695523236a4b1beda7b83d3c5e1f81f0`  
		Last Modified: Thu, 11 May 2023 22:42:04 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c88f233dd9fff98948615a6df572b8c67a541fd6ce3b0c4114d7b1e03fdefd91`  
		Last Modified: Thu, 11 May 2023 22:42:14 GMT  
		Size: 83.7 MB (83740634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f1679c43a84e621dee437597b92a93c8de99d9fe7f87be1b5c901f83330bfd5`  
		Last Modified: Thu, 11 May 2023 22:42:04 GMT  
		Size: 3.5 KB (3525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cda206453094f2f73822b11389450f876d6058ce5ec473b4e3512f6c33932e8`  
		Last Modified: Thu, 11 May 2023 22:42:04 GMT  
		Size: 7.5 KB (7508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.10` - linux; ppc64le

```console
$ docker pull mariadb@sha256:fa3b1aade7d591835cc57876fed09019b5bcc9490481665bab5fc741279a9ddb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.9 MB (131860635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d04750f2ca8bb84feb9dc78ed845e0650691b84aee9ce581867c85593adcdad6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:17 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:18 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:21 GMT
ADD file:e75f08a67f0576b5441bb2fe454cad4b5b31a9d4efea23be791af62e1e0c712f in / 
# Tue, 25 Apr 2023 17:30:21 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 14:29:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 14:29:33 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 14:29:33 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 14:30:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 14:30:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 14:30:21 GMT
ENV LANG=C.UTF-8
# Thu, 04 May 2023 14:33:19 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.10.3 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 04 May 2023 14:33:20 GMT
ARG MARIADB_VERSION=1:10.10.3+maria~ubu2204
# Thu, 04 May 2023 14:33:20 GMT
ENV MARIADB_VERSION=1:10.10.3+maria~ubu2204
# Thu, 04 May 2023 14:33:22 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.3/repo/ubuntu/ jammy main
# Thu, 04 May 2023 14:33:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 04 May 2023 14:34:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 04 May 2023 14:34:48 GMT
VOLUME [/var/lib/mysql]
# Thu, 04 May 2023 14:34:48 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 04 May 2023 14:34:49 GMT
COPY file:ebdfbcbc74dda1874f1c75d86e1c32733edb402d13440b2b7140a952010bc21f in /usr/local/bin/ 
# Thu, 04 May 2023 14:34:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 May 2023 14:34:50 GMT
EXPOSE 3306
# Thu, 04 May 2023 14:34:51 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:f6a63d8cd043e76933823b18cbb7057a55bb4d66d64639c81e15a4700c101582`  
		Last Modified: Wed, 03 May 2023 17:09:07 GMT  
		Size: 35.7 MB (35712706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df46cdfc9a45a40dd254c1a0f2ccb2b0020e6852a5fb101d44d79250da5ddc69`  
		Last Modified: Thu, 04 May 2023 14:38:11 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11d1aa00f5a23d7276d6c701876911c79820fef6401156510e68eecb03012091`  
		Last Modified: Thu, 04 May 2023 14:38:12 GMT  
		Size: 6.0 MB (6021655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ec0fb2f57daffaea6b67a61d9012d55d4fcef64766481235d00d0438513793b`  
		Last Modified: Thu, 04 May 2023 14:38:08 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc64165564818d6f7c5bd3654049a59f7d34cc8b7cdbe17ea333597744dad6a5`  
		Last Modified: Thu, 04 May 2023 14:39:39 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d7571a5b82caf449fa96ec78c5894f9cd9816d79fdb2e2dd66ba43a100681a`  
		Last Modified: Thu, 04 May 2023 14:40:04 GMT  
		Size: 90.1 MB (90113553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af684a3f61e35eb9b20cf6bf5d44b0df1d4e4b670ce196cd6a9532bd1ae38c62`  
		Last Modified: Thu, 04 May 2023 14:39:39 GMT  
		Size: 3.5 KB (3526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f42ccb5c5b10fa301cd08f0c5f42b9d097967883a4d06a2927f4913792dffa5c`  
		Last Modified: Thu, 04 May 2023 14:39:40 GMT  
		Size: 7.0 KB (6969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.10` - linux; s390x

```console
$ docker pull mariadb@sha256:f17fc55a7391da4e0f6562c6c935553144f2f96fc3e6f855007e6c4927fd47a9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121441634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86f63ab941bb0d6f4a3fd8e9bd46a62064482698ecf5cafac85282b42ff7b4a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 26 Jan 2023 05:08:35 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:08:35 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:08:36 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:08:36 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:08:37 GMT
ADD file:a9794efc1a102ab6a7160e660a63f4b267797b8b7e0b0bfd9c04ed62846cfb36 in / 
# Thu, 26 Jan 2023 05:08:38 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:42:50 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 31 Jan 2023 18:42:50 GMT
ENV GOSU_VERSION=1.14
# Tue, 31 Jan 2023 18:42:50 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 31 Jan 2023 18:43:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 31 Jan 2023 18:43:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 31 Jan 2023 18:43:06 GMT
ENV LANG=C.UTF-8
# Tue, 07 Feb 2023 01:45:23 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.10.3 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 07 Feb 2023 01:45:23 GMT
ARG MARIADB_VERSION=1:10.10.3+maria~ubu2204
# Tue, 07 Feb 2023 01:45:24 GMT
ENV MARIADB_VERSION=1:10.10.3+maria~ubu2204
# Tue, 07 Feb 2023 01:45:24 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.3/repo/ubuntu/ jammy main
# Tue, 07 Feb 2023 01:45:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Feb 2023 01:46:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 07 Feb 2023 01:46:25 GMT
VOLUME [/var/lib/mysql]
# Sat, 25 Feb 2023 04:00:38 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Sat, 25 Feb 2023 04:00:38 GMT
COPY file:ebdfbcbc74dda1874f1c75d86e1c32733edb402d13440b2b7140a952010bc21f in /usr/local/bin/ 
# Sat, 25 Feb 2023 04:00:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 25 Feb 2023 04:00:39 GMT
EXPOSE 3306
# Sat, 25 Feb 2023 04:00:39 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:dd969ed9de43018fe5442c859bf66eabf23145b966b9338392ea707aed18b26f`  
		Last Modified: Tue, 31 Jan 2023 17:55:34 GMT  
		Size: 28.6 MB (28641926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b702438b56d7a6aaaad49e2be85e1bb2f3beb85406f6b9db1a232f798c558b3`  
		Last Modified: Tue, 31 Jan 2023 18:48:25 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60737998d0295bde808ca8856933482817ca605937f714f3cfca1ab0b4ca99ed`  
		Last Modified: Tue, 31 Jan 2023 18:48:26 GMT  
		Size: 5.4 MB (5401827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6e12a0288bb0803aeb23e581ca842e1fdf826fa28b4a730dd83585ea125ff8`  
		Last Modified: Tue, 31 Jan 2023 18:48:24 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31fff35d394db6493876d324e36fde17f105189c479b762183e37b7efa89a80c`  
		Last Modified: Tue, 07 Feb 2023 01:52:48 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c59b6dadd508b82a333b18b82dcb7f68938ecf2c3703eb27b5bf76d3733bea`  
		Last Modified: Tue, 07 Feb 2023 01:53:01 GMT  
		Size: 87.4 MB (87385164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49de064a4ca872f387cb409872789d76b06d5d225787dbc4ff2c719a00eed8fe`  
		Last Modified: Sat, 25 Feb 2023 04:02:35 GMT  
		Size: 3.5 KB (3522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d31a278a6c54dd19180b2f5e161c832a144ed9fb8a5a980eb005af8327a5f3bb`  
		Last Modified: Sat, 25 Feb 2023 04:02:35 GMT  
		Size: 7.0 KB (6967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.10-jammy`

```console
$ docker pull mariadb@sha256:4757ffc13119ddab0be0c56f9b96429884f111d26cc7a16a42b8bd2cf16b12d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.10-jammy` - linux; amd64

```console
$ docker pull mariadb@sha256:5c8108be2a1fee4e67b0c457b0d270fe2952808b72a67b99e46288bb7642bcf5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (123005292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22f577dc07cda75b8814ba97db4f5d740d7d80c859a3887b67d0311551cc1c18`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 07:52:03 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 07:52:03 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 07:52:03 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 07:52:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 07:52:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 07:52:19 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:54:12 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.10.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:54:12 GMT
ARG MARIADB_VERSION=1:10.10.4+maria~ubu2204
# Thu, 11 May 2023 22:54:12 GMT
ENV MARIADB_VERSION=1:10.10.4+maria~ubu2204
# Thu, 11 May 2023 22:54:12 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.4/repo/ubuntu/ jammy main
# Thu, 11 May 2023 22:54:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:54:31 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:54:31 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:54:31 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:54:31 GMT
COPY file:94a071210c811522ac7cb9cd9b6d33b1df5eb056971fbdeefa8e9bc2e8a2d629 in /usr/local/bin/ 
# Thu, 11 May 2023 22:54:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:54:32 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:54:32 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:1bc677758ad7fa4503417ae5be18809c5a8679b5b36fcd1464d5a8e41cb13305`  
		Last Modified: Tue, 25 Apr 2023 22:54:44 GMT  
		Size: 30.4 MB (30430220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196e1740aea41b9915498de02cc132de54583dad1a212d06c9f6eb4690e1e0cb`  
		Last Modified: Thu, 04 May 2023 07:54:52 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4df0997938e5fd755403145484e1253115d3739285c704f562cf3bd6d89ec8`  
		Last Modified: Thu, 04 May 2023 07:54:53 GMT  
		Size: 5.6 MB (5595975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa4e41848249471f699386db900347fa61b39622dfba140344d9c51b264e7db`  
		Last Modified: Thu, 04 May 2023 07:54:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca0f9117e04f38fb2ca9e302a6c40b1f4364fce2a057901ef29cdbddf5008647`  
		Last Modified: Thu, 11 May 2023 22:58:34 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64be93be0d00fccf0a5c024dc96532effc8c2764df0ec2afabaa9db3d0f7e716`  
		Last Modified: Thu, 11 May 2023 22:58:46 GMT  
		Size: 87.0 MB (86965834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e2a65579dc5b4c25a213ea1725a0a9d5f6e773b3d400d590b9498c2925d70e`  
		Last Modified: Thu, 11 May 2023 22:58:34 GMT  
		Size: 3.5 KB (3524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5616973b9970f93a5c1f077e9829b21f7bd1d772703020f3c37993bb7a4b1c`  
		Last Modified: Thu, 11 May 2023 22:58:34 GMT  
		Size: 7.5 KB (7513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.10-jammy` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:bb0deb17cbfc05502af1b7f21f8b57da00fc4546697931f415deff2cc8cc11ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117553164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1462cc7b3f97cf672d7ecdca1e996dab61c3bb0763d716b91d48754ab08d3137`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 03:46:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 03:46:08 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 03:46:08 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 03:46:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 03:46:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 03:46:28 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:37:53 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.10.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:37:53 GMT
ARG MARIADB_VERSION=1:10.10.4+maria~ubu2204
# Thu, 11 May 2023 22:37:53 GMT
ENV MARIADB_VERSION=1:10.10.4+maria~ubu2204
# Thu, 11 May 2023 22:37:54 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.4/repo/ubuntu/ jammy main
# Thu, 11 May 2023 22:37:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:38:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:38:12 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:38:13 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:38:13 GMT
COPY file:94a071210c811522ac7cb9cd9b6d33b1df5eb056971fbdeefa8e9bc2e8a2d629 in /usr/local/bin/ 
# Thu, 11 May 2023 22:38:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:38:13 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:38:13 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:f3f60f415e9a03eed88bd5dd5268c841cde08dacf16911a3ef1e4e0fcdd76568`  
		Last Modified: Wed, 26 Apr 2023 02:08:37 GMT  
		Size: 28.4 MB (28389440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bfb87016de46ece16208cd39b5fa89740b8e8db147c2da2f6483551b3e8d521`  
		Last Modified: Thu, 04 May 2023 03:49:02 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8bd3f48f8f1fc94a1a143132ba91e005df50ee4327d0e209553cc89145a91f`  
		Last Modified: Thu, 04 May 2023 03:49:03 GMT  
		Size: 5.4 MB (5409831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ebb0502bf43d03d32f27b6cfa9ea349e89bccb62bd1ef3cf96a9a769e6c1fa`  
		Last Modified: Thu, 04 May 2023 03:49:00 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:828adc034bf64362d646efa73f61fa80695523236a4b1beda7b83d3c5e1f81f0`  
		Last Modified: Thu, 11 May 2023 22:42:04 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c88f233dd9fff98948615a6df572b8c67a541fd6ce3b0c4114d7b1e03fdefd91`  
		Last Modified: Thu, 11 May 2023 22:42:14 GMT  
		Size: 83.7 MB (83740634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f1679c43a84e621dee437597b92a93c8de99d9fe7f87be1b5c901f83330bfd5`  
		Last Modified: Thu, 11 May 2023 22:42:04 GMT  
		Size: 3.5 KB (3525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cda206453094f2f73822b11389450f876d6058ce5ec473b4e3512f6c33932e8`  
		Last Modified: Thu, 11 May 2023 22:42:04 GMT  
		Size: 7.5 KB (7508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.10-jammy` - linux; ppc64le

```console
$ docker pull mariadb@sha256:fa3b1aade7d591835cc57876fed09019b5bcc9490481665bab5fc741279a9ddb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.9 MB (131860635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d04750f2ca8bb84feb9dc78ed845e0650691b84aee9ce581867c85593adcdad6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:17 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:18 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:21 GMT
ADD file:e75f08a67f0576b5441bb2fe454cad4b5b31a9d4efea23be791af62e1e0c712f in / 
# Tue, 25 Apr 2023 17:30:21 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 14:29:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 14:29:33 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 14:29:33 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 14:30:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 14:30:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 14:30:21 GMT
ENV LANG=C.UTF-8
# Thu, 04 May 2023 14:33:19 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.10.3 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 04 May 2023 14:33:20 GMT
ARG MARIADB_VERSION=1:10.10.3+maria~ubu2204
# Thu, 04 May 2023 14:33:20 GMT
ENV MARIADB_VERSION=1:10.10.3+maria~ubu2204
# Thu, 04 May 2023 14:33:22 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.3/repo/ubuntu/ jammy main
# Thu, 04 May 2023 14:33:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 04 May 2023 14:34:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 04 May 2023 14:34:48 GMT
VOLUME [/var/lib/mysql]
# Thu, 04 May 2023 14:34:48 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 04 May 2023 14:34:49 GMT
COPY file:ebdfbcbc74dda1874f1c75d86e1c32733edb402d13440b2b7140a952010bc21f in /usr/local/bin/ 
# Thu, 04 May 2023 14:34:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 May 2023 14:34:50 GMT
EXPOSE 3306
# Thu, 04 May 2023 14:34:51 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:f6a63d8cd043e76933823b18cbb7057a55bb4d66d64639c81e15a4700c101582`  
		Last Modified: Wed, 03 May 2023 17:09:07 GMT  
		Size: 35.7 MB (35712706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df46cdfc9a45a40dd254c1a0f2ccb2b0020e6852a5fb101d44d79250da5ddc69`  
		Last Modified: Thu, 04 May 2023 14:38:11 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11d1aa00f5a23d7276d6c701876911c79820fef6401156510e68eecb03012091`  
		Last Modified: Thu, 04 May 2023 14:38:12 GMT  
		Size: 6.0 MB (6021655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ec0fb2f57daffaea6b67a61d9012d55d4fcef64766481235d00d0438513793b`  
		Last Modified: Thu, 04 May 2023 14:38:08 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc64165564818d6f7c5bd3654049a59f7d34cc8b7cdbe17ea333597744dad6a5`  
		Last Modified: Thu, 04 May 2023 14:39:39 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d7571a5b82caf449fa96ec78c5894f9cd9816d79fdb2e2dd66ba43a100681a`  
		Last Modified: Thu, 04 May 2023 14:40:04 GMT  
		Size: 90.1 MB (90113553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af684a3f61e35eb9b20cf6bf5d44b0df1d4e4b670ce196cd6a9532bd1ae38c62`  
		Last Modified: Thu, 04 May 2023 14:39:39 GMT  
		Size: 3.5 KB (3526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f42ccb5c5b10fa301cd08f0c5f42b9d097967883a4d06a2927f4913792dffa5c`  
		Last Modified: Thu, 04 May 2023 14:39:40 GMT  
		Size: 7.0 KB (6969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.10-jammy` - linux; s390x

```console
$ docker pull mariadb@sha256:f17fc55a7391da4e0f6562c6c935553144f2f96fc3e6f855007e6c4927fd47a9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121441634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86f63ab941bb0d6f4a3fd8e9bd46a62064482698ecf5cafac85282b42ff7b4a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 26 Jan 2023 05:08:35 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:08:35 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:08:36 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:08:36 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:08:37 GMT
ADD file:a9794efc1a102ab6a7160e660a63f4b267797b8b7e0b0bfd9c04ed62846cfb36 in / 
# Thu, 26 Jan 2023 05:08:38 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:42:50 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 31 Jan 2023 18:42:50 GMT
ENV GOSU_VERSION=1.14
# Tue, 31 Jan 2023 18:42:50 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 31 Jan 2023 18:43:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 31 Jan 2023 18:43:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 31 Jan 2023 18:43:06 GMT
ENV LANG=C.UTF-8
# Tue, 07 Feb 2023 01:45:23 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.10.3 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 07 Feb 2023 01:45:23 GMT
ARG MARIADB_VERSION=1:10.10.3+maria~ubu2204
# Tue, 07 Feb 2023 01:45:24 GMT
ENV MARIADB_VERSION=1:10.10.3+maria~ubu2204
# Tue, 07 Feb 2023 01:45:24 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.3/repo/ubuntu/ jammy main
# Tue, 07 Feb 2023 01:45:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Feb 2023 01:46:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 07 Feb 2023 01:46:25 GMT
VOLUME [/var/lib/mysql]
# Sat, 25 Feb 2023 04:00:38 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Sat, 25 Feb 2023 04:00:38 GMT
COPY file:ebdfbcbc74dda1874f1c75d86e1c32733edb402d13440b2b7140a952010bc21f in /usr/local/bin/ 
# Sat, 25 Feb 2023 04:00:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 25 Feb 2023 04:00:39 GMT
EXPOSE 3306
# Sat, 25 Feb 2023 04:00:39 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:dd969ed9de43018fe5442c859bf66eabf23145b966b9338392ea707aed18b26f`  
		Last Modified: Tue, 31 Jan 2023 17:55:34 GMT  
		Size: 28.6 MB (28641926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b702438b56d7a6aaaad49e2be85e1bb2f3beb85406f6b9db1a232f798c558b3`  
		Last Modified: Tue, 31 Jan 2023 18:48:25 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60737998d0295bde808ca8856933482817ca605937f714f3cfca1ab0b4ca99ed`  
		Last Modified: Tue, 31 Jan 2023 18:48:26 GMT  
		Size: 5.4 MB (5401827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6e12a0288bb0803aeb23e581ca842e1fdf826fa28b4a730dd83585ea125ff8`  
		Last Modified: Tue, 31 Jan 2023 18:48:24 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31fff35d394db6493876d324e36fde17f105189c479b762183e37b7efa89a80c`  
		Last Modified: Tue, 07 Feb 2023 01:52:48 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c59b6dadd508b82a333b18b82dcb7f68938ecf2c3703eb27b5bf76d3733bea`  
		Last Modified: Tue, 07 Feb 2023 01:53:01 GMT  
		Size: 87.4 MB (87385164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49de064a4ca872f387cb409872789d76b06d5d225787dbc4ff2c719a00eed8fe`  
		Last Modified: Sat, 25 Feb 2023 04:02:35 GMT  
		Size: 3.5 KB (3522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d31a278a6c54dd19180b2f5e161c832a144ed9fb8a5a980eb005af8327a5f3bb`  
		Last Modified: Sat, 25 Feb 2023 04:02:35 GMT  
		Size: 7.0 KB (6967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.10.4`

```console
$ docker pull mariadb@sha256:4ee21b4e2054795781560560fcecbce552d02bb8978dd86be1a30fcd0dd8dcf8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mariadb:10.10.4` - linux; amd64

```console
$ docker pull mariadb@sha256:5c8108be2a1fee4e67b0c457b0d270fe2952808b72a67b99e46288bb7642bcf5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (123005292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22f577dc07cda75b8814ba97db4f5d740d7d80c859a3887b67d0311551cc1c18`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 07:52:03 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 07:52:03 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 07:52:03 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 07:52:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 07:52:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 07:52:19 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:54:12 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.10.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:54:12 GMT
ARG MARIADB_VERSION=1:10.10.4+maria~ubu2204
# Thu, 11 May 2023 22:54:12 GMT
ENV MARIADB_VERSION=1:10.10.4+maria~ubu2204
# Thu, 11 May 2023 22:54:12 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.4/repo/ubuntu/ jammy main
# Thu, 11 May 2023 22:54:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:54:31 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:54:31 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:54:31 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:54:31 GMT
COPY file:94a071210c811522ac7cb9cd9b6d33b1df5eb056971fbdeefa8e9bc2e8a2d629 in /usr/local/bin/ 
# Thu, 11 May 2023 22:54:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:54:32 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:54:32 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:1bc677758ad7fa4503417ae5be18809c5a8679b5b36fcd1464d5a8e41cb13305`  
		Last Modified: Tue, 25 Apr 2023 22:54:44 GMT  
		Size: 30.4 MB (30430220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196e1740aea41b9915498de02cc132de54583dad1a212d06c9f6eb4690e1e0cb`  
		Last Modified: Thu, 04 May 2023 07:54:52 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4df0997938e5fd755403145484e1253115d3739285c704f562cf3bd6d89ec8`  
		Last Modified: Thu, 04 May 2023 07:54:53 GMT  
		Size: 5.6 MB (5595975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa4e41848249471f699386db900347fa61b39622dfba140344d9c51b264e7db`  
		Last Modified: Thu, 04 May 2023 07:54:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca0f9117e04f38fb2ca9e302a6c40b1f4364fce2a057901ef29cdbddf5008647`  
		Last Modified: Thu, 11 May 2023 22:58:34 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64be93be0d00fccf0a5c024dc96532effc8c2764df0ec2afabaa9db3d0f7e716`  
		Last Modified: Thu, 11 May 2023 22:58:46 GMT  
		Size: 87.0 MB (86965834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e2a65579dc5b4c25a213ea1725a0a9d5f6e773b3d400d590b9498c2925d70e`  
		Last Modified: Thu, 11 May 2023 22:58:34 GMT  
		Size: 3.5 KB (3524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5616973b9970f93a5c1f077e9829b21f7bd1d772703020f3c37993bb7a4b1c`  
		Last Modified: Thu, 11 May 2023 22:58:34 GMT  
		Size: 7.5 KB (7513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.10.4` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:bb0deb17cbfc05502af1b7f21f8b57da00fc4546697931f415deff2cc8cc11ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117553164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1462cc7b3f97cf672d7ecdca1e996dab61c3bb0763d716b91d48754ab08d3137`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 03:46:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 03:46:08 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 03:46:08 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 03:46:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 03:46:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 03:46:28 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:37:53 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.10.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:37:53 GMT
ARG MARIADB_VERSION=1:10.10.4+maria~ubu2204
# Thu, 11 May 2023 22:37:53 GMT
ENV MARIADB_VERSION=1:10.10.4+maria~ubu2204
# Thu, 11 May 2023 22:37:54 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.4/repo/ubuntu/ jammy main
# Thu, 11 May 2023 22:37:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:38:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:38:12 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:38:13 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:38:13 GMT
COPY file:94a071210c811522ac7cb9cd9b6d33b1df5eb056971fbdeefa8e9bc2e8a2d629 in /usr/local/bin/ 
# Thu, 11 May 2023 22:38:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:38:13 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:38:13 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:f3f60f415e9a03eed88bd5dd5268c841cde08dacf16911a3ef1e4e0fcdd76568`  
		Last Modified: Wed, 26 Apr 2023 02:08:37 GMT  
		Size: 28.4 MB (28389440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bfb87016de46ece16208cd39b5fa89740b8e8db147c2da2f6483551b3e8d521`  
		Last Modified: Thu, 04 May 2023 03:49:02 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8bd3f48f8f1fc94a1a143132ba91e005df50ee4327d0e209553cc89145a91f`  
		Last Modified: Thu, 04 May 2023 03:49:03 GMT  
		Size: 5.4 MB (5409831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ebb0502bf43d03d32f27b6cfa9ea349e89bccb62bd1ef3cf96a9a769e6c1fa`  
		Last Modified: Thu, 04 May 2023 03:49:00 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:828adc034bf64362d646efa73f61fa80695523236a4b1beda7b83d3c5e1f81f0`  
		Last Modified: Thu, 11 May 2023 22:42:04 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c88f233dd9fff98948615a6df572b8c67a541fd6ce3b0c4114d7b1e03fdefd91`  
		Last Modified: Thu, 11 May 2023 22:42:14 GMT  
		Size: 83.7 MB (83740634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f1679c43a84e621dee437597b92a93c8de99d9fe7f87be1b5c901f83330bfd5`  
		Last Modified: Thu, 11 May 2023 22:42:04 GMT  
		Size: 3.5 KB (3525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cda206453094f2f73822b11389450f876d6058ce5ec473b4e3512f6c33932e8`  
		Last Modified: Thu, 11 May 2023 22:42:04 GMT  
		Size: 7.5 KB (7508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.10.4-jammy`

```console
$ docker pull mariadb@sha256:4ee21b4e2054795781560560fcecbce552d02bb8978dd86be1a30fcd0dd8dcf8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mariadb:10.10.4-jammy` - linux; amd64

```console
$ docker pull mariadb@sha256:5c8108be2a1fee4e67b0c457b0d270fe2952808b72a67b99e46288bb7642bcf5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (123005292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22f577dc07cda75b8814ba97db4f5d740d7d80c859a3887b67d0311551cc1c18`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 07:52:03 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 07:52:03 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 07:52:03 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 07:52:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 07:52:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 07:52:19 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:54:12 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.10.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:54:12 GMT
ARG MARIADB_VERSION=1:10.10.4+maria~ubu2204
# Thu, 11 May 2023 22:54:12 GMT
ENV MARIADB_VERSION=1:10.10.4+maria~ubu2204
# Thu, 11 May 2023 22:54:12 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.4/repo/ubuntu/ jammy main
# Thu, 11 May 2023 22:54:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:54:31 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:54:31 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:54:31 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:54:31 GMT
COPY file:94a071210c811522ac7cb9cd9b6d33b1df5eb056971fbdeefa8e9bc2e8a2d629 in /usr/local/bin/ 
# Thu, 11 May 2023 22:54:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:54:32 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:54:32 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:1bc677758ad7fa4503417ae5be18809c5a8679b5b36fcd1464d5a8e41cb13305`  
		Last Modified: Tue, 25 Apr 2023 22:54:44 GMT  
		Size: 30.4 MB (30430220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196e1740aea41b9915498de02cc132de54583dad1a212d06c9f6eb4690e1e0cb`  
		Last Modified: Thu, 04 May 2023 07:54:52 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4df0997938e5fd755403145484e1253115d3739285c704f562cf3bd6d89ec8`  
		Last Modified: Thu, 04 May 2023 07:54:53 GMT  
		Size: 5.6 MB (5595975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa4e41848249471f699386db900347fa61b39622dfba140344d9c51b264e7db`  
		Last Modified: Thu, 04 May 2023 07:54:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca0f9117e04f38fb2ca9e302a6c40b1f4364fce2a057901ef29cdbddf5008647`  
		Last Modified: Thu, 11 May 2023 22:58:34 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64be93be0d00fccf0a5c024dc96532effc8c2764df0ec2afabaa9db3d0f7e716`  
		Last Modified: Thu, 11 May 2023 22:58:46 GMT  
		Size: 87.0 MB (86965834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e2a65579dc5b4c25a213ea1725a0a9d5f6e773b3d400d590b9498c2925d70e`  
		Last Modified: Thu, 11 May 2023 22:58:34 GMT  
		Size: 3.5 KB (3524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5616973b9970f93a5c1f077e9829b21f7bd1d772703020f3c37993bb7a4b1c`  
		Last Modified: Thu, 11 May 2023 22:58:34 GMT  
		Size: 7.5 KB (7513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.10.4-jammy` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:bb0deb17cbfc05502af1b7f21f8b57da00fc4546697931f415deff2cc8cc11ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117553164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1462cc7b3f97cf672d7ecdca1e996dab61c3bb0763d716b91d48754ab08d3137`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 03:46:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 03:46:08 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 03:46:08 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 03:46:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 03:46:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 03:46:28 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:37:53 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.10.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:37:53 GMT
ARG MARIADB_VERSION=1:10.10.4+maria~ubu2204
# Thu, 11 May 2023 22:37:53 GMT
ENV MARIADB_VERSION=1:10.10.4+maria~ubu2204
# Thu, 11 May 2023 22:37:54 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.4/repo/ubuntu/ jammy main
# Thu, 11 May 2023 22:37:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:38:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:38:12 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:38:13 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:38:13 GMT
COPY file:94a071210c811522ac7cb9cd9b6d33b1df5eb056971fbdeefa8e9bc2e8a2d629 in /usr/local/bin/ 
# Thu, 11 May 2023 22:38:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:38:13 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:38:13 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:f3f60f415e9a03eed88bd5dd5268c841cde08dacf16911a3ef1e4e0fcdd76568`  
		Last Modified: Wed, 26 Apr 2023 02:08:37 GMT  
		Size: 28.4 MB (28389440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bfb87016de46ece16208cd39b5fa89740b8e8db147c2da2f6483551b3e8d521`  
		Last Modified: Thu, 04 May 2023 03:49:02 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8bd3f48f8f1fc94a1a143132ba91e005df50ee4327d0e209553cc89145a91f`  
		Last Modified: Thu, 04 May 2023 03:49:03 GMT  
		Size: 5.4 MB (5409831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ebb0502bf43d03d32f27b6cfa9ea349e89bccb62bd1ef3cf96a9a769e6c1fa`  
		Last Modified: Thu, 04 May 2023 03:49:00 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:828adc034bf64362d646efa73f61fa80695523236a4b1beda7b83d3c5e1f81f0`  
		Last Modified: Thu, 11 May 2023 22:42:04 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c88f233dd9fff98948615a6df572b8c67a541fd6ce3b0c4114d7b1e03fdefd91`  
		Last Modified: Thu, 11 May 2023 22:42:14 GMT  
		Size: 83.7 MB (83740634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f1679c43a84e621dee437597b92a93c8de99d9fe7f87be1b5c901f83330bfd5`  
		Last Modified: Thu, 11 May 2023 22:42:04 GMT  
		Size: 3.5 KB (3525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cda206453094f2f73822b11389450f876d6058ce5ec473b4e3512f6c33932e8`  
		Last Modified: Thu, 11 May 2023 22:42:04 GMT  
		Size: 7.5 KB (7508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.11`

```console
$ docker pull mariadb@sha256:5701c619e8f355f7d4d601f0007f1138f35d02882e206106e5d4a747a6805ed8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.11` - linux; amd64

```console
$ docker pull mariadb@sha256:f77c69a548d1a948f59d6b5eacf25903410cc156f84f33102cc4c662435dea72
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123112287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4af0c16be4b1af0799fd6f831b4fe63eab4ebe5e47d45bedac69b31d23c298e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 07:52:03 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 07:52:03 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 07:52:03 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 07:52:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 07:52:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 07:52:19 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:53:38 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.3 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:53:39 GMT
ARG MARIADB_VERSION=1:10.11.3+maria~ubu2204
# Thu, 11 May 2023 22:53:39 GMT
ENV MARIADB_VERSION=1:10.11.3+maria~ubu2204
# Thu, 11 May 2023 22:53:39 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
# Thu, 11 May 2023 22:53:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:54:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:54:06 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:54:06 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:54:06 GMT
COPY file:94a071210c811522ac7cb9cd9b6d33b1df5eb056971fbdeefa8e9bc2e8a2d629 in /usr/local/bin/ 
# Thu, 11 May 2023 22:54:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:54:06 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:54:07 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:1bc677758ad7fa4503417ae5be18809c5a8679b5b36fcd1464d5a8e41cb13305`  
		Last Modified: Tue, 25 Apr 2023 22:54:44 GMT  
		Size: 30.4 MB (30430220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196e1740aea41b9915498de02cc132de54583dad1a212d06c9f6eb4690e1e0cb`  
		Last Modified: Thu, 04 May 2023 07:54:52 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4df0997938e5fd755403145484e1253115d3739285c704f562cf3bd6d89ec8`  
		Last Modified: Thu, 04 May 2023 07:54:53 GMT  
		Size: 5.6 MB (5595975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa4e41848249471f699386db900347fa61b39622dfba140344d9c51b264e7db`  
		Last Modified: Thu, 04 May 2023 07:54:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a134c78ed13cbf2e6ac7f37c3ef851e65671664763a229e5460065d76e2ed7fa`  
		Last Modified: Thu, 11 May 2023 22:57:57 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7cd475067d8253d1d2cd28269770d3abf6eb40757983f4c92ae62f7a89b5535`  
		Last Modified: Thu, 11 May 2023 22:58:09 GMT  
		Size: 87.1 MB (87072824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348ae7ff2d74996bdc3e5da86e199b871eac8e2f86e7e15f7d03cbccc7231fa5`  
		Last Modified: Thu, 11 May 2023 22:57:57 GMT  
		Size: 3.5 KB (3528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e83ab58cb77ae0bded1f1bbd34ccc3c633547646227392d393af71e8b24a893`  
		Last Modified: Thu, 11 May 2023 22:57:57 GMT  
		Size: 7.5 KB (7516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.11` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:b180bb51094778a95fb835b429cfc2583d0f4e8e666cab652c221f3f03b6708b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117608447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ba3efd0815f87edbc030f0f8d50f783c1c9aa0c47ffec82ab94c6bad5822d7d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 03:46:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 03:46:08 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 03:46:08 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 03:46:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 03:46:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 03:46:28 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:37:14 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.3 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:37:14 GMT
ARG MARIADB_VERSION=1:10.11.3+maria~ubu2204
# Thu, 11 May 2023 22:37:14 GMT
ENV MARIADB_VERSION=1:10.11.3+maria~ubu2204
# Thu, 11 May 2023 22:37:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
# Thu, 11 May 2023 22:37:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:37:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:37:46 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:37:46 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:37:46 GMT
COPY file:94a071210c811522ac7cb9cd9b6d33b1df5eb056971fbdeefa8e9bc2e8a2d629 in /usr/local/bin/ 
# Thu, 11 May 2023 22:37:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:37:46 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:37:46 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:f3f60f415e9a03eed88bd5dd5268c841cde08dacf16911a3ef1e4e0fcdd76568`  
		Last Modified: Wed, 26 Apr 2023 02:08:37 GMT  
		Size: 28.4 MB (28389440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bfb87016de46ece16208cd39b5fa89740b8e8db147c2da2f6483551b3e8d521`  
		Last Modified: Thu, 04 May 2023 03:49:02 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8bd3f48f8f1fc94a1a143132ba91e005df50ee4327d0e209553cc89145a91f`  
		Last Modified: Thu, 04 May 2023 03:49:03 GMT  
		Size: 5.4 MB (5409831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ebb0502bf43d03d32f27b6cfa9ea349e89bccb62bd1ef3cf96a9a769e6c1fa`  
		Last Modified: Thu, 04 May 2023 03:49:00 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c39b9daac872cd7020c71e2bcfb8c097a1ea4c92c6e75f0fa1c5457a9793fabd`  
		Last Modified: Thu, 11 May 2023 22:41:30 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d0e97236e823170f83bde496cd664d5a354bdc0e3812e70d9e9dc434a067506`  
		Last Modified: Thu, 11 May 2023 22:41:40 GMT  
		Size: 83.8 MB (83795910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b5a4e92f3071fd8c0fcaba769b1d01c887847907025859069a695bebdfd2ca`  
		Last Modified: Thu, 11 May 2023 22:41:30 GMT  
		Size: 3.5 KB (3527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e100a9688501846d85a74ce52c2427d070849317340c48bdb06946ff8f89178`  
		Last Modified: Thu, 11 May 2023 22:41:30 GMT  
		Size: 7.5 KB (7515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.11` - linux; ppc64le

```console
$ docker pull mariadb@sha256:4d240e05dd2101a66ba61dd58ddc69e210df50aeefa05a74cbf242c6662dd584
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.9 MB (131883188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f8168152d1fd9b321f68df36d3f926ad414075ce59cb8a0b139cc40dc3a652c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:17 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:18 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:21 GMT
ADD file:e75f08a67f0576b5441bb2fe454cad4b5b31a9d4efea23be791af62e1e0c712f in / 
# Tue, 25 Apr 2023 17:30:21 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 14:29:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 14:29:33 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 14:29:33 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 14:30:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 14:30:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 14:30:21 GMT
ENV LANG=C.UTF-8
# Thu, 04 May 2023 14:31:55 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.2 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 04 May 2023 14:31:55 GMT
ARG MARIADB_VERSION=1:10.11.2+maria~ubu2204
# Thu, 04 May 2023 14:31:56 GMT
ENV MARIADB_VERSION=1:10.11.2+maria~ubu2204
# Thu, 04 May 2023 14:31:56 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.2/repo/ubuntu/ jammy main
# Thu, 04 May 2023 14:31:58 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 04 May 2023 14:32:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 04 May 2023 14:33:04 GMT
VOLUME [/var/lib/mysql]
# Thu, 04 May 2023 14:33:05 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 04 May 2023 14:33:05 GMT
COPY file:ebdfbcbc74dda1874f1c75d86e1c32733edb402d13440b2b7140a952010bc21f in /usr/local/bin/ 
# Thu, 04 May 2023 14:33:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 May 2023 14:33:07 GMT
EXPOSE 3306
# Thu, 04 May 2023 14:33:07 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:f6a63d8cd043e76933823b18cbb7057a55bb4d66d64639c81e15a4700c101582`  
		Last Modified: Wed, 03 May 2023 17:09:07 GMT  
		Size: 35.7 MB (35712706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df46cdfc9a45a40dd254c1a0f2ccb2b0020e6852a5fb101d44d79250da5ddc69`  
		Last Modified: Thu, 04 May 2023 14:38:11 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11d1aa00f5a23d7276d6c701876911c79820fef6401156510e68eecb03012091`  
		Last Modified: Thu, 04 May 2023 14:38:12 GMT  
		Size: 6.0 MB (6021655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ec0fb2f57daffaea6b67a61d9012d55d4fcef64766481235d00d0438513793b`  
		Last Modified: Thu, 04 May 2023 14:38:08 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5222456a7c2bfe3bf5175c63ee69047694ca04828ae27b736d3e365bb098e6`  
		Last Modified: Thu, 04 May 2023 14:38:49 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c483e4bc0a4a66eedb7d32ac48ebb035053d2581b308082f7f73aae65b5695`  
		Last Modified: Thu, 04 May 2023 14:39:13 GMT  
		Size: 90.1 MB (90136103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c20716d8d6a4a6fffb6a1a4433d2c519498b3245749451035f81128a7d9d6f5a`  
		Last Modified: Thu, 04 May 2023 14:38:49 GMT  
		Size: 3.5 KB (3526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92aecaeb58f118d19cc858ade38f52e5cc3f8fbd518c7cd5d71caecd07b49db`  
		Last Modified: Thu, 04 May 2023 14:38:49 GMT  
		Size: 7.0 KB (6970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.11` - linux; s390x

```console
$ docker pull mariadb@sha256:6776cef0f480be971c0746153bfc7d3c6a6ba04acb53448303d2ee7fd50b10d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121445424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5c39fb429a2411a98cc5e9ce78feeefc35cd3d0d3f948609f9d0d7162e091bf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 26 Jan 2023 05:08:35 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:08:35 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:08:36 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:08:36 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:08:37 GMT
ADD file:a9794efc1a102ab6a7160e660a63f4b267797b8b7e0b0bfd9c04ed62846cfb36 in / 
# Thu, 26 Jan 2023 05:08:38 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:42:50 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 31 Jan 2023 18:42:50 GMT
ENV GOSU_VERSION=1.14
# Tue, 31 Jan 2023 18:42:50 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 31 Jan 2023 18:43:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 31 Jan 2023 18:43:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 31 Jan 2023 18:43:06 GMT
ENV LANG=C.UTF-8
# Sat, 18 Feb 2023 00:39:43 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.2 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Sat, 18 Feb 2023 00:39:43 GMT
ARG MARIADB_VERSION=1:10.11.2+maria~ubu2204
# Sat, 18 Feb 2023 00:39:43 GMT
ENV MARIADB_VERSION=1:10.11.2+maria~ubu2204
# Sat, 18 Feb 2023 00:39:44 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.2/repo/ubuntu/ jammy main
# Sat, 18 Feb 2023 00:39:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 18 Feb 2023 00:40:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Sat, 18 Feb 2023 00:40:18 GMT
VOLUME [/var/lib/mysql]
# Sat, 25 Feb 2023 04:00:33 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Sat, 25 Feb 2023 04:00:33 GMT
COPY file:ebdfbcbc74dda1874f1c75d86e1c32733edb402d13440b2b7140a952010bc21f in /usr/local/bin/ 
# Sat, 25 Feb 2023 04:00:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 25 Feb 2023 04:00:33 GMT
EXPOSE 3306
# Sat, 25 Feb 2023 04:00:33 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:dd969ed9de43018fe5442c859bf66eabf23145b966b9338392ea707aed18b26f`  
		Last Modified: Tue, 31 Jan 2023 17:55:34 GMT  
		Size: 28.6 MB (28641926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b702438b56d7a6aaaad49e2be85e1bb2f3beb85406f6b9db1a232f798c558b3`  
		Last Modified: Tue, 31 Jan 2023 18:48:25 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60737998d0295bde808ca8856933482817ca605937f714f3cfca1ab0b4ca99ed`  
		Last Modified: Tue, 31 Jan 2023 18:48:26 GMT  
		Size: 5.4 MB (5401827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6e12a0288bb0803aeb23e581ca842e1fdf826fa28b4a730dd83585ea125ff8`  
		Last Modified: Tue, 31 Jan 2023 18:48:24 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36528da402899a29c65aec506cc3573ecd9edf046e710740371ea56b98466ce`  
		Last Modified: Sat, 18 Feb 2023 00:42:04 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c45532e045d6549e8a41f2b8cce4c9cc336de9d1dac3d929d2a7ea3fee6fcf`  
		Last Modified: Sat, 18 Feb 2023 00:42:16 GMT  
		Size: 87.4 MB (87388947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf76dfdfa839489a3b54c3eb3679f8718726a96a30cc2049089b7ac593b41ae`  
		Last Modified: Sat, 25 Feb 2023 04:02:18 GMT  
		Size: 3.5 KB (3526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f477561fbd237479df484d7fc122750ffa7b64e394c3ca9d2cc6e5072810967d`  
		Last Modified: Sat, 25 Feb 2023 04:02:18 GMT  
		Size: 7.0 KB (6971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.11-jammy`

```console
$ docker pull mariadb@sha256:5701c619e8f355f7d4d601f0007f1138f35d02882e206106e5d4a747a6805ed8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.11-jammy` - linux; amd64

```console
$ docker pull mariadb@sha256:f77c69a548d1a948f59d6b5eacf25903410cc156f84f33102cc4c662435dea72
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123112287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4af0c16be4b1af0799fd6f831b4fe63eab4ebe5e47d45bedac69b31d23c298e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 07:52:03 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 07:52:03 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 07:52:03 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 07:52:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 07:52:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 07:52:19 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:53:38 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.3 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:53:39 GMT
ARG MARIADB_VERSION=1:10.11.3+maria~ubu2204
# Thu, 11 May 2023 22:53:39 GMT
ENV MARIADB_VERSION=1:10.11.3+maria~ubu2204
# Thu, 11 May 2023 22:53:39 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
# Thu, 11 May 2023 22:53:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:54:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:54:06 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:54:06 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:54:06 GMT
COPY file:94a071210c811522ac7cb9cd9b6d33b1df5eb056971fbdeefa8e9bc2e8a2d629 in /usr/local/bin/ 
# Thu, 11 May 2023 22:54:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:54:06 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:54:07 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:1bc677758ad7fa4503417ae5be18809c5a8679b5b36fcd1464d5a8e41cb13305`  
		Last Modified: Tue, 25 Apr 2023 22:54:44 GMT  
		Size: 30.4 MB (30430220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196e1740aea41b9915498de02cc132de54583dad1a212d06c9f6eb4690e1e0cb`  
		Last Modified: Thu, 04 May 2023 07:54:52 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4df0997938e5fd755403145484e1253115d3739285c704f562cf3bd6d89ec8`  
		Last Modified: Thu, 04 May 2023 07:54:53 GMT  
		Size: 5.6 MB (5595975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa4e41848249471f699386db900347fa61b39622dfba140344d9c51b264e7db`  
		Last Modified: Thu, 04 May 2023 07:54:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a134c78ed13cbf2e6ac7f37c3ef851e65671664763a229e5460065d76e2ed7fa`  
		Last Modified: Thu, 11 May 2023 22:57:57 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7cd475067d8253d1d2cd28269770d3abf6eb40757983f4c92ae62f7a89b5535`  
		Last Modified: Thu, 11 May 2023 22:58:09 GMT  
		Size: 87.1 MB (87072824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348ae7ff2d74996bdc3e5da86e199b871eac8e2f86e7e15f7d03cbccc7231fa5`  
		Last Modified: Thu, 11 May 2023 22:57:57 GMT  
		Size: 3.5 KB (3528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e83ab58cb77ae0bded1f1bbd34ccc3c633547646227392d393af71e8b24a893`  
		Last Modified: Thu, 11 May 2023 22:57:57 GMT  
		Size: 7.5 KB (7516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.11-jammy` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:b180bb51094778a95fb835b429cfc2583d0f4e8e666cab652c221f3f03b6708b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117608447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ba3efd0815f87edbc030f0f8d50f783c1c9aa0c47ffec82ab94c6bad5822d7d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 03:46:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 03:46:08 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 03:46:08 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 03:46:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 03:46:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 03:46:28 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:37:14 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.3 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:37:14 GMT
ARG MARIADB_VERSION=1:10.11.3+maria~ubu2204
# Thu, 11 May 2023 22:37:14 GMT
ENV MARIADB_VERSION=1:10.11.3+maria~ubu2204
# Thu, 11 May 2023 22:37:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
# Thu, 11 May 2023 22:37:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:37:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:37:46 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:37:46 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:37:46 GMT
COPY file:94a071210c811522ac7cb9cd9b6d33b1df5eb056971fbdeefa8e9bc2e8a2d629 in /usr/local/bin/ 
# Thu, 11 May 2023 22:37:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:37:46 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:37:46 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:f3f60f415e9a03eed88bd5dd5268c841cde08dacf16911a3ef1e4e0fcdd76568`  
		Last Modified: Wed, 26 Apr 2023 02:08:37 GMT  
		Size: 28.4 MB (28389440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bfb87016de46ece16208cd39b5fa89740b8e8db147c2da2f6483551b3e8d521`  
		Last Modified: Thu, 04 May 2023 03:49:02 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8bd3f48f8f1fc94a1a143132ba91e005df50ee4327d0e209553cc89145a91f`  
		Last Modified: Thu, 04 May 2023 03:49:03 GMT  
		Size: 5.4 MB (5409831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ebb0502bf43d03d32f27b6cfa9ea349e89bccb62bd1ef3cf96a9a769e6c1fa`  
		Last Modified: Thu, 04 May 2023 03:49:00 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c39b9daac872cd7020c71e2bcfb8c097a1ea4c92c6e75f0fa1c5457a9793fabd`  
		Last Modified: Thu, 11 May 2023 22:41:30 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d0e97236e823170f83bde496cd664d5a354bdc0e3812e70d9e9dc434a067506`  
		Last Modified: Thu, 11 May 2023 22:41:40 GMT  
		Size: 83.8 MB (83795910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b5a4e92f3071fd8c0fcaba769b1d01c887847907025859069a695bebdfd2ca`  
		Last Modified: Thu, 11 May 2023 22:41:30 GMT  
		Size: 3.5 KB (3527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e100a9688501846d85a74ce52c2427d070849317340c48bdb06946ff8f89178`  
		Last Modified: Thu, 11 May 2023 22:41:30 GMT  
		Size: 7.5 KB (7515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.11-jammy` - linux; ppc64le

```console
$ docker pull mariadb@sha256:4d240e05dd2101a66ba61dd58ddc69e210df50aeefa05a74cbf242c6662dd584
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.9 MB (131883188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f8168152d1fd9b321f68df36d3f926ad414075ce59cb8a0b139cc40dc3a652c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:17 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:18 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:21 GMT
ADD file:e75f08a67f0576b5441bb2fe454cad4b5b31a9d4efea23be791af62e1e0c712f in / 
# Tue, 25 Apr 2023 17:30:21 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 14:29:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 14:29:33 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 14:29:33 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 14:30:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 14:30:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 14:30:21 GMT
ENV LANG=C.UTF-8
# Thu, 04 May 2023 14:31:55 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.2 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 04 May 2023 14:31:55 GMT
ARG MARIADB_VERSION=1:10.11.2+maria~ubu2204
# Thu, 04 May 2023 14:31:56 GMT
ENV MARIADB_VERSION=1:10.11.2+maria~ubu2204
# Thu, 04 May 2023 14:31:56 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.2/repo/ubuntu/ jammy main
# Thu, 04 May 2023 14:31:58 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 04 May 2023 14:32:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 04 May 2023 14:33:04 GMT
VOLUME [/var/lib/mysql]
# Thu, 04 May 2023 14:33:05 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 04 May 2023 14:33:05 GMT
COPY file:ebdfbcbc74dda1874f1c75d86e1c32733edb402d13440b2b7140a952010bc21f in /usr/local/bin/ 
# Thu, 04 May 2023 14:33:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 May 2023 14:33:07 GMT
EXPOSE 3306
# Thu, 04 May 2023 14:33:07 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:f6a63d8cd043e76933823b18cbb7057a55bb4d66d64639c81e15a4700c101582`  
		Last Modified: Wed, 03 May 2023 17:09:07 GMT  
		Size: 35.7 MB (35712706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df46cdfc9a45a40dd254c1a0f2ccb2b0020e6852a5fb101d44d79250da5ddc69`  
		Last Modified: Thu, 04 May 2023 14:38:11 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11d1aa00f5a23d7276d6c701876911c79820fef6401156510e68eecb03012091`  
		Last Modified: Thu, 04 May 2023 14:38:12 GMT  
		Size: 6.0 MB (6021655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ec0fb2f57daffaea6b67a61d9012d55d4fcef64766481235d00d0438513793b`  
		Last Modified: Thu, 04 May 2023 14:38:08 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5222456a7c2bfe3bf5175c63ee69047694ca04828ae27b736d3e365bb098e6`  
		Last Modified: Thu, 04 May 2023 14:38:49 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c483e4bc0a4a66eedb7d32ac48ebb035053d2581b308082f7f73aae65b5695`  
		Last Modified: Thu, 04 May 2023 14:39:13 GMT  
		Size: 90.1 MB (90136103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c20716d8d6a4a6fffb6a1a4433d2c519498b3245749451035f81128a7d9d6f5a`  
		Last Modified: Thu, 04 May 2023 14:38:49 GMT  
		Size: 3.5 KB (3526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92aecaeb58f118d19cc858ade38f52e5cc3f8fbd518c7cd5d71caecd07b49db`  
		Last Modified: Thu, 04 May 2023 14:38:49 GMT  
		Size: 7.0 KB (6970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.11-jammy` - linux; s390x

```console
$ docker pull mariadb@sha256:6776cef0f480be971c0746153bfc7d3c6a6ba04acb53448303d2ee7fd50b10d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121445424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5c39fb429a2411a98cc5e9ce78feeefc35cd3d0d3f948609f9d0d7162e091bf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 26 Jan 2023 05:08:35 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:08:35 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:08:36 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:08:36 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:08:37 GMT
ADD file:a9794efc1a102ab6a7160e660a63f4b267797b8b7e0b0bfd9c04ed62846cfb36 in / 
# Thu, 26 Jan 2023 05:08:38 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:42:50 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 31 Jan 2023 18:42:50 GMT
ENV GOSU_VERSION=1.14
# Tue, 31 Jan 2023 18:42:50 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 31 Jan 2023 18:43:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 31 Jan 2023 18:43:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 31 Jan 2023 18:43:06 GMT
ENV LANG=C.UTF-8
# Sat, 18 Feb 2023 00:39:43 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.2 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Sat, 18 Feb 2023 00:39:43 GMT
ARG MARIADB_VERSION=1:10.11.2+maria~ubu2204
# Sat, 18 Feb 2023 00:39:43 GMT
ENV MARIADB_VERSION=1:10.11.2+maria~ubu2204
# Sat, 18 Feb 2023 00:39:44 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.2/repo/ubuntu/ jammy main
# Sat, 18 Feb 2023 00:39:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 18 Feb 2023 00:40:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Sat, 18 Feb 2023 00:40:18 GMT
VOLUME [/var/lib/mysql]
# Sat, 25 Feb 2023 04:00:33 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Sat, 25 Feb 2023 04:00:33 GMT
COPY file:ebdfbcbc74dda1874f1c75d86e1c32733edb402d13440b2b7140a952010bc21f in /usr/local/bin/ 
# Sat, 25 Feb 2023 04:00:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 25 Feb 2023 04:00:33 GMT
EXPOSE 3306
# Sat, 25 Feb 2023 04:00:33 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:dd969ed9de43018fe5442c859bf66eabf23145b966b9338392ea707aed18b26f`  
		Last Modified: Tue, 31 Jan 2023 17:55:34 GMT  
		Size: 28.6 MB (28641926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b702438b56d7a6aaaad49e2be85e1bb2f3beb85406f6b9db1a232f798c558b3`  
		Last Modified: Tue, 31 Jan 2023 18:48:25 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60737998d0295bde808ca8856933482817ca605937f714f3cfca1ab0b4ca99ed`  
		Last Modified: Tue, 31 Jan 2023 18:48:26 GMT  
		Size: 5.4 MB (5401827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6e12a0288bb0803aeb23e581ca842e1fdf826fa28b4a730dd83585ea125ff8`  
		Last Modified: Tue, 31 Jan 2023 18:48:24 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36528da402899a29c65aec506cc3573ecd9edf046e710740371ea56b98466ce`  
		Last Modified: Sat, 18 Feb 2023 00:42:04 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c45532e045d6549e8a41f2b8cce4c9cc336de9d1dac3d929d2a7ea3fee6fcf`  
		Last Modified: Sat, 18 Feb 2023 00:42:16 GMT  
		Size: 87.4 MB (87388947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf76dfdfa839489a3b54c3eb3679f8718726a96a30cc2049089b7ac593b41ae`  
		Last Modified: Sat, 25 Feb 2023 04:02:18 GMT  
		Size: 3.5 KB (3526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f477561fbd237479df484d7fc122750ffa7b64e394c3ca9d2cc6e5072810967d`  
		Last Modified: Sat, 25 Feb 2023 04:02:18 GMT  
		Size: 7.0 KB (6971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.11.3`

```console
$ docker pull mariadb@sha256:ab92bf22ba67bfd1f6b1f8c065e73613308dabb5e4abe00e1f42206100696f74
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mariadb:10.11.3` - linux; amd64

```console
$ docker pull mariadb@sha256:f77c69a548d1a948f59d6b5eacf25903410cc156f84f33102cc4c662435dea72
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123112287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4af0c16be4b1af0799fd6f831b4fe63eab4ebe5e47d45bedac69b31d23c298e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 07:52:03 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 07:52:03 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 07:52:03 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 07:52:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 07:52:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 07:52:19 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:53:38 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.3 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:53:39 GMT
ARG MARIADB_VERSION=1:10.11.3+maria~ubu2204
# Thu, 11 May 2023 22:53:39 GMT
ENV MARIADB_VERSION=1:10.11.3+maria~ubu2204
# Thu, 11 May 2023 22:53:39 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
# Thu, 11 May 2023 22:53:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:54:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:54:06 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:54:06 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:54:06 GMT
COPY file:94a071210c811522ac7cb9cd9b6d33b1df5eb056971fbdeefa8e9bc2e8a2d629 in /usr/local/bin/ 
# Thu, 11 May 2023 22:54:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:54:06 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:54:07 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:1bc677758ad7fa4503417ae5be18809c5a8679b5b36fcd1464d5a8e41cb13305`  
		Last Modified: Tue, 25 Apr 2023 22:54:44 GMT  
		Size: 30.4 MB (30430220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196e1740aea41b9915498de02cc132de54583dad1a212d06c9f6eb4690e1e0cb`  
		Last Modified: Thu, 04 May 2023 07:54:52 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4df0997938e5fd755403145484e1253115d3739285c704f562cf3bd6d89ec8`  
		Last Modified: Thu, 04 May 2023 07:54:53 GMT  
		Size: 5.6 MB (5595975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa4e41848249471f699386db900347fa61b39622dfba140344d9c51b264e7db`  
		Last Modified: Thu, 04 May 2023 07:54:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a134c78ed13cbf2e6ac7f37c3ef851e65671664763a229e5460065d76e2ed7fa`  
		Last Modified: Thu, 11 May 2023 22:57:57 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7cd475067d8253d1d2cd28269770d3abf6eb40757983f4c92ae62f7a89b5535`  
		Last Modified: Thu, 11 May 2023 22:58:09 GMT  
		Size: 87.1 MB (87072824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348ae7ff2d74996bdc3e5da86e199b871eac8e2f86e7e15f7d03cbccc7231fa5`  
		Last Modified: Thu, 11 May 2023 22:57:57 GMT  
		Size: 3.5 KB (3528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e83ab58cb77ae0bded1f1bbd34ccc3c633547646227392d393af71e8b24a893`  
		Last Modified: Thu, 11 May 2023 22:57:57 GMT  
		Size: 7.5 KB (7516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.11.3` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:b180bb51094778a95fb835b429cfc2583d0f4e8e666cab652c221f3f03b6708b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117608447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ba3efd0815f87edbc030f0f8d50f783c1c9aa0c47ffec82ab94c6bad5822d7d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 03:46:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 03:46:08 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 03:46:08 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 03:46:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 03:46:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 03:46:28 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:37:14 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.3 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:37:14 GMT
ARG MARIADB_VERSION=1:10.11.3+maria~ubu2204
# Thu, 11 May 2023 22:37:14 GMT
ENV MARIADB_VERSION=1:10.11.3+maria~ubu2204
# Thu, 11 May 2023 22:37:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
# Thu, 11 May 2023 22:37:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:37:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:37:46 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:37:46 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:37:46 GMT
COPY file:94a071210c811522ac7cb9cd9b6d33b1df5eb056971fbdeefa8e9bc2e8a2d629 in /usr/local/bin/ 
# Thu, 11 May 2023 22:37:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:37:46 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:37:46 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:f3f60f415e9a03eed88bd5dd5268c841cde08dacf16911a3ef1e4e0fcdd76568`  
		Last Modified: Wed, 26 Apr 2023 02:08:37 GMT  
		Size: 28.4 MB (28389440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bfb87016de46ece16208cd39b5fa89740b8e8db147c2da2f6483551b3e8d521`  
		Last Modified: Thu, 04 May 2023 03:49:02 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8bd3f48f8f1fc94a1a143132ba91e005df50ee4327d0e209553cc89145a91f`  
		Last Modified: Thu, 04 May 2023 03:49:03 GMT  
		Size: 5.4 MB (5409831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ebb0502bf43d03d32f27b6cfa9ea349e89bccb62bd1ef3cf96a9a769e6c1fa`  
		Last Modified: Thu, 04 May 2023 03:49:00 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c39b9daac872cd7020c71e2bcfb8c097a1ea4c92c6e75f0fa1c5457a9793fabd`  
		Last Modified: Thu, 11 May 2023 22:41:30 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d0e97236e823170f83bde496cd664d5a354bdc0e3812e70d9e9dc434a067506`  
		Last Modified: Thu, 11 May 2023 22:41:40 GMT  
		Size: 83.8 MB (83795910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b5a4e92f3071fd8c0fcaba769b1d01c887847907025859069a695bebdfd2ca`  
		Last Modified: Thu, 11 May 2023 22:41:30 GMT  
		Size: 3.5 KB (3527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e100a9688501846d85a74ce52c2427d070849317340c48bdb06946ff8f89178`  
		Last Modified: Thu, 11 May 2023 22:41:30 GMT  
		Size: 7.5 KB (7515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.11.3-jammy`

```console
$ docker pull mariadb@sha256:ab92bf22ba67bfd1f6b1f8c065e73613308dabb5e4abe00e1f42206100696f74
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mariadb:10.11.3-jammy` - linux; amd64

```console
$ docker pull mariadb@sha256:f77c69a548d1a948f59d6b5eacf25903410cc156f84f33102cc4c662435dea72
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123112287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4af0c16be4b1af0799fd6f831b4fe63eab4ebe5e47d45bedac69b31d23c298e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 07:52:03 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 07:52:03 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 07:52:03 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 07:52:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 07:52:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 07:52:19 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:53:38 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.3 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:53:39 GMT
ARG MARIADB_VERSION=1:10.11.3+maria~ubu2204
# Thu, 11 May 2023 22:53:39 GMT
ENV MARIADB_VERSION=1:10.11.3+maria~ubu2204
# Thu, 11 May 2023 22:53:39 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
# Thu, 11 May 2023 22:53:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:54:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:54:06 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:54:06 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:54:06 GMT
COPY file:94a071210c811522ac7cb9cd9b6d33b1df5eb056971fbdeefa8e9bc2e8a2d629 in /usr/local/bin/ 
# Thu, 11 May 2023 22:54:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:54:06 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:54:07 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:1bc677758ad7fa4503417ae5be18809c5a8679b5b36fcd1464d5a8e41cb13305`  
		Last Modified: Tue, 25 Apr 2023 22:54:44 GMT  
		Size: 30.4 MB (30430220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196e1740aea41b9915498de02cc132de54583dad1a212d06c9f6eb4690e1e0cb`  
		Last Modified: Thu, 04 May 2023 07:54:52 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4df0997938e5fd755403145484e1253115d3739285c704f562cf3bd6d89ec8`  
		Last Modified: Thu, 04 May 2023 07:54:53 GMT  
		Size: 5.6 MB (5595975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa4e41848249471f699386db900347fa61b39622dfba140344d9c51b264e7db`  
		Last Modified: Thu, 04 May 2023 07:54:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a134c78ed13cbf2e6ac7f37c3ef851e65671664763a229e5460065d76e2ed7fa`  
		Last Modified: Thu, 11 May 2023 22:57:57 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7cd475067d8253d1d2cd28269770d3abf6eb40757983f4c92ae62f7a89b5535`  
		Last Modified: Thu, 11 May 2023 22:58:09 GMT  
		Size: 87.1 MB (87072824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348ae7ff2d74996bdc3e5da86e199b871eac8e2f86e7e15f7d03cbccc7231fa5`  
		Last Modified: Thu, 11 May 2023 22:57:57 GMT  
		Size: 3.5 KB (3528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e83ab58cb77ae0bded1f1bbd34ccc3c633547646227392d393af71e8b24a893`  
		Last Modified: Thu, 11 May 2023 22:57:57 GMT  
		Size: 7.5 KB (7516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.11.3-jammy` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:b180bb51094778a95fb835b429cfc2583d0f4e8e666cab652c221f3f03b6708b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117608447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ba3efd0815f87edbc030f0f8d50f783c1c9aa0c47ffec82ab94c6bad5822d7d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 03:46:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 03:46:08 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 03:46:08 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 03:46:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 03:46:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 03:46:28 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:37:14 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.3 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:37:14 GMT
ARG MARIADB_VERSION=1:10.11.3+maria~ubu2204
# Thu, 11 May 2023 22:37:14 GMT
ENV MARIADB_VERSION=1:10.11.3+maria~ubu2204
# Thu, 11 May 2023 22:37:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
# Thu, 11 May 2023 22:37:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:37:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:37:46 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:37:46 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:37:46 GMT
COPY file:94a071210c811522ac7cb9cd9b6d33b1df5eb056971fbdeefa8e9bc2e8a2d629 in /usr/local/bin/ 
# Thu, 11 May 2023 22:37:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:37:46 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:37:46 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:f3f60f415e9a03eed88bd5dd5268c841cde08dacf16911a3ef1e4e0fcdd76568`  
		Last Modified: Wed, 26 Apr 2023 02:08:37 GMT  
		Size: 28.4 MB (28389440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bfb87016de46ece16208cd39b5fa89740b8e8db147c2da2f6483551b3e8d521`  
		Last Modified: Thu, 04 May 2023 03:49:02 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8bd3f48f8f1fc94a1a143132ba91e005df50ee4327d0e209553cc89145a91f`  
		Last Modified: Thu, 04 May 2023 03:49:03 GMT  
		Size: 5.4 MB (5409831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ebb0502bf43d03d32f27b6cfa9ea349e89bccb62bd1ef3cf96a9a769e6c1fa`  
		Last Modified: Thu, 04 May 2023 03:49:00 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c39b9daac872cd7020c71e2bcfb8c097a1ea4c92c6e75f0fa1c5457a9793fabd`  
		Last Modified: Thu, 11 May 2023 22:41:30 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d0e97236e823170f83bde496cd664d5a354bdc0e3812e70d9e9dc434a067506`  
		Last Modified: Thu, 11 May 2023 22:41:40 GMT  
		Size: 83.8 MB (83795910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b5a4e92f3071fd8c0fcaba769b1d01c887847907025859069a695bebdfd2ca`  
		Last Modified: Thu, 11 May 2023 22:41:30 GMT  
		Size: 3.5 KB (3527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e100a9688501846d85a74ce52c2427d070849317340c48bdb06946ff8f89178`  
		Last Modified: Thu, 11 May 2023 22:41:30 GMT  
		Size: 7.5 KB (7515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3`

```console
$ docker pull mariadb@sha256:39eabe08ce454d2f4b0d09cb4e27613efd8e9cd3b3793bc620d37ec5b5fd12c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3` - linux; amd64

```console
$ docker pull mariadb@sha256:a4b57b620852e26f2c306c79fd8a61e22c7cd6e55d0a55d5521854ed2c370102
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113523856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1172e50de4349638bab15b56ded75a75c16312c73cf895e045b21da3cff82948`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:25:16 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 18 Apr 2023 02:25:16 GMT
ENV GOSU_VERSION=1.14
# Tue, 18 Apr 2023 02:25:17 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 18 Apr 2023 02:25:35 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 18 Apr 2023 02:25:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 18 Apr 2023 02:25:36 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:56:48 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.3.39 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:56:48 GMT
ARG MARIADB_MAJOR=10.3
# Thu, 11 May 2023 22:56:49 GMT
ENV MARIADB_MAJOR=10.3
# Thu, 11 May 2023 22:56:49 GMT
ARG MARIADB_VERSION=1:10.3.39+maria~ubu2004
# Thu, 11 May 2023 22:56:49 GMT
ENV MARIADB_VERSION=1:10.3.39+maria~ubu2004
# Thu, 11 May 2023 22:56:49 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.39/repo/ubuntu/ focal main
# Thu, 11 May 2023 22:56:49 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.39/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:57:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.39/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:57:15 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:57:15 GMT
COPY file:797eec99bf55d77c916c240bbbe1453b1ba37340268a58d0681bf242c87643e5 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:57:15 GMT
COPY file:c7fbba94efc312a3d294c85b73b08c1a46929becfffb48a76d1ebb6a9b0e785a in /usr/local/bin/ 
# Thu, 11 May 2023 22:57:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.39/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 11 May 2023 22:57:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:57:15 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:57:15 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8bc823a83fdf1329ae53f092d8f3641a60f92ee9f69e8785f5a3fd046eee30f`  
		Last Modified: Tue, 18 Apr 2023 02:28:38 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16685f710f5dded64d14b2537a025d665da5e257c4be3d921737f5f246b0fb9a`  
		Last Modified: Tue, 18 Apr 2023 02:28:40 GMT  
		Size: 7.1 MB (7058710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5660ff630580a5fee05c112e916f0bbca3234820aea68e604a23dba51f23d65`  
		Last Modified: Tue, 18 Apr 2023 02:28:36 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c894f2a9f3adc4894205ef1b27eebd977ca84b98e22289e07391fd8f59aa8e92`  
		Last Modified: Thu, 11 May 2023 23:01:07 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18232e17ddffcf5ddb5360e227f2d93ba169defd86f4ecb9a8cb697ac182c6eb`  
		Last Modified: Thu, 11 May 2023 23:01:18 GMT  
		Size: 77.9 MB (77873214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c25f07aa4d2e4a28771df971896c0b7b201732ed5d9d9b49d0c8c02122b11440`  
		Last Modified: Thu, 11 May 2023 23:01:07 GMT  
		Size: 3.5 KB (3531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc3d12d5ef10f6e5907461b37aac126f5bca7b47f562053c8ec75e43041fa13`  
		Last Modified: Thu, 11 May 2023 23:01:07 GMT  
		Size: 7.5 KB (7492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:806077d08135696457e6efc0abb72b11133ded3cf124c39332ad8c93ac5f360b`  
		Last Modified: Thu, 11 May 2023 23:01:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:d162a04f42d4281b08047ca6e1a204062d348537a621d12a734b68d64ecf2919
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.2 MB (111207186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c465ff0642c26a4bc683e58b9b68d6343072d6d738fed8bec2a84e539fa39fc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:00:47 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 18 Apr 2023 02:00:47 GMT
ENV GOSU_VERSION=1.14
# Tue, 18 Apr 2023 02:00:47 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 18 Apr 2023 02:01:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 18 Apr 2023 02:01:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 18 Apr 2023 02:01:03 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:40:28 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.3.39 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:40:28 GMT
ARG MARIADB_MAJOR=10.3
# Thu, 11 May 2023 22:40:28 GMT
ENV MARIADB_MAJOR=10.3
# Thu, 11 May 2023 22:40:28 GMT
ARG MARIADB_VERSION=1:10.3.39+maria~ubu2004
# Thu, 11 May 2023 22:40:29 GMT
ENV MARIADB_VERSION=1:10.3.39+maria~ubu2004
# Thu, 11 May 2023 22:40:29 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.39/repo/ubuntu/ focal main
# Thu, 11 May 2023 22:40:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.39/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:40:52 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.39/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:40:53 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:40:54 GMT
COPY file:797eec99bf55d77c916c240bbbe1453b1ba37340268a58d0681bf242c87643e5 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:40:54 GMT
COPY file:c7fbba94efc312a3d294c85b73b08c1a46929becfffb48a76d1ebb6a9b0e785a in /usr/local/bin/ 
# Thu, 11 May 2023 22:40:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.39/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 11 May 2023 22:40:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:40:54 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:40:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c227d9b91d2b3157f8d92aefc5896243bf63953d9852e7e73c79ddf26159c9`  
		Last Modified: Tue, 18 Apr 2023 02:03:42 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d0716d74d0fd81781cc567eced35e6c95c70a0e2709606996e1c20c5bda20c`  
		Last Modified: Tue, 18 Apr 2023 02:03:43 GMT  
		Size: 6.8 MB (6786196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673f317ed7421a7da75b11d78e42cce7972ab1b727ed5f537ca1c6f859941bee`  
		Last Modified: Tue, 18 Apr 2023 02:03:40 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d78d0014f8174891036b809aecf02b443cb1d056af6121ad230ae9fcdd6a81b`  
		Last Modified: Thu, 11 May 2023 22:44:14 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185e70d205e5e1112a8071980dcda0832e25cd9ffed15c44478ef70abb92aaf2`  
		Last Modified: Thu, 11 May 2023 22:44:23 GMT  
		Size: 77.2 MB (77211227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4534fea313e22f23f289be73740fff7e6f235e8cea13f298e186edf899f38f28`  
		Last Modified: Thu, 11 May 2023 22:44:14 GMT  
		Size: 3.5 KB (3529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b164fe961089bfa107c19582daef69db5f8fdee46d89f9bf8bc5c1aec32126c`  
		Last Modified: Thu, 11 May 2023 22:44:14 GMT  
		Size: 7.5 KB (7491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2fc3b92caa691c0c514c2766f2d4364c5352618e67da214f782ca725fcd0e7`  
		Last Modified: Thu, 11 May 2023 22:44:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3` - linux; ppc64le

```console
$ docker pull mariadb@sha256:252a0a31952d96c118d80f8d19697baeda44a4c4f8ea276382ecc4b9028d65d7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.4 MB (123423181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6f132fd388b4467e86fda960cd3414c1c7be2dbd7c943458b6a1b7e12e1c2cf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:36 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:37 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:40 GMT
ADD file:faba3891f58656ec753ba6ca4b63e7c1f27bcd236b665634b05d5bc1b1ceee0a in / 
# Thu, 13 Apr 2023 13:09:40 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:51:07 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 18 Apr 2023 01:51:07 GMT
ENV GOSU_VERSION=1.14
# Tue, 18 Apr 2023 01:51:07 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 18 Apr 2023 01:51:40 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 18 Apr 2023 01:51:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 18 Apr 2023 01:51:42 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 01:55:52 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.3.38 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 18 Apr 2023 01:55:52 GMT
ARG MARIADB_MAJOR=10.3
# Tue, 18 Apr 2023 01:55:53 GMT
ENV MARIADB_MAJOR=10.3
# Tue, 18 Apr 2023 01:55:53 GMT
ARG MARIADB_VERSION=1:10.3.38+maria~ubu2004
# Tue, 18 Apr 2023 01:55:53 GMT
ENV MARIADB_VERSION=1:10.3.38+maria~ubu2004
# Tue, 18 Apr 2023 01:55:53 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.38/repo/ubuntu/ focal main
# Tue, 18 Apr 2023 01:55:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.38/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 18 Apr 2023 01:56:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.38/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 18 Apr 2023 01:56:41 GMT
VOLUME [/var/lib/mysql]
# Tue, 18 Apr 2023 01:56:42 GMT
COPY file:797eec99bf55d77c916c240bbbe1453b1ba37340268a58d0681bf242c87643e5 in /usr/local/bin/healthcheck.sh 
# Tue, 18 Apr 2023 01:56:42 GMT
COPY file:ddd629156267c0caa8ab015799dddda644c1de941e71781975267ef22ad8e315 in /usr/local/bin/ 
# Tue, 18 Apr 2023 01:56:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.38/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 18 Apr 2023 01:56:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 18 Apr 2023 01:56:44 GMT
EXPOSE 3306
# Tue, 18 Apr 2023 01:56:44 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d276072145993a42aed3e2b3e8cd26b6e08aab266d9c9d792ee89b26150681da`  
		Last Modified: Fri, 14 Apr 2023 09:36:00 GMT  
		Size: 33.3 MB (33300980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a173b48773a6ef3fc242fca8702df8e2e401cebf5d6eead9c2e8b679d8f8d57`  
		Last Modified: Tue, 18 Apr 2023 01:57:20 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a525710ca72c2fa19727739f7053c36e5bcc630c19dc9bc5a95f6758c57c071c`  
		Last Modified: Tue, 18 Apr 2023 01:57:22 GMT  
		Size: 7.8 MB (7771035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d96443e2327325857d538e8a99972d2e2cd67c59a3c89cbdfb282cd5b80f87`  
		Last Modified: Tue, 18 Apr 2023 01:57:17 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4476fe179087e19bbb749b8e5a2640d95dcda073ff9949139d36ec1647784509`  
		Last Modified: Tue, 18 Apr 2023 01:59:45 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60cbed7d4bdb781e8591215a28d38ce25bb9249716ae478e24c1d6d7845810bb`  
		Last Modified: Tue, 18 Apr 2023 02:00:07 GMT  
		Size: 82.3 MB (82338346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c353ff6d5c2caa5af0666de2c100df4c0e784ef664b98c6f6312e9dcc82e4136`  
		Last Modified: Tue, 18 Apr 2023 01:59:45 GMT  
		Size: 3.5 KB (3530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbcdb15474b7ab41801fab1dcd883c1a2fdac7aa5b16e3c792051b6c1a536f9d`  
		Last Modified: Tue, 18 Apr 2023 01:59:45 GMT  
		Size: 6.9 KB (6945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef1fb8d931d36b9fa00684746446a5ed0da7edf186ba3a1d5e4716c03e2eaaf9`  
		Last Modified: Tue, 18 Apr 2023 01:59:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3-focal`

```console
$ docker pull mariadb@sha256:39eabe08ce454d2f4b0d09cb4e27613efd8e9cd3b3793bc620d37ec5b5fd12c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:a4b57b620852e26f2c306c79fd8a61e22c7cd6e55d0a55d5521854ed2c370102
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113523856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1172e50de4349638bab15b56ded75a75c16312c73cf895e045b21da3cff82948`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:25:16 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 18 Apr 2023 02:25:16 GMT
ENV GOSU_VERSION=1.14
# Tue, 18 Apr 2023 02:25:17 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 18 Apr 2023 02:25:35 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 18 Apr 2023 02:25:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 18 Apr 2023 02:25:36 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:56:48 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.3.39 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:56:48 GMT
ARG MARIADB_MAJOR=10.3
# Thu, 11 May 2023 22:56:49 GMT
ENV MARIADB_MAJOR=10.3
# Thu, 11 May 2023 22:56:49 GMT
ARG MARIADB_VERSION=1:10.3.39+maria~ubu2004
# Thu, 11 May 2023 22:56:49 GMT
ENV MARIADB_VERSION=1:10.3.39+maria~ubu2004
# Thu, 11 May 2023 22:56:49 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.39/repo/ubuntu/ focal main
# Thu, 11 May 2023 22:56:49 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.39/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:57:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.39/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:57:15 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:57:15 GMT
COPY file:797eec99bf55d77c916c240bbbe1453b1ba37340268a58d0681bf242c87643e5 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:57:15 GMT
COPY file:c7fbba94efc312a3d294c85b73b08c1a46929becfffb48a76d1ebb6a9b0e785a in /usr/local/bin/ 
# Thu, 11 May 2023 22:57:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.39/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 11 May 2023 22:57:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:57:15 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:57:15 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8bc823a83fdf1329ae53f092d8f3641a60f92ee9f69e8785f5a3fd046eee30f`  
		Last Modified: Tue, 18 Apr 2023 02:28:38 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16685f710f5dded64d14b2537a025d665da5e257c4be3d921737f5f246b0fb9a`  
		Last Modified: Tue, 18 Apr 2023 02:28:40 GMT  
		Size: 7.1 MB (7058710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5660ff630580a5fee05c112e916f0bbca3234820aea68e604a23dba51f23d65`  
		Last Modified: Tue, 18 Apr 2023 02:28:36 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c894f2a9f3adc4894205ef1b27eebd977ca84b98e22289e07391fd8f59aa8e92`  
		Last Modified: Thu, 11 May 2023 23:01:07 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18232e17ddffcf5ddb5360e227f2d93ba169defd86f4ecb9a8cb697ac182c6eb`  
		Last Modified: Thu, 11 May 2023 23:01:18 GMT  
		Size: 77.9 MB (77873214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c25f07aa4d2e4a28771df971896c0b7b201732ed5d9d9b49d0c8c02122b11440`  
		Last Modified: Thu, 11 May 2023 23:01:07 GMT  
		Size: 3.5 KB (3531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc3d12d5ef10f6e5907461b37aac126f5bca7b47f562053c8ec75e43041fa13`  
		Last Modified: Thu, 11 May 2023 23:01:07 GMT  
		Size: 7.5 KB (7492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:806077d08135696457e6efc0abb72b11133ded3cf124c39332ad8c93ac5f360b`  
		Last Modified: Thu, 11 May 2023 23:01:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:d162a04f42d4281b08047ca6e1a204062d348537a621d12a734b68d64ecf2919
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.2 MB (111207186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c465ff0642c26a4bc683e58b9b68d6343072d6d738fed8bec2a84e539fa39fc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:00:47 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 18 Apr 2023 02:00:47 GMT
ENV GOSU_VERSION=1.14
# Tue, 18 Apr 2023 02:00:47 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 18 Apr 2023 02:01:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 18 Apr 2023 02:01:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 18 Apr 2023 02:01:03 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:40:28 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.3.39 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:40:28 GMT
ARG MARIADB_MAJOR=10.3
# Thu, 11 May 2023 22:40:28 GMT
ENV MARIADB_MAJOR=10.3
# Thu, 11 May 2023 22:40:28 GMT
ARG MARIADB_VERSION=1:10.3.39+maria~ubu2004
# Thu, 11 May 2023 22:40:29 GMT
ENV MARIADB_VERSION=1:10.3.39+maria~ubu2004
# Thu, 11 May 2023 22:40:29 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.39/repo/ubuntu/ focal main
# Thu, 11 May 2023 22:40:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.39/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:40:52 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.39/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:40:53 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:40:54 GMT
COPY file:797eec99bf55d77c916c240bbbe1453b1ba37340268a58d0681bf242c87643e5 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:40:54 GMT
COPY file:c7fbba94efc312a3d294c85b73b08c1a46929becfffb48a76d1ebb6a9b0e785a in /usr/local/bin/ 
# Thu, 11 May 2023 22:40:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.39/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 11 May 2023 22:40:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:40:54 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:40:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c227d9b91d2b3157f8d92aefc5896243bf63953d9852e7e73c79ddf26159c9`  
		Last Modified: Tue, 18 Apr 2023 02:03:42 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d0716d74d0fd81781cc567eced35e6c95c70a0e2709606996e1c20c5bda20c`  
		Last Modified: Tue, 18 Apr 2023 02:03:43 GMT  
		Size: 6.8 MB (6786196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673f317ed7421a7da75b11d78e42cce7972ab1b727ed5f537ca1c6f859941bee`  
		Last Modified: Tue, 18 Apr 2023 02:03:40 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d78d0014f8174891036b809aecf02b443cb1d056af6121ad230ae9fcdd6a81b`  
		Last Modified: Thu, 11 May 2023 22:44:14 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185e70d205e5e1112a8071980dcda0832e25cd9ffed15c44478ef70abb92aaf2`  
		Last Modified: Thu, 11 May 2023 22:44:23 GMT  
		Size: 77.2 MB (77211227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4534fea313e22f23f289be73740fff7e6f235e8cea13f298e186edf899f38f28`  
		Last Modified: Thu, 11 May 2023 22:44:14 GMT  
		Size: 3.5 KB (3529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b164fe961089bfa107c19582daef69db5f8fdee46d89f9bf8bc5c1aec32126c`  
		Last Modified: Thu, 11 May 2023 22:44:14 GMT  
		Size: 7.5 KB (7491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2fc3b92caa691c0c514c2766f2d4364c5352618e67da214f782ca725fcd0e7`  
		Last Modified: Thu, 11 May 2023 22:44:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:252a0a31952d96c118d80f8d19697baeda44a4c4f8ea276382ecc4b9028d65d7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.4 MB (123423181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6f132fd388b4467e86fda960cd3414c1c7be2dbd7c943458b6a1b7e12e1c2cf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:36 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:37 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:40 GMT
ADD file:faba3891f58656ec753ba6ca4b63e7c1f27bcd236b665634b05d5bc1b1ceee0a in / 
# Thu, 13 Apr 2023 13:09:40 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:51:07 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 18 Apr 2023 01:51:07 GMT
ENV GOSU_VERSION=1.14
# Tue, 18 Apr 2023 01:51:07 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 18 Apr 2023 01:51:40 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 18 Apr 2023 01:51:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 18 Apr 2023 01:51:42 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 01:55:52 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.3.38 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 18 Apr 2023 01:55:52 GMT
ARG MARIADB_MAJOR=10.3
# Tue, 18 Apr 2023 01:55:53 GMT
ENV MARIADB_MAJOR=10.3
# Tue, 18 Apr 2023 01:55:53 GMT
ARG MARIADB_VERSION=1:10.3.38+maria~ubu2004
# Tue, 18 Apr 2023 01:55:53 GMT
ENV MARIADB_VERSION=1:10.3.38+maria~ubu2004
# Tue, 18 Apr 2023 01:55:53 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.38/repo/ubuntu/ focal main
# Tue, 18 Apr 2023 01:55:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.38/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 18 Apr 2023 01:56:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.38/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 18 Apr 2023 01:56:41 GMT
VOLUME [/var/lib/mysql]
# Tue, 18 Apr 2023 01:56:42 GMT
COPY file:797eec99bf55d77c916c240bbbe1453b1ba37340268a58d0681bf242c87643e5 in /usr/local/bin/healthcheck.sh 
# Tue, 18 Apr 2023 01:56:42 GMT
COPY file:ddd629156267c0caa8ab015799dddda644c1de941e71781975267ef22ad8e315 in /usr/local/bin/ 
# Tue, 18 Apr 2023 01:56:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.38/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 18 Apr 2023 01:56:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 18 Apr 2023 01:56:44 GMT
EXPOSE 3306
# Tue, 18 Apr 2023 01:56:44 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d276072145993a42aed3e2b3e8cd26b6e08aab266d9c9d792ee89b26150681da`  
		Last Modified: Fri, 14 Apr 2023 09:36:00 GMT  
		Size: 33.3 MB (33300980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a173b48773a6ef3fc242fca8702df8e2e401cebf5d6eead9c2e8b679d8f8d57`  
		Last Modified: Tue, 18 Apr 2023 01:57:20 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a525710ca72c2fa19727739f7053c36e5bcc630c19dc9bc5a95f6758c57c071c`  
		Last Modified: Tue, 18 Apr 2023 01:57:22 GMT  
		Size: 7.8 MB (7771035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d96443e2327325857d538e8a99972d2e2cd67c59a3c89cbdfb282cd5b80f87`  
		Last Modified: Tue, 18 Apr 2023 01:57:17 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4476fe179087e19bbb749b8e5a2640d95dcda073ff9949139d36ec1647784509`  
		Last Modified: Tue, 18 Apr 2023 01:59:45 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60cbed7d4bdb781e8591215a28d38ce25bb9249716ae478e24c1d6d7845810bb`  
		Last Modified: Tue, 18 Apr 2023 02:00:07 GMT  
		Size: 82.3 MB (82338346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c353ff6d5c2caa5af0666de2c100df4c0e784ef664b98c6f6312e9dcc82e4136`  
		Last Modified: Tue, 18 Apr 2023 01:59:45 GMT  
		Size: 3.5 KB (3530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbcdb15474b7ab41801fab1dcd883c1a2fdac7aa5b16e3c792051b6c1a536f9d`  
		Last Modified: Tue, 18 Apr 2023 01:59:45 GMT  
		Size: 6.9 KB (6945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef1fb8d931d36b9fa00684746446a5ed0da7edf186ba3a1d5e4716c03e2eaaf9`  
		Last Modified: Tue, 18 Apr 2023 01:59:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3.39`

```console
$ docker pull mariadb@sha256:7a4dae7e5bfc5199f10aa14f94f9c33db4bf931fd6e61c808871f22cbb1910ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mariadb:10.3.39` - linux; amd64

```console
$ docker pull mariadb@sha256:a4b57b620852e26f2c306c79fd8a61e22c7cd6e55d0a55d5521854ed2c370102
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113523856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1172e50de4349638bab15b56ded75a75c16312c73cf895e045b21da3cff82948`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:25:16 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 18 Apr 2023 02:25:16 GMT
ENV GOSU_VERSION=1.14
# Tue, 18 Apr 2023 02:25:17 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 18 Apr 2023 02:25:35 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 18 Apr 2023 02:25:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 18 Apr 2023 02:25:36 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:56:48 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.3.39 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:56:48 GMT
ARG MARIADB_MAJOR=10.3
# Thu, 11 May 2023 22:56:49 GMT
ENV MARIADB_MAJOR=10.3
# Thu, 11 May 2023 22:56:49 GMT
ARG MARIADB_VERSION=1:10.3.39+maria~ubu2004
# Thu, 11 May 2023 22:56:49 GMT
ENV MARIADB_VERSION=1:10.3.39+maria~ubu2004
# Thu, 11 May 2023 22:56:49 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.39/repo/ubuntu/ focal main
# Thu, 11 May 2023 22:56:49 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.39/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:57:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.39/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:57:15 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:57:15 GMT
COPY file:797eec99bf55d77c916c240bbbe1453b1ba37340268a58d0681bf242c87643e5 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:57:15 GMT
COPY file:c7fbba94efc312a3d294c85b73b08c1a46929becfffb48a76d1ebb6a9b0e785a in /usr/local/bin/ 
# Thu, 11 May 2023 22:57:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.39/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 11 May 2023 22:57:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:57:15 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:57:15 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8bc823a83fdf1329ae53f092d8f3641a60f92ee9f69e8785f5a3fd046eee30f`  
		Last Modified: Tue, 18 Apr 2023 02:28:38 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16685f710f5dded64d14b2537a025d665da5e257c4be3d921737f5f246b0fb9a`  
		Last Modified: Tue, 18 Apr 2023 02:28:40 GMT  
		Size: 7.1 MB (7058710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5660ff630580a5fee05c112e916f0bbca3234820aea68e604a23dba51f23d65`  
		Last Modified: Tue, 18 Apr 2023 02:28:36 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c894f2a9f3adc4894205ef1b27eebd977ca84b98e22289e07391fd8f59aa8e92`  
		Last Modified: Thu, 11 May 2023 23:01:07 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18232e17ddffcf5ddb5360e227f2d93ba169defd86f4ecb9a8cb697ac182c6eb`  
		Last Modified: Thu, 11 May 2023 23:01:18 GMT  
		Size: 77.9 MB (77873214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c25f07aa4d2e4a28771df971896c0b7b201732ed5d9d9b49d0c8c02122b11440`  
		Last Modified: Thu, 11 May 2023 23:01:07 GMT  
		Size: 3.5 KB (3531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc3d12d5ef10f6e5907461b37aac126f5bca7b47f562053c8ec75e43041fa13`  
		Last Modified: Thu, 11 May 2023 23:01:07 GMT  
		Size: 7.5 KB (7492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:806077d08135696457e6efc0abb72b11133ded3cf124c39332ad8c93ac5f360b`  
		Last Modified: Thu, 11 May 2023 23:01:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.39` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:d162a04f42d4281b08047ca6e1a204062d348537a621d12a734b68d64ecf2919
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.2 MB (111207186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c465ff0642c26a4bc683e58b9b68d6343072d6d738fed8bec2a84e539fa39fc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:00:47 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 18 Apr 2023 02:00:47 GMT
ENV GOSU_VERSION=1.14
# Tue, 18 Apr 2023 02:00:47 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 18 Apr 2023 02:01:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 18 Apr 2023 02:01:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 18 Apr 2023 02:01:03 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:40:28 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.3.39 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:40:28 GMT
ARG MARIADB_MAJOR=10.3
# Thu, 11 May 2023 22:40:28 GMT
ENV MARIADB_MAJOR=10.3
# Thu, 11 May 2023 22:40:28 GMT
ARG MARIADB_VERSION=1:10.3.39+maria~ubu2004
# Thu, 11 May 2023 22:40:29 GMT
ENV MARIADB_VERSION=1:10.3.39+maria~ubu2004
# Thu, 11 May 2023 22:40:29 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.39/repo/ubuntu/ focal main
# Thu, 11 May 2023 22:40:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.39/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:40:52 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.39/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:40:53 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:40:54 GMT
COPY file:797eec99bf55d77c916c240bbbe1453b1ba37340268a58d0681bf242c87643e5 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:40:54 GMT
COPY file:c7fbba94efc312a3d294c85b73b08c1a46929becfffb48a76d1ebb6a9b0e785a in /usr/local/bin/ 
# Thu, 11 May 2023 22:40:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.39/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 11 May 2023 22:40:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:40:54 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:40:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c227d9b91d2b3157f8d92aefc5896243bf63953d9852e7e73c79ddf26159c9`  
		Last Modified: Tue, 18 Apr 2023 02:03:42 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d0716d74d0fd81781cc567eced35e6c95c70a0e2709606996e1c20c5bda20c`  
		Last Modified: Tue, 18 Apr 2023 02:03:43 GMT  
		Size: 6.8 MB (6786196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673f317ed7421a7da75b11d78e42cce7972ab1b727ed5f537ca1c6f859941bee`  
		Last Modified: Tue, 18 Apr 2023 02:03:40 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d78d0014f8174891036b809aecf02b443cb1d056af6121ad230ae9fcdd6a81b`  
		Last Modified: Thu, 11 May 2023 22:44:14 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185e70d205e5e1112a8071980dcda0832e25cd9ffed15c44478ef70abb92aaf2`  
		Last Modified: Thu, 11 May 2023 22:44:23 GMT  
		Size: 77.2 MB (77211227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4534fea313e22f23f289be73740fff7e6f235e8cea13f298e186edf899f38f28`  
		Last Modified: Thu, 11 May 2023 22:44:14 GMT  
		Size: 3.5 KB (3529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b164fe961089bfa107c19582daef69db5f8fdee46d89f9bf8bc5c1aec32126c`  
		Last Modified: Thu, 11 May 2023 22:44:14 GMT  
		Size: 7.5 KB (7491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2fc3b92caa691c0c514c2766f2d4364c5352618e67da214f782ca725fcd0e7`  
		Last Modified: Thu, 11 May 2023 22:44:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3.39-focal`

```console
$ docker pull mariadb@sha256:7a4dae7e5bfc5199f10aa14f94f9c33db4bf931fd6e61c808871f22cbb1910ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mariadb:10.3.39-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:a4b57b620852e26f2c306c79fd8a61e22c7cd6e55d0a55d5521854ed2c370102
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113523856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1172e50de4349638bab15b56ded75a75c16312c73cf895e045b21da3cff82948`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:25:16 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 18 Apr 2023 02:25:16 GMT
ENV GOSU_VERSION=1.14
# Tue, 18 Apr 2023 02:25:17 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 18 Apr 2023 02:25:35 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 18 Apr 2023 02:25:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 18 Apr 2023 02:25:36 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:56:48 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.3.39 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:56:48 GMT
ARG MARIADB_MAJOR=10.3
# Thu, 11 May 2023 22:56:49 GMT
ENV MARIADB_MAJOR=10.3
# Thu, 11 May 2023 22:56:49 GMT
ARG MARIADB_VERSION=1:10.3.39+maria~ubu2004
# Thu, 11 May 2023 22:56:49 GMT
ENV MARIADB_VERSION=1:10.3.39+maria~ubu2004
# Thu, 11 May 2023 22:56:49 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.39/repo/ubuntu/ focal main
# Thu, 11 May 2023 22:56:49 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.39/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:57:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.39/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:57:15 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:57:15 GMT
COPY file:797eec99bf55d77c916c240bbbe1453b1ba37340268a58d0681bf242c87643e5 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:57:15 GMT
COPY file:c7fbba94efc312a3d294c85b73b08c1a46929becfffb48a76d1ebb6a9b0e785a in /usr/local/bin/ 
# Thu, 11 May 2023 22:57:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.39/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 11 May 2023 22:57:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:57:15 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:57:15 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8bc823a83fdf1329ae53f092d8f3641a60f92ee9f69e8785f5a3fd046eee30f`  
		Last Modified: Tue, 18 Apr 2023 02:28:38 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16685f710f5dded64d14b2537a025d665da5e257c4be3d921737f5f246b0fb9a`  
		Last Modified: Tue, 18 Apr 2023 02:28:40 GMT  
		Size: 7.1 MB (7058710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5660ff630580a5fee05c112e916f0bbca3234820aea68e604a23dba51f23d65`  
		Last Modified: Tue, 18 Apr 2023 02:28:36 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c894f2a9f3adc4894205ef1b27eebd977ca84b98e22289e07391fd8f59aa8e92`  
		Last Modified: Thu, 11 May 2023 23:01:07 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18232e17ddffcf5ddb5360e227f2d93ba169defd86f4ecb9a8cb697ac182c6eb`  
		Last Modified: Thu, 11 May 2023 23:01:18 GMT  
		Size: 77.9 MB (77873214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c25f07aa4d2e4a28771df971896c0b7b201732ed5d9d9b49d0c8c02122b11440`  
		Last Modified: Thu, 11 May 2023 23:01:07 GMT  
		Size: 3.5 KB (3531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc3d12d5ef10f6e5907461b37aac126f5bca7b47f562053c8ec75e43041fa13`  
		Last Modified: Thu, 11 May 2023 23:01:07 GMT  
		Size: 7.5 KB (7492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:806077d08135696457e6efc0abb72b11133ded3cf124c39332ad8c93ac5f360b`  
		Last Modified: Thu, 11 May 2023 23:01:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.39-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:d162a04f42d4281b08047ca6e1a204062d348537a621d12a734b68d64ecf2919
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.2 MB (111207186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c465ff0642c26a4bc683e58b9b68d6343072d6d738fed8bec2a84e539fa39fc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:00:47 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 18 Apr 2023 02:00:47 GMT
ENV GOSU_VERSION=1.14
# Tue, 18 Apr 2023 02:00:47 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 18 Apr 2023 02:01:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 18 Apr 2023 02:01:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 18 Apr 2023 02:01:03 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:40:28 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.3.39 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:40:28 GMT
ARG MARIADB_MAJOR=10.3
# Thu, 11 May 2023 22:40:28 GMT
ENV MARIADB_MAJOR=10.3
# Thu, 11 May 2023 22:40:28 GMT
ARG MARIADB_VERSION=1:10.3.39+maria~ubu2004
# Thu, 11 May 2023 22:40:29 GMT
ENV MARIADB_VERSION=1:10.3.39+maria~ubu2004
# Thu, 11 May 2023 22:40:29 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.39/repo/ubuntu/ focal main
# Thu, 11 May 2023 22:40:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.39/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:40:52 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.39/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:40:53 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:40:54 GMT
COPY file:797eec99bf55d77c916c240bbbe1453b1ba37340268a58d0681bf242c87643e5 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:40:54 GMT
COPY file:c7fbba94efc312a3d294c85b73b08c1a46929becfffb48a76d1ebb6a9b0e785a in /usr/local/bin/ 
# Thu, 11 May 2023 22:40:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.39/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 11 May 2023 22:40:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:40:54 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:40:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c227d9b91d2b3157f8d92aefc5896243bf63953d9852e7e73c79ddf26159c9`  
		Last Modified: Tue, 18 Apr 2023 02:03:42 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d0716d74d0fd81781cc567eced35e6c95c70a0e2709606996e1c20c5bda20c`  
		Last Modified: Tue, 18 Apr 2023 02:03:43 GMT  
		Size: 6.8 MB (6786196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673f317ed7421a7da75b11d78e42cce7972ab1b727ed5f537ca1c6f859941bee`  
		Last Modified: Tue, 18 Apr 2023 02:03:40 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d78d0014f8174891036b809aecf02b443cb1d056af6121ad230ae9fcdd6a81b`  
		Last Modified: Thu, 11 May 2023 22:44:14 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185e70d205e5e1112a8071980dcda0832e25cd9ffed15c44478ef70abb92aaf2`  
		Last Modified: Thu, 11 May 2023 22:44:23 GMT  
		Size: 77.2 MB (77211227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4534fea313e22f23f289be73740fff7e6f235e8cea13f298e186edf899f38f28`  
		Last Modified: Thu, 11 May 2023 22:44:14 GMT  
		Size: 3.5 KB (3529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b164fe961089bfa107c19582daef69db5f8fdee46d89f9bf8bc5c1aec32126c`  
		Last Modified: Thu, 11 May 2023 22:44:14 GMT  
		Size: 7.5 KB (7491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2fc3b92caa691c0c514c2766f2d4364c5352618e67da214f782ca725fcd0e7`  
		Last Modified: Thu, 11 May 2023 22:44:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4`

```console
$ docker pull mariadb@sha256:52f288566f3b245c1eca47d4afad5783de1ade3d37ccd55a23de8b1eeb0cde70
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4` - linux; amd64

```console
$ docker pull mariadb@sha256:f9f3c4b8fd9dc7717a903c79d847af9c783771b9e0ff3cc4fc983a40e9e5972d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.0 MB (118979095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4192ed85e762898319e99f2255e94c3b752e69ca0d0472ab852fe96ff95906da`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:25:16 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 18 Apr 2023 02:25:16 GMT
ENV GOSU_VERSION=1.14
# Tue, 18 Apr 2023 02:25:17 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 18 Apr 2023 02:25:35 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 18 Apr 2023 02:25:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 18 Apr 2023 02:25:36 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:56:20 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.4.29 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:56:20 GMT
ARG MARIADB_MAJOR=10.4
# Thu, 11 May 2023 22:56:20 GMT
ENV MARIADB_MAJOR=10.4
# Thu, 11 May 2023 22:56:20 GMT
ARG MARIADB_VERSION=1:10.4.29+maria~ubu2004
# Thu, 11 May 2023 22:56:20 GMT
ENV MARIADB_VERSION=1:10.4.29+maria~ubu2004
# Thu, 11 May 2023 22:56:21 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.29/repo/ubuntu/ focal main
# Thu, 11 May 2023 22:56:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.29/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:56:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.29/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:56:43 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:56:43 GMT
COPY file:797eec99bf55d77c916c240bbbe1453b1ba37340268a58d0681bf242c87643e5 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:56:43 GMT
COPY file:c7fbba94efc312a3d294c85b73b08c1a46929becfffb48a76d1ebb6a9b0e785a in /usr/local/bin/ 
# Thu, 11 May 2023 22:56:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.29/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 11 May 2023 22:56:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:56:44 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:56:44 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8bc823a83fdf1329ae53f092d8f3641a60f92ee9f69e8785f5a3fd046eee30f`  
		Last Modified: Tue, 18 Apr 2023 02:28:38 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16685f710f5dded64d14b2537a025d665da5e257c4be3d921737f5f246b0fb9a`  
		Last Modified: Tue, 18 Apr 2023 02:28:40 GMT  
		Size: 7.1 MB (7058710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5660ff630580a5fee05c112e916f0bbca3234820aea68e604a23dba51f23d65`  
		Last Modified: Tue, 18 Apr 2023 02:28:36 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa7ed7a919d7aafc6368987ae312c3e0155c916f465453c2317e8120983bfc9`  
		Last Modified: Thu, 11 May 2023 23:00:43 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09afbb4d4d00f406a83b53c66f338d357a9a6c0ff911cab92f65fe501e3e2fa6`  
		Last Modified: Thu, 11 May 2023 23:00:54 GMT  
		Size: 83.3 MB (83328455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a0e865b236c70e066726e6c46820c043801f6138b60f7df2c11dc68edc9338`  
		Last Modified: Thu, 11 May 2023 23:00:43 GMT  
		Size: 3.5 KB (3530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:464e829278234489f3a326e4a6dd6fa135c3a4e22012311698c1b0f9897a5008`  
		Last Modified: Thu, 11 May 2023 23:00:43 GMT  
		Size: 7.5 KB (7491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfaa3a5c705f9b43c162f83bffc9c80dc6e8002b69f5020d1e2d05de4e6420d1`  
		Last Modified: Thu, 11 May 2023 23:00:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:96652b616dacb0d393fdfd197d12dae5cc57db87fcebbd4be5558996ecdff0c2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.5 MB (116533934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e061cc874d93b0b4f6b6dc368bd507fabc6db71466c7b56fa7625a7cd1cd4416`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:00:47 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 18 Apr 2023 02:00:47 GMT
ENV GOSU_VERSION=1.14
# Tue, 18 Apr 2023 02:00:47 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 18 Apr 2023 02:01:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 18 Apr 2023 02:01:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 18 Apr 2023 02:01:03 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:40:05 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.4.29 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:40:05 GMT
ARG MARIADB_MAJOR=10.4
# Thu, 11 May 2023 22:40:05 GMT
ENV MARIADB_MAJOR=10.4
# Thu, 11 May 2023 22:40:05 GMT
ARG MARIADB_VERSION=1:10.4.29+maria~ubu2004
# Thu, 11 May 2023 22:40:06 GMT
ENV MARIADB_VERSION=1:10.4.29+maria~ubu2004
# Thu, 11 May 2023 22:40:06 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.29/repo/ubuntu/ focal main
# Thu, 11 May 2023 22:40:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.29/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:40:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.29/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:40:26 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:40:26 GMT
COPY file:797eec99bf55d77c916c240bbbe1453b1ba37340268a58d0681bf242c87643e5 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:40:26 GMT
COPY file:c7fbba94efc312a3d294c85b73b08c1a46929becfffb48a76d1ebb6a9b0e785a in /usr/local/bin/ 
# Thu, 11 May 2023 22:40:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.29/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 11 May 2023 22:40:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:40:27 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:40:27 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c227d9b91d2b3157f8d92aefc5896243bf63953d9852e7e73c79ddf26159c9`  
		Last Modified: Tue, 18 Apr 2023 02:03:42 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d0716d74d0fd81781cc567eced35e6c95c70a0e2709606996e1c20c5bda20c`  
		Last Modified: Tue, 18 Apr 2023 02:03:43 GMT  
		Size: 6.8 MB (6786196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673f317ed7421a7da75b11d78e42cce7972ab1b727ed5f537ca1c6f859941bee`  
		Last Modified: Tue, 18 Apr 2023 02:03:40 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c076e8e334d90f19028dad74643678bec03e1045ddbef9716c04adae5a8dc193`  
		Last Modified: Thu, 11 May 2023 22:43:52 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc09c149b2f0fbd59ff421e570e0ded105eaef38e0e8a63f6dc51815bd89c55b`  
		Last Modified: Thu, 11 May 2023 22:44:02 GMT  
		Size: 82.5 MB (82537975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:727806fc86a44865004802e93acd1710bd4e1a2d4a672841baa8e8078859a576`  
		Last Modified: Thu, 11 May 2023 22:43:52 GMT  
		Size: 3.5 KB (3530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e48c3a1b1c0f256b54b47204f6cc2c0401bdebacb711ed52bbd3c693bf3c265f`  
		Last Modified: Thu, 11 May 2023 22:43:52 GMT  
		Size: 7.5 KB (7490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891b4c7813158fabf57ee06389cd16b707a41681fb46c611c07efc5a962fd4fe`  
		Last Modified: Thu, 11 May 2023 22:43:52 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4` - linux; ppc64le

```console
$ docker pull mariadb@sha256:567eea9cb1a758a34fe1007701925c6e9fe02e4a498905c14068eef0abbb4c9b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.9 MB (128889553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c78faca279126581362da95a067d1e5fbcbffd4a7a0f83f2f320ebadcc610c0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:36 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:37 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:40 GMT
ADD file:faba3891f58656ec753ba6ca4b63e7c1f27bcd236b665634b05d5bc1b1ceee0a in / 
# Thu, 13 Apr 2023 13:09:40 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:51:07 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 18 Apr 2023 01:51:07 GMT
ENV GOSU_VERSION=1.14
# Tue, 18 Apr 2023 01:51:07 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 18 Apr 2023 01:51:40 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 18 Apr 2023 01:51:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 18 Apr 2023 01:51:42 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 01:54:53 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.4.28 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 18 Apr 2023 01:54:54 GMT
ARG MARIADB_MAJOR=10.4
# Tue, 18 Apr 2023 01:54:54 GMT
ENV MARIADB_MAJOR=10.4
# Tue, 18 Apr 2023 01:54:54 GMT
ARG MARIADB_VERSION=1:10.4.28+maria~ubu2004
# Tue, 18 Apr 2023 01:54:55 GMT
ENV MARIADB_VERSION=1:10.4.28+maria~ubu2004
# Tue, 18 Apr 2023 01:54:55 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.28/repo/ubuntu/ focal main
# Tue, 18 Apr 2023 01:54:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.28/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 18 Apr 2023 01:55:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.28/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 18 Apr 2023 01:55:43 GMT
VOLUME [/var/lib/mysql]
# Tue, 18 Apr 2023 01:55:43 GMT
COPY file:797eec99bf55d77c916c240bbbe1453b1ba37340268a58d0681bf242c87643e5 in /usr/local/bin/healthcheck.sh 
# Tue, 18 Apr 2023 01:55:43 GMT
COPY file:ddd629156267c0caa8ab015799dddda644c1de941e71781975267ef22ad8e315 in /usr/local/bin/ 
# Tue, 18 Apr 2023 01:55:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.28/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 18 Apr 2023 01:55:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 18 Apr 2023 01:55:45 GMT
EXPOSE 3306
# Tue, 18 Apr 2023 01:55:45 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d276072145993a42aed3e2b3e8cd26b6e08aab266d9c9d792ee89b26150681da`  
		Last Modified: Fri, 14 Apr 2023 09:36:00 GMT  
		Size: 33.3 MB (33300980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a173b48773a6ef3fc242fca8702df8e2e401cebf5d6eead9c2e8b679d8f8d57`  
		Last Modified: Tue, 18 Apr 2023 01:57:20 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a525710ca72c2fa19727739f7053c36e5bcc630c19dc9bc5a95f6758c57c071c`  
		Last Modified: Tue, 18 Apr 2023 01:57:22 GMT  
		Size: 7.8 MB (7771035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d96443e2327325857d538e8a99972d2e2cd67c59a3c89cbdfb282cd5b80f87`  
		Last Modified: Tue, 18 Apr 2023 01:57:17 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466e318e3b274927098fd3ca73e4170618bbdafc9cf7cedf017065a9e6fc3d98`  
		Last Modified: Tue, 18 Apr 2023 01:59:09 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf8e45d90f81ac80dc7166e419857bec65e2d1decbd11f066294a859b8447c97`  
		Last Modified: Tue, 18 Apr 2023 01:59:32 GMT  
		Size: 87.8 MB (87804724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b499e0712f84c323f01ecc273808a106479ba46f90f10fbef72093b1ad661d9`  
		Last Modified: Tue, 18 Apr 2023 01:59:09 GMT  
		Size: 3.5 KB (3528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84cd053f1a7667bf4b1eec8af5a2a867595979ecd7e8bc34717949dd8d044f49`  
		Last Modified: Tue, 18 Apr 2023 01:59:09 GMT  
		Size: 6.9 KB (6943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:648f2b9d83283ec720b471a7b7540a085a8a1fe0d73530726405eb161f4fce6c`  
		Last Modified: Tue, 18 Apr 2023 01:59:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4-focal`

```console
$ docker pull mariadb@sha256:52f288566f3b245c1eca47d4afad5783de1ade3d37ccd55a23de8b1eeb0cde70
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:f9f3c4b8fd9dc7717a903c79d847af9c783771b9e0ff3cc4fc983a40e9e5972d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.0 MB (118979095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4192ed85e762898319e99f2255e94c3b752e69ca0d0472ab852fe96ff95906da`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:25:16 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 18 Apr 2023 02:25:16 GMT
ENV GOSU_VERSION=1.14
# Tue, 18 Apr 2023 02:25:17 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 18 Apr 2023 02:25:35 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 18 Apr 2023 02:25:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 18 Apr 2023 02:25:36 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:56:20 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.4.29 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:56:20 GMT
ARG MARIADB_MAJOR=10.4
# Thu, 11 May 2023 22:56:20 GMT
ENV MARIADB_MAJOR=10.4
# Thu, 11 May 2023 22:56:20 GMT
ARG MARIADB_VERSION=1:10.4.29+maria~ubu2004
# Thu, 11 May 2023 22:56:20 GMT
ENV MARIADB_VERSION=1:10.4.29+maria~ubu2004
# Thu, 11 May 2023 22:56:21 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.29/repo/ubuntu/ focal main
# Thu, 11 May 2023 22:56:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.29/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:56:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.29/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:56:43 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:56:43 GMT
COPY file:797eec99bf55d77c916c240bbbe1453b1ba37340268a58d0681bf242c87643e5 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:56:43 GMT
COPY file:c7fbba94efc312a3d294c85b73b08c1a46929becfffb48a76d1ebb6a9b0e785a in /usr/local/bin/ 
# Thu, 11 May 2023 22:56:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.29/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 11 May 2023 22:56:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:56:44 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:56:44 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8bc823a83fdf1329ae53f092d8f3641a60f92ee9f69e8785f5a3fd046eee30f`  
		Last Modified: Tue, 18 Apr 2023 02:28:38 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16685f710f5dded64d14b2537a025d665da5e257c4be3d921737f5f246b0fb9a`  
		Last Modified: Tue, 18 Apr 2023 02:28:40 GMT  
		Size: 7.1 MB (7058710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5660ff630580a5fee05c112e916f0bbca3234820aea68e604a23dba51f23d65`  
		Last Modified: Tue, 18 Apr 2023 02:28:36 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa7ed7a919d7aafc6368987ae312c3e0155c916f465453c2317e8120983bfc9`  
		Last Modified: Thu, 11 May 2023 23:00:43 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09afbb4d4d00f406a83b53c66f338d357a9a6c0ff911cab92f65fe501e3e2fa6`  
		Last Modified: Thu, 11 May 2023 23:00:54 GMT  
		Size: 83.3 MB (83328455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a0e865b236c70e066726e6c46820c043801f6138b60f7df2c11dc68edc9338`  
		Last Modified: Thu, 11 May 2023 23:00:43 GMT  
		Size: 3.5 KB (3530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:464e829278234489f3a326e4a6dd6fa135c3a4e22012311698c1b0f9897a5008`  
		Last Modified: Thu, 11 May 2023 23:00:43 GMT  
		Size: 7.5 KB (7491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfaa3a5c705f9b43c162f83bffc9c80dc6e8002b69f5020d1e2d05de4e6420d1`  
		Last Modified: Thu, 11 May 2023 23:00:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:96652b616dacb0d393fdfd197d12dae5cc57db87fcebbd4be5558996ecdff0c2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.5 MB (116533934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e061cc874d93b0b4f6b6dc368bd507fabc6db71466c7b56fa7625a7cd1cd4416`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:00:47 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 18 Apr 2023 02:00:47 GMT
ENV GOSU_VERSION=1.14
# Tue, 18 Apr 2023 02:00:47 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 18 Apr 2023 02:01:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 18 Apr 2023 02:01:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 18 Apr 2023 02:01:03 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:40:05 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.4.29 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:40:05 GMT
ARG MARIADB_MAJOR=10.4
# Thu, 11 May 2023 22:40:05 GMT
ENV MARIADB_MAJOR=10.4
# Thu, 11 May 2023 22:40:05 GMT
ARG MARIADB_VERSION=1:10.4.29+maria~ubu2004
# Thu, 11 May 2023 22:40:06 GMT
ENV MARIADB_VERSION=1:10.4.29+maria~ubu2004
# Thu, 11 May 2023 22:40:06 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.29/repo/ubuntu/ focal main
# Thu, 11 May 2023 22:40:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.29/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:40:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.29/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:40:26 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:40:26 GMT
COPY file:797eec99bf55d77c916c240bbbe1453b1ba37340268a58d0681bf242c87643e5 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:40:26 GMT
COPY file:c7fbba94efc312a3d294c85b73b08c1a46929becfffb48a76d1ebb6a9b0e785a in /usr/local/bin/ 
# Thu, 11 May 2023 22:40:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.29/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 11 May 2023 22:40:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:40:27 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:40:27 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c227d9b91d2b3157f8d92aefc5896243bf63953d9852e7e73c79ddf26159c9`  
		Last Modified: Tue, 18 Apr 2023 02:03:42 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d0716d74d0fd81781cc567eced35e6c95c70a0e2709606996e1c20c5bda20c`  
		Last Modified: Tue, 18 Apr 2023 02:03:43 GMT  
		Size: 6.8 MB (6786196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673f317ed7421a7da75b11d78e42cce7972ab1b727ed5f537ca1c6f859941bee`  
		Last Modified: Tue, 18 Apr 2023 02:03:40 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c076e8e334d90f19028dad74643678bec03e1045ddbef9716c04adae5a8dc193`  
		Last Modified: Thu, 11 May 2023 22:43:52 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc09c149b2f0fbd59ff421e570e0ded105eaef38e0e8a63f6dc51815bd89c55b`  
		Last Modified: Thu, 11 May 2023 22:44:02 GMT  
		Size: 82.5 MB (82537975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:727806fc86a44865004802e93acd1710bd4e1a2d4a672841baa8e8078859a576`  
		Last Modified: Thu, 11 May 2023 22:43:52 GMT  
		Size: 3.5 KB (3530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e48c3a1b1c0f256b54b47204f6cc2c0401bdebacb711ed52bbd3c693bf3c265f`  
		Last Modified: Thu, 11 May 2023 22:43:52 GMT  
		Size: 7.5 KB (7490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891b4c7813158fabf57ee06389cd16b707a41681fb46c611c07efc5a962fd4fe`  
		Last Modified: Thu, 11 May 2023 22:43:52 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:567eea9cb1a758a34fe1007701925c6e9fe02e4a498905c14068eef0abbb4c9b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.9 MB (128889553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c78faca279126581362da95a067d1e5fbcbffd4a7a0f83f2f320ebadcc610c0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:36 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:37 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:40 GMT
ADD file:faba3891f58656ec753ba6ca4b63e7c1f27bcd236b665634b05d5bc1b1ceee0a in / 
# Thu, 13 Apr 2023 13:09:40 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:51:07 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 18 Apr 2023 01:51:07 GMT
ENV GOSU_VERSION=1.14
# Tue, 18 Apr 2023 01:51:07 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 18 Apr 2023 01:51:40 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 18 Apr 2023 01:51:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 18 Apr 2023 01:51:42 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 01:54:53 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.4.28 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 18 Apr 2023 01:54:54 GMT
ARG MARIADB_MAJOR=10.4
# Tue, 18 Apr 2023 01:54:54 GMT
ENV MARIADB_MAJOR=10.4
# Tue, 18 Apr 2023 01:54:54 GMT
ARG MARIADB_VERSION=1:10.4.28+maria~ubu2004
# Tue, 18 Apr 2023 01:54:55 GMT
ENV MARIADB_VERSION=1:10.4.28+maria~ubu2004
# Tue, 18 Apr 2023 01:54:55 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.28/repo/ubuntu/ focal main
# Tue, 18 Apr 2023 01:54:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.28/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 18 Apr 2023 01:55:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.28/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 18 Apr 2023 01:55:43 GMT
VOLUME [/var/lib/mysql]
# Tue, 18 Apr 2023 01:55:43 GMT
COPY file:797eec99bf55d77c916c240bbbe1453b1ba37340268a58d0681bf242c87643e5 in /usr/local/bin/healthcheck.sh 
# Tue, 18 Apr 2023 01:55:43 GMT
COPY file:ddd629156267c0caa8ab015799dddda644c1de941e71781975267ef22ad8e315 in /usr/local/bin/ 
# Tue, 18 Apr 2023 01:55:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.28/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 18 Apr 2023 01:55:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 18 Apr 2023 01:55:45 GMT
EXPOSE 3306
# Tue, 18 Apr 2023 01:55:45 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d276072145993a42aed3e2b3e8cd26b6e08aab266d9c9d792ee89b26150681da`  
		Last Modified: Fri, 14 Apr 2023 09:36:00 GMT  
		Size: 33.3 MB (33300980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a173b48773a6ef3fc242fca8702df8e2e401cebf5d6eead9c2e8b679d8f8d57`  
		Last Modified: Tue, 18 Apr 2023 01:57:20 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a525710ca72c2fa19727739f7053c36e5bcc630c19dc9bc5a95f6758c57c071c`  
		Last Modified: Tue, 18 Apr 2023 01:57:22 GMT  
		Size: 7.8 MB (7771035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d96443e2327325857d538e8a99972d2e2cd67c59a3c89cbdfb282cd5b80f87`  
		Last Modified: Tue, 18 Apr 2023 01:57:17 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466e318e3b274927098fd3ca73e4170618bbdafc9cf7cedf017065a9e6fc3d98`  
		Last Modified: Tue, 18 Apr 2023 01:59:09 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf8e45d90f81ac80dc7166e419857bec65e2d1decbd11f066294a859b8447c97`  
		Last Modified: Tue, 18 Apr 2023 01:59:32 GMT  
		Size: 87.8 MB (87804724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b499e0712f84c323f01ecc273808a106479ba46f90f10fbef72093b1ad661d9`  
		Last Modified: Tue, 18 Apr 2023 01:59:09 GMT  
		Size: 3.5 KB (3528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84cd053f1a7667bf4b1eec8af5a2a867595979ecd7e8bc34717949dd8d044f49`  
		Last Modified: Tue, 18 Apr 2023 01:59:09 GMT  
		Size: 6.9 KB (6943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:648f2b9d83283ec720b471a7b7540a085a8a1fe0d73530726405eb161f4fce6c`  
		Last Modified: Tue, 18 Apr 2023 01:59:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4.29`

```console
$ docker pull mariadb@sha256:efaaf189d058f51e568deeaec28da814b950a6660016e6faa0ea32c1f16c0e4f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mariadb:10.4.29` - linux; amd64

```console
$ docker pull mariadb@sha256:f9f3c4b8fd9dc7717a903c79d847af9c783771b9e0ff3cc4fc983a40e9e5972d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.0 MB (118979095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4192ed85e762898319e99f2255e94c3b752e69ca0d0472ab852fe96ff95906da`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:25:16 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 18 Apr 2023 02:25:16 GMT
ENV GOSU_VERSION=1.14
# Tue, 18 Apr 2023 02:25:17 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 18 Apr 2023 02:25:35 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 18 Apr 2023 02:25:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 18 Apr 2023 02:25:36 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:56:20 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.4.29 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:56:20 GMT
ARG MARIADB_MAJOR=10.4
# Thu, 11 May 2023 22:56:20 GMT
ENV MARIADB_MAJOR=10.4
# Thu, 11 May 2023 22:56:20 GMT
ARG MARIADB_VERSION=1:10.4.29+maria~ubu2004
# Thu, 11 May 2023 22:56:20 GMT
ENV MARIADB_VERSION=1:10.4.29+maria~ubu2004
# Thu, 11 May 2023 22:56:21 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.29/repo/ubuntu/ focal main
# Thu, 11 May 2023 22:56:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.29/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:56:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.29/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:56:43 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:56:43 GMT
COPY file:797eec99bf55d77c916c240bbbe1453b1ba37340268a58d0681bf242c87643e5 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:56:43 GMT
COPY file:c7fbba94efc312a3d294c85b73b08c1a46929becfffb48a76d1ebb6a9b0e785a in /usr/local/bin/ 
# Thu, 11 May 2023 22:56:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.29/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 11 May 2023 22:56:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:56:44 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:56:44 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8bc823a83fdf1329ae53f092d8f3641a60f92ee9f69e8785f5a3fd046eee30f`  
		Last Modified: Tue, 18 Apr 2023 02:28:38 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16685f710f5dded64d14b2537a025d665da5e257c4be3d921737f5f246b0fb9a`  
		Last Modified: Tue, 18 Apr 2023 02:28:40 GMT  
		Size: 7.1 MB (7058710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5660ff630580a5fee05c112e916f0bbca3234820aea68e604a23dba51f23d65`  
		Last Modified: Tue, 18 Apr 2023 02:28:36 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa7ed7a919d7aafc6368987ae312c3e0155c916f465453c2317e8120983bfc9`  
		Last Modified: Thu, 11 May 2023 23:00:43 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09afbb4d4d00f406a83b53c66f338d357a9a6c0ff911cab92f65fe501e3e2fa6`  
		Last Modified: Thu, 11 May 2023 23:00:54 GMT  
		Size: 83.3 MB (83328455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a0e865b236c70e066726e6c46820c043801f6138b60f7df2c11dc68edc9338`  
		Last Modified: Thu, 11 May 2023 23:00:43 GMT  
		Size: 3.5 KB (3530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:464e829278234489f3a326e4a6dd6fa135c3a4e22012311698c1b0f9897a5008`  
		Last Modified: Thu, 11 May 2023 23:00:43 GMT  
		Size: 7.5 KB (7491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfaa3a5c705f9b43c162f83bffc9c80dc6e8002b69f5020d1e2d05de4e6420d1`  
		Last Modified: Thu, 11 May 2023 23:00:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.29` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:96652b616dacb0d393fdfd197d12dae5cc57db87fcebbd4be5558996ecdff0c2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.5 MB (116533934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e061cc874d93b0b4f6b6dc368bd507fabc6db71466c7b56fa7625a7cd1cd4416`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:00:47 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 18 Apr 2023 02:00:47 GMT
ENV GOSU_VERSION=1.14
# Tue, 18 Apr 2023 02:00:47 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 18 Apr 2023 02:01:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 18 Apr 2023 02:01:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 18 Apr 2023 02:01:03 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:40:05 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.4.29 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:40:05 GMT
ARG MARIADB_MAJOR=10.4
# Thu, 11 May 2023 22:40:05 GMT
ENV MARIADB_MAJOR=10.4
# Thu, 11 May 2023 22:40:05 GMT
ARG MARIADB_VERSION=1:10.4.29+maria~ubu2004
# Thu, 11 May 2023 22:40:06 GMT
ENV MARIADB_VERSION=1:10.4.29+maria~ubu2004
# Thu, 11 May 2023 22:40:06 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.29/repo/ubuntu/ focal main
# Thu, 11 May 2023 22:40:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.29/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:40:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.29/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:40:26 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:40:26 GMT
COPY file:797eec99bf55d77c916c240bbbe1453b1ba37340268a58d0681bf242c87643e5 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:40:26 GMT
COPY file:c7fbba94efc312a3d294c85b73b08c1a46929becfffb48a76d1ebb6a9b0e785a in /usr/local/bin/ 
# Thu, 11 May 2023 22:40:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.29/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 11 May 2023 22:40:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:40:27 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:40:27 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c227d9b91d2b3157f8d92aefc5896243bf63953d9852e7e73c79ddf26159c9`  
		Last Modified: Tue, 18 Apr 2023 02:03:42 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d0716d74d0fd81781cc567eced35e6c95c70a0e2709606996e1c20c5bda20c`  
		Last Modified: Tue, 18 Apr 2023 02:03:43 GMT  
		Size: 6.8 MB (6786196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673f317ed7421a7da75b11d78e42cce7972ab1b727ed5f537ca1c6f859941bee`  
		Last Modified: Tue, 18 Apr 2023 02:03:40 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c076e8e334d90f19028dad74643678bec03e1045ddbef9716c04adae5a8dc193`  
		Last Modified: Thu, 11 May 2023 22:43:52 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc09c149b2f0fbd59ff421e570e0ded105eaef38e0e8a63f6dc51815bd89c55b`  
		Last Modified: Thu, 11 May 2023 22:44:02 GMT  
		Size: 82.5 MB (82537975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:727806fc86a44865004802e93acd1710bd4e1a2d4a672841baa8e8078859a576`  
		Last Modified: Thu, 11 May 2023 22:43:52 GMT  
		Size: 3.5 KB (3530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e48c3a1b1c0f256b54b47204f6cc2c0401bdebacb711ed52bbd3c693bf3c265f`  
		Last Modified: Thu, 11 May 2023 22:43:52 GMT  
		Size: 7.5 KB (7490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891b4c7813158fabf57ee06389cd16b707a41681fb46c611c07efc5a962fd4fe`  
		Last Modified: Thu, 11 May 2023 22:43:52 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4.29-focal`

```console
$ docker pull mariadb@sha256:efaaf189d058f51e568deeaec28da814b950a6660016e6faa0ea32c1f16c0e4f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mariadb:10.4.29-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:f9f3c4b8fd9dc7717a903c79d847af9c783771b9e0ff3cc4fc983a40e9e5972d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.0 MB (118979095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4192ed85e762898319e99f2255e94c3b752e69ca0d0472ab852fe96ff95906da`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:25:16 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 18 Apr 2023 02:25:16 GMT
ENV GOSU_VERSION=1.14
# Tue, 18 Apr 2023 02:25:17 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 18 Apr 2023 02:25:35 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 18 Apr 2023 02:25:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 18 Apr 2023 02:25:36 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:56:20 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.4.29 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:56:20 GMT
ARG MARIADB_MAJOR=10.4
# Thu, 11 May 2023 22:56:20 GMT
ENV MARIADB_MAJOR=10.4
# Thu, 11 May 2023 22:56:20 GMT
ARG MARIADB_VERSION=1:10.4.29+maria~ubu2004
# Thu, 11 May 2023 22:56:20 GMT
ENV MARIADB_VERSION=1:10.4.29+maria~ubu2004
# Thu, 11 May 2023 22:56:21 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.29/repo/ubuntu/ focal main
# Thu, 11 May 2023 22:56:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.29/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:56:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.29/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:56:43 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:56:43 GMT
COPY file:797eec99bf55d77c916c240bbbe1453b1ba37340268a58d0681bf242c87643e5 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:56:43 GMT
COPY file:c7fbba94efc312a3d294c85b73b08c1a46929becfffb48a76d1ebb6a9b0e785a in /usr/local/bin/ 
# Thu, 11 May 2023 22:56:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.29/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 11 May 2023 22:56:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:56:44 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:56:44 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8bc823a83fdf1329ae53f092d8f3641a60f92ee9f69e8785f5a3fd046eee30f`  
		Last Modified: Tue, 18 Apr 2023 02:28:38 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16685f710f5dded64d14b2537a025d665da5e257c4be3d921737f5f246b0fb9a`  
		Last Modified: Tue, 18 Apr 2023 02:28:40 GMT  
		Size: 7.1 MB (7058710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5660ff630580a5fee05c112e916f0bbca3234820aea68e604a23dba51f23d65`  
		Last Modified: Tue, 18 Apr 2023 02:28:36 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa7ed7a919d7aafc6368987ae312c3e0155c916f465453c2317e8120983bfc9`  
		Last Modified: Thu, 11 May 2023 23:00:43 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09afbb4d4d00f406a83b53c66f338d357a9a6c0ff911cab92f65fe501e3e2fa6`  
		Last Modified: Thu, 11 May 2023 23:00:54 GMT  
		Size: 83.3 MB (83328455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a0e865b236c70e066726e6c46820c043801f6138b60f7df2c11dc68edc9338`  
		Last Modified: Thu, 11 May 2023 23:00:43 GMT  
		Size: 3.5 KB (3530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:464e829278234489f3a326e4a6dd6fa135c3a4e22012311698c1b0f9897a5008`  
		Last Modified: Thu, 11 May 2023 23:00:43 GMT  
		Size: 7.5 KB (7491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfaa3a5c705f9b43c162f83bffc9c80dc6e8002b69f5020d1e2d05de4e6420d1`  
		Last Modified: Thu, 11 May 2023 23:00:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.29-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:96652b616dacb0d393fdfd197d12dae5cc57db87fcebbd4be5558996ecdff0c2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.5 MB (116533934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e061cc874d93b0b4f6b6dc368bd507fabc6db71466c7b56fa7625a7cd1cd4416`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:00:47 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 18 Apr 2023 02:00:47 GMT
ENV GOSU_VERSION=1.14
# Tue, 18 Apr 2023 02:00:47 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 18 Apr 2023 02:01:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 18 Apr 2023 02:01:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 18 Apr 2023 02:01:03 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:40:05 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.4.29 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:40:05 GMT
ARG MARIADB_MAJOR=10.4
# Thu, 11 May 2023 22:40:05 GMT
ENV MARIADB_MAJOR=10.4
# Thu, 11 May 2023 22:40:05 GMT
ARG MARIADB_VERSION=1:10.4.29+maria~ubu2004
# Thu, 11 May 2023 22:40:06 GMT
ENV MARIADB_VERSION=1:10.4.29+maria~ubu2004
# Thu, 11 May 2023 22:40:06 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.29/repo/ubuntu/ focal main
# Thu, 11 May 2023 22:40:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.29/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:40:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.29/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:40:26 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:40:26 GMT
COPY file:797eec99bf55d77c916c240bbbe1453b1ba37340268a58d0681bf242c87643e5 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:40:26 GMT
COPY file:c7fbba94efc312a3d294c85b73b08c1a46929becfffb48a76d1ebb6a9b0e785a in /usr/local/bin/ 
# Thu, 11 May 2023 22:40:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.29/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 11 May 2023 22:40:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:40:27 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:40:27 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c227d9b91d2b3157f8d92aefc5896243bf63953d9852e7e73c79ddf26159c9`  
		Last Modified: Tue, 18 Apr 2023 02:03:42 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d0716d74d0fd81781cc567eced35e6c95c70a0e2709606996e1c20c5bda20c`  
		Last Modified: Tue, 18 Apr 2023 02:03:43 GMT  
		Size: 6.8 MB (6786196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673f317ed7421a7da75b11d78e42cce7972ab1b727ed5f537ca1c6f859941bee`  
		Last Modified: Tue, 18 Apr 2023 02:03:40 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c076e8e334d90f19028dad74643678bec03e1045ddbef9716c04adae5a8dc193`  
		Last Modified: Thu, 11 May 2023 22:43:52 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc09c149b2f0fbd59ff421e570e0ded105eaef38e0e8a63f6dc51815bd89c55b`  
		Last Modified: Thu, 11 May 2023 22:44:02 GMT  
		Size: 82.5 MB (82537975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:727806fc86a44865004802e93acd1710bd4e1a2d4a672841baa8e8078859a576`  
		Last Modified: Thu, 11 May 2023 22:43:52 GMT  
		Size: 3.5 KB (3530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e48c3a1b1c0f256b54b47204f6cc2c0401bdebacb711ed52bbd3c693bf3c265f`  
		Last Modified: Thu, 11 May 2023 22:43:52 GMT  
		Size: 7.5 KB (7490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891b4c7813158fabf57ee06389cd16b707a41681fb46c611c07efc5a962fd4fe`  
		Last Modified: Thu, 11 May 2023 22:43:52 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5`

```console
$ docker pull mariadb@sha256:a45e4916fd632b65b6d401058f9efb43f694591e687272e3f0fa835ee33f8513
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.5` - linux; amd64

```console
$ docker pull mariadb@sha256:0a9681b82efd8cb4e19d0931d2d597c03c4deb453004e9ccb6488bf33edfbf84
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.2 MB (121244540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76a5b2d8081aa97ba3e19d6256070d7c4fa9408a735c319dbbbba751be35df3a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:25:16 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 18 Apr 2023 02:25:16 GMT
ENV GOSU_VERSION=1.14
# Tue, 18 Apr 2023 02:25:17 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 18 Apr 2023 02:25:35 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 18 Apr 2023 02:25:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 18 Apr 2023 02:25:36 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:55:56 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.5.20 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:55:57 GMT
ARG MARIADB_MAJOR=10.5
# Thu, 11 May 2023 22:55:57 GMT
ENV MARIADB_MAJOR=10.5
# Thu, 11 May 2023 22:55:57 GMT
ARG MARIADB_VERSION=1:10.5.20+maria~ubu2004
# Thu, 11 May 2023 22:55:57 GMT
ENV MARIADB_VERSION=1:10.5.20+maria~ubu2004
# Thu, 11 May 2023 22:55:57 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.20/repo/ubuntu/ focal main
# Thu, 11 May 2023 22:55:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.20/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:56:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.20/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:56:18 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:56:18 GMT
COPY file:797eec99bf55d77c916c240bbbe1453b1ba37340268a58d0681bf242c87643e5 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:56:18 GMT
COPY file:e632ff8de201e30e52a350b1db7d277c1a9e5d053f830a65d1762771a6554a01 in /usr/local/bin/ 
# Thu, 11 May 2023 22:56:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:56:18 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:56:18 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8bc823a83fdf1329ae53f092d8f3641a60f92ee9f69e8785f5a3fd046eee30f`  
		Last Modified: Tue, 18 Apr 2023 02:28:38 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16685f710f5dded64d14b2537a025d665da5e257c4be3d921737f5f246b0fb9a`  
		Last Modified: Tue, 18 Apr 2023 02:28:40 GMT  
		Size: 7.1 MB (7058710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5660ff630580a5fee05c112e916f0bbca3234820aea68e604a23dba51f23d65`  
		Last Modified: Tue, 18 Apr 2023 02:28:36 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb5880d2d3596aabd567b0ab0fab78495b9da6a156f37d8b56a9e97cb0585e38`  
		Last Modified: Thu, 11 May 2023 23:00:18 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baf131972ef1c5c9bcc6b3bbba83d5446f291b8c41882f2c798e2ee639e143fb`  
		Last Modified: Thu, 11 May 2023 23:00:30 GMT  
		Size: 85.6 MB (85594026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2969c5907ed889bece6adf3b46b510705cfb7e14ff05653411f94e475514a62b`  
		Last Modified: Thu, 11 May 2023 23:00:18 GMT  
		Size: 3.5 KB (3530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:178375b1f8ced0ce2951db2d0c117891276795f7f37b2e3261d49dcd93ae8038`  
		Last Modified: Thu, 11 May 2023 23:00:18 GMT  
		Size: 7.5 KB (7487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:c5b30b0dd3e2264a31ee6e0b066c9f23cdcdce5ad9062186ff25f00998c0b3eb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.7 MB (118711396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ae32401c9ae8e249487985100cf7d9151d589739bb4fe761d25042652c48e75`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:00:47 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 18 Apr 2023 02:00:47 GMT
ENV GOSU_VERSION=1.14
# Tue, 18 Apr 2023 02:00:47 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 18 Apr 2023 02:01:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 18 Apr 2023 02:01:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 18 Apr 2023 02:01:03 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:39:42 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.5.20 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:39:42 GMT
ARG MARIADB_MAJOR=10.5
# Thu, 11 May 2023 22:39:42 GMT
ENV MARIADB_MAJOR=10.5
# Thu, 11 May 2023 22:39:42 GMT
ARG MARIADB_VERSION=1:10.5.20+maria~ubu2004
# Thu, 11 May 2023 22:39:43 GMT
ENV MARIADB_VERSION=1:10.5.20+maria~ubu2004
# Thu, 11 May 2023 22:39:43 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.20/repo/ubuntu/ focal main
# Thu, 11 May 2023 22:39:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.20/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:40:00 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.20/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:40:01 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:40:01 GMT
COPY file:797eec99bf55d77c916c240bbbe1453b1ba37340268a58d0681bf242c87643e5 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:40:02 GMT
COPY file:e632ff8de201e30e52a350b1db7d277c1a9e5d053f830a65d1762771a6554a01 in /usr/local/bin/ 
# Thu, 11 May 2023 22:40:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:40:02 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:40:02 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c227d9b91d2b3157f8d92aefc5896243bf63953d9852e7e73c79ddf26159c9`  
		Last Modified: Tue, 18 Apr 2023 02:03:42 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d0716d74d0fd81781cc567eced35e6c95c70a0e2709606996e1c20c5bda20c`  
		Last Modified: Tue, 18 Apr 2023 02:03:43 GMT  
		Size: 6.8 MB (6786196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673f317ed7421a7da75b11d78e42cce7972ab1b727ed5f537ca1c6f859941bee`  
		Last Modified: Tue, 18 Apr 2023 02:03:40 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98228e73f9a07adba2d89ff5cc45438491b85ab6774a546e35a764749e150ce5`  
		Last Modified: Thu, 11 May 2023 22:43:31 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f32cc43641b887abe1278d424bf6244c03e6cd542757e4d5a9df7ddaf1440155`  
		Last Modified: Thu, 11 May 2023 22:43:40 GMT  
		Size: 84.7 MB (84715562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d25fb18406a930eb0603235fa042b51ccbefe4b82637663368aab16e85a766`  
		Last Modified: Thu, 11 May 2023 22:43:31 GMT  
		Size: 3.5 KB (3531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842adf5985b6c2d1aee37edf536230abcde66ca70ec1f5d78d66b7dba7140bd8`  
		Last Modified: Thu, 11 May 2023 22:43:31 GMT  
		Size: 7.5 KB (7485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; ppc64le

```console
$ docker pull mariadb@sha256:5e73dbd6a685dea75f9497fb9554fe46834c268b8c46664e254f6fc36fec0b1b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.1 MB (131132288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10d683fef680c984209568ab0c76815c6da23d0a9e2f0427a2318813c3a07a8d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:36 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:37 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:40 GMT
ADD file:faba3891f58656ec753ba6ca4b63e7c1f27bcd236b665634b05d5bc1b1ceee0a in / 
# Thu, 13 Apr 2023 13:09:40 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:51:07 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 18 Apr 2023 01:51:07 GMT
ENV GOSU_VERSION=1.14
# Tue, 18 Apr 2023 01:51:07 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 18 Apr 2023 01:51:40 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 18 Apr 2023 01:51:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 18 Apr 2023 01:51:42 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 01:53:43 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.5.19 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 18 Apr 2023 01:53:44 GMT
ARG MARIADB_MAJOR=10.5
# Tue, 18 Apr 2023 01:53:44 GMT
ENV MARIADB_MAJOR=10.5
# Tue, 18 Apr 2023 01:53:44 GMT
ARG MARIADB_VERSION=1:10.5.19+maria~ubu2004
# Tue, 18 Apr 2023 01:53:44 GMT
ENV MARIADB_VERSION=1:10.5.19+maria~ubu2004
# Tue, 18 Apr 2023 01:53:45 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.19/repo/ubuntu/ focal main
# Tue, 18 Apr 2023 01:53:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.19/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 18 Apr 2023 01:54:35 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.19/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 18 Apr 2023 01:54:39 GMT
VOLUME [/var/lib/mysql]
# Tue, 18 Apr 2023 01:54:39 GMT
COPY file:797eec99bf55d77c916c240bbbe1453b1ba37340268a58d0681bf242c87643e5 in /usr/local/bin/healthcheck.sh 
# Tue, 18 Apr 2023 01:54:39 GMT
COPY file:ddd629156267c0caa8ab015799dddda644c1de941e71781975267ef22ad8e315 in /usr/local/bin/ 
# Tue, 18 Apr 2023 01:54:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 18 Apr 2023 01:54:40 GMT
EXPOSE 3306
# Tue, 18 Apr 2023 01:54:40 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d276072145993a42aed3e2b3e8cd26b6e08aab266d9c9d792ee89b26150681da`  
		Last Modified: Fri, 14 Apr 2023 09:36:00 GMT  
		Size: 33.3 MB (33300980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a173b48773a6ef3fc242fca8702df8e2e401cebf5d6eead9c2e8b679d8f8d57`  
		Last Modified: Tue, 18 Apr 2023 01:57:20 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a525710ca72c2fa19727739f7053c36e5bcc630c19dc9bc5a95f6758c57c071c`  
		Last Modified: Tue, 18 Apr 2023 01:57:22 GMT  
		Size: 7.8 MB (7771035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d96443e2327325857d538e8a99972d2e2cd67c59a3c89cbdfb282cd5b80f87`  
		Last Modified: Tue, 18 Apr 2023 01:57:17 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88260df5f4be201ff1c18b9414669b8a9a77ded7617685dd1f2501924a10aec8`  
		Last Modified: Tue, 18 Apr 2023 01:58:32 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f7de1c204d4fecc3382a47dd7f72da76d628091c2e15bcbc7689a237104b00`  
		Last Modified: Tue, 18 Apr 2023 01:58:55 GMT  
		Size: 90.0 MB (90047584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a519e128c0a7a2470abf3596536e33a68fe66ae8f9a412b21ee80971286c488d`  
		Last Modified: Tue, 18 Apr 2023 01:58:32 GMT  
		Size: 3.5 KB (3527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef3884cc311713347b382b33af979d846644ace8193bda66a6e89b026b4d9da`  
		Last Modified: Tue, 18 Apr 2023 01:58:32 GMT  
		Size: 6.9 KB (6942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; s390x

```console
$ docker pull mariadb@sha256:6b37574e1613dd098d5b971db31c4144c67b59b0d7d888c8bfcbd35b8a5f88bb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.5 MB (120465542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb11b06ec287a697029397ceeb83c7e1d270663d1bd8de68f78b9bd067ab5649`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:35 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:35 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:35 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:35 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:37 GMT
ADD file:44c66c03ba0afcc05de1b2078f83e8bfe04706b31491fcd3fdd93cfc88d5f06c in / 
# Thu, 13 Apr 2023 13:09:37 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 16:33:09 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 18 Apr 2023 16:33:09 GMT
ENV GOSU_VERSION=1.14
# Tue, 18 Apr 2023 16:33:09 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 18 Apr 2023 16:33:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 18 Apr 2023 16:33:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 18 Apr 2023 16:33:38 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 16:34:42 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.5.19 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 18 Apr 2023 16:34:43 GMT
ARG MARIADB_MAJOR=10.5
# Tue, 18 Apr 2023 16:34:43 GMT
ENV MARIADB_MAJOR=10.5
# Tue, 18 Apr 2023 16:34:43 GMT
ARG MARIADB_VERSION=1:10.5.19+maria~ubu2004
# Tue, 18 Apr 2023 16:34:43 GMT
ENV MARIADB_VERSION=1:10.5.19+maria~ubu2004
# Tue, 18 Apr 2023 16:34:43 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.19/repo/ubuntu/ focal main
# Tue, 18 Apr 2023 16:34:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.19/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 18 Apr 2023 16:35:01 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.19/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 18 Apr 2023 16:35:05 GMT
VOLUME [/var/lib/mysql]
# Tue, 18 Apr 2023 16:35:05 GMT
COPY file:797eec99bf55d77c916c240bbbe1453b1ba37340268a58d0681bf242c87643e5 in /usr/local/bin/healthcheck.sh 
# Tue, 18 Apr 2023 16:35:05 GMT
COPY file:ddd629156267c0caa8ab015799dddda644c1de941e71781975267ef22ad8e315 in /usr/local/bin/ 
# Tue, 18 Apr 2023 16:35:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 18 Apr 2023 16:35:05 GMT
EXPOSE 3306
# Tue, 18 Apr 2023 16:35:05 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:f11b609b1d63f2d37c0e3789823e7a7e62a078bddca7c46da8602655989c62d9`  
		Last Modified: Fri, 14 Apr 2023 09:38:39 GMT  
		Size: 27.0 MB (27016370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184f14ef3f9ff48410469ecdcf8d758d86092d41a732adcdcba4969b30b63272`  
		Last Modified: Tue, 18 Apr 2023 16:35:26 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17716ec3f50471a011fcf739f209ad3c5df9a3f808a38dc40e4079efb79e4d41`  
		Last Modified: Tue, 18 Apr 2023 16:35:26 GMT  
		Size: 6.6 MB (6609307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:235b8a8d1aa17dd5727bbfb2d4fb8393a20bc83e8f81325993515261956592de`  
		Last Modified: Tue, 18 Apr 2023 16:35:24 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:879f065971bfdade7d296be6d2402cab9d929e84a377f14b2147ca2ced5748a4`  
		Last Modified: Tue, 18 Apr 2023 16:36:07 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db25963f09a210d4d455d167e574b5fdc39d0793a1f4d2fada531c8112c0983`  
		Last Modified: Tue, 18 Apr 2023 16:36:19 GMT  
		Size: 86.8 MB (86827163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0344a26c0d5fba1c770c4a899e4e4dbd3e0f861c353050dc6e483dea5f04dfeb`  
		Last Modified: Tue, 18 Apr 2023 16:36:07 GMT  
		Size: 3.5 KB (3530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ff79e081e64c85ff129c0625c481c581c86d440e3031c18ea91264ecaaf506`  
		Last Modified: Tue, 18 Apr 2023 16:36:07 GMT  
		Size: 6.9 KB (6943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5-focal`

```console
$ docker pull mariadb@sha256:a45e4916fd632b65b6d401058f9efb43f694591e687272e3f0fa835ee33f8513
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.5-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:0a9681b82efd8cb4e19d0931d2d597c03c4deb453004e9ccb6488bf33edfbf84
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.2 MB (121244540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76a5b2d8081aa97ba3e19d6256070d7c4fa9408a735c319dbbbba751be35df3a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:25:16 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 18 Apr 2023 02:25:16 GMT
ENV GOSU_VERSION=1.14
# Tue, 18 Apr 2023 02:25:17 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 18 Apr 2023 02:25:35 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 18 Apr 2023 02:25:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 18 Apr 2023 02:25:36 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:55:56 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.5.20 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:55:57 GMT
ARG MARIADB_MAJOR=10.5
# Thu, 11 May 2023 22:55:57 GMT
ENV MARIADB_MAJOR=10.5
# Thu, 11 May 2023 22:55:57 GMT
ARG MARIADB_VERSION=1:10.5.20+maria~ubu2004
# Thu, 11 May 2023 22:55:57 GMT
ENV MARIADB_VERSION=1:10.5.20+maria~ubu2004
# Thu, 11 May 2023 22:55:57 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.20/repo/ubuntu/ focal main
# Thu, 11 May 2023 22:55:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.20/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:56:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.20/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:56:18 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:56:18 GMT
COPY file:797eec99bf55d77c916c240bbbe1453b1ba37340268a58d0681bf242c87643e5 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:56:18 GMT
COPY file:e632ff8de201e30e52a350b1db7d277c1a9e5d053f830a65d1762771a6554a01 in /usr/local/bin/ 
# Thu, 11 May 2023 22:56:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:56:18 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:56:18 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8bc823a83fdf1329ae53f092d8f3641a60f92ee9f69e8785f5a3fd046eee30f`  
		Last Modified: Tue, 18 Apr 2023 02:28:38 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16685f710f5dded64d14b2537a025d665da5e257c4be3d921737f5f246b0fb9a`  
		Last Modified: Tue, 18 Apr 2023 02:28:40 GMT  
		Size: 7.1 MB (7058710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5660ff630580a5fee05c112e916f0bbca3234820aea68e604a23dba51f23d65`  
		Last Modified: Tue, 18 Apr 2023 02:28:36 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb5880d2d3596aabd567b0ab0fab78495b9da6a156f37d8b56a9e97cb0585e38`  
		Last Modified: Thu, 11 May 2023 23:00:18 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baf131972ef1c5c9bcc6b3bbba83d5446f291b8c41882f2c798e2ee639e143fb`  
		Last Modified: Thu, 11 May 2023 23:00:30 GMT  
		Size: 85.6 MB (85594026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2969c5907ed889bece6adf3b46b510705cfb7e14ff05653411f94e475514a62b`  
		Last Modified: Thu, 11 May 2023 23:00:18 GMT  
		Size: 3.5 KB (3530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:178375b1f8ced0ce2951db2d0c117891276795f7f37b2e3261d49dcd93ae8038`  
		Last Modified: Thu, 11 May 2023 23:00:18 GMT  
		Size: 7.5 KB (7487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:c5b30b0dd3e2264a31ee6e0b066c9f23cdcdce5ad9062186ff25f00998c0b3eb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.7 MB (118711396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ae32401c9ae8e249487985100cf7d9151d589739bb4fe761d25042652c48e75`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:00:47 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 18 Apr 2023 02:00:47 GMT
ENV GOSU_VERSION=1.14
# Tue, 18 Apr 2023 02:00:47 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 18 Apr 2023 02:01:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 18 Apr 2023 02:01:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 18 Apr 2023 02:01:03 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:39:42 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.5.20 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:39:42 GMT
ARG MARIADB_MAJOR=10.5
# Thu, 11 May 2023 22:39:42 GMT
ENV MARIADB_MAJOR=10.5
# Thu, 11 May 2023 22:39:42 GMT
ARG MARIADB_VERSION=1:10.5.20+maria~ubu2004
# Thu, 11 May 2023 22:39:43 GMT
ENV MARIADB_VERSION=1:10.5.20+maria~ubu2004
# Thu, 11 May 2023 22:39:43 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.20/repo/ubuntu/ focal main
# Thu, 11 May 2023 22:39:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.20/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:40:00 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.20/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:40:01 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:40:01 GMT
COPY file:797eec99bf55d77c916c240bbbe1453b1ba37340268a58d0681bf242c87643e5 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:40:02 GMT
COPY file:e632ff8de201e30e52a350b1db7d277c1a9e5d053f830a65d1762771a6554a01 in /usr/local/bin/ 
# Thu, 11 May 2023 22:40:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:40:02 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:40:02 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c227d9b91d2b3157f8d92aefc5896243bf63953d9852e7e73c79ddf26159c9`  
		Last Modified: Tue, 18 Apr 2023 02:03:42 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d0716d74d0fd81781cc567eced35e6c95c70a0e2709606996e1c20c5bda20c`  
		Last Modified: Tue, 18 Apr 2023 02:03:43 GMT  
		Size: 6.8 MB (6786196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673f317ed7421a7da75b11d78e42cce7972ab1b727ed5f537ca1c6f859941bee`  
		Last Modified: Tue, 18 Apr 2023 02:03:40 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98228e73f9a07adba2d89ff5cc45438491b85ab6774a546e35a764749e150ce5`  
		Last Modified: Thu, 11 May 2023 22:43:31 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f32cc43641b887abe1278d424bf6244c03e6cd542757e4d5a9df7ddaf1440155`  
		Last Modified: Thu, 11 May 2023 22:43:40 GMT  
		Size: 84.7 MB (84715562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d25fb18406a930eb0603235fa042b51ccbefe4b82637663368aab16e85a766`  
		Last Modified: Thu, 11 May 2023 22:43:31 GMT  
		Size: 3.5 KB (3531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842adf5985b6c2d1aee37edf536230abcde66ca70ec1f5d78d66b7dba7140bd8`  
		Last Modified: Thu, 11 May 2023 22:43:31 GMT  
		Size: 7.5 KB (7485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:5e73dbd6a685dea75f9497fb9554fe46834c268b8c46664e254f6fc36fec0b1b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.1 MB (131132288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10d683fef680c984209568ab0c76815c6da23d0a9e2f0427a2318813c3a07a8d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:36 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:37 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:40 GMT
ADD file:faba3891f58656ec753ba6ca4b63e7c1f27bcd236b665634b05d5bc1b1ceee0a in / 
# Thu, 13 Apr 2023 13:09:40 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:51:07 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 18 Apr 2023 01:51:07 GMT
ENV GOSU_VERSION=1.14
# Tue, 18 Apr 2023 01:51:07 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 18 Apr 2023 01:51:40 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 18 Apr 2023 01:51:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 18 Apr 2023 01:51:42 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 01:53:43 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.5.19 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 18 Apr 2023 01:53:44 GMT
ARG MARIADB_MAJOR=10.5
# Tue, 18 Apr 2023 01:53:44 GMT
ENV MARIADB_MAJOR=10.5
# Tue, 18 Apr 2023 01:53:44 GMT
ARG MARIADB_VERSION=1:10.5.19+maria~ubu2004
# Tue, 18 Apr 2023 01:53:44 GMT
ENV MARIADB_VERSION=1:10.5.19+maria~ubu2004
# Tue, 18 Apr 2023 01:53:45 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.19/repo/ubuntu/ focal main
# Tue, 18 Apr 2023 01:53:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.19/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 18 Apr 2023 01:54:35 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.19/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 18 Apr 2023 01:54:39 GMT
VOLUME [/var/lib/mysql]
# Tue, 18 Apr 2023 01:54:39 GMT
COPY file:797eec99bf55d77c916c240bbbe1453b1ba37340268a58d0681bf242c87643e5 in /usr/local/bin/healthcheck.sh 
# Tue, 18 Apr 2023 01:54:39 GMT
COPY file:ddd629156267c0caa8ab015799dddda644c1de941e71781975267ef22ad8e315 in /usr/local/bin/ 
# Tue, 18 Apr 2023 01:54:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 18 Apr 2023 01:54:40 GMT
EXPOSE 3306
# Tue, 18 Apr 2023 01:54:40 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d276072145993a42aed3e2b3e8cd26b6e08aab266d9c9d792ee89b26150681da`  
		Last Modified: Fri, 14 Apr 2023 09:36:00 GMT  
		Size: 33.3 MB (33300980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a173b48773a6ef3fc242fca8702df8e2e401cebf5d6eead9c2e8b679d8f8d57`  
		Last Modified: Tue, 18 Apr 2023 01:57:20 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a525710ca72c2fa19727739f7053c36e5bcc630c19dc9bc5a95f6758c57c071c`  
		Last Modified: Tue, 18 Apr 2023 01:57:22 GMT  
		Size: 7.8 MB (7771035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d96443e2327325857d538e8a99972d2e2cd67c59a3c89cbdfb282cd5b80f87`  
		Last Modified: Tue, 18 Apr 2023 01:57:17 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88260df5f4be201ff1c18b9414669b8a9a77ded7617685dd1f2501924a10aec8`  
		Last Modified: Tue, 18 Apr 2023 01:58:32 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f7de1c204d4fecc3382a47dd7f72da76d628091c2e15bcbc7689a237104b00`  
		Last Modified: Tue, 18 Apr 2023 01:58:55 GMT  
		Size: 90.0 MB (90047584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a519e128c0a7a2470abf3596536e33a68fe66ae8f9a412b21ee80971286c488d`  
		Last Modified: Tue, 18 Apr 2023 01:58:32 GMT  
		Size: 3.5 KB (3527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef3884cc311713347b382b33af979d846644ace8193bda66a6e89b026b4d9da`  
		Last Modified: Tue, 18 Apr 2023 01:58:32 GMT  
		Size: 6.9 KB (6942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:6b37574e1613dd098d5b971db31c4144c67b59b0d7d888c8bfcbd35b8a5f88bb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.5 MB (120465542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb11b06ec287a697029397ceeb83c7e1d270663d1bd8de68f78b9bd067ab5649`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:35 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:35 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:35 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:35 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:37 GMT
ADD file:44c66c03ba0afcc05de1b2078f83e8bfe04706b31491fcd3fdd93cfc88d5f06c in / 
# Thu, 13 Apr 2023 13:09:37 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 16:33:09 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 18 Apr 2023 16:33:09 GMT
ENV GOSU_VERSION=1.14
# Tue, 18 Apr 2023 16:33:09 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 18 Apr 2023 16:33:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 18 Apr 2023 16:33:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 18 Apr 2023 16:33:38 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 16:34:42 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.5.19 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 18 Apr 2023 16:34:43 GMT
ARG MARIADB_MAJOR=10.5
# Tue, 18 Apr 2023 16:34:43 GMT
ENV MARIADB_MAJOR=10.5
# Tue, 18 Apr 2023 16:34:43 GMT
ARG MARIADB_VERSION=1:10.5.19+maria~ubu2004
# Tue, 18 Apr 2023 16:34:43 GMT
ENV MARIADB_VERSION=1:10.5.19+maria~ubu2004
# Tue, 18 Apr 2023 16:34:43 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.19/repo/ubuntu/ focal main
# Tue, 18 Apr 2023 16:34:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.19/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 18 Apr 2023 16:35:01 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.19/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 18 Apr 2023 16:35:05 GMT
VOLUME [/var/lib/mysql]
# Tue, 18 Apr 2023 16:35:05 GMT
COPY file:797eec99bf55d77c916c240bbbe1453b1ba37340268a58d0681bf242c87643e5 in /usr/local/bin/healthcheck.sh 
# Tue, 18 Apr 2023 16:35:05 GMT
COPY file:ddd629156267c0caa8ab015799dddda644c1de941e71781975267ef22ad8e315 in /usr/local/bin/ 
# Tue, 18 Apr 2023 16:35:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 18 Apr 2023 16:35:05 GMT
EXPOSE 3306
# Tue, 18 Apr 2023 16:35:05 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:f11b609b1d63f2d37c0e3789823e7a7e62a078bddca7c46da8602655989c62d9`  
		Last Modified: Fri, 14 Apr 2023 09:38:39 GMT  
		Size: 27.0 MB (27016370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184f14ef3f9ff48410469ecdcf8d758d86092d41a732adcdcba4969b30b63272`  
		Last Modified: Tue, 18 Apr 2023 16:35:26 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17716ec3f50471a011fcf739f209ad3c5df9a3f808a38dc40e4079efb79e4d41`  
		Last Modified: Tue, 18 Apr 2023 16:35:26 GMT  
		Size: 6.6 MB (6609307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:235b8a8d1aa17dd5727bbfb2d4fb8393a20bc83e8f81325993515261956592de`  
		Last Modified: Tue, 18 Apr 2023 16:35:24 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:879f065971bfdade7d296be6d2402cab9d929e84a377f14b2147ca2ced5748a4`  
		Last Modified: Tue, 18 Apr 2023 16:36:07 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db25963f09a210d4d455d167e574b5fdc39d0793a1f4d2fada531c8112c0983`  
		Last Modified: Tue, 18 Apr 2023 16:36:19 GMT  
		Size: 86.8 MB (86827163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0344a26c0d5fba1c770c4a899e4e4dbd3e0f861c353050dc6e483dea5f04dfeb`  
		Last Modified: Tue, 18 Apr 2023 16:36:07 GMT  
		Size: 3.5 KB (3530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ff79e081e64c85ff129c0625c481c581c86d440e3031c18ea91264ecaaf506`  
		Last Modified: Tue, 18 Apr 2023 16:36:07 GMT  
		Size: 6.9 KB (6943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5.20`

```console
$ docker pull mariadb@sha256:f75675445a176589ccd13131c1dfc443d7f2017692cb7b536cb1c293072f4f96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mariadb:10.5.20` - linux; amd64

```console
$ docker pull mariadb@sha256:0a9681b82efd8cb4e19d0931d2d597c03c4deb453004e9ccb6488bf33edfbf84
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.2 MB (121244540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76a5b2d8081aa97ba3e19d6256070d7c4fa9408a735c319dbbbba751be35df3a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:25:16 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 18 Apr 2023 02:25:16 GMT
ENV GOSU_VERSION=1.14
# Tue, 18 Apr 2023 02:25:17 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 18 Apr 2023 02:25:35 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 18 Apr 2023 02:25:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 18 Apr 2023 02:25:36 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:55:56 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.5.20 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:55:57 GMT
ARG MARIADB_MAJOR=10.5
# Thu, 11 May 2023 22:55:57 GMT
ENV MARIADB_MAJOR=10.5
# Thu, 11 May 2023 22:55:57 GMT
ARG MARIADB_VERSION=1:10.5.20+maria~ubu2004
# Thu, 11 May 2023 22:55:57 GMT
ENV MARIADB_VERSION=1:10.5.20+maria~ubu2004
# Thu, 11 May 2023 22:55:57 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.20/repo/ubuntu/ focal main
# Thu, 11 May 2023 22:55:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.20/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:56:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.20/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:56:18 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:56:18 GMT
COPY file:797eec99bf55d77c916c240bbbe1453b1ba37340268a58d0681bf242c87643e5 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:56:18 GMT
COPY file:e632ff8de201e30e52a350b1db7d277c1a9e5d053f830a65d1762771a6554a01 in /usr/local/bin/ 
# Thu, 11 May 2023 22:56:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:56:18 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:56:18 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8bc823a83fdf1329ae53f092d8f3641a60f92ee9f69e8785f5a3fd046eee30f`  
		Last Modified: Tue, 18 Apr 2023 02:28:38 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16685f710f5dded64d14b2537a025d665da5e257c4be3d921737f5f246b0fb9a`  
		Last Modified: Tue, 18 Apr 2023 02:28:40 GMT  
		Size: 7.1 MB (7058710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5660ff630580a5fee05c112e916f0bbca3234820aea68e604a23dba51f23d65`  
		Last Modified: Tue, 18 Apr 2023 02:28:36 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb5880d2d3596aabd567b0ab0fab78495b9da6a156f37d8b56a9e97cb0585e38`  
		Last Modified: Thu, 11 May 2023 23:00:18 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baf131972ef1c5c9bcc6b3bbba83d5446f291b8c41882f2c798e2ee639e143fb`  
		Last Modified: Thu, 11 May 2023 23:00:30 GMT  
		Size: 85.6 MB (85594026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2969c5907ed889bece6adf3b46b510705cfb7e14ff05653411f94e475514a62b`  
		Last Modified: Thu, 11 May 2023 23:00:18 GMT  
		Size: 3.5 KB (3530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:178375b1f8ced0ce2951db2d0c117891276795f7f37b2e3261d49dcd93ae8038`  
		Last Modified: Thu, 11 May 2023 23:00:18 GMT  
		Size: 7.5 KB (7487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.20` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:c5b30b0dd3e2264a31ee6e0b066c9f23cdcdce5ad9062186ff25f00998c0b3eb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.7 MB (118711396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ae32401c9ae8e249487985100cf7d9151d589739bb4fe761d25042652c48e75`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:00:47 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 18 Apr 2023 02:00:47 GMT
ENV GOSU_VERSION=1.14
# Tue, 18 Apr 2023 02:00:47 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 18 Apr 2023 02:01:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 18 Apr 2023 02:01:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 18 Apr 2023 02:01:03 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:39:42 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.5.20 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:39:42 GMT
ARG MARIADB_MAJOR=10.5
# Thu, 11 May 2023 22:39:42 GMT
ENV MARIADB_MAJOR=10.5
# Thu, 11 May 2023 22:39:42 GMT
ARG MARIADB_VERSION=1:10.5.20+maria~ubu2004
# Thu, 11 May 2023 22:39:43 GMT
ENV MARIADB_VERSION=1:10.5.20+maria~ubu2004
# Thu, 11 May 2023 22:39:43 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.20/repo/ubuntu/ focal main
# Thu, 11 May 2023 22:39:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.20/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:40:00 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.20/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:40:01 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:40:01 GMT
COPY file:797eec99bf55d77c916c240bbbe1453b1ba37340268a58d0681bf242c87643e5 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:40:02 GMT
COPY file:e632ff8de201e30e52a350b1db7d277c1a9e5d053f830a65d1762771a6554a01 in /usr/local/bin/ 
# Thu, 11 May 2023 22:40:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:40:02 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:40:02 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c227d9b91d2b3157f8d92aefc5896243bf63953d9852e7e73c79ddf26159c9`  
		Last Modified: Tue, 18 Apr 2023 02:03:42 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d0716d74d0fd81781cc567eced35e6c95c70a0e2709606996e1c20c5bda20c`  
		Last Modified: Tue, 18 Apr 2023 02:03:43 GMT  
		Size: 6.8 MB (6786196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673f317ed7421a7da75b11d78e42cce7972ab1b727ed5f537ca1c6f859941bee`  
		Last Modified: Tue, 18 Apr 2023 02:03:40 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98228e73f9a07adba2d89ff5cc45438491b85ab6774a546e35a764749e150ce5`  
		Last Modified: Thu, 11 May 2023 22:43:31 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f32cc43641b887abe1278d424bf6244c03e6cd542757e4d5a9df7ddaf1440155`  
		Last Modified: Thu, 11 May 2023 22:43:40 GMT  
		Size: 84.7 MB (84715562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d25fb18406a930eb0603235fa042b51ccbefe4b82637663368aab16e85a766`  
		Last Modified: Thu, 11 May 2023 22:43:31 GMT  
		Size: 3.5 KB (3531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842adf5985b6c2d1aee37edf536230abcde66ca70ec1f5d78d66b7dba7140bd8`  
		Last Modified: Thu, 11 May 2023 22:43:31 GMT  
		Size: 7.5 KB (7485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5.20-focal`

```console
$ docker pull mariadb@sha256:f75675445a176589ccd13131c1dfc443d7f2017692cb7b536cb1c293072f4f96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mariadb:10.5.20-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:0a9681b82efd8cb4e19d0931d2d597c03c4deb453004e9ccb6488bf33edfbf84
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.2 MB (121244540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76a5b2d8081aa97ba3e19d6256070d7c4fa9408a735c319dbbbba751be35df3a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:25:16 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 18 Apr 2023 02:25:16 GMT
ENV GOSU_VERSION=1.14
# Tue, 18 Apr 2023 02:25:17 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 18 Apr 2023 02:25:35 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 18 Apr 2023 02:25:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 18 Apr 2023 02:25:36 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:55:56 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.5.20 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:55:57 GMT
ARG MARIADB_MAJOR=10.5
# Thu, 11 May 2023 22:55:57 GMT
ENV MARIADB_MAJOR=10.5
# Thu, 11 May 2023 22:55:57 GMT
ARG MARIADB_VERSION=1:10.5.20+maria~ubu2004
# Thu, 11 May 2023 22:55:57 GMT
ENV MARIADB_VERSION=1:10.5.20+maria~ubu2004
# Thu, 11 May 2023 22:55:57 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.20/repo/ubuntu/ focal main
# Thu, 11 May 2023 22:55:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.20/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:56:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.20/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:56:18 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:56:18 GMT
COPY file:797eec99bf55d77c916c240bbbe1453b1ba37340268a58d0681bf242c87643e5 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:56:18 GMT
COPY file:e632ff8de201e30e52a350b1db7d277c1a9e5d053f830a65d1762771a6554a01 in /usr/local/bin/ 
# Thu, 11 May 2023 22:56:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:56:18 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:56:18 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8bc823a83fdf1329ae53f092d8f3641a60f92ee9f69e8785f5a3fd046eee30f`  
		Last Modified: Tue, 18 Apr 2023 02:28:38 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16685f710f5dded64d14b2537a025d665da5e257c4be3d921737f5f246b0fb9a`  
		Last Modified: Tue, 18 Apr 2023 02:28:40 GMT  
		Size: 7.1 MB (7058710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5660ff630580a5fee05c112e916f0bbca3234820aea68e604a23dba51f23d65`  
		Last Modified: Tue, 18 Apr 2023 02:28:36 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb5880d2d3596aabd567b0ab0fab78495b9da6a156f37d8b56a9e97cb0585e38`  
		Last Modified: Thu, 11 May 2023 23:00:18 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baf131972ef1c5c9bcc6b3bbba83d5446f291b8c41882f2c798e2ee639e143fb`  
		Last Modified: Thu, 11 May 2023 23:00:30 GMT  
		Size: 85.6 MB (85594026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2969c5907ed889bece6adf3b46b510705cfb7e14ff05653411f94e475514a62b`  
		Last Modified: Thu, 11 May 2023 23:00:18 GMT  
		Size: 3.5 KB (3530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:178375b1f8ced0ce2951db2d0c117891276795f7f37b2e3261d49dcd93ae8038`  
		Last Modified: Thu, 11 May 2023 23:00:18 GMT  
		Size: 7.5 KB (7487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.20-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:c5b30b0dd3e2264a31ee6e0b066c9f23cdcdce5ad9062186ff25f00998c0b3eb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.7 MB (118711396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ae32401c9ae8e249487985100cf7d9151d589739bb4fe761d25042652c48e75`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:00:47 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 18 Apr 2023 02:00:47 GMT
ENV GOSU_VERSION=1.14
# Tue, 18 Apr 2023 02:00:47 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 18 Apr 2023 02:01:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 18 Apr 2023 02:01:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 18 Apr 2023 02:01:03 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:39:42 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.5.20 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:39:42 GMT
ARG MARIADB_MAJOR=10.5
# Thu, 11 May 2023 22:39:42 GMT
ENV MARIADB_MAJOR=10.5
# Thu, 11 May 2023 22:39:42 GMT
ARG MARIADB_VERSION=1:10.5.20+maria~ubu2004
# Thu, 11 May 2023 22:39:43 GMT
ENV MARIADB_VERSION=1:10.5.20+maria~ubu2004
# Thu, 11 May 2023 22:39:43 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.20/repo/ubuntu/ focal main
# Thu, 11 May 2023 22:39:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.20/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:40:00 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.20/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:40:01 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:40:01 GMT
COPY file:797eec99bf55d77c916c240bbbe1453b1ba37340268a58d0681bf242c87643e5 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:40:02 GMT
COPY file:e632ff8de201e30e52a350b1db7d277c1a9e5d053f830a65d1762771a6554a01 in /usr/local/bin/ 
# Thu, 11 May 2023 22:40:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:40:02 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:40:02 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c227d9b91d2b3157f8d92aefc5896243bf63953d9852e7e73c79ddf26159c9`  
		Last Modified: Tue, 18 Apr 2023 02:03:42 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d0716d74d0fd81781cc567eced35e6c95c70a0e2709606996e1c20c5bda20c`  
		Last Modified: Tue, 18 Apr 2023 02:03:43 GMT  
		Size: 6.8 MB (6786196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673f317ed7421a7da75b11d78e42cce7972ab1b727ed5f537ca1c6f859941bee`  
		Last Modified: Tue, 18 Apr 2023 02:03:40 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98228e73f9a07adba2d89ff5cc45438491b85ab6774a546e35a764749e150ce5`  
		Last Modified: Thu, 11 May 2023 22:43:31 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f32cc43641b887abe1278d424bf6244c03e6cd542757e4d5a9df7ddaf1440155`  
		Last Modified: Thu, 11 May 2023 22:43:40 GMT  
		Size: 84.7 MB (84715562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d25fb18406a930eb0603235fa042b51ccbefe4b82637663368aab16e85a766`  
		Last Modified: Thu, 11 May 2023 22:43:31 GMT  
		Size: 3.5 KB (3531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842adf5985b6c2d1aee37edf536230abcde66ca70ec1f5d78d66b7dba7140bd8`  
		Last Modified: Thu, 11 May 2023 22:43:31 GMT  
		Size: 7.5 KB (7485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.6`

```console
$ docker pull mariadb@sha256:9a1682e8339e2202e7f19dea86c4687889deb59c52eaf31e9acab5ccfd05ae59
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.6` - linux; amd64

```console
$ docker pull mariadb@sha256:664ae2582a348dece2df9b2af345606bf30bc046a3d8a9b203baf850d53e20be
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.6 MB (121568426 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73d5a17928951435f495b3f6c279ea2fdad541be6b8ce46066b254eeda1833a8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:25:16 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 18 Apr 2023 02:25:16 GMT
ENV GOSU_VERSION=1.14
# Tue, 18 Apr 2023 02:25:17 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 18 Apr 2023 02:25:35 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 18 Apr 2023 02:25:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 18 Apr 2023 02:25:36 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:55:23 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.6.13 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:55:23 GMT
ARG MARIADB_MAJOR=10.6
# Thu, 11 May 2023 22:55:23 GMT
ENV MARIADB_MAJOR=10.6
# Thu, 11 May 2023 22:55:23 GMT
ARG MARIADB_VERSION=1:10.6.13+maria~ubu2004
# Thu, 11 May 2023 22:55:23 GMT
ENV MARIADB_VERSION=1:10.6.13+maria~ubu2004
# Thu, 11 May 2023 22:55:23 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.13/repo/ubuntu/ focal main
# Thu, 11 May 2023 22:55:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.13/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:55:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.13/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:55:51 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:55:52 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:55:52 GMT
COPY file:94a071210c811522ac7cb9cd9b6d33b1df5eb056971fbdeefa8e9bc2e8a2d629 in /usr/local/bin/ 
# Thu, 11 May 2023 22:55:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:55:52 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:55:52 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8bc823a83fdf1329ae53f092d8f3641a60f92ee9f69e8785f5a3fd046eee30f`  
		Last Modified: Tue, 18 Apr 2023 02:28:38 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16685f710f5dded64d14b2537a025d665da5e257c4be3d921737f5f246b0fb9a`  
		Last Modified: Tue, 18 Apr 2023 02:28:40 GMT  
		Size: 7.1 MB (7058710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5660ff630580a5fee05c112e916f0bbca3234820aea68e604a23dba51f23d65`  
		Last Modified: Tue, 18 Apr 2023 02:28:36 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c5db5fb6e2482f50c297f95ec676a17db981586e722eea7a73b7b581db17fe`  
		Last Modified: Thu, 11 May 2023 22:59:47 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f01d739390db01d5e87759ec089733bf1e7c8daefac2beac5c95fbc1d735cf3`  
		Last Modified: Thu, 11 May 2023 22:59:59 GMT  
		Size: 85.9 MB (85917891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e935b35439efcf527a39dc7f0412917828821e387ebe3dbd3a94d146ee7bb64`  
		Last Modified: Thu, 11 May 2023 22:59:47 GMT  
		Size: 3.5 KB (3526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ea977c20c6a5935cc184fb665caedd11a0a98c6c843645eac806fedb5ae733`  
		Last Modified: Thu, 11 May 2023 22:59:47 GMT  
		Size: 7.5 KB (7511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:6118d391c3ed0c297acf9bd7ac8d75ae616982be2e7cb95cb5153fbaab7cc4bf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.9 MB (118880104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:058799e91f5b13299b4ec7d871690530c2f373f294584dc3244e1c8ee464a860`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:00:47 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 18 Apr 2023 02:00:47 GMT
ENV GOSU_VERSION=1.14
# Tue, 18 Apr 2023 02:00:47 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 18 Apr 2023 02:01:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 18 Apr 2023 02:01:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 18 Apr 2023 02:01:03 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:39:02 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.6.13 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:39:02 GMT
ARG MARIADB_MAJOR=10.6
# Thu, 11 May 2023 22:39:03 GMT
ENV MARIADB_MAJOR=10.6
# Thu, 11 May 2023 22:39:03 GMT
ARG MARIADB_VERSION=1:10.6.13+maria~ubu2004
# Thu, 11 May 2023 22:39:03 GMT
ENV MARIADB_VERSION=1:10.6.13+maria~ubu2004
# Thu, 11 May 2023 22:39:03 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.13/repo/ubuntu/ focal main
# Thu, 11 May 2023 22:39:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.13/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:39:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.13/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:39:39 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:39:39 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:39:39 GMT
COPY file:94a071210c811522ac7cb9cd9b6d33b1df5eb056971fbdeefa8e9bc2e8a2d629 in /usr/local/bin/ 
# Thu, 11 May 2023 22:39:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:39:39 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:39:39 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c227d9b91d2b3157f8d92aefc5896243bf63953d9852e7e73c79ddf26159c9`  
		Last Modified: Tue, 18 Apr 2023 02:03:42 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d0716d74d0fd81781cc567eced35e6c95c70a0e2709606996e1c20c5bda20c`  
		Last Modified: Tue, 18 Apr 2023 02:03:43 GMT  
		Size: 6.8 MB (6786196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673f317ed7421a7da75b11d78e42cce7972ab1b727ed5f537ca1c6f859941bee`  
		Last Modified: Tue, 18 Apr 2023 02:03:40 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:423a7192aa8a16cf05246ee47174fa168664224d18278f8c2c6b5dbb23283d44`  
		Last Modified: Thu, 11 May 2023 22:43:09 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b36d026317d638b8318243cc2695bfbed24f39080a807858b8d981d7ea4bf49`  
		Last Modified: Thu, 11 May 2023 22:43:18 GMT  
		Size: 84.9 MB (84884249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:022835b49cff082ff2a96dc7082923cd9a41dc9a59ac0648cc3bd2ec488a3aac`  
		Last Modified: Thu, 11 May 2023 22:43:09 GMT  
		Size: 3.5 KB (3526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce8690f9fef3a6c2421c1a876b6e17cd5927259675053caad1d4a2f2e26b2dc`  
		Last Modified: Thu, 11 May 2023 22:43:09 GMT  
		Size: 7.5 KB (7511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6` - linux; ppc64le

```console
$ docker pull mariadb@sha256:efe41e15c4a361988b05e78bff421f743f7f7479b86f3fe353d3e151e38b206d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.2 MB (131187770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bd606804280cfe2cdb410edfd0a8349ab37e60bbf288afb4d62651dac6f7e98`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:36 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:37 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:40 GMT
ADD file:faba3891f58656ec753ba6ca4b63e7c1f27bcd236b665634b05d5bc1b1ceee0a in / 
# Thu, 13 Apr 2023 13:09:40 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:51:07 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 18 Apr 2023 01:51:07 GMT
ENV GOSU_VERSION=1.14
# Tue, 18 Apr 2023 01:51:07 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 18 Apr 2023 01:51:40 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 18 Apr 2023 01:51:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 18 Apr 2023 01:51:42 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 01:52:45 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.6.12 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 18 Apr 2023 01:52:45 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 18 Apr 2023 01:52:45 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 18 Apr 2023 01:52:45 GMT
ARG MARIADB_VERSION=1:10.6.12+maria~ubu2004
# Tue, 18 Apr 2023 01:52:46 GMT
ENV MARIADB_VERSION=1:10.6.12+maria~ubu2004
# Tue, 18 Apr 2023 01:52:46 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.12/repo/ubuntu/ focal main
# Tue, 18 Apr 2023 01:52:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.12/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 18 Apr 2023 01:53:31 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.12/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 18 Apr 2023 01:53:35 GMT
VOLUME [/var/lib/mysql]
# Tue, 18 Apr 2023 01:53:35 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Tue, 18 Apr 2023 01:53:36 GMT
COPY file:ebdfbcbc74dda1874f1c75d86e1c32733edb402d13440b2b7140a952010bc21f in /usr/local/bin/ 
# Tue, 18 Apr 2023 01:53:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 18 Apr 2023 01:53:36 GMT
EXPOSE 3306
# Tue, 18 Apr 2023 01:53:37 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d276072145993a42aed3e2b3e8cd26b6e08aab266d9c9d792ee89b26150681da`  
		Last Modified: Fri, 14 Apr 2023 09:36:00 GMT  
		Size: 33.3 MB (33300980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a173b48773a6ef3fc242fca8702df8e2e401cebf5d6eead9c2e8b679d8f8d57`  
		Last Modified: Tue, 18 Apr 2023 01:57:20 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a525710ca72c2fa19727739f7053c36e5bcc630c19dc9bc5a95f6758c57c071c`  
		Last Modified: Tue, 18 Apr 2023 01:57:22 GMT  
		Size: 7.8 MB (7771035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d96443e2327325857d538e8a99972d2e2cd67c59a3c89cbdfb282cd5b80f87`  
		Last Modified: Tue, 18 Apr 2023 01:57:17 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56306cf8e98f5c8af6dbca481ae82847b9f89b4705e8d3f244e2912005792d9d`  
		Last Modified: Tue, 18 Apr 2023 01:57:55 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29eae6f1832ca11f7b6381758de645b5415f0c43f5d431ca6c61a1d75c51e73`  
		Last Modified: Tue, 18 Apr 2023 01:58:18 GMT  
		Size: 90.1 MB (90103031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:323b15ed75eda94ca77ce3808d082fdfdbddead87cc7c7d6f3997bbc799c1cb8`  
		Last Modified: Tue, 18 Apr 2023 01:57:55 GMT  
		Size: 3.5 KB (3528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e0cddc73dff430712fc90e35bb8067a10c9feaadd9d0832487b1fa913547f6`  
		Last Modified: Tue, 18 Apr 2023 01:57:55 GMT  
		Size: 7.0 KB (6973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6` - linux; s390x

```console
$ docker pull mariadb@sha256:522cffa5d0042438a9197767d3d7a799eb7084bd711ebe86d4bd8c820803c15f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.5 MB (120502582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e228961b7ef5147c910b3871951211357c504b16ce3c514de453f66fc4be714c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:35 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:35 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:35 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:35 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:37 GMT
ADD file:44c66c03ba0afcc05de1b2078f83e8bfe04706b31491fcd3fdd93cfc88d5f06c in / 
# Thu, 13 Apr 2023 13:09:37 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 16:33:09 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 18 Apr 2023 16:33:09 GMT
ENV GOSU_VERSION=1.14
# Tue, 18 Apr 2023 16:33:09 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 18 Apr 2023 16:33:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 18 Apr 2023 16:33:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 18 Apr 2023 16:33:38 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 16:34:15 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.6.12 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 18 Apr 2023 16:34:15 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 18 Apr 2023 16:34:15 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 18 Apr 2023 16:34:16 GMT
ARG MARIADB_VERSION=1:10.6.12+maria~ubu2004
# Tue, 18 Apr 2023 16:34:16 GMT
ENV MARIADB_VERSION=1:10.6.12+maria~ubu2004
# Tue, 18 Apr 2023 16:34:16 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.12/repo/ubuntu/ focal main
# Tue, 18 Apr 2023 16:34:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.12/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 18 Apr 2023 16:34:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.12/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 18 Apr 2023 16:34:37 GMT
VOLUME [/var/lib/mysql]
# Tue, 18 Apr 2023 16:34:37 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Tue, 18 Apr 2023 16:34:37 GMT
COPY file:ebdfbcbc74dda1874f1c75d86e1c32733edb402d13440b2b7140a952010bc21f in /usr/local/bin/ 
# Tue, 18 Apr 2023 16:34:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 18 Apr 2023 16:34:38 GMT
EXPOSE 3306
# Tue, 18 Apr 2023 16:34:38 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:f11b609b1d63f2d37c0e3789823e7a7e62a078bddca7c46da8602655989c62d9`  
		Last Modified: Fri, 14 Apr 2023 09:38:39 GMT  
		Size: 27.0 MB (27016370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184f14ef3f9ff48410469ecdcf8d758d86092d41a732adcdcba4969b30b63272`  
		Last Modified: Tue, 18 Apr 2023 16:35:26 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17716ec3f50471a011fcf739f209ad3c5df9a3f808a38dc40e4079efb79e4d41`  
		Last Modified: Tue, 18 Apr 2023 16:35:26 GMT  
		Size: 6.6 MB (6609307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:235b8a8d1aa17dd5727bbfb2d4fb8393a20bc83e8f81325993515261956592de`  
		Last Modified: Tue, 18 Apr 2023 16:35:24 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc2b71d6f9cae39a466446449271210be4178fd5a80244f91b9f5293677c7fe8`  
		Last Modified: Tue, 18 Apr 2023 16:35:46 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c82cb9df0ecf4ade673dee516140b79cd301afe13c168e3eafe69a122bf1a1bc`  
		Last Modified: Tue, 18 Apr 2023 16:35:59 GMT  
		Size: 86.9 MB (86864177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39238df54b6b5f086294e3433ef51b249f830cf3936b271555fa502651301bba`  
		Last Modified: Tue, 18 Apr 2023 16:35:46 GMT  
		Size: 3.5 KB (3528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a2ac466aa70a9b6f41c33abd187c64f369b14a4b82a6ad520fac357ffde59a`  
		Last Modified: Tue, 18 Apr 2023 16:35:46 GMT  
		Size: 7.0 KB (6971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.6-focal`

```console
$ docker pull mariadb@sha256:9a1682e8339e2202e7f19dea86c4687889deb59c52eaf31e9acab5ccfd05ae59
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.6-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:664ae2582a348dece2df9b2af345606bf30bc046a3d8a9b203baf850d53e20be
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.6 MB (121568426 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73d5a17928951435f495b3f6c279ea2fdad541be6b8ce46066b254eeda1833a8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:25:16 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 18 Apr 2023 02:25:16 GMT
ENV GOSU_VERSION=1.14
# Tue, 18 Apr 2023 02:25:17 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 18 Apr 2023 02:25:35 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 18 Apr 2023 02:25:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 18 Apr 2023 02:25:36 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:55:23 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.6.13 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:55:23 GMT
ARG MARIADB_MAJOR=10.6
# Thu, 11 May 2023 22:55:23 GMT
ENV MARIADB_MAJOR=10.6
# Thu, 11 May 2023 22:55:23 GMT
ARG MARIADB_VERSION=1:10.6.13+maria~ubu2004
# Thu, 11 May 2023 22:55:23 GMT
ENV MARIADB_VERSION=1:10.6.13+maria~ubu2004
# Thu, 11 May 2023 22:55:23 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.13/repo/ubuntu/ focal main
# Thu, 11 May 2023 22:55:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.13/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:55:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.13/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:55:51 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:55:52 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:55:52 GMT
COPY file:94a071210c811522ac7cb9cd9b6d33b1df5eb056971fbdeefa8e9bc2e8a2d629 in /usr/local/bin/ 
# Thu, 11 May 2023 22:55:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:55:52 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:55:52 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8bc823a83fdf1329ae53f092d8f3641a60f92ee9f69e8785f5a3fd046eee30f`  
		Last Modified: Tue, 18 Apr 2023 02:28:38 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16685f710f5dded64d14b2537a025d665da5e257c4be3d921737f5f246b0fb9a`  
		Last Modified: Tue, 18 Apr 2023 02:28:40 GMT  
		Size: 7.1 MB (7058710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5660ff630580a5fee05c112e916f0bbca3234820aea68e604a23dba51f23d65`  
		Last Modified: Tue, 18 Apr 2023 02:28:36 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c5db5fb6e2482f50c297f95ec676a17db981586e722eea7a73b7b581db17fe`  
		Last Modified: Thu, 11 May 2023 22:59:47 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f01d739390db01d5e87759ec089733bf1e7c8daefac2beac5c95fbc1d735cf3`  
		Last Modified: Thu, 11 May 2023 22:59:59 GMT  
		Size: 85.9 MB (85917891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e935b35439efcf527a39dc7f0412917828821e387ebe3dbd3a94d146ee7bb64`  
		Last Modified: Thu, 11 May 2023 22:59:47 GMT  
		Size: 3.5 KB (3526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ea977c20c6a5935cc184fb665caedd11a0a98c6c843645eac806fedb5ae733`  
		Last Modified: Thu, 11 May 2023 22:59:47 GMT  
		Size: 7.5 KB (7511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:6118d391c3ed0c297acf9bd7ac8d75ae616982be2e7cb95cb5153fbaab7cc4bf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.9 MB (118880104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:058799e91f5b13299b4ec7d871690530c2f373f294584dc3244e1c8ee464a860`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:00:47 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 18 Apr 2023 02:00:47 GMT
ENV GOSU_VERSION=1.14
# Tue, 18 Apr 2023 02:00:47 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 18 Apr 2023 02:01:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 18 Apr 2023 02:01:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 18 Apr 2023 02:01:03 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:39:02 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.6.13 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:39:02 GMT
ARG MARIADB_MAJOR=10.6
# Thu, 11 May 2023 22:39:03 GMT
ENV MARIADB_MAJOR=10.6
# Thu, 11 May 2023 22:39:03 GMT
ARG MARIADB_VERSION=1:10.6.13+maria~ubu2004
# Thu, 11 May 2023 22:39:03 GMT
ENV MARIADB_VERSION=1:10.6.13+maria~ubu2004
# Thu, 11 May 2023 22:39:03 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.13/repo/ubuntu/ focal main
# Thu, 11 May 2023 22:39:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.13/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:39:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.13/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:39:39 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:39:39 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:39:39 GMT
COPY file:94a071210c811522ac7cb9cd9b6d33b1df5eb056971fbdeefa8e9bc2e8a2d629 in /usr/local/bin/ 
# Thu, 11 May 2023 22:39:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:39:39 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:39:39 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c227d9b91d2b3157f8d92aefc5896243bf63953d9852e7e73c79ddf26159c9`  
		Last Modified: Tue, 18 Apr 2023 02:03:42 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d0716d74d0fd81781cc567eced35e6c95c70a0e2709606996e1c20c5bda20c`  
		Last Modified: Tue, 18 Apr 2023 02:03:43 GMT  
		Size: 6.8 MB (6786196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673f317ed7421a7da75b11d78e42cce7972ab1b727ed5f537ca1c6f859941bee`  
		Last Modified: Tue, 18 Apr 2023 02:03:40 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:423a7192aa8a16cf05246ee47174fa168664224d18278f8c2c6b5dbb23283d44`  
		Last Modified: Thu, 11 May 2023 22:43:09 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b36d026317d638b8318243cc2695bfbed24f39080a807858b8d981d7ea4bf49`  
		Last Modified: Thu, 11 May 2023 22:43:18 GMT  
		Size: 84.9 MB (84884249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:022835b49cff082ff2a96dc7082923cd9a41dc9a59ac0648cc3bd2ec488a3aac`  
		Last Modified: Thu, 11 May 2023 22:43:09 GMT  
		Size: 3.5 KB (3526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce8690f9fef3a6c2421c1a876b6e17cd5927259675053caad1d4a2f2e26b2dc`  
		Last Modified: Thu, 11 May 2023 22:43:09 GMT  
		Size: 7.5 KB (7511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:efe41e15c4a361988b05e78bff421f743f7f7479b86f3fe353d3e151e38b206d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.2 MB (131187770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bd606804280cfe2cdb410edfd0a8349ab37e60bbf288afb4d62651dac6f7e98`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:36 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:37 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:40 GMT
ADD file:faba3891f58656ec753ba6ca4b63e7c1f27bcd236b665634b05d5bc1b1ceee0a in / 
# Thu, 13 Apr 2023 13:09:40 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:51:07 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 18 Apr 2023 01:51:07 GMT
ENV GOSU_VERSION=1.14
# Tue, 18 Apr 2023 01:51:07 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 18 Apr 2023 01:51:40 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 18 Apr 2023 01:51:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 18 Apr 2023 01:51:42 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 01:52:45 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.6.12 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 18 Apr 2023 01:52:45 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 18 Apr 2023 01:52:45 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 18 Apr 2023 01:52:45 GMT
ARG MARIADB_VERSION=1:10.6.12+maria~ubu2004
# Tue, 18 Apr 2023 01:52:46 GMT
ENV MARIADB_VERSION=1:10.6.12+maria~ubu2004
# Tue, 18 Apr 2023 01:52:46 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.12/repo/ubuntu/ focal main
# Tue, 18 Apr 2023 01:52:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.12/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 18 Apr 2023 01:53:31 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.12/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 18 Apr 2023 01:53:35 GMT
VOLUME [/var/lib/mysql]
# Tue, 18 Apr 2023 01:53:35 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Tue, 18 Apr 2023 01:53:36 GMT
COPY file:ebdfbcbc74dda1874f1c75d86e1c32733edb402d13440b2b7140a952010bc21f in /usr/local/bin/ 
# Tue, 18 Apr 2023 01:53:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 18 Apr 2023 01:53:36 GMT
EXPOSE 3306
# Tue, 18 Apr 2023 01:53:37 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d276072145993a42aed3e2b3e8cd26b6e08aab266d9c9d792ee89b26150681da`  
		Last Modified: Fri, 14 Apr 2023 09:36:00 GMT  
		Size: 33.3 MB (33300980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a173b48773a6ef3fc242fca8702df8e2e401cebf5d6eead9c2e8b679d8f8d57`  
		Last Modified: Tue, 18 Apr 2023 01:57:20 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a525710ca72c2fa19727739f7053c36e5bcc630c19dc9bc5a95f6758c57c071c`  
		Last Modified: Tue, 18 Apr 2023 01:57:22 GMT  
		Size: 7.8 MB (7771035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d96443e2327325857d538e8a99972d2e2cd67c59a3c89cbdfb282cd5b80f87`  
		Last Modified: Tue, 18 Apr 2023 01:57:17 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56306cf8e98f5c8af6dbca481ae82847b9f89b4705e8d3f244e2912005792d9d`  
		Last Modified: Tue, 18 Apr 2023 01:57:55 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29eae6f1832ca11f7b6381758de645b5415f0c43f5d431ca6c61a1d75c51e73`  
		Last Modified: Tue, 18 Apr 2023 01:58:18 GMT  
		Size: 90.1 MB (90103031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:323b15ed75eda94ca77ce3808d082fdfdbddead87cc7c7d6f3997bbc799c1cb8`  
		Last Modified: Tue, 18 Apr 2023 01:57:55 GMT  
		Size: 3.5 KB (3528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e0cddc73dff430712fc90e35bb8067a10c9feaadd9d0832487b1fa913547f6`  
		Last Modified: Tue, 18 Apr 2023 01:57:55 GMT  
		Size: 7.0 KB (6973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:522cffa5d0042438a9197767d3d7a799eb7084bd711ebe86d4bd8c820803c15f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.5 MB (120502582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e228961b7ef5147c910b3871951211357c504b16ce3c514de453f66fc4be714c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:35 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:35 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:35 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:35 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:37 GMT
ADD file:44c66c03ba0afcc05de1b2078f83e8bfe04706b31491fcd3fdd93cfc88d5f06c in / 
# Thu, 13 Apr 2023 13:09:37 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 16:33:09 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 18 Apr 2023 16:33:09 GMT
ENV GOSU_VERSION=1.14
# Tue, 18 Apr 2023 16:33:09 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 18 Apr 2023 16:33:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 18 Apr 2023 16:33:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 18 Apr 2023 16:33:38 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 16:34:15 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.6.12 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 18 Apr 2023 16:34:15 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 18 Apr 2023 16:34:15 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 18 Apr 2023 16:34:16 GMT
ARG MARIADB_VERSION=1:10.6.12+maria~ubu2004
# Tue, 18 Apr 2023 16:34:16 GMT
ENV MARIADB_VERSION=1:10.6.12+maria~ubu2004
# Tue, 18 Apr 2023 16:34:16 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.12/repo/ubuntu/ focal main
# Tue, 18 Apr 2023 16:34:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.12/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 18 Apr 2023 16:34:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.12/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 18 Apr 2023 16:34:37 GMT
VOLUME [/var/lib/mysql]
# Tue, 18 Apr 2023 16:34:37 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Tue, 18 Apr 2023 16:34:37 GMT
COPY file:ebdfbcbc74dda1874f1c75d86e1c32733edb402d13440b2b7140a952010bc21f in /usr/local/bin/ 
# Tue, 18 Apr 2023 16:34:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 18 Apr 2023 16:34:38 GMT
EXPOSE 3306
# Tue, 18 Apr 2023 16:34:38 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:f11b609b1d63f2d37c0e3789823e7a7e62a078bddca7c46da8602655989c62d9`  
		Last Modified: Fri, 14 Apr 2023 09:38:39 GMT  
		Size: 27.0 MB (27016370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184f14ef3f9ff48410469ecdcf8d758d86092d41a732adcdcba4969b30b63272`  
		Last Modified: Tue, 18 Apr 2023 16:35:26 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17716ec3f50471a011fcf739f209ad3c5df9a3f808a38dc40e4079efb79e4d41`  
		Last Modified: Tue, 18 Apr 2023 16:35:26 GMT  
		Size: 6.6 MB (6609307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:235b8a8d1aa17dd5727bbfb2d4fb8393a20bc83e8f81325993515261956592de`  
		Last Modified: Tue, 18 Apr 2023 16:35:24 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc2b71d6f9cae39a466446449271210be4178fd5a80244f91b9f5293677c7fe8`  
		Last Modified: Tue, 18 Apr 2023 16:35:46 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c82cb9df0ecf4ade673dee516140b79cd301afe13c168e3eafe69a122bf1a1bc`  
		Last Modified: Tue, 18 Apr 2023 16:35:59 GMT  
		Size: 86.9 MB (86864177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39238df54b6b5f086294e3433ef51b249f830cf3936b271555fa502651301bba`  
		Last Modified: Tue, 18 Apr 2023 16:35:46 GMT  
		Size: 3.5 KB (3528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a2ac466aa70a9b6f41c33abd187c64f369b14a4b82a6ad520fac357ffde59a`  
		Last Modified: Tue, 18 Apr 2023 16:35:46 GMT  
		Size: 7.0 KB (6971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.6.13`

```console
$ docker pull mariadb@sha256:d166cd985603c0cacc83fe01efe3bac89dc797113e6ba314b3ae366da093284c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mariadb:10.6.13` - linux; amd64

```console
$ docker pull mariadb@sha256:664ae2582a348dece2df9b2af345606bf30bc046a3d8a9b203baf850d53e20be
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.6 MB (121568426 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73d5a17928951435f495b3f6c279ea2fdad541be6b8ce46066b254eeda1833a8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:25:16 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 18 Apr 2023 02:25:16 GMT
ENV GOSU_VERSION=1.14
# Tue, 18 Apr 2023 02:25:17 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 18 Apr 2023 02:25:35 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 18 Apr 2023 02:25:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 18 Apr 2023 02:25:36 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:55:23 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.6.13 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:55:23 GMT
ARG MARIADB_MAJOR=10.6
# Thu, 11 May 2023 22:55:23 GMT
ENV MARIADB_MAJOR=10.6
# Thu, 11 May 2023 22:55:23 GMT
ARG MARIADB_VERSION=1:10.6.13+maria~ubu2004
# Thu, 11 May 2023 22:55:23 GMT
ENV MARIADB_VERSION=1:10.6.13+maria~ubu2004
# Thu, 11 May 2023 22:55:23 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.13/repo/ubuntu/ focal main
# Thu, 11 May 2023 22:55:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.13/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:55:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.13/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:55:51 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:55:52 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:55:52 GMT
COPY file:94a071210c811522ac7cb9cd9b6d33b1df5eb056971fbdeefa8e9bc2e8a2d629 in /usr/local/bin/ 
# Thu, 11 May 2023 22:55:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:55:52 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:55:52 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8bc823a83fdf1329ae53f092d8f3641a60f92ee9f69e8785f5a3fd046eee30f`  
		Last Modified: Tue, 18 Apr 2023 02:28:38 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16685f710f5dded64d14b2537a025d665da5e257c4be3d921737f5f246b0fb9a`  
		Last Modified: Tue, 18 Apr 2023 02:28:40 GMT  
		Size: 7.1 MB (7058710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5660ff630580a5fee05c112e916f0bbca3234820aea68e604a23dba51f23d65`  
		Last Modified: Tue, 18 Apr 2023 02:28:36 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c5db5fb6e2482f50c297f95ec676a17db981586e722eea7a73b7b581db17fe`  
		Last Modified: Thu, 11 May 2023 22:59:47 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f01d739390db01d5e87759ec089733bf1e7c8daefac2beac5c95fbc1d735cf3`  
		Last Modified: Thu, 11 May 2023 22:59:59 GMT  
		Size: 85.9 MB (85917891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e935b35439efcf527a39dc7f0412917828821e387ebe3dbd3a94d146ee7bb64`  
		Last Modified: Thu, 11 May 2023 22:59:47 GMT  
		Size: 3.5 KB (3526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ea977c20c6a5935cc184fb665caedd11a0a98c6c843645eac806fedb5ae733`  
		Last Modified: Thu, 11 May 2023 22:59:47 GMT  
		Size: 7.5 KB (7511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6.13` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:6118d391c3ed0c297acf9bd7ac8d75ae616982be2e7cb95cb5153fbaab7cc4bf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.9 MB (118880104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:058799e91f5b13299b4ec7d871690530c2f373f294584dc3244e1c8ee464a860`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:00:47 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 18 Apr 2023 02:00:47 GMT
ENV GOSU_VERSION=1.14
# Tue, 18 Apr 2023 02:00:47 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 18 Apr 2023 02:01:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 18 Apr 2023 02:01:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 18 Apr 2023 02:01:03 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:39:02 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.6.13 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:39:02 GMT
ARG MARIADB_MAJOR=10.6
# Thu, 11 May 2023 22:39:03 GMT
ENV MARIADB_MAJOR=10.6
# Thu, 11 May 2023 22:39:03 GMT
ARG MARIADB_VERSION=1:10.6.13+maria~ubu2004
# Thu, 11 May 2023 22:39:03 GMT
ENV MARIADB_VERSION=1:10.6.13+maria~ubu2004
# Thu, 11 May 2023 22:39:03 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.13/repo/ubuntu/ focal main
# Thu, 11 May 2023 22:39:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.13/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:39:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.13/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:39:39 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:39:39 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:39:39 GMT
COPY file:94a071210c811522ac7cb9cd9b6d33b1df5eb056971fbdeefa8e9bc2e8a2d629 in /usr/local/bin/ 
# Thu, 11 May 2023 22:39:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:39:39 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:39:39 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c227d9b91d2b3157f8d92aefc5896243bf63953d9852e7e73c79ddf26159c9`  
		Last Modified: Tue, 18 Apr 2023 02:03:42 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d0716d74d0fd81781cc567eced35e6c95c70a0e2709606996e1c20c5bda20c`  
		Last Modified: Tue, 18 Apr 2023 02:03:43 GMT  
		Size: 6.8 MB (6786196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673f317ed7421a7da75b11d78e42cce7972ab1b727ed5f537ca1c6f859941bee`  
		Last Modified: Tue, 18 Apr 2023 02:03:40 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:423a7192aa8a16cf05246ee47174fa168664224d18278f8c2c6b5dbb23283d44`  
		Last Modified: Thu, 11 May 2023 22:43:09 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b36d026317d638b8318243cc2695bfbed24f39080a807858b8d981d7ea4bf49`  
		Last Modified: Thu, 11 May 2023 22:43:18 GMT  
		Size: 84.9 MB (84884249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:022835b49cff082ff2a96dc7082923cd9a41dc9a59ac0648cc3bd2ec488a3aac`  
		Last Modified: Thu, 11 May 2023 22:43:09 GMT  
		Size: 3.5 KB (3526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce8690f9fef3a6c2421c1a876b6e17cd5927259675053caad1d4a2f2e26b2dc`  
		Last Modified: Thu, 11 May 2023 22:43:09 GMT  
		Size: 7.5 KB (7511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.6.13-focal`

```console
$ docker pull mariadb@sha256:d166cd985603c0cacc83fe01efe3bac89dc797113e6ba314b3ae366da093284c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mariadb:10.6.13-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:664ae2582a348dece2df9b2af345606bf30bc046a3d8a9b203baf850d53e20be
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.6 MB (121568426 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73d5a17928951435f495b3f6c279ea2fdad541be6b8ce46066b254eeda1833a8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:25:16 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 18 Apr 2023 02:25:16 GMT
ENV GOSU_VERSION=1.14
# Tue, 18 Apr 2023 02:25:17 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 18 Apr 2023 02:25:35 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 18 Apr 2023 02:25:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 18 Apr 2023 02:25:36 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:55:23 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.6.13 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:55:23 GMT
ARG MARIADB_MAJOR=10.6
# Thu, 11 May 2023 22:55:23 GMT
ENV MARIADB_MAJOR=10.6
# Thu, 11 May 2023 22:55:23 GMT
ARG MARIADB_VERSION=1:10.6.13+maria~ubu2004
# Thu, 11 May 2023 22:55:23 GMT
ENV MARIADB_VERSION=1:10.6.13+maria~ubu2004
# Thu, 11 May 2023 22:55:23 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.13/repo/ubuntu/ focal main
# Thu, 11 May 2023 22:55:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.13/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:55:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.13/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:55:51 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:55:52 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:55:52 GMT
COPY file:94a071210c811522ac7cb9cd9b6d33b1df5eb056971fbdeefa8e9bc2e8a2d629 in /usr/local/bin/ 
# Thu, 11 May 2023 22:55:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:55:52 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:55:52 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8bc823a83fdf1329ae53f092d8f3641a60f92ee9f69e8785f5a3fd046eee30f`  
		Last Modified: Tue, 18 Apr 2023 02:28:38 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16685f710f5dded64d14b2537a025d665da5e257c4be3d921737f5f246b0fb9a`  
		Last Modified: Tue, 18 Apr 2023 02:28:40 GMT  
		Size: 7.1 MB (7058710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5660ff630580a5fee05c112e916f0bbca3234820aea68e604a23dba51f23d65`  
		Last Modified: Tue, 18 Apr 2023 02:28:36 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c5db5fb6e2482f50c297f95ec676a17db981586e722eea7a73b7b581db17fe`  
		Last Modified: Thu, 11 May 2023 22:59:47 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f01d739390db01d5e87759ec089733bf1e7c8daefac2beac5c95fbc1d735cf3`  
		Last Modified: Thu, 11 May 2023 22:59:59 GMT  
		Size: 85.9 MB (85917891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e935b35439efcf527a39dc7f0412917828821e387ebe3dbd3a94d146ee7bb64`  
		Last Modified: Thu, 11 May 2023 22:59:47 GMT  
		Size: 3.5 KB (3526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ea977c20c6a5935cc184fb665caedd11a0a98c6c843645eac806fedb5ae733`  
		Last Modified: Thu, 11 May 2023 22:59:47 GMT  
		Size: 7.5 KB (7511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6.13-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:6118d391c3ed0c297acf9bd7ac8d75ae616982be2e7cb95cb5153fbaab7cc4bf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.9 MB (118880104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:058799e91f5b13299b4ec7d871690530c2f373f294584dc3244e1c8ee464a860`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:00:47 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 18 Apr 2023 02:00:47 GMT
ENV GOSU_VERSION=1.14
# Tue, 18 Apr 2023 02:00:47 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 18 Apr 2023 02:01:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 18 Apr 2023 02:01:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 18 Apr 2023 02:01:03 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:39:02 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.6.13 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:39:02 GMT
ARG MARIADB_MAJOR=10.6
# Thu, 11 May 2023 22:39:03 GMT
ENV MARIADB_MAJOR=10.6
# Thu, 11 May 2023 22:39:03 GMT
ARG MARIADB_VERSION=1:10.6.13+maria~ubu2004
# Thu, 11 May 2023 22:39:03 GMT
ENV MARIADB_VERSION=1:10.6.13+maria~ubu2004
# Thu, 11 May 2023 22:39:03 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.13/repo/ubuntu/ focal main
# Thu, 11 May 2023 22:39:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.13/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:39:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.13/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:39:39 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:39:39 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:39:39 GMT
COPY file:94a071210c811522ac7cb9cd9b6d33b1df5eb056971fbdeefa8e9bc2e8a2d629 in /usr/local/bin/ 
# Thu, 11 May 2023 22:39:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:39:39 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:39:39 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c227d9b91d2b3157f8d92aefc5896243bf63953d9852e7e73c79ddf26159c9`  
		Last Modified: Tue, 18 Apr 2023 02:03:42 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d0716d74d0fd81781cc567eced35e6c95c70a0e2709606996e1c20c5bda20c`  
		Last Modified: Tue, 18 Apr 2023 02:03:43 GMT  
		Size: 6.8 MB (6786196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673f317ed7421a7da75b11d78e42cce7972ab1b727ed5f537ca1c6f859941bee`  
		Last Modified: Tue, 18 Apr 2023 02:03:40 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:423a7192aa8a16cf05246ee47174fa168664224d18278f8c2c6b5dbb23283d44`  
		Last Modified: Thu, 11 May 2023 22:43:09 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b36d026317d638b8318243cc2695bfbed24f39080a807858b8d981d7ea4bf49`  
		Last Modified: Thu, 11 May 2023 22:43:18 GMT  
		Size: 84.9 MB (84884249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:022835b49cff082ff2a96dc7082923cd9a41dc9a59ac0648cc3bd2ec488a3aac`  
		Last Modified: Thu, 11 May 2023 22:43:09 GMT  
		Size: 3.5 KB (3526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce8690f9fef3a6c2421c1a876b6e17cd5927259675053caad1d4a2f2e26b2dc`  
		Last Modified: Thu, 11 May 2023 22:43:09 GMT  
		Size: 7.5 KB (7511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.8`

```console
$ docker pull mariadb@sha256:fd9f55cb67c7b261995a20514c9e5d57e37fc3f6c1d46810c38b36dc23088f0c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.8` - linux; amd64

```console
$ docker pull mariadb@sha256:a3b3746dc60ab692c1e8116afdc36977c99e1196bc2c0253cc7ea9bed8f2a84f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.3 MB (119326364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91a5024e053f9e04c27f81a94c360d0fa172ffde9591d12cfe3b96419cbc69c0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 07:52:03 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 07:52:03 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 07:52:03 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 07:52:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 07:52:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 07:52:19 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:54:59 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.8.8 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:54:59 GMT
ARG MARIADB_MAJOR=10.8
# Thu, 11 May 2023 22:54:59 GMT
ENV MARIADB_MAJOR=10.8
# Thu, 11 May 2023 22:54:59 GMT
ARG MARIADB_VERSION=1:10.8.8+maria~ubu2204
# Thu, 11 May 2023 22:54:59 GMT
ENV MARIADB_VERSION=1:10.8.8+maria~ubu2204
# Thu, 11 May 2023 22:55:00 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.8/repo/ubuntu/ jammy main
# Thu, 11 May 2023 22:55:00 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.8/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:55:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.8/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:55:17 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:55:18 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:55:18 GMT
COPY file:94a071210c811522ac7cb9cd9b6d33b1df5eb056971fbdeefa8e9bc2e8a2d629 in /usr/local/bin/ 
# Thu, 11 May 2023 22:55:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:55:18 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:55:18 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:1bc677758ad7fa4503417ae5be18809c5a8679b5b36fcd1464d5a8e41cb13305`  
		Last Modified: Tue, 25 Apr 2023 22:54:44 GMT  
		Size: 30.4 MB (30430220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196e1740aea41b9915498de02cc132de54583dad1a212d06c9f6eb4690e1e0cb`  
		Last Modified: Thu, 04 May 2023 07:54:52 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4df0997938e5fd755403145484e1253115d3739285c704f562cf3bd6d89ec8`  
		Last Modified: Thu, 04 May 2023 07:54:53 GMT  
		Size: 5.6 MB (5595975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa4e41848249471f699386db900347fa61b39622dfba140344d9c51b264e7db`  
		Last Modified: Thu, 04 May 2023 07:54:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49e668d986b90318149d51109182a73222ad43b6b3e481eaf5d441cab78559d`  
		Last Modified: Thu, 11 May 2023 22:59:22 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cc871714a591c2a3250454c26604f654409930c77c8a3717eb0073e1e0e718e`  
		Last Modified: Thu, 11 May 2023 22:59:34 GMT  
		Size: 83.3 MB (83286903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c7a49739d5940a004b85da792032e062b7d03f4c0efe09b2961508b8b3cb63e`  
		Last Modified: Thu, 11 May 2023 22:59:23 GMT  
		Size: 3.5 KB (3526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1abfccf36f9db1fdfaefcf6054d581545cf4ea012707bb11f41a1ed18adfc9f7`  
		Last Modified: Thu, 11 May 2023 22:59:23 GMT  
		Size: 7.5 KB (7515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:921e80a9b908dd181ce2d5bf6a98fabdc515eecc8a507a51e3dc845ae32b0792
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.9 MB (113914811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc532e8de402f89ad865a711e6235f267442512f7ef485090d3a150b2f8399ee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 03:46:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 03:46:08 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 03:46:08 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 03:46:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 03:46:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 03:46:28 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:38:39 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.8.8 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:38:40 GMT
ARG MARIADB_MAJOR=10.8
# Thu, 11 May 2023 22:38:40 GMT
ENV MARIADB_MAJOR=10.8
# Thu, 11 May 2023 22:38:40 GMT
ARG MARIADB_VERSION=1:10.8.8+maria~ubu2204
# Thu, 11 May 2023 22:38:40 GMT
ENV MARIADB_VERSION=1:10.8.8+maria~ubu2204
# Thu, 11 May 2023 22:38:40 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.8/repo/ubuntu/ jammy main
# Thu, 11 May 2023 22:38:40 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.8/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:38:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.8/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:38:58 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:38:58 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:38:59 GMT
COPY file:94a071210c811522ac7cb9cd9b6d33b1df5eb056971fbdeefa8e9bc2e8a2d629 in /usr/local/bin/ 
# Thu, 11 May 2023 22:38:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:38:59 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:38:59 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:f3f60f415e9a03eed88bd5dd5268c841cde08dacf16911a3ef1e4e0fcdd76568`  
		Last Modified: Wed, 26 Apr 2023 02:08:37 GMT  
		Size: 28.4 MB (28389440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bfb87016de46ece16208cd39b5fa89740b8e8db147c2da2f6483551b3e8d521`  
		Last Modified: Thu, 04 May 2023 03:49:02 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8bd3f48f8f1fc94a1a143132ba91e005df50ee4327d0e209553cc89145a91f`  
		Last Modified: Thu, 04 May 2023 03:49:03 GMT  
		Size: 5.4 MB (5409831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ebb0502bf43d03d32f27b6cfa9ea349e89bccb62bd1ef3cf96a9a769e6c1fa`  
		Last Modified: Thu, 04 May 2023 03:49:00 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9ae9fcfb680e43985085538f34194a9a0d84f3e12417a217b6844374a73e2b`  
		Last Modified: Thu, 11 May 2023 22:42:48 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:594723f411cfaf9d0917e9fb5bf0f7391d81e93de1d2fc5436a97359125e62a2`  
		Last Modified: Thu, 11 May 2023 22:42:56 GMT  
		Size: 80.1 MB (80102275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a02297f142711ade1e6c84bf8116721de20651ad48a4ba847b6726dd9ee20687`  
		Last Modified: Thu, 11 May 2023 22:42:47 GMT  
		Size: 3.5 KB (3526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28b2d7c377aef74345f95ce57ed6659d928f08a59e02708e2244f93204b75442`  
		Last Modified: Thu, 11 May 2023 22:42:47 GMT  
		Size: 7.5 KB (7515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8` - linux; ppc64le

```console
$ docker pull mariadb@sha256:1f04aef4b2d19b4ba8c833b0d60c216d6c077158aa33b14f02e057d7edf16c3a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.9 MB (127901997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fff19fe85fc19d84e05f676f7927e975eca043b0f8418d9435ace8adf9635af5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:17 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:18 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:21 GMT
ADD file:e75f08a67f0576b5441bb2fe454cad4b5b31a9d4efea23be791af62e1e0c712f in / 
# Tue, 25 Apr 2023 17:30:21 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 14:29:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 14:29:33 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 14:29:33 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 14:30:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 14:30:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 14:30:21 GMT
ENV LANG=C.UTF-8
# Thu, 04 May 2023 14:36:23 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.8.7 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 04 May 2023 14:36:23 GMT
ARG MARIADB_MAJOR=10.8
# Thu, 04 May 2023 14:36:24 GMT
ENV MARIADB_MAJOR=10.8
# Thu, 04 May 2023 14:36:25 GMT
ARG MARIADB_VERSION=1:10.8.7+maria~ubu2204
# Thu, 04 May 2023 14:36:25 GMT
ENV MARIADB_VERSION=1:10.8.7+maria~ubu2204
# Thu, 04 May 2023 14:36:26 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.7/repo/ubuntu/ jammy main
# Thu, 04 May 2023 14:36:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.7/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 04 May 2023 14:37:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.7/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 04 May 2023 14:37:29 GMT
VOLUME [/var/lib/mysql]
# Thu, 04 May 2023 14:37:29 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 04 May 2023 14:37:30 GMT
COPY file:ebdfbcbc74dda1874f1c75d86e1c32733edb402d13440b2b7140a952010bc21f in /usr/local/bin/ 
# Thu, 04 May 2023 14:37:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 May 2023 14:37:30 GMT
EXPOSE 3306
# Thu, 04 May 2023 14:37:31 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:f6a63d8cd043e76933823b18cbb7057a55bb4d66d64639c81e15a4700c101582`  
		Last Modified: Wed, 03 May 2023 17:09:07 GMT  
		Size: 35.7 MB (35712706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df46cdfc9a45a40dd254c1a0f2ccb2b0020e6852a5fb101d44d79250da5ddc69`  
		Last Modified: Thu, 04 May 2023 14:38:11 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11d1aa00f5a23d7276d6c701876911c79820fef6401156510e68eecb03012091`  
		Last Modified: Thu, 04 May 2023 14:38:12 GMT  
		Size: 6.0 MB (6021655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ec0fb2f57daffaea6b67a61d9012d55d4fcef64766481235d00d0438513793b`  
		Last Modified: Thu, 04 May 2023 14:38:08 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08cfaf41665f3a11466489fa4332df8fc382accf2d4a45319f4c250fd2156a70`  
		Last Modified: Thu, 04 May 2023 14:40:55 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ed2fcff548b07dc439eda80da108a1d53203f5d86d3f0de78d23a2e909c7dc6`  
		Last Modified: Thu, 04 May 2023 14:41:18 GMT  
		Size: 86.2 MB (86154912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e872108202c7d6442cf1512b325bfdc4680d3fbabba5a34c2a63e63a21a78325`  
		Last Modified: Thu, 04 May 2023 14:40:55 GMT  
		Size: 3.5 KB (3526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:494ee9af52d7390c87b779cbc83c2873316efb23a25e517fb55c9fda0ea0e702`  
		Last Modified: Thu, 04 May 2023 14:40:55 GMT  
		Size: 7.0 KB (6972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8` - linux; s390x

```console
$ docker pull mariadb@sha256:b92f82557df3713441544fecc9f714c2c686d731ebc969bdd6e975bd7f04ed14
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.8 MB (116777515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cca63cef0ab6c4e52a0ab56de7ab6eb113dd41788afc557c4e056b20aec13ba7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 26 Jan 2023 05:08:35 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:08:35 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:08:36 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:08:36 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:08:37 GMT
ADD file:a9794efc1a102ab6a7160e660a63f4b267797b8b7e0b0bfd9c04ed62846cfb36 in / 
# Thu, 26 Jan 2023 05:08:38 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:42:50 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 31 Jan 2023 18:42:50 GMT
ENV GOSU_VERSION=1.14
# Tue, 31 Jan 2023 18:42:50 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 31 Jan 2023 18:43:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 31 Jan 2023 18:43:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 31 Jan 2023 18:43:06 GMT
ENV LANG=C.UTF-8
# Tue, 07 Feb 2023 01:48:05 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.8.7 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 07 Feb 2023 01:48:05 GMT
ARG MARIADB_MAJOR=10.8
# Tue, 07 Feb 2023 01:48:05 GMT
ENV MARIADB_MAJOR=10.8
# Tue, 07 Feb 2023 01:48:06 GMT
ARG MARIADB_VERSION=1:10.8.7+maria~ubu2204
# Tue, 07 Feb 2023 01:48:06 GMT
ENV MARIADB_VERSION=1:10.8.7+maria~ubu2204
# Tue, 07 Feb 2023 01:48:06 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.7/repo/ubuntu/ jammy main
# Tue, 07 Feb 2023 01:48:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.7/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Feb 2023 01:48:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.7/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 07 Feb 2023 01:48:44 GMT
VOLUME [/var/lib/mysql]
# Sat, 25 Feb 2023 04:00:50 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Sat, 25 Feb 2023 04:00:50 GMT
COPY file:ebdfbcbc74dda1874f1c75d86e1c32733edb402d13440b2b7140a952010bc21f in /usr/local/bin/ 
# Sat, 25 Feb 2023 04:00:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 25 Feb 2023 04:00:50 GMT
EXPOSE 3306
# Sat, 25 Feb 2023 04:00:50 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:dd969ed9de43018fe5442c859bf66eabf23145b966b9338392ea707aed18b26f`  
		Last Modified: Tue, 31 Jan 2023 17:55:34 GMT  
		Size: 28.6 MB (28641926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b702438b56d7a6aaaad49e2be85e1bb2f3beb85406f6b9db1a232f798c558b3`  
		Last Modified: Tue, 31 Jan 2023 18:48:25 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60737998d0295bde808ca8856933482817ca605937f714f3cfca1ab0b4ca99ed`  
		Last Modified: Tue, 31 Jan 2023 18:48:26 GMT  
		Size: 5.4 MB (5401827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6e12a0288bb0803aeb23e581ca842e1fdf826fa28b4a730dd83585ea125ff8`  
		Last Modified: Tue, 31 Jan 2023 18:48:24 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a521985064ee3063bb3cd2edc44453d254baed98cb527acbdfaecb2fc3417952`  
		Last Modified: Tue, 07 Feb 2023 01:53:42 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43022d2479b063053f0a4f7cfa2e7d4164662db2e5a91351a42e8e24b146eddd`  
		Last Modified: Tue, 07 Feb 2023 01:53:53 GMT  
		Size: 82.7 MB (82721043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07535bc5dbd54e6b2ce7a722cecfc8c143d9d0750f01cd711da909c77485e949`  
		Last Modified: Sat, 25 Feb 2023 04:02:56 GMT  
		Size: 3.5 KB (3523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83b93a94d7abb56931fa6e741b37f71223e88ab92cc631aef69abec58fa5632`  
		Last Modified: Sat, 25 Feb 2023 04:02:55 GMT  
		Size: 7.0 KB (6969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.8-jammy`

```console
$ docker pull mariadb@sha256:fd9f55cb67c7b261995a20514c9e5d57e37fc3f6c1d46810c38b36dc23088f0c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.8-jammy` - linux; amd64

```console
$ docker pull mariadb@sha256:a3b3746dc60ab692c1e8116afdc36977c99e1196bc2c0253cc7ea9bed8f2a84f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.3 MB (119326364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91a5024e053f9e04c27f81a94c360d0fa172ffde9591d12cfe3b96419cbc69c0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 07:52:03 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 07:52:03 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 07:52:03 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 07:52:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 07:52:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 07:52:19 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:54:59 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.8.8 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:54:59 GMT
ARG MARIADB_MAJOR=10.8
# Thu, 11 May 2023 22:54:59 GMT
ENV MARIADB_MAJOR=10.8
# Thu, 11 May 2023 22:54:59 GMT
ARG MARIADB_VERSION=1:10.8.8+maria~ubu2204
# Thu, 11 May 2023 22:54:59 GMT
ENV MARIADB_VERSION=1:10.8.8+maria~ubu2204
# Thu, 11 May 2023 22:55:00 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.8/repo/ubuntu/ jammy main
# Thu, 11 May 2023 22:55:00 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.8/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:55:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.8/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:55:17 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:55:18 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:55:18 GMT
COPY file:94a071210c811522ac7cb9cd9b6d33b1df5eb056971fbdeefa8e9bc2e8a2d629 in /usr/local/bin/ 
# Thu, 11 May 2023 22:55:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:55:18 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:55:18 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:1bc677758ad7fa4503417ae5be18809c5a8679b5b36fcd1464d5a8e41cb13305`  
		Last Modified: Tue, 25 Apr 2023 22:54:44 GMT  
		Size: 30.4 MB (30430220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196e1740aea41b9915498de02cc132de54583dad1a212d06c9f6eb4690e1e0cb`  
		Last Modified: Thu, 04 May 2023 07:54:52 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4df0997938e5fd755403145484e1253115d3739285c704f562cf3bd6d89ec8`  
		Last Modified: Thu, 04 May 2023 07:54:53 GMT  
		Size: 5.6 MB (5595975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa4e41848249471f699386db900347fa61b39622dfba140344d9c51b264e7db`  
		Last Modified: Thu, 04 May 2023 07:54:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49e668d986b90318149d51109182a73222ad43b6b3e481eaf5d441cab78559d`  
		Last Modified: Thu, 11 May 2023 22:59:22 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cc871714a591c2a3250454c26604f654409930c77c8a3717eb0073e1e0e718e`  
		Last Modified: Thu, 11 May 2023 22:59:34 GMT  
		Size: 83.3 MB (83286903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c7a49739d5940a004b85da792032e062b7d03f4c0efe09b2961508b8b3cb63e`  
		Last Modified: Thu, 11 May 2023 22:59:23 GMT  
		Size: 3.5 KB (3526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1abfccf36f9db1fdfaefcf6054d581545cf4ea012707bb11f41a1ed18adfc9f7`  
		Last Modified: Thu, 11 May 2023 22:59:23 GMT  
		Size: 7.5 KB (7515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8-jammy` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:921e80a9b908dd181ce2d5bf6a98fabdc515eecc8a507a51e3dc845ae32b0792
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.9 MB (113914811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc532e8de402f89ad865a711e6235f267442512f7ef485090d3a150b2f8399ee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 03:46:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 03:46:08 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 03:46:08 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 03:46:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 03:46:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 03:46:28 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:38:39 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.8.8 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:38:40 GMT
ARG MARIADB_MAJOR=10.8
# Thu, 11 May 2023 22:38:40 GMT
ENV MARIADB_MAJOR=10.8
# Thu, 11 May 2023 22:38:40 GMT
ARG MARIADB_VERSION=1:10.8.8+maria~ubu2204
# Thu, 11 May 2023 22:38:40 GMT
ENV MARIADB_VERSION=1:10.8.8+maria~ubu2204
# Thu, 11 May 2023 22:38:40 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.8/repo/ubuntu/ jammy main
# Thu, 11 May 2023 22:38:40 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.8/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:38:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.8/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:38:58 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:38:58 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:38:59 GMT
COPY file:94a071210c811522ac7cb9cd9b6d33b1df5eb056971fbdeefa8e9bc2e8a2d629 in /usr/local/bin/ 
# Thu, 11 May 2023 22:38:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:38:59 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:38:59 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:f3f60f415e9a03eed88bd5dd5268c841cde08dacf16911a3ef1e4e0fcdd76568`  
		Last Modified: Wed, 26 Apr 2023 02:08:37 GMT  
		Size: 28.4 MB (28389440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bfb87016de46ece16208cd39b5fa89740b8e8db147c2da2f6483551b3e8d521`  
		Last Modified: Thu, 04 May 2023 03:49:02 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8bd3f48f8f1fc94a1a143132ba91e005df50ee4327d0e209553cc89145a91f`  
		Last Modified: Thu, 04 May 2023 03:49:03 GMT  
		Size: 5.4 MB (5409831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ebb0502bf43d03d32f27b6cfa9ea349e89bccb62bd1ef3cf96a9a769e6c1fa`  
		Last Modified: Thu, 04 May 2023 03:49:00 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9ae9fcfb680e43985085538f34194a9a0d84f3e12417a217b6844374a73e2b`  
		Last Modified: Thu, 11 May 2023 22:42:48 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:594723f411cfaf9d0917e9fb5bf0f7391d81e93de1d2fc5436a97359125e62a2`  
		Last Modified: Thu, 11 May 2023 22:42:56 GMT  
		Size: 80.1 MB (80102275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a02297f142711ade1e6c84bf8116721de20651ad48a4ba847b6726dd9ee20687`  
		Last Modified: Thu, 11 May 2023 22:42:47 GMT  
		Size: 3.5 KB (3526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28b2d7c377aef74345f95ce57ed6659d928f08a59e02708e2244f93204b75442`  
		Last Modified: Thu, 11 May 2023 22:42:47 GMT  
		Size: 7.5 KB (7515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8-jammy` - linux; ppc64le

```console
$ docker pull mariadb@sha256:1f04aef4b2d19b4ba8c833b0d60c216d6c077158aa33b14f02e057d7edf16c3a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.9 MB (127901997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fff19fe85fc19d84e05f676f7927e975eca043b0f8418d9435ace8adf9635af5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:17 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:18 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:21 GMT
ADD file:e75f08a67f0576b5441bb2fe454cad4b5b31a9d4efea23be791af62e1e0c712f in / 
# Tue, 25 Apr 2023 17:30:21 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 14:29:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 14:29:33 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 14:29:33 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 14:30:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 14:30:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 14:30:21 GMT
ENV LANG=C.UTF-8
# Thu, 04 May 2023 14:36:23 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.8.7 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 04 May 2023 14:36:23 GMT
ARG MARIADB_MAJOR=10.8
# Thu, 04 May 2023 14:36:24 GMT
ENV MARIADB_MAJOR=10.8
# Thu, 04 May 2023 14:36:25 GMT
ARG MARIADB_VERSION=1:10.8.7+maria~ubu2204
# Thu, 04 May 2023 14:36:25 GMT
ENV MARIADB_VERSION=1:10.8.7+maria~ubu2204
# Thu, 04 May 2023 14:36:26 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.7/repo/ubuntu/ jammy main
# Thu, 04 May 2023 14:36:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.7/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 04 May 2023 14:37:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.7/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 04 May 2023 14:37:29 GMT
VOLUME [/var/lib/mysql]
# Thu, 04 May 2023 14:37:29 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 04 May 2023 14:37:30 GMT
COPY file:ebdfbcbc74dda1874f1c75d86e1c32733edb402d13440b2b7140a952010bc21f in /usr/local/bin/ 
# Thu, 04 May 2023 14:37:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 May 2023 14:37:30 GMT
EXPOSE 3306
# Thu, 04 May 2023 14:37:31 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:f6a63d8cd043e76933823b18cbb7057a55bb4d66d64639c81e15a4700c101582`  
		Last Modified: Wed, 03 May 2023 17:09:07 GMT  
		Size: 35.7 MB (35712706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df46cdfc9a45a40dd254c1a0f2ccb2b0020e6852a5fb101d44d79250da5ddc69`  
		Last Modified: Thu, 04 May 2023 14:38:11 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11d1aa00f5a23d7276d6c701876911c79820fef6401156510e68eecb03012091`  
		Last Modified: Thu, 04 May 2023 14:38:12 GMT  
		Size: 6.0 MB (6021655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ec0fb2f57daffaea6b67a61d9012d55d4fcef64766481235d00d0438513793b`  
		Last Modified: Thu, 04 May 2023 14:38:08 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08cfaf41665f3a11466489fa4332df8fc382accf2d4a45319f4c250fd2156a70`  
		Last Modified: Thu, 04 May 2023 14:40:55 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ed2fcff548b07dc439eda80da108a1d53203f5d86d3f0de78d23a2e909c7dc6`  
		Last Modified: Thu, 04 May 2023 14:41:18 GMT  
		Size: 86.2 MB (86154912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e872108202c7d6442cf1512b325bfdc4680d3fbabba5a34c2a63e63a21a78325`  
		Last Modified: Thu, 04 May 2023 14:40:55 GMT  
		Size: 3.5 KB (3526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:494ee9af52d7390c87b779cbc83c2873316efb23a25e517fb55c9fda0ea0e702`  
		Last Modified: Thu, 04 May 2023 14:40:55 GMT  
		Size: 7.0 KB (6972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8-jammy` - linux; s390x

```console
$ docker pull mariadb@sha256:b92f82557df3713441544fecc9f714c2c686d731ebc969bdd6e975bd7f04ed14
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.8 MB (116777515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cca63cef0ab6c4e52a0ab56de7ab6eb113dd41788afc557c4e056b20aec13ba7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 26 Jan 2023 05:08:35 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:08:35 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:08:36 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:08:36 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:08:37 GMT
ADD file:a9794efc1a102ab6a7160e660a63f4b267797b8b7e0b0bfd9c04ed62846cfb36 in / 
# Thu, 26 Jan 2023 05:08:38 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:42:50 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 31 Jan 2023 18:42:50 GMT
ENV GOSU_VERSION=1.14
# Tue, 31 Jan 2023 18:42:50 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 31 Jan 2023 18:43:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 31 Jan 2023 18:43:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 31 Jan 2023 18:43:06 GMT
ENV LANG=C.UTF-8
# Tue, 07 Feb 2023 01:48:05 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.8.7 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 07 Feb 2023 01:48:05 GMT
ARG MARIADB_MAJOR=10.8
# Tue, 07 Feb 2023 01:48:05 GMT
ENV MARIADB_MAJOR=10.8
# Tue, 07 Feb 2023 01:48:06 GMT
ARG MARIADB_VERSION=1:10.8.7+maria~ubu2204
# Tue, 07 Feb 2023 01:48:06 GMT
ENV MARIADB_VERSION=1:10.8.7+maria~ubu2204
# Tue, 07 Feb 2023 01:48:06 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.7/repo/ubuntu/ jammy main
# Tue, 07 Feb 2023 01:48:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.7/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Feb 2023 01:48:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.7/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 07 Feb 2023 01:48:44 GMT
VOLUME [/var/lib/mysql]
# Sat, 25 Feb 2023 04:00:50 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Sat, 25 Feb 2023 04:00:50 GMT
COPY file:ebdfbcbc74dda1874f1c75d86e1c32733edb402d13440b2b7140a952010bc21f in /usr/local/bin/ 
# Sat, 25 Feb 2023 04:00:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 25 Feb 2023 04:00:50 GMT
EXPOSE 3306
# Sat, 25 Feb 2023 04:00:50 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:dd969ed9de43018fe5442c859bf66eabf23145b966b9338392ea707aed18b26f`  
		Last Modified: Tue, 31 Jan 2023 17:55:34 GMT  
		Size: 28.6 MB (28641926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b702438b56d7a6aaaad49e2be85e1bb2f3beb85406f6b9db1a232f798c558b3`  
		Last Modified: Tue, 31 Jan 2023 18:48:25 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60737998d0295bde808ca8856933482817ca605937f714f3cfca1ab0b4ca99ed`  
		Last Modified: Tue, 31 Jan 2023 18:48:26 GMT  
		Size: 5.4 MB (5401827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6e12a0288bb0803aeb23e581ca842e1fdf826fa28b4a730dd83585ea125ff8`  
		Last Modified: Tue, 31 Jan 2023 18:48:24 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a521985064ee3063bb3cd2edc44453d254baed98cb527acbdfaecb2fc3417952`  
		Last Modified: Tue, 07 Feb 2023 01:53:42 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43022d2479b063053f0a4f7cfa2e7d4164662db2e5a91351a42e8e24b146eddd`  
		Last Modified: Tue, 07 Feb 2023 01:53:53 GMT  
		Size: 82.7 MB (82721043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07535bc5dbd54e6b2ce7a722cecfc8c143d9d0750f01cd711da909c77485e949`  
		Last Modified: Sat, 25 Feb 2023 04:02:56 GMT  
		Size: 3.5 KB (3523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83b93a94d7abb56931fa6e741b37f71223e88ab92cc631aef69abec58fa5632`  
		Last Modified: Sat, 25 Feb 2023 04:02:55 GMT  
		Size: 7.0 KB (6969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.8.8`

```console
$ docker pull mariadb@sha256:cd5ba5f0a63b022aae3494a923e0daba2b25d9a8945a0230cda75b298f98af4c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mariadb:10.8.8` - linux; amd64

```console
$ docker pull mariadb@sha256:a3b3746dc60ab692c1e8116afdc36977c99e1196bc2c0253cc7ea9bed8f2a84f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.3 MB (119326364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91a5024e053f9e04c27f81a94c360d0fa172ffde9591d12cfe3b96419cbc69c0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 07:52:03 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 07:52:03 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 07:52:03 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 07:52:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 07:52:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 07:52:19 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:54:59 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.8.8 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:54:59 GMT
ARG MARIADB_MAJOR=10.8
# Thu, 11 May 2023 22:54:59 GMT
ENV MARIADB_MAJOR=10.8
# Thu, 11 May 2023 22:54:59 GMT
ARG MARIADB_VERSION=1:10.8.8+maria~ubu2204
# Thu, 11 May 2023 22:54:59 GMT
ENV MARIADB_VERSION=1:10.8.8+maria~ubu2204
# Thu, 11 May 2023 22:55:00 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.8/repo/ubuntu/ jammy main
# Thu, 11 May 2023 22:55:00 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.8/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:55:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.8/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:55:17 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:55:18 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:55:18 GMT
COPY file:94a071210c811522ac7cb9cd9b6d33b1df5eb056971fbdeefa8e9bc2e8a2d629 in /usr/local/bin/ 
# Thu, 11 May 2023 22:55:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:55:18 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:55:18 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:1bc677758ad7fa4503417ae5be18809c5a8679b5b36fcd1464d5a8e41cb13305`  
		Last Modified: Tue, 25 Apr 2023 22:54:44 GMT  
		Size: 30.4 MB (30430220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196e1740aea41b9915498de02cc132de54583dad1a212d06c9f6eb4690e1e0cb`  
		Last Modified: Thu, 04 May 2023 07:54:52 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4df0997938e5fd755403145484e1253115d3739285c704f562cf3bd6d89ec8`  
		Last Modified: Thu, 04 May 2023 07:54:53 GMT  
		Size: 5.6 MB (5595975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa4e41848249471f699386db900347fa61b39622dfba140344d9c51b264e7db`  
		Last Modified: Thu, 04 May 2023 07:54:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49e668d986b90318149d51109182a73222ad43b6b3e481eaf5d441cab78559d`  
		Last Modified: Thu, 11 May 2023 22:59:22 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cc871714a591c2a3250454c26604f654409930c77c8a3717eb0073e1e0e718e`  
		Last Modified: Thu, 11 May 2023 22:59:34 GMT  
		Size: 83.3 MB (83286903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c7a49739d5940a004b85da792032e062b7d03f4c0efe09b2961508b8b3cb63e`  
		Last Modified: Thu, 11 May 2023 22:59:23 GMT  
		Size: 3.5 KB (3526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1abfccf36f9db1fdfaefcf6054d581545cf4ea012707bb11f41a1ed18adfc9f7`  
		Last Modified: Thu, 11 May 2023 22:59:23 GMT  
		Size: 7.5 KB (7515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8.8` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:921e80a9b908dd181ce2d5bf6a98fabdc515eecc8a507a51e3dc845ae32b0792
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.9 MB (113914811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc532e8de402f89ad865a711e6235f267442512f7ef485090d3a150b2f8399ee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 03:46:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 03:46:08 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 03:46:08 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 03:46:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 03:46:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 03:46:28 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:38:39 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.8.8 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:38:40 GMT
ARG MARIADB_MAJOR=10.8
# Thu, 11 May 2023 22:38:40 GMT
ENV MARIADB_MAJOR=10.8
# Thu, 11 May 2023 22:38:40 GMT
ARG MARIADB_VERSION=1:10.8.8+maria~ubu2204
# Thu, 11 May 2023 22:38:40 GMT
ENV MARIADB_VERSION=1:10.8.8+maria~ubu2204
# Thu, 11 May 2023 22:38:40 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.8/repo/ubuntu/ jammy main
# Thu, 11 May 2023 22:38:40 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.8/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:38:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.8/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:38:58 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:38:58 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:38:59 GMT
COPY file:94a071210c811522ac7cb9cd9b6d33b1df5eb056971fbdeefa8e9bc2e8a2d629 in /usr/local/bin/ 
# Thu, 11 May 2023 22:38:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:38:59 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:38:59 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:f3f60f415e9a03eed88bd5dd5268c841cde08dacf16911a3ef1e4e0fcdd76568`  
		Last Modified: Wed, 26 Apr 2023 02:08:37 GMT  
		Size: 28.4 MB (28389440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bfb87016de46ece16208cd39b5fa89740b8e8db147c2da2f6483551b3e8d521`  
		Last Modified: Thu, 04 May 2023 03:49:02 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8bd3f48f8f1fc94a1a143132ba91e005df50ee4327d0e209553cc89145a91f`  
		Last Modified: Thu, 04 May 2023 03:49:03 GMT  
		Size: 5.4 MB (5409831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ebb0502bf43d03d32f27b6cfa9ea349e89bccb62bd1ef3cf96a9a769e6c1fa`  
		Last Modified: Thu, 04 May 2023 03:49:00 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9ae9fcfb680e43985085538f34194a9a0d84f3e12417a217b6844374a73e2b`  
		Last Modified: Thu, 11 May 2023 22:42:48 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:594723f411cfaf9d0917e9fb5bf0f7391d81e93de1d2fc5436a97359125e62a2`  
		Last Modified: Thu, 11 May 2023 22:42:56 GMT  
		Size: 80.1 MB (80102275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a02297f142711ade1e6c84bf8116721de20651ad48a4ba847b6726dd9ee20687`  
		Last Modified: Thu, 11 May 2023 22:42:47 GMT  
		Size: 3.5 KB (3526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28b2d7c377aef74345f95ce57ed6659d928f08a59e02708e2244f93204b75442`  
		Last Modified: Thu, 11 May 2023 22:42:47 GMT  
		Size: 7.5 KB (7515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.8.8-jammy`

```console
$ docker pull mariadb@sha256:cd5ba5f0a63b022aae3494a923e0daba2b25d9a8945a0230cda75b298f98af4c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mariadb:10.8.8-jammy` - linux; amd64

```console
$ docker pull mariadb@sha256:a3b3746dc60ab692c1e8116afdc36977c99e1196bc2c0253cc7ea9bed8f2a84f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.3 MB (119326364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91a5024e053f9e04c27f81a94c360d0fa172ffde9591d12cfe3b96419cbc69c0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 07:52:03 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 07:52:03 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 07:52:03 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 07:52:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 07:52:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 07:52:19 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:54:59 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.8.8 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:54:59 GMT
ARG MARIADB_MAJOR=10.8
# Thu, 11 May 2023 22:54:59 GMT
ENV MARIADB_MAJOR=10.8
# Thu, 11 May 2023 22:54:59 GMT
ARG MARIADB_VERSION=1:10.8.8+maria~ubu2204
# Thu, 11 May 2023 22:54:59 GMT
ENV MARIADB_VERSION=1:10.8.8+maria~ubu2204
# Thu, 11 May 2023 22:55:00 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.8/repo/ubuntu/ jammy main
# Thu, 11 May 2023 22:55:00 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.8/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:55:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.8/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:55:17 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:55:18 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:55:18 GMT
COPY file:94a071210c811522ac7cb9cd9b6d33b1df5eb056971fbdeefa8e9bc2e8a2d629 in /usr/local/bin/ 
# Thu, 11 May 2023 22:55:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:55:18 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:55:18 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:1bc677758ad7fa4503417ae5be18809c5a8679b5b36fcd1464d5a8e41cb13305`  
		Last Modified: Tue, 25 Apr 2023 22:54:44 GMT  
		Size: 30.4 MB (30430220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196e1740aea41b9915498de02cc132de54583dad1a212d06c9f6eb4690e1e0cb`  
		Last Modified: Thu, 04 May 2023 07:54:52 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4df0997938e5fd755403145484e1253115d3739285c704f562cf3bd6d89ec8`  
		Last Modified: Thu, 04 May 2023 07:54:53 GMT  
		Size: 5.6 MB (5595975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa4e41848249471f699386db900347fa61b39622dfba140344d9c51b264e7db`  
		Last Modified: Thu, 04 May 2023 07:54:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49e668d986b90318149d51109182a73222ad43b6b3e481eaf5d441cab78559d`  
		Last Modified: Thu, 11 May 2023 22:59:22 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cc871714a591c2a3250454c26604f654409930c77c8a3717eb0073e1e0e718e`  
		Last Modified: Thu, 11 May 2023 22:59:34 GMT  
		Size: 83.3 MB (83286903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c7a49739d5940a004b85da792032e062b7d03f4c0efe09b2961508b8b3cb63e`  
		Last Modified: Thu, 11 May 2023 22:59:23 GMT  
		Size: 3.5 KB (3526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1abfccf36f9db1fdfaefcf6054d581545cf4ea012707bb11f41a1ed18adfc9f7`  
		Last Modified: Thu, 11 May 2023 22:59:23 GMT  
		Size: 7.5 KB (7515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8.8-jammy` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:921e80a9b908dd181ce2d5bf6a98fabdc515eecc8a507a51e3dc845ae32b0792
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.9 MB (113914811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc532e8de402f89ad865a711e6235f267442512f7ef485090d3a150b2f8399ee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 03:46:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 03:46:08 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 03:46:08 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 03:46:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 03:46:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 03:46:28 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:38:39 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.8.8 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:38:40 GMT
ARG MARIADB_MAJOR=10.8
# Thu, 11 May 2023 22:38:40 GMT
ENV MARIADB_MAJOR=10.8
# Thu, 11 May 2023 22:38:40 GMT
ARG MARIADB_VERSION=1:10.8.8+maria~ubu2204
# Thu, 11 May 2023 22:38:40 GMT
ENV MARIADB_VERSION=1:10.8.8+maria~ubu2204
# Thu, 11 May 2023 22:38:40 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.8/repo/ubuntu/ jammy main
# Thu, 11 May 2023 22:38:40 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.8/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:38:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.8/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:38:58 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:38:58 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:38:59 GMT
COPY file:94a071210c811522ac7cb9cd9b6d33b1df5eb056971fbdeefa8e9bc2e8a2d629 in /usr/local/bin/ 
# Thu, 11 May 2023 22:38:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:38:59 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:38:59 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:f3f60f415e9a03eed88bd5dd5268c841cde08dacf16911a3ef1e4e0fcdd76568`  
		Last Modified: Wed, 26 Apr 2023 02:08:37 GMT  
		Size: 28.4 MB (28389440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bfb87016de46ece16208cd39b5fa89740b8e8db147c2da2f6483551b3e8d521`  
		Last Modified: Thu, 04 May 2023 03:49:02 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8bd3f48f8f1fc94a1a143132ba91e005df50ee4327d0e209553cc89145a91f`  
		Last Modified: Thu, 04 May 2023 03:49:03 GMT  
		Size: 5.4 MB (5409831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ebb0502bf43d03d32f27b6cfa9ea349e89bccb62bd1ef3cf96a9a769e6c1fa`  
		Last Modified: Thu, 04 May 2023 03:49:00 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9ae9fcfb680e43985085538f34194a9a0d84f3e12417a217b6844374a73e2b`  
		Last Modified: Thu, 11 May 2023 22:42:48 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:594723f411cfaf9d0917e9fb5bf0f7391d81e93de1d2fc5436a97359125e62a2`  
		Last Modified: Thu, 11 May 2023 22:42:56 GMT  
		Size: 80.1 MB (80102275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a02297f142711ade1e6c84bf8116721de20651ad48a4ba847b6726dd9ee20687`  
		Last Modified: Thu, 11 May 2023 22:42:47 GMT  
		Size: 3.5 KB (3526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28b2d7c377aef74345f95ce57ed6659d928f08a59e02708e2244f93204b75442`  
		Last Modified: Thu, 11 May 2023 22:42:47 GMT  
		Size: 7.5 KB (7515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.9`

```console
$ docker pull mariadb@sha256:c6800adbd095f2fb3bc3ae59d189755166595c1ef42fe32b3da421f6d69b2fa2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.9` - linux; amd64

```console
$ docker pull mariadb@sha256:1bbd4b8a0cca7b9c8ef2cfceca9582e160c667a82c134bc580b9d2c73f6fa297
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.4 MB (119400307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4076abc3d9d65253fa06f2c39365686780123a0c7ebcd3fb0e4916b6db00dc67`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 07:52:03 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 07:52:03 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 07:52:03 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 07:52:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 07:52:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 07:52:19 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:54:36 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.9.6 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:54:36 GMT
ARG MARIADB_VERSION=1:10.9.6+maria~ubu2204
# Thu, 11 May 2023 22:54:36 GMT
ENV MARIADB_VERSION=1:10.9.6+maria~ubu2204
# Thu, 11 May 2023 22:54:36 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.6/repo/ubuntu/ jammy main
# Thu, 11 May 2023 22:54:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.6/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:54:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.6/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:54:54 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:54:54 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:54:54 GMT
COPY file:94a071210c811522ac7cb9cd9b6d33b1df5eb056971fbdeefa8e9bc2e8a2d629 in /usr/local/bin/ 
# Thu, 11 May 2023 22:54:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:54:54 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:54:54 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:1bc677758ad7fa4503417ae5be18809c5a8679b5b36fcd1464d5a8e41cb13305`  
		Last Modified: Tue, 25 Apr 2023 22:54:44 GMT  
		Size: 30.4 MB (30430220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196e1740aea41b9915498de02cc132de54583dad1a212d06c9f6eb4690e1e0cb`  
		Last Modified: Thu, 04 May 2023 07:54:52 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4df0997938e5fd755403145484e1253115d3739285c704f562cf3bd6d89ec8`  
		Last Modified: Thu, 04 May 2023 07:54:53 GMT  
		Size: 5.6 MB (5595975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa4e41848249471f699386db900347fa61b39622dfba140344d9c51b264e7db`  
		Last Modified: Thu, 04 May 2023 07:54:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ac2d3b46fd64af7e90a89f270773b33d74514b9f634f18258776fbfd7c6bd1d`  
		Last Modified: Thu, 11 May 2023 22:58:59 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f7204e4367d7d18cd01bfc9b225102d3793392998e1e98622578659c7b6aa4`  
		Last Modified: Thu, 11 May 2023 22:59:10 GMT  
		Size: 83.4 MB (83360849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9757240e491172cbe025fb85afaac9890815fa635d426f6e098d5e6ed91d747c`  
		Last Modified: Thu, 11 May 2023 22:58:59 GMT  
		Size: 3.5 KB (3525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdffa7896ef0eee2b8dbd7ffb08520e9e07b47a51c530564315cb5b1739d9f46`  
		Last Modified: Thu, 11 May 2023 22:58:59 GMT  
		Size: 7.5 KB (7514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.9` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:359439cad072caa3eb08b44ac60d322b55ae83f1a7e8436f9a39183be6b2ba26
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (113979112 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a96a720da688aa8ee4361bfcf6a7a6fff7371bd02600f8b929bc9486f02a0ee8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 03:46:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 03:46:08 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 03:46:08 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 03:46:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 03:46:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 03:46:28 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:38:16 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.9.6 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:38:16 GMT
ARG MARIADB_VERSION=1:10.9.6+maria~ubu2204
# Thu, 11 May 2023 22:38:17 GMT
ENV MARIADB_VERSION=1:10.9.6+maria~ubu2204
# Thu, 11 May 2023 22:38:17 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.6/repo/ubuntu/ jammy main
# Thu, 11 May 2023 22:38:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.6/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:38:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.6/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:38:35 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:38:35 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:38:35 GMT
COPY file:94a071210c811522ac7cb9cd9b6d33b1df5eb056971fbdeefa8e9bc2e8a2d629 in /usr/local/bin/ 
# Thu, 11 May 2023 22:38:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:38:35 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:38:35 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:f3f60f415e9a03eed88bd5dd5268c841cde08dacf16911a3ef1e4e0fcdd76568`  
		Last Modified: Wed, 26 Apr 2023 02:08:37 GMT  
		Size: 28.4 MB (28389440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bfb87016de46ece16208cd39b5fa89740b8e8db147c2da2f6483551b3e8d521`  
		Last Modified: Thu, 04 May 2023 03:49:02 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8bd3f48f8f1fc94a1a143132ba91e005df50ee4327d0e209553cc89145a91f`  
		Last Modified: Thu, 04 May 2023 03:49:03 GMT  
		Size: 5.4 MB (5409831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ebb0502bf43d03d32f27b6cfa9ea349e89bccb62bd1ef3cf96a9a769e6c1fa`  
		Last Modified: Thu, 04 May 2023 03:49:00 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e71be3203371bc838f308b37c6191c81d6e4b9d1f80eb9ab8af5c758931c0e4`  
		Last Modified: Thu, 11 May 2023 22:42:27 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79fd566f0f92301f68512080c230b09d076fc0a1fb2ba3eb323b97f688d1423a`  
		Last Modified: Thu, 11 May 2023 22:42:35 GMT  
		Size: 80.2 MB (80166574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a4eaa7924e745081a848d3c916211ebb639ee4a2a55bc9d48cc10a5cd425163`  
		Last Modified: Thu, 11 May 2023 22:42:26 GMT  
		Size: 3.5 KB (3526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aefd1736befe72cd3e30b7c72cc07f832de8b42a576c89af447f0ec2546246cf`  
		Last Modified: Thu, 11 May 2023 22:42:26 GMT  
		Size: 7.5 KB (7515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.9` - linux; ppc64le

```console
$ docker pull mariadb@sha256:6130d631e7edfac2f9d7668e3c3800a6f1b9aa87ed5c108621254864020dc5ac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.0 MB (127954665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef0e99473faf550e550b63fa42737349bdc06c679eab5b921c27d9be8c309fb6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:17 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:18 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:21 GMT
ADD file:e75f08a67f0576b5441bb2fe454cad4b5b31a9d4efea23be791af62e1e0c712f in / 
# Tue, 25 Apr 2023 17:30:21 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 14:29:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 14:29:33 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 14:29:33 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 14:30:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 14:30:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 14:30:21 GMT
ENV LANG=C.UTF-8
# Thu, 04 May 2023 14:34:59 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.9.5 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 04 May 2023 14:34:59 GMT
ARG MARIADB_VERSION=1:10.9.5+maria~ubu2204
# Thu, 04 May 2023 14:35:00 GMT
ENV MARIADB_VERSION=1:10.9.5+maria~ubu2204
# Thu, 04 May 2023 14:35:00 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.5/repo/ubuntu/ jammy main
# Thu, 04 May 2023 14:35:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.5/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 04 May 2023 14:36:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.5/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 04 May 2023 14:36:07 GMT
VOLUME [/var/lib/mysql]
# Thu, 04 May 2023 14:36:08 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 04 May 2023 14:36:09 GMT
COPY file:ebdfbcbc74dda1874f1c75d86e1c32733edb402d13440b2b7140a952010bc21f in /usr/local/bin/ 
# Thu, 04 May 2023 14:36:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 May 2023 14:36:10 GMT
EXPOSE 3306
# Thu, 04 May 2023 14:36:11 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:f6a63d8cd043e76933823b18cbb7057a55bb4d66d64639c81e15a4700c101582`  
		Last Modified: Wed, 03 May 2023 17:09:07 GMT  
		Size: 35.7 MB (35712706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df46cdfc9a45a40dd254c1a0f2ccb2b0020e6852a5fb101d44d79250da5ddc69`  
		Last Modified: Thu, 04 May 2023 14:38:11 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11d1aa00f5a23d7276d6c701876911c79820fef6401156510e68eecb03012091`  
		Last Modified: Thu, 04 May 2023 14:38:12 GMT  
		Size: 6.0 MB (6021655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ec0fb2f57daffaea6b67a61d9012d55d4fcef64766481235d00d0438513793b`  
		Last Modified: Thu, 04 May 2023 14:38:08 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61127d91d4cc1f181a1f269ca4c7939d3d0ab5d9087bfe31ea6aef7642153037`  
		Last Modified: Thu, 04 May 2023 14:40:18 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:225bbdccde46808924922d5cf217b517f1f45a5b199fd36d045dee82c5a832a2`  
		Last Modified: Thu, 04 May 2023 14:40:41 GMT  
		Size: 86.2 MB (86207580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b74ef83bf5c842e1603eaa856d2e512252e529ab47be3c29e2c7b14b117e2553`  
		Last Modified: Thu, 04 May 2023 14:40:18 GMT  
		Size: 3.5 KB (3525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:826aeb447b7264cf9d6c64d7475eb32921acd92acdbd4dfe79d9134e7feba091`  
		Last Modified: Thu, 04 May 2023 14:40:18 GMT  
		Size: 7.0 KB (6971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.9` - linux; s390x

```console
$ docker pull mariadb@sha256:9a3420caeed1470c3d4a4e596be0c7e127a0a68ab480e736a68b6e018a13a35b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.9 MB (116862787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c9892bc7fe4e3c78e07bb22afac5365aac96fb6bec9b87aac7a65a150fc9802`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 26 Jan 2023 05:08:35 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:08:35 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:08:36 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:08:36 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:08:37 GMT
ADD file:a9794efc1a102ab6a7160e660a63f4b267797b8b7e0b0bfd9c04ed62846cfb36 in / 
# Thu, 26 Jan 2023 05:08:38 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:42:50 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 31 Jan 2023 18:42:50 GMT
ENV GOSU_VERSION=1.14
# Tue, 31 Jan 2023 18:42:50 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 31 Jan 2023 18:43:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 31 Jan 2023 18:43:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 31 Jan 2023 18:43:06 GMT
ENV LANG=C.UTF-8
# Tue, 07 Feb 2023 01:46:31 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.9.5 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 07 Feb 2023 01:46:31 GMT
ARG MARIADB_VERSION=1:10.9.5+maria~ubu2204
# Tue, 07 Feb 2023 01:46:31 GMT
ENV MARIADB_VERSION=1:10.9.5+maria~ubu2204
# Tue, 07 Feb 2023 01:46:31 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.5/repo/ubuntu/ jammy main
# Tue, 07 Feb 2023 01:46:31 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.5/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Feb 2023 01:47:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.5/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 07 Feb 2023 01:47:55 GMT
VOLUME [/var/lib/mysql]
# Sat, 25 Feb 2023 04:00:44 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Sat, 25 Feb 2023 04:00:44 GMT
COPY file:ebdfbcbc74dda1874f1c75d86e1c32733edb402d13440b2b7140a952010bc21f in /usr/local/bin/ 
# Sat, 25 Feb 2023 04:00:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 25 Feb 2023 04:00:44 GMT
EXPOSE 3306
# Sat, 25 Feb 2023 04:00:44 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:dd969ed9de43018fe5442c859bf66eabf23145b966b9338392ea707aed18b26f`  
		Last Modified: Tue, 31 Jan 2023 17:55:34 GMT  
		Size: 28.6 MB (28641926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b702438b56d7a6aaaad49e2be85e1bb2f3beb85406f6b9db1a232f798c558b3`  
		Last Modified: Tue, 31 Jan 2023 18:48:25 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60737998d0295bde808ca8856933482817ca605937f714f3cfca1ab0b4ca99ed`  
		Last Modified: Tue, 31 Jan 2023 18:48:26 GMT  
		Size: 5.4 MB (5401827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6e12a0288bb0803aeb23e581ca842e1fdf826fa28b4a730dd83585ea125ff8`  
		Last Modified: Tue, 31 Jan 2023 18:48:24 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bd9f37d6077bd4d53c1025b28b34b11f3914692580487a0c8a8543db52b49ec`  
		Last Modified: Tue, 07 Feb 2023 01:53:20 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef21e6e5463c9bc6dc2becf5d96956d56591411fc7fca77a15677bd1813dc27`  
		Last Modified: Tue, 07 Feb 2023 01:53:31 GMT  
		Size: 82.8 MB (82806308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f10acebb01fdb2c03f4103f2f610a229b1dddd5a561f8b7d73bb81cdb65078a4`  
		Last Modified: Sat, 25 Feb 2023 04:02:45 GMT  
		Size: 3.5 KB (3527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9039abe8d8aff0067a7617d29ee388aeda386ba0b61bf2b99ced5f00a69769f1`  
		Last Modified: Sat, 25 Feb 2023 04:02:45 GMT  
		Size: 7.0 KB (6972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.9-jammy`

```console
$ docker pull mariadb@sha256:c6800adbd095f2fb3bc3ae59d189755166595c1ef42fe32b3da421f6d69b2fa2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.9-jammy` - linux; amd64

```console
$ docker pull mariadb@sha256:1bbd4b8a0cca7b9c8ef2cfceca9582e160c667a82c134bc580b9d2c73f6fa297
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.4 MB (119400307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4076abc3d9d65253fa06f2c39365686780123a0c7ebcd3fb0e4916b6db00dc67`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 07:52:03 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 07:52:03 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 07:52:03 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 07:52:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 07:52:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 07:52:19 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:54:36 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.9.6 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:54:36 GMT
ARG MARIADB_VERSION=1:10.9.6+maria~ubu2204
# Thu, 11 May 2023 22:54:36 GMT
ENV MARIADB_VERSION=1:10.9.6+maria~ubu2204
# Thu, 11 May 2023 22:54:36 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.6/repo/ubuntu/ jammy main
# Thu, 11 May 2023 22:54:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.6/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:54:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.6/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:54:54 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:54:54 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:54:54 GMT
COPY file:94a071210c811522ac7cb9cd9b6d33b1df5eb056971fbdeefa8e9bc2e8a2d629 in /usr/local/bin/ 
# Thu, 11 May 2023 22:54:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:54:54 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:54:54 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:1bc677758ad7fa4503417ae5be18809c5a8679b5b36fcd1464d5a8e41cb13305`  
		Last Modified: Tue, 25 Apr 2023 22:54:44 GMT  
		Size: 30.4 MB (30430220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196e1740aea41b9915498de02cc132de54583dad1a212d06c9f6eb4690e1e0cb`  
		Last Modified: Thu, 04 May 2023 07:54:52 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4df0997938e5fd755403145484e1253115d3739285c704f562cf3bd6d89ec8`  
		Last Modified: Thu, 04 May 2023 07:54:53 GMT  
		Size: 5.6 MB (5595975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa4e41848249471f699386db900347fa61b39622dfba140344d9c51b264e7db`  
		Last Modified: Thu, 04 May 2023 07:54:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ac2d3b46fd64af7e90a89f270773b33d74514b9f634f18258776fbfd7c6bd1d`  
		Last Modified: Thu, 11 May 2023 22:58:59 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f7204e4367d7d18cd01bfc9b225102d3793392998e1e98622578659c7b6aa4`  
		Last Modified: Thu, 11 May 2023 22:59:10 GMT  
		Size: 83.4 MB (83360849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9757240e491172cbe025fb85afaac9890815fa635d426f6e098d5e6ed91d747c`  
		Last Modified: Thu, 11 May 2023 22:58:59 GMT  
		Size: 3.5 KB (3525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdffa7896ef0eee2b8dbd7ffb08520e9e07b47a51c530564315cb5b1739d9f46`  
		Last Modified: Thu, 11 May 2023 22:58:59 GMT  
		Size: 7.5 KB (7514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.9-jammy` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:359439cad072caa3eb08b44ac60d322b55ae83f1a7e8436f9a39183be6b2ba26
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (113979112 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a96a720da688aa8ee4361bfcf6a7a6fff7371bd02600f8b929bc9486f02a0ee8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 03:46:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 03:46:08 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 03:46:08 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 03:46:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 03:46:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 03:46:28 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:38:16 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.9.6 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:38:16 GMT
ARG MARIADB_VERSION=1:10.9.6+maria~ubu2204
# Thu, 11 May 2023 22:38:17 GMT
ENV MARIADB_VERSION=1:10.9.6+maria~ubu2204
# Thu, 11 May 2023 22:38:17 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.6/repo/ubuntu/ jammy main
# Thu, 11 May 2023 22:38:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.6/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:38:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.6/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:38:35 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:38:35 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:38:35 GMT
COPY file:94a071210c811522ac7cb9cd9b6d33b1df5eb056971fbdeefa8e9bc2e8a2d629 in /usr/local/bin/ 
# Thu, 11 May 2023 22:38:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:38:35 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:38:35 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:f3f60f415e9a03eed88bd5dd5268c841cde08dacf16911a3ef1e4e0fcdd76568`  
		Last Modified: Wed, 26 Apr 2023 02:08:37 GMT  
		Size: 28.4 MB (28389440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bfb87016de46ece16208cd39b5fa89740b8e8db147c2da2f6483551b3e8d521`  
		Last Modified: Thu, 04 May 2023 03:49:02 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8bd3f48f8f1fc94a1a143132ba91e005df50ee4327d0e209553cc89145a91f`  
		Last Modified: Thu, 04 May 2023 03:49:03 GMT  
		Size: 5.4 MB (5409831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ebb0502bf43d03d32f27b6cfa9ea349e89bccb62bd1ef3cf96a9a769e6c1fa`  
		Last Modified: Thu, 04 May 2023 03:49:00 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e71be3203371bc838f308b37c6191c81d6e4b9d1f80eb9ab8af5c758931c0e4`  
		Last Modified: Thu, 11 May 2023 22:42:27 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79fd566f0f92301f68512080c230b09d076fc0a1fb2ba3eb323b97f688d1423a`  
		Last Modified: Thu, 11 May 2023 22:42:35 GMT  
		Size: 80.2 MB (80166574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a4eaa7924e745081a848d3c916211ebb639ee4a2a55bc9d48cc10a5cd425163`  
		Last Modified: Thu, 11 May 2023 22:42:26 GMT  
		Size: 3.5 KB (3526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aefd1736befe72cd3e30b7c72cc07f832de8b42a576c89af447f0ec2546246cf`  
		Last Modified: Thu, 11 May 2023 22:42:26 GMT  
		Size: 7.5 KB (7515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.9-jammy` - linux; ppc64le

```console
$ docker pull mariadb@sha256:6130d631e7edfac2f9d7668e3c3800a6f1b9aa87ed5c108621254864020dc5ac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.0 MB (127954665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef0e99473faf550e550b63fa42737349bdc06c679eab5b921c27d9be8c309fb6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:17 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:18 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:21 GMT
ADD file:e75f08a67f0576b5441bb2fe454cad4b5b31a9d4efea23be791af62e1e0c712f in / 
# Tue, 25 Apr 2023 17:30:21 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 14:29:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 14:29:33 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 14:29:33 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 14:30:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 14:30:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 14:30:21 GMT
ENV LANG=C.UTF-8
# Thu, 04 May 2023 14:34:59 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.9.5 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 04 May 2023 14:34:59 GMT
ARG MARIADB_VERSION=1:10.9.5+maria~ubu2204
# Thu, 04 May 2023 14:35:00 GMT
ENV MARIADB_VERSION=1:10.9.5+maria~ubu2204
# Thu, 04 May 2023 14:35:00 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.5/repo/ubuntu/ jammy main
# Thu, 04 May 2023 14:35:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.5/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 04 May 2023 14:36:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.5/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 04 May 2023 14:36:07 GMT
VOLUME [/var/lib/mysql]
# Thu, 04 May 2023 14:36:08 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 04 May 2023 14:36:09 GMT
COPY file:ebdfbcbc74dda1874f1c75d86e1c32733edb402d13440b2b7140a952010bc21f in /usr/local/bin/ 
# Thu, 04 May 2023 14:36:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 May 2023 14:36:10 GMT
EXPOSE 3306
# Thu, 04 May 2023 14:36:11 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:f6a63d8cd043e76933823b18cbb7057a55bb4d66d64639c81e15a4700c101582`  
		Last Modified: Wed, 03 May 2023 17:09:07 GMT  
		Size: 35.7 MB (35712706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df46cdfc9a45a40dd254c1a0f2ccb2b0020e6852a5fb101d44d79250da5ddc69`  
		Last Modified: Thu, 04 May 2023 14:38:11 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11d1aa00f5a23d7276d6c701876911c79820fef6401156510e68eecb03012091`  
		Last Modified: Thu, 04 May 2023 14:38:12 GMT  
		Size: 6.0 MB (6021655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ec0fb2f57daffaea6b67a61d9012d55d4fcef64766481235d00d0438513793b`  
		Last Modified: Thu, 04 May 2023 14:38:08 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61127d91d4cc1f181a1f269ca4c7939d3d0ab5d9087bfe31ea6aef7642153037`  
		Last Modified: Thu, 04 May 2023 14:40:18 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:225bbdccde46808924922d5cf217b517f1f45a5b199fd36d045dee82c5a832a2`  
		Last Modified: Thu, 04 May 2023 14:40:41 GMT  
		Size: 86.2 MB (86207580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b74ef83bf5c842e1603eaa856d2e512252e529ab47be3c29e2c7b14b117e2553`  
		Last Modified: Thu, 04 May 2023 14:40:18 GMT  
		Size: 3.5 KB (3525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:826aeb447b7264cf9d6c64d7475eb32921acd92acdbd4dfe79d9134e7feba091`  
		Last Modified: Thu, 04 May 2023 14:40:18 GMT  
		Size: 7.0 KB (6971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.9-jammy` - linux; s390x

```console
$ docker pull mariadb@sha256:9a3420caeed1470c3d4a4e596be0c7e127a0a68ab480e736a68b6e018a13a35b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.9 MB (116862787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c9892bc7fe4e3c78e07bb22afac5365aac96fb6bec9b87aac7a65a150fc9802`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 26 Jan 2023 05:08:35 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:08:35 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:08:36 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:08:36 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:08:37 GMT
ADD file:a9794efc1a102ab6a7160e660a63f4b267797b8b7e0b0bfd9c04ed62846cfb36 in / 
# Thu, 26 Jan 2023 05:08:38 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:42:50 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 31 Jan 2023 18:42:50 GMT
ENV GOSU_VERSION=1.14
# Tue, 31 Jan 2023 18:42:50 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 31 Jan 2023 18:43:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 31 Jan 2023 18:43:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 31 Jan 2023 18:43:06 GMT
ENV LANG=C.UTF-8
# Tue, 07 Feb 2023 01:46:31 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.9.5 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 07 Feb 2023 01:46:31 GMT
ARG MARIADB_VERSION=1:10.9.5+maria~ubu2204
# Tue, 07 Feb 2023 01:46:31 GMT
ENV MARIADB_VERSION=1:10.9.5+maria~ubu2204
# Tue, 07 Feb 2023 01:46:31 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.5/repo/ubuntu/ jammy main
# Tue, 07 Feb 2023 01:46:31 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.5/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Feb 2023 01:47:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.5/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 07 Feb 2023 01:47:55 GMT
VOLUME [/var/lib/mysql]
# Sat, 25 Feb 2023 04:00:44 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Sat, 25 Feb 2023 04:00:44 GMT
COPY file:ebdfbcbc74dda1874f1c75d86e1c32733edb402d13440b2b7140a952010bc21f in /usr/local/bin/ 
# Sat, 25 Feb 2023 04:00:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 25 Feb 2023 04:00:44 GMT
EXPOSE 3306
# Sat, 25 Feb 2023 04:00:44 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:dd969ed9de43018fe5442c859bf66eabf23145b966b9338392ea707aed18b26f`  
		Last Modified: Tue, 31 Jan 2023 17:55:34 GMT  
		Size: 28.6 MB (28641926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b702438b56d7a6aaaad49e2be85e1bb2f3beb85406f6b9db1a232f798c558b3`  
		Last Modified: Tue, 31 Jan 2023 18:48:25 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60737998d0295bde808ca8856933482817ca605937f714f3cfca1ab0b4ca99ed`  
		Last Modified: Tue, 31 Jan 2023 18:48:26 GMT  
		Size: 5.4 MB (5401827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6e12a0288bb0803aeb23e581ca842e1fdf826fa28b4a730dd83585ea125ff8`  
		Last Modified: Tue, 31 Jan 2023 18:48:24 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bd9f37d6077bd4d53c1025b28b34b11f3914692580487a0c8a8543db52b49ec`  
		Last Modified: Tue, 07 Feb 2023 01:53:20 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef21e6e5463c9bc6dc2becf5d96956d56591411fc7fca77a15677bd1813dc27`  
		Last Modified: Tue, 07 Feb 2023 01:53:31 GMT  
		Size: 82.8 MB (82806308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f10acebb01fdb2c03f4103f2f610a229b1dddd5a561f8b7d73bb81cdb65078a4`  
		Last Modified: Sat, 25 Feb 2023 04:02:45 GMT  
		Size: 3.5 KB (3527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9039abe8d8aff0067a7617d29ee388aeda386ba0b61bf2b99ced5f00a69769f1`  
		Last Modified: Sat, 25 Feb 2023 04:02:45 GMT  
		Size: 7.0 KB (6972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.9.6`

```console
$ docker pull mariadb@sha256:7b3391cae3039e32c71bfc221451dd83c9d08ecb81658a7bc3cbfe60af5d09e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mariadb:10.9.6` - linux; amd64

```console
$ docker pull mariadb@sha256:1bbd4b8a0cca7b9c8ef2cfceca9582e160c667a82c134bc580b9d2c73f6fa297
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.4 MB (119400307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4076abc3d9d65253fa06f2c39365686780123a0c7ebcd3fb0e4916b6db00dc67`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 07:52:03 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 07:52:03 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 07:52:03 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 07:52:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 07:52:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 07:52:19 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:54:36 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.9.6 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:54:36 GMT
ARG MARIADB_VERSION=1:10.9.6+maria~ubu2204
# Thu, 11 May 2023 22:54:36 GMT
ENV MARIADB_VERSION=1:10.9.6+maria~ubu2204
# Thu, 11 May 2023 22:54:36 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.6/repo/ubuntu/ jammy main
# Thu, 11 May 2023 22:54:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.6/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:54:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.6/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:54:54 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:54:54 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:54:54 GMT
COPY file:94a071210c811522ac7cb9cd9b6d33b1df5eb056971fbdeefa8e9bc2e8a2d629 in /usr/local/bin/ 
# Thu, 11 May 2023 22:54:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:54:54 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:54:54 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:1bc677758ad7fa4503417ae5be18809c5a8679b5b36fcd1464d5a8e41cb13305`  
		Last Modified: Tue, 25 Apr 2023 22:54:44 GMT  
		Size: 30.4 MB (30430220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196e1740aea41b9915498de02cc132de54583dad1a212d06c9f6eb4690e1e0cb`  
		Last Modified: Thu, 04 May 2023 07:54:52 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4df0997938e5fd755403145484e1253115d3739285c704f562cf3bd6d89ec8`  
		Last Modified: Thu, 04 May 2023 07:54:53 GMT  
		Size: 5.6 MB (5595975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa4e41848249471f699386db900347fa61b39622dfba140344d9c51b264e7db`  
		Last Modified: Thu, 04 May 2023 07:54:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ac2d3b46fd64af7e90a89f270773b33d74514b9f634f18258776fbfd7c6bd1d`  
		Last Modified: Thu, 11 May 2023 22:58:59 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f7204e4367d7d18cd01bfc9b225102d3793392998e1e98622578659c7b6aa4`  
		Last Modified: Thu, 11 May 2023 22:59:10 GMT  
		Size: 83.4 MB (83360849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9757240e491172cbe025fb85afaac9890815fa635d426f6e098d5e6ed91d747c`  
		Last Modified: Thu, 11 May 2023 22:58:59 GMT  
		Size: 3.5 KB (3525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdffa7896ef0eee2b8dbd7ffb08520e9e07b47a51c530564315cb5b1739d9f46`  
		Last Modified: Thu, 11 May 2023 22:58:59 GMT  
		Size: 7.5 KB (7514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.9.6` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:359439cad072caa3eb08b44ac60d322b55ae83f1a7e8436f9a39183be6b2ba26
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (113979112 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a96a720da688aa8ee4361bfcf6a7a6fff7371bd02600f8b929bc9486f02a0ee8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 03:46:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 03:46:08 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 03:46:08 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 03:46:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 03:46:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 03:46:28 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:38:16 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.9.6 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:38:16 GMT
ARG MARIADB_VERSION=1:10.9.6+maria~ubu2204
# Thu, 11 May 2023 22:38:17 GMT
ENV MARIADB_VERSION=1:10.9.6+maria~ubu2204
# Thu, 11 May 2023 22:38:17 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.6/repo/ubuntu/ jammy main
# Thu, 11 May 2023 22:38:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.6/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:38:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.6/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:38:35 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:38:35 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:38:35 GMT
COPY file:94a071210c811522ac7cb9cd9b6d33b1df5eb056971fbdeefa8e9bc2e8a2d629 in /usr/local/bin/ 
# Thu, 11 May 2023 22:38:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:38:35 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:38:35 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:f3f60f415e9a03eed88bd5dd5268c841cde08dacf16911a3ef1e4e0fcdd76568`  
		Last Modified: Wed, 26 Apr 2023 02:08:37 GMT  
		Size: 28.4 MB (28389440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bfb87016de46ece16208cd39b5fa89740b8e8db147c2da2f6483551b3e8d521`  
		Last Modified: Thu, 04 May 2023 03:49:02 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8bd3f48f8f1fc94a1a143132ba91e005df50ee4327d0e209553cc89145a91f`  
		Last Modified: Thu, 04 May 2023 03:49:03 GMT  
		Size: 5.4 MB (5409831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ebb0502bf43d03d32f27b6cfa9ea349e89bccb62bd1ef3cf96a9a769e6c1fa`  
		Last Modified: Thu, 04 May 2023 03:49:00 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e71be3203371bc838f308b37c6191c81d6e4b9d1f80eb9ab8af5c758931c0e4`  
		Last Modified: Thu, 11 May 2023 22:42:27 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79fd566f0f92301f68512080c230b09d076fc0a1fb2ba3eb323b97f688d1423a`  
		Last Modified: Thu, 11 May 2023 22:42:35 GMT  
		Size: 80.2 MB (80166574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a4eaa7924e745081a848d3c916211ebb639ee4a2a55bc9d48cc10a5cd425163`  
		Last Modified: Thu, 11 May 2023 22:42:26 GMT  
		Size: 3.5 KB (3526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aefd1736befe72cd3e30b7c72cc07f832de8b42a576c89af447f0ec2546246cf`  
		Last Modified: Thu, 11 May 2023 22:42:26 GMT  
		Size: 7.5 KB (7515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.9.6-jammy`

```console
$ docker pull mariadb@sha256:7b3391cae3039e32c71bfc221451dd83c9d08ecb81658a7bc3cbfe60af5d09e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mariadb:10.9.6-jammy` - linux; amd64

```console
$ docker pull mariadb@sha256:1bbd4b8a0cca7b9c8ef2cfceca9582e160c667a82c134bc580b9d2c73f6fa297
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.4 MB (119400307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4076abc3d9d65253fa06f2c39365686780123a0c7ebcd3fb0e4916b6db00dc67`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 07:52:03 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 07:52:03 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 07:52:03 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 07:52:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 07:52:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 07:52:19 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:54:36 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.9.6 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:54:36 GMT
ARG MARIADB_VERSION=1:10.9.6+maria~ubu2204
# Thu, 11 May 2023 22:54:36 GMT
ENV MARIADB_VERSION=1:10.9.6+maria~ubu2204
# Thu, 11 May 2023 22:54:36 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.6/repo/ubuntu/ jammy main
# Thu, 11 May 2023 22:54:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.6/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:54:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.6/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:54:54 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:54:54 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:54:54 GMT
COPY file:94a071210c811522ac7cb9cd9b6d33b1df5eb056971fbdeefa8e9bc2e8a2d629 in /usr/local/bin/ 
# Thu, 11 May 2023 22:54:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:54:54 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:54:54 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:1bc677758ad7fa4503417ae5be18809c5a8679b5b36fcd1464d5a8e41cb13305`  
		Last Modified: Tue, 25 Apr 2023 22:54:44 GMT  
		Size: 30.4 MB (30430220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196e1740aea41b9915498de02cc132de54583dad1a212d06c9f6eb4690e1e0cb`  
		Last Modified: Thu, 04 May 2023 07:54:52 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4df0997938e5fd755403145484e1253115d3739285c704f562cf3bd6d89ec8`  
		Last Modified: Thu, 04 May 2023 07:54:53 GMT  
		Size: 5.6 MB (5595975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa4e41848249471f699386db900347fa61b39622dfba140344d9c51b264e7db`  
		Last Modified: Thu, 04 May 2023 07:54:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ac2d3b46fd64af7e90a89f270773b33d74514b9f634f18258776fbfd7c6bd1d`  
		Last Modified: Thu, 11 May 2023 22:58:59 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f7204e4367d7d18cd01bfc9b225102d3793392998e1e98622578659c7b6aa4`  
		Last Modified: Thu, 11 May 2023 22:59:10 GMT  
		Size: 83.4 MB (83360849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9757240e491172cbe025fb85afaac9890815fa635d426f6e098d5e6ed91d747c`  
		Last Modified: Thu, 11 May 2023 22:58:59 GMT  
		Size: 3.5 KB (3525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdffa7896ef0eee2b8dbd7ffb08520e9e07b47a51c530564315cb5b1739d9f46`  
		Last Modified: Thu, 11 May 2023 22:58:59 GMT  
		Size: 7.5 KB (7514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.9.6-jammy` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:359439cad072caa3eb08b44ac60d322b55ae83f1a7e8436f9a39183be6b2ba26
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (113979112 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a96a720da688aa8ee4361bfcf6a7a6fff7371bd02600f8b929bc9486f02a0ee8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 03:46:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 03:46:08 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 03:46:08 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 03:46:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 03:46:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 03:46:28 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:38:16 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.9.6 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:38:16 GMT
ARG MARIADB_VERSION=1:10.9.6+maria~ubu2204
# Thu, 11 May 2023 22:38:17 GMT
ENV MARIADB_VERSION=1:10.9.6+maria~ubu2204
# Thu, 11 May 2023 22:38:17 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.6/repo/ubuntu/ jammy main
# Thu, 11 May 2023 22:38:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.6/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:38:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.6/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:38:35 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:38:35 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:38:35 GMT
COPY file:94a071210c811522ac7cb9cd9b6d33b1df5eb056971fbdeefa8e9bc2e8a2d629 in /usr/local/bin/ 
# Thu, 11 May 2023 22:38:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:38:35 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:38:35 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:f3f60f415e9a03eed88bd5dd5268c841cde08dacf16911a3ef1e4e0fcdd76568`  
		Last Modified: Wed, 26 Apr 2023 02:08:37 GMT  
		Size: 28.4 MB (28389440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bfb87016de46ece16208cd39b5fa89740b8e8db147c2da2f6483551b3e8d521`  
		Last Modified: Thu, 04 May 2023 03:49:02 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8bd3f48f8f1fc94a1a143132ba91e005df50ee4327d0e209553cc89145a91f`  
		Last Modified: Thu, 04 May 2023 03:49:03 GMT  
		Size: 5.4 MB (5409831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ebb0502bf43d03d32f27b6cfa9ea349e89bccb62bd1ef3cf96a9a769e6c1fa`  
		Last Modified: Thu, 04 May 2023 03:49:00 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e71be3203371bc838f308b37c6191c81d6e4b9d1f80eb9ab8af5c758931c0e4`  
		Last Modified: Thu, 11 May 2023 22:42:27 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79fd566f0f92301f68512080c230b09d076fc0a1fb2ba3eb323b97f688d1423a`  
		Last Modified: Thu, 11 May 2023 22:42:35 GMT  
		Size: 80.2 MB (80166574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a4eaa7924e745081a848d3c916211ebb639ee4a2a55bc9d48cc10a5cd425163`  
		Last Modified: Thu, 11 May 2023 22:42:26 GMT  
		Size: 3.5 KB (3526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aefd1736befe72cd3e30b7c72cc07f832de8b42a576c89af447f0ec2546246cf`  
		Last Modified: Thu, 11 May 2023 22:42:26 GMT  
		Size: 7.5 KB (7515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:11.0-rc`

```console
$ docker pull mariadb@sha256:66e4fc66cb399cd1b56ec22d76e3eb943cf8a77b30d7273dfbf012c82a08e8ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:11.0-rc` - linux; amd64

```console
$ docker pull mariadb@sha256:fa7dbb0d75d5e1340ea42979890440f5e203a6a8c8f639d94e7edf1654539f9a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123135683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b7dd234f6f74207acbee402400fe7cfbd8df037fe4226256b4a0e74120296be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 07:52:03 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 07:52:03 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 07:52:03 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 07:52:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 07:52:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 07:52:19 GMT
ENV LANG=C.UTF-8
# Thu, 04 May 2023 07:52:20 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.0.1 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 04 May 2023 07:52:20 GMT
ARG MARIADB_VERSION=1:11.0.1+maria~ubu2204
# Thu, 04 May 2023 07:52:20 GMT
ENV MARIADB_VERSION=1:11.0.1+maria~ubu2204
# Thu, 04 May 2023 07:52:20 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.0.1/repo/ubuntu/ jammy main
# Thu, 04 May 2023 07:52:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 04 May 2023 07:52:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 04 May 2023 07:52:42 GMT
VOLUME [/var/lib/mysql]
# Thu, 04 May 2023 07:52:42 GMT
COPY file:835b387376a8b7e7292ae71352abf1c02fc75f579bcc76af370b0497b20be068 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:53:36 GMT
COPY file:0cfb36b89ea7e201c0cb92247b6a2a66bfa340811c384afdccafa204099bdb3e in /usr/local/bin/ 
# Thu, 11 May 2023 22:53:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:53:36 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:53:37 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:1bc677758ad7fa4503417ae5be18809c5a8679b5b36fcd1464d5a8e41cb13305`  
		Last Modified: Tue, 25 Apr 2023 22:54:44 GMT  
		Size: 30.4 MB (30430220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196e1740aea41b9915498de02cc132de54583dad1a212d06c9f6eb4690e1e0cb`  
		Last Modified: Thu, 04 May 2023 07:54:52 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4df0997938e5fd755403145484e1253115d3739285c704f562cf3bd6d89ec8`  
		Last Modified: Thu, 04 May 2023 07:54:53 GMT  
		Size: 5.6 MB (5595975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa4e41848249471f699386db900347fa61b39622dfba140344d9c51b264e7db`  
		Last Modified: Thu, 04 May 2023 07:54:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298b08277d883961f219f21b86ce87a02336d55ae03b4186bd1b21f0eee8eb6b`  
		Last Modified: Thu, 04 May 2023 07:54:50 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c4bb8c9a1da4655139eb8364ca356bf6b58881b7c9a815e0a15c506f5e22b9`  
		Last Modified: Thu, 04 May 2023 07:55:02 GMT  
		Size: 87.1 MB (87096235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22c03a3e9a83a6f9633a015d6175a472304b83a83595bb7cb942f98864ba5e13`  
		Last Modified: Thu, 04 May 2023 07:54:50 GMT  
		Size: 3.5 KB (3523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aed58337e012889836f45cdc9aee0fbf5bd5cef70b928ac82c5c80b5c8ce4dd`  
		Last Modified: Thu, 11 May 2023 22:57:46 GMT  
		Size: 7.5 KB (7507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:11.0-rc` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:0d36e41f674131459b6480e687efed07562d4226fb6ded4db541bd9a28963e67
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117654753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:930552c12c06e0e7908e46b378a522d69951612b1e7fa09e584a1bfb58f65c8b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 03:46:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 03:46:08 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 03:46:08 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 03:46:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 03:46:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 03:46:28 GMT
ENV LANG=C.UTF-8
# Thu, 04 May 2023 03:46:28 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.0.1 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 04 May 2023 03:46:28 GMT
ARG MARIADB_VERSION=1:11.0.1+maria~ubu2204
# Thu, 04 May 2023 03:46:28 GMT
ENV MARIADB_VERSION=1:11.0.1+maria~ubu2204
# Thu, 04 May 2023 03:46:28 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.0.1/repo/ubuntu/ jammy main
# Thu, 04 May 2023 03:46:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 04 May 2023 03:46:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 04 May 2023 03:46:55 GMT
VOLUME [/var/lib/mysql]
# Thu, 04 May 2023 03:46:55 GMT
COPY file:835b387376a8b7e7292ae71352abf1c02fc75f579bcc76af370b0497b20be068 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:37:12 GMT
COPY file:0cfb36b89ea7e201c0cb92247b6a2a66bfa340811c384afdccafa204099bdb3e in /usr/local/bin/ 
# Thu, 11 May 2023 22:37:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:37:12 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:37:12 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:f3f60f415e9a03eed88bd5dd5268c841cde08dacf16911a3ef1e4e0fcdd76568`  
		Last Modified: Wed, 26 Apr 2023 02:08:37 GMT  
		Size: 28.4 MB (28389440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bfb87016de46ece16208cd39b5fa89740b8e8db147c2da2f6483551b3e8d521`  
		Last Modified: Thu, 04 May 2023 03:49:02 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8bd3f48f8f1fc94a1a143132ba91e005df50ee4327d0e209553cc89145a91f`  
		Last Modified: Thu, 04 May 2023 03:49:03 GMT  
		Size: 5.4 MB (5409831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ebb0502bf43d03d32f27b6cfa9ea349e89bccb62bd1ef3cf96a9a769e6c1fa`  
		Last Modified: Thu, 04 May 2023 03:49:00 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2781286fffdc0538506f5be1d6f1f14d737c66d7042a4c789ba3cd1d9c4c67e0`  
		Last Modified: Thu, 04 May 2023 03:49:00 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9436d24f9f9a4f77f8c5771fd454a56daa38a048ff78bcf8c908b9d4e9c4b6b4`  
		Last Modified: Thu, 04 May 2023 03:49:10 GMT  
		Size: 83.8 MB (83842223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed17c6611459f4902ac4ab4133d421b4b3055df090b0dfd458888a1038afe8a8`  
		Last Modified: Thu, 04 May 2023 03:49:00 GMT  
		Size: 3.5 KB (3524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59d01f0bdbb58bb671f458a3d2b0c2023d43b7b43469e169c9836740b860cd12`  
		Last Modified: Thu, 11 May 2023 22:41:19 GMT  
		Size: 7.5 KB (7509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:11.0-rc` - linux; ppc64le

```console
$ docker pull mariadb@sha256:c9885378c109b81e8051d8891c798457f76e3574c0eff74b319e765c161d3048
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131835507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b97d568e2c7b0ebdf0c4c35d67e1f0d7985964eb03bde2ec2a3787c439da969d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:17 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:18 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:21 GMT
ADD file:e75f08a67f0576b5441bb2fe454cad4b5b31a9d4efea23be791af62e1e0c712f in / 
# Tue, 25 Apr 2023 17:30:21 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 14:29:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 14:29:33 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 14:29:33 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 14:30:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 14:30:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 14:30:21 GMT
ENV LANG=C.UTF-8
# Thu, 04 May 2023 14:30:22 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.0.1 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 04 May 2023 14:30:22 GMT
ARG MARIADB_VERSION=1:11.0.1+maria~ubu2204
# Thu, 04 May 2023 14:30:22 GMT
ENV MARIADB_VERSION=1:11.0.1+maria~ubu2204
# Thu, 04 May 2023 14:30:23 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.0.1/repo/ubuntu/ jammy main
# Thu, 04 May 2023 14:30:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 04 May 2023 14:31:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 04 May 2023 14:31:37 GMT
VOLUME [/var/lib/mysql]
# Thu, 04 May 2023 14:31:38 GMT
COPY file:835b387376a8b7e7292ae71352abf1c02fc75f579bcc76af370b0497b20be068 in /usr/local/bin/healthcheck.sh 
# Thu, 04 May 2023 14:31:38 GMT
COPY file:81e2f110d5c7749483b612be77bb7deed9454bc875e251b8a1354a08473aaadb in /usr/local/bin/ 
# Thu, 04 May 2023 14:31:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 May 2023 14:31:39 GMT
EXPOSE 3306
# Thu, 04 May 2023 14:31:40 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:f6a63d8cd043e76933823b18cbb7057a55bb4d66d64639c81e15a4700c101582`  
		Last Modified: Wed, 03 May 2023 17:09:07 GMT  
		Size: 35.7 MB (35712706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df46cdfc9a45a40dd254c1a0f2ccb2b0020e6852a5fb101d44d79250da5ddc69`  
		Last Modified: Thu, 04 May 2023 14:38:11 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11d1aa00f5a23d7276d6c701876911c79820fef6401156510e68eecb03012091`  
		Last Modified: Thu, 04 May 2023 14:38:12 GMT  
		Size: 6.0 MB (6021655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ec0fb2f57daffaea6b67a61d9012d55d4fcef64766481235d00d0438513793b`  
		Last Modified: Thu, 04 May 2023 14:38:08 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a9a3df1d262b9ef8d4b687aed77dabc8d34b2f6ed59b470ad317891ab5fbfb`  
		Last Modified: Thu, 04 May 2023 14:38:08 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f17883769bd005b95135d09d695fce9357488323dff767b6a0bc532f47275827`  
		Last Modified: Thu, 04 May 2023 14:38:34 GMT  
		Size: 90.1 MB (90088429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16795b3e8f390730bc01666cd286a2e80748d891f5740c9b4b532c0ee0d4b7c3`  
		Last Modified: Thu, 04 May 2023 14:38:08 GMT  
		Size: 3.5 KB (3523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:074e2195362442b49218ef41ae40a0134e956b45d3f6400b054a8eee63bb4117`  
		Last Modified: Thu, 04 May 2023 14:38:08 GMT  
		Size: 7.0 KB (6968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:11.0-rc-jammy`

```console
$ docker pull mariadb@sha256:66e4fc66cb399cd1b56ec22d76e3eb943cf8a77b30d7273dfbf012c82a08e8ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:11.0-rc-jammy` - linux; amd64

```console
$ docker pull mariadb@sha256:fa7dbb0d75d5e1340ea42979890440f5e203a6a8c8f639d94e7edf1654539f9a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123135683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b7dd234f6f74207acbee402400fe7cfbd8df037fe4226256b4a0e74120296be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 07:52:03 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 07:52:03 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 07:52:03 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 07:52:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 07:52:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 07:52:19 GMT
ENV LANG=C.UTF-8
# Thu, 04 May 2023 07:52:20 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.0.1 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 04 May 2023 07:52:20 GMT
ARG MARIADB_VERSION=1:11.0.1+maria~ubu2204
# Thu, 04 May 2023 07:52:20 GMT
ENV MARIADB_VERSION=1:11.0.1+maria~ubu2204
# Thu, 04 May 2023 07:52:20 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.0.1/repo/ubuntu/ jammy main
# Thu, 04 May 2023 07:52:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 04 May 2023 07:52:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 04 May 2023 07:52:42 GMT
VOLUME [/var/lib/mysql]
# Thu, 04 May 2023 07:52:42 GMT
COPY file:835b387376a8b7e7292ae71352abf1c02fc75f579bcc76af370b0497b20be068 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:53:36 GMT
COPY file:0cfb36b89ea7e201c0cb92247b6a2a66bfa340811c384afdccafa204099bdb3e in /usr/local/bin/ 
# Thu, 11 May 2023 22:53:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:53:36 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:53:37 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:1bc677758ad7fa4503417ae5be18809c5a8679b5b36fcd1464d5a8e41cb13305`  
		Last Modified: Tue, 25 Apr 2023 22:54:44 GMT  
		Size: 30.4 MB (30430220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196e1740aea41b9915498de02cc132de54583dad1a212d06c9f6eb4690e1e0cb`  
		Last Modified: Thu, 04 May 2023 07:54:52 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4df0997938e5fd755403145484e1253115d3739285c704f562cf3bd6d89ec8`  
		Last Modified: Thu, 04 May 2023 07:54:53 GMT  
		Size: 5.6 MB (5595975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa4e41848249471f699386db900347fa61b39622dfba140344d9c51b264e7db`  
		Last Modified: Thu, 04 May 2023 07:54:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298b08277d883961f219f21b86ce87a02336d55ae03b4186bd1b21f0eee8eb6b`  
		Last Modified: Thu, 04 May 2023 07:54:50 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c4bb8c9a1da4655139eb8364ca356bf6b58881b7c9a815e0a15c506f5e22b9`  
		Last Modified: Thu, 04 May 2023 07:55:02 GMT  
		Size: 87.1 MB (87096235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22c03a3e9a83a6f9633a015d6175a472304b83a83595bb7cb942f98864ba5e13`  
		Last Modified: Thu, 04 May 2023 07:54:50 GMT  
		Size: 3.5 KB (3523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aed58337e012889836f45cdc9aee0fbf5bd5cef70b928ac82c5c80b5c8ce4dd`  
		Last Modified: Thu, 11 May 2023 22:57:46 GMT  
		Size: 7.5 KB (7507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:11.0-rc-jammy` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:0d36e41f674131459b6480e687efed07562d4226fb6ded4db541bd9a28963e67
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117654753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:930552c12c06e0e7908e46b378a522d69951612b1e7fa09e584a1bfb58f65c8b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 03:46:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 03:46:08 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 03:46:08 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 03:46:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 03:46:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 03:46:28 GMT
ENV LANG=C.UTF-8
# Thu, 04 May 2023 03:46:28 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.0.1 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 04 May 2023 03:46:28 GMT
ARG MARIADB_VERSION=1:11.0.1+maria~ubu2204
# Thu, 04 May 2023 03:46:28 GMT
ENV MARIADB_VERSION=1:11.0.1+maria~ubu2204
# Thu, 04 May 2023 03:46:28 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.0.1/repo/ubuntu/ jammy main
# Thu, 04 May 2023 03:46:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 04 May 2023 03:46:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 04 May 2023 03:46:55 GMT
VOLUME [/var/lib/mysql]
# Thu, 04 May 2023 03:46:55 GMT
COPY file:835b387376a8b7e7292ae71352abf1c02fc75f579bcc76af370b0497b20be068 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:37:12 GMT
COPY file:0cfb36b89ea7e201c0cb92247b6a2a66bfa340811c384afdccafa204099bdb3e in /usr/local/bin/ 
# Thu, 11 May 2023 22:37:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:37:12 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:37:12 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:f3f60f415e9a03eed88bd5dd5268c841cde08dacf16911a3ef1e4e0fcdd76568`  
		Last Modified: Wed, 26 Apr 2023 02:08:37 GMT  
		Size: 28.4 MB (28389440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bfb87016de46ece16208cd39b5fa89740b8e8db147c2da2f6483551b3e8d521`  
		Last Modified: Thu, 04 May 2023 03:49:02 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8bd3f48f8f1fc94a1a143132ba91e005df50ee4327d0e209553cc89145a91f`  
		Last Modified: Thu, 04 May 2023 03:49:03 GMT  
		Size: 5.4 MB (5409831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ebb0502bf43d03d32f27b6cfa9ea349e89bccb62bd1ef3cf96a9a769e6c1fa`  
		Last Modified: Thu, 04 May 2023 03:49:00 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2781286fffdc0538506f5be1d6f1f14d737c66d7042a4c789ba3cd1d9c4c67e0`  
		Last Modified: Thu, 04 May 2023 03:49:00 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9436d24f9f9a4f77f8c5771fd454a56daa38a048ff78bcf8c908b9d4e9c4b6b4`  
		Last Modified: Thu, 04 May 2023 03:49:10 GMT  
		Size: 83.8 MB (83842223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed17c6611459f4902ac4ab4133d421b4b3055df090b0dfd458888a1038afe8a8`  
		Last Modified: Thu, 04 May 2023 03:49:00 GMT  
		Size: 3.5 KB (3524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59d01f0bdbb58bb671f458a3d2b0c2023d43b7b43469e169c9836740b860cd12`  
		Last Modified: Thu, 11 May 2023 22:41:19 GMT  
		Size: 7.5 KB (7509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:11.0-rc-jammy` - linux; ppc64le

```console
$ docker pull mariadb@sha256:c9885378c109b81e8051d8891c798457f76e3574c0eff74b319e765c161d3048
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131835507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b97d568e2c7b0ebdf0c4c35d67e1f0d7985964eb03bde2ec2a3787c439da969d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:17 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:18 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:21 GMT
ADD file:e75f08a67f0576b5441bb2fe454cad4b5b31a9d4efea23be791af62e1e0c712f in / 
# Tue, 25 Apr 2023 17:30:21 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 14:29:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 14:29:33 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 14:29:33 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 14:30:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 14:30:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 14:30:21 GMT
ENV LANG=C.UTF-8
# Thu, 04 May 2023 14:30:22 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.0.1 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 04 May 2023 14:30:22 GMT
ARG MARIADB_VERSION=1:11.0.1+maria~ubu2204
# Thu, 04 May 2023 14:30:22 GMT
ENV MARIADB_VERSION=1:11.0.1+maria~ubu2204
# Thu, 04 May 2023 14:30:23 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.0.1/repo/ubuntu/ jammy main
# Thu, 04 May 2023 14:30:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 04 May 2023 14:31:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 04 May 2023 14:31:37 GMT
VOLUME [/var/lib/mysql]
# Thu, 04 May 2023 14:31:38 GMT
COPY file:835b387376a8b7e7292ae71352abf1c02fc75f579bcc76af370b0497b20be068 in /usr/local/bin/healthcheck.sh 
# Thu, 04 May 2023 14:31:38 GMT
COPY file:81e2f110d5c7749483b612be77bb7deed9454bc875e251b8a1354a08473aaadb in /usr/local/bin/ 
# Thu, 04 May 2023 14:31:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 May 2023 14:31:39 GMT
EXPOSE 3306
# Thu, 04 May 2023 14:31:40 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:f6a63d8cd043e76933823b18cbb7057a55bb4d66d64639c81e15a4700c101582`  
		Last Modified: Wed, 03 May 2023 17:09:07 GMT  
		Size: 35.7 MB (35712706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df46cdfc9a45a40dd254c1a0f2ccb2b0020e6852a5fb101d44d79250da5ddc69`  
		Last Modified: Thu, 04 May 2023 14:38:11 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11d1aa00f5a23d7276d6c701876911c79820fef6401156510e68eecb03012091`  
		Last Modified: Thu, 04 May 2023 14:38:12 GMT  
		Size: 6.0 MB (6021655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ec0fb2f57daffaea6b67a61d9012d55d4fcef64766481235d00d0438513793b`  
		Last Modified: Thu, 04 May 2023 14:38:08 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a9a3df1d262b9ef8d4b687aed77dabc8d34b2f6ed59b470ad317891ab5fbfb`  
		Last Modified: Thu, 04 May 2023 14:38:08 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f17883769bd005b95135d09d695fce9357488323dff767b6a0bc532f47275827`  
		Last Modified: Thu, 04 May 2023 14:38:34 GMT  
		Size: 90.1 MB (90088429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16795b3e8f390730bc01666cd286a2e80748d891f5740c9b4b532c0ee0d4b7c3`  
		Last Modified: Thu, 04 May 2023 14:38:08 GMT  
		Size: 3.5 KB (3523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:074e2195362442b49218ef41ae40a0134e956b45d3f6400b054a8eee63bb4117`  
		Last Modified: Thu, 04 May 2023 14:38:08 GMT  
		Size: 7.0 KB (6968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:11.0.1-rc`

```console
$ docker pull mariadb@sha256:66e4fc66cb399cd1b56ec22d76e3eb943cf8a77b30d7273dfbf012c82a08e8ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:11.0.1-rc` - linux; amd64

```console
$ docker pull mariadb@sha256:fa7dbb0d75d5e1340ea42979890440f5e203a6a8c8f639d94e7edf1654539f9a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123135683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b7dd234f6f74207acbee402400fe7cfbd8df037fe4226256b4a0e74120296be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 07:52:03 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 07:52:03 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 07:52:03 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 07:52:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 07:52:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 07:52:19 GMT
ENV LANG=C.UTF-8
# Thu, 04 May 2023 07:52:20 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.0.1 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 04 May 2023 07:52:20 GMT
ARG MARIADB_VERSION=1:11.0.1+maria~ubu2204
# Thu, 04 May 2023 07:52:20 GMT
ENV MARIADB_VERSION=1:11.0.1+maria~ubu2204
# Thu, 04 May 2023 07:52:20 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.0.1/repo/ubuntu/ jammy main
# Thu, 04 May 2023 07:52:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 04 May 2023 07:52:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 04 May 2023 07:52:42 GMT
VOLUME [/var/lib/mysql]
# Thu, 04 May 2023 07:52:42 GMT
COPY file:835b387376a8b7e7292ae71352abf1c02fc75f579bcc76af370b0497b20be068 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:53:36 GMT
COPY file:0cfb36b89ea7e201c0cb92247b6a2a66bfa340811c384afdccafa204099bdb3e in /usr/local/bin/ 
# Thu, 11 May 2023 22:53:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:53:36 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:53:37 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:1bc677758ad7fa4503417ae5be18809c5a8679b5b36fcd1464d5a8e41cb13305`  
		Last Modified: Tue, 25 Apr 2023 22:54:44 GMT  
		Size: 30.4 MB (30430220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196e1740aea41b9915498de02cc132de54583dad1a212d06c9f6eb4690e1e0cb`  
		Last Modified: Thu, 04 May 2023 07:54:52 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4df0997938e5fd755403145484e1253115d3739285c704f562cf3bd6d89ec8`  
		Last Modified: Thu, 04 May 2023 07:54:53 GMT  
		Size: 5.6 MB (5595975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa4e41848249471f699386db900347fa61b39622dfba140344d9c51b264e7db`  
		Last Modified: Thu, 04 May 2023 07:54:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298b08277d883961f219f21b86ce87a02336d55ae03b4186bd1b21f0eee8eb6b`  
		Last Modified: Thu, 04 May 2023 07:54:50 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c4bb8c9a1da4655139eb8364ca356bf6b58881b7c9a815e0a15c506f5e22b9`  
		Last Modified: Thu, 04 May 2023 07:55:02 GMT  
		Size: 87.1 MB (87096235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22c03a3e9a83a6f9633a015d6175a472304b83a83595bb7cb942f98864ba5e13`  
		Last Modified: Thu, 04 May 2023 07:54:50 GMT  
		Size: 3.5 KB (3523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aed58337e012889836f45cdc9aee0fbf5bd5cef70b928ac82c5c80b5c8ce4dd`  
		Last Modified: Thu, 11 May 2023 22:57:46 GMT  
		Size: 7.5 KB (7507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:11.0.1-rc` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:0d36e41f674131459b6480e687efed07562d4226fb6ded4db541bd9a28963e67
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117654753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:930552c12c06e0e7908e46b378a522d69951612b1e7fa09e584a1bfb58f65c8b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 03:46:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 03:46:08 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 03:46:08 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 03:46:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 03:46:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 03:46:28 GMT
ENV LANG=C.UTF-8
# Thu, 04 May 2023 03:46:28 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.0.1 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 04 May 2023 03:46:28 GMT
ARG MARIADB_VERSION=1:11.0.1+maria~ubu2204
# Thu, 04 May 2023 03:46:28 GMT
ENV MARIADB_VERSION=1:11.0.1+maria~ubu2204
# Thu, 04 May 2023 03:46:28 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.0.1/repo/ubuntu/ jammy main
# Thu, 04 May 2023 03:46:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 04 May 2023 03:46:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 04 May 2023 03:46:55 GMT
VOLUME [/var/lib/mysql]
# Thu, 04 May 2023 03:46:55 GMT
COPY file:835b387376a8b7e7292ae71352abf1c02fc75f579bcc76af370b0497b20be068 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:37:12 GMT
COPY file:0cfb36b89ea7e201c0cb92247b6a2a66bfa340811c384afdccafa204099bdb3e in /usr/local/bin/ 
# Thu, 11 May 2023 22:37:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:37:12 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:37:12 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:f3f60f415e9a03eed88bd5dd5268c841cde08dacf16911a3ef1e4e0fcdd76568`  
		Last Modified: Wed, 26 Apr 2023 02:08:37 GMT  
		Size: 28.4 MB (28389440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bfb87016de46ece16208cd39b5fa89740b8e8db147c2da2f6483551b3e8d521`  
		Last Modified: Thu, 04 May 2023 03:49:02 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8bd3f48f8f1fc94a1a143132ba91e005df50ee4327d0e209553cc89145a91f`  
		Last Modified: Thu, 04 May 2023 03:49:03 GMT  
		Size: 5.4 MB (5409831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ebb0502bf43d03d32f27b6cfa9ea349e89bccb62bd1ef3cf96a9a769e6c1fa`  
		Last Modified: Thu, 04 May 2023 03:49:00 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2781286fffdc0538506f5be1d6f1f14d737c66d7042a4c789ba3cd1d9c4c67e0`  
		Last Modified: Thu, 04 May 2023 03:49:00 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9436d24f9f9a4f77f8c5771fd454a56daa38a048ff78bcf8c908b9d4e9c4b6b4`  
		Last Modified: Thu, 04 May 2023 03:49:10 GMT  
		Size: 83.8 MB (83842223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed17c6611459f4902ac4ab4133d421b4b3055df090b0dfd458888a1038afe8a8`  
		Last Modified: Thu, 04 May 2023 03:49:00 GMT  
		Size: 3.5 KB (3524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59d01f0bdbb58bb671f458a3d2b0c2023d43b7b43469e169c9836740b860cd12`  
		Last Modified: Thu, 11 May 2023 22:41:19 GMT  
		Size: 7.5 KB (7509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:11.0.1-rc` - linux; ppc64le

```console
$ docker pull mariadb@sha256:c9885378c109b81e8051d8891c798457f76e3574c0eff74b319e765c161d3048
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131835507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b97d568e2c7b0ebdf0c4c35d67e1f0d7985964eb03bde2ec2a3787c439da969d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:17 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:18 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:21 GMT
ADD file:e75f08a67f0576b5441bb2fe454cad4b5b31a9d4efea23be791af62e1e0c712f in / 
# Tue, 25 Apr 2023 17:30:21 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 14:29:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 14:29:33 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 14:29:33 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 14:30:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 14:30:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 14:30:21 GMT
ENV LANG=C.UTF-8
# Thu, 04 May 2023 14:30:22 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.0.1 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 04 May 2023 14:30:22 GMT
ARG MARIADB_VERSION=1:11.0.1+maria~ubu2204
# Thu, 04 May 2023 14:30:22 GMT
ENV MARIADB_VERSION=1:11.0.1+maria~ubu2204
# Thu, 04 May 2023 14:30:23 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.0.1/repo/ubuntu/ jammy main
# Thu, 04 May 2023 14:30:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 04 May 2023 14:31:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 04 May 2023 14:31:37 GMT
VOLUME [/var/lib/mysql]
# Thu, 04 May 2023 14:31:38 GMT
COPY file:835b387376a8b7e7292ae71352abf1c02fc75f579bcc76af370b0497b20be068 in /usr/local/bin/healthcheck.sh 
# Thu, 04 May 2023 14:31:38 GMT
COPY file:81e2f110d5c7749483b612be77bb7deed9454bc875e251b8a1354a08473aaadb in /usr/local/bin/ 
# Thu, 04 May 2023 14:31:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 May 2023 14:31:39 GMT
EXPOSE 3306
# Thu, 04 May 2023 14:31:40 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:f6a63d8cd043e76933823b18cbb7057a55bb4d66d64639c81e15a4700c101582`  
		Last Modified: Wed, 03 May 2023 17:09:07 GMT  
		Size: 35.7 MB (35712706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df46cdfc9a45a40dd254c1a0f2ccb2b0020e6852a5fb101d44d79250da5ddc69`  
		Last Modified: Thu, 04 May 2023 14:38:11 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11d1aa00f5a23d7276d6c701876911c79820fef6401156510e68eecb03012091`  
		Last Modified: Thu, 04 May 2023 14:38:12 GMT  
		Size: 6.0 MB (6021655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ec0fb2f57daffaea6b67a61d9012d55d4fcef64766481235d00d0438513793b`  
		Last Modified: Thu, 04 May 2023 14:38:08 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a9a3df1d262b9ef8d4b687aed77dabc8d34b2f6ed59b470ad317891ab5fbfb`  
		Last Modified: Thu, 04 May 2023 14:38:08 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f17883769bd005b95135d09d695fce9357488323dff767b6a0bc532f47275827`  
		Last Modified: Thu, 04 May 2023 14:38:34 GMT  
		Size: 90.1 MB (90088429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16795b3e8f390730bc01666cd286a2e80748d891f5740c9b4b532c0ee0d4b7c3`  
		Last Modified: Thu, 04 May 2023 14:38:08 GMT  
		Size: 3.5 KB (3523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:074e2195362442b49218ef41ae40a0134e956b45d3f6400b054a8eee63bb4117`  
		Last Modified: Thu, 04 May 2023 14:38:08 GMT  
		Size: 7.0 KB (6968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:11.0.1-rc-jammy`

```console
$ docker pull mariadb@sha256:66e4fc66cb399cd1b56ec22d76e3eb943cf8a77b30d7273dfbf012c82a08e8ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:11.0.1-rc-jammy` - linux; amd64

```console
$ docker pull mariadb@sha256:fa7dbb0d75d5e1340ea42979890440f5e203a6a8c8f639d94e7edf1654539f9a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123135683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b7dd234f6f74207acbee402400fe7cfbd8df037fe4226256b4a0e74120296be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 07:52:03 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 07:52:03 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 07:52:03 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 07:52:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 07:52:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 07:52:19 GMT
ENV LANG=C.UTF-8
# Thu, 04 May 2023 07:52:20 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.0.1 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 04 May 2023 07:52:20 GMT
ARG MARIADB_VERSION=1:11.0.1+maria~ubu2204
# Thu, 04 May 2023 07:52:20 GMT
ENV MARIADB_VERSION=1:11.0.1+maria~ubu2204
# Thu, 04 May 2023 07:52:20 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.0.1/repo/ubuntu/ jammy main
# Thu, 04 May 2023 07:52:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 04 May 2023 07:52:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 04 May 2023 07:52:42 GMT
VOLUME [/var/lib/mysql]
# Thu, 04 May 2023 07:52:42 GMT
COPY file:835b387376a8b7e7292ae71352abf1c02fc75f579bcc76af370b0497b20be068 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:53:36 GMT
COPY file:0cfb36b89ea7e201c0cb92247b6a2a66bfa340811c384afdccafa204099bdb3e in /usr/local/bin/ 
# Thu, 11 May 2023 22:53:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:53:36 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:53:37 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:1bc677758ad7fa4503417ae5be18809c5a8679b5b36fcd1464d5a8e41cb13305`  
		Last Modified: Tue, 25 Apr 2023 22:54:44 GMT  
		Size: 30.4 MB (30430220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196e1740aea41b9915498de02cc132de54583dad1a212d06c9f6eb4690e1e0cb`  
		Last Modified: Thu, 04 May 2023 07:54:52 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4df0997938e5fd755403145484e1253115d3739285c704f562cf3bd6d89ec8`  
		Last Modified: Thu, 04 May 2023 07:54:53 GMT  
		Size: 5.6 MB (5595975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa4e41848249471f699386db900347fa61b39622dfba140344d9c51b264e7db`  
		Last Modified: Thu, 04 May 2023 07:54:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298b08277d883961f219f21b86ce87a02336d55ae03b4186bd1b21f0eee8eb6b`  
		Last Modified: Thu, 04 May 2023 07:54:50 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c4bb8c9a1da4655139eb8364ca356bf6b58881b7c9a815e0a15c506f5e22b9`  
		Last Modified: Thu, 04 May 2023 07:55:02 GMT  
		Size: 87.1 MB (87096235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22c03a3e9a83a6f9633a015d6175a472304b83a83595bb7cb942f98864ba5e13`  
		Last Modified: Thu, 04 May 2023 07:54:50 GMT  
		Size: 3.5 KB (3523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aed58337e012889836f45cdc9aee0fbf5bd5cef70b928ac82c5c80b5c8ce4dd`  
		Last Modified: Thu, 11 May 2023 22:57:46 GMT  
		Size: 7.5 KB (7507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:11.0.1-rc-jammy` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:0d36e41f674131459b6480e687efed07562d4226fb6ded4db541bd9a28963e67
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117654753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:930552c12c06e0e7908e46b378a522d69951612b1e7fa09e584a1bfb58f65c8b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 03:46:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 03:46:08 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 03:46:08 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 03:46:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 03:46:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 03:46:28 GMT
ENV LANG=C.UTF-8
# Thu, 04 May 2023 03:46:28 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.0.1 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 04 May 2023 03:46:28 GMT
ARG MARIADB_VERSION=1:11.0.1+maria~ubu2204
# Thu, 04 May 2023 03:46:28 GMT
ENV MARIADB_VERSION=1:11.0.1+maria~ubu2204
# Thu, 04 May 2023 03:46:28 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.0.1/repo/ubuntu/ jammy main
# Thu, 04 May 2023 03:46:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 04 May 2023 03:46:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 04 May 2023 03:46:55 GMT
VOLUME [/var/lib/mysql]
# Thu, 04 May 2023 03:46:55 GMT
COPY file:835b387376a8b7e7292ae71352abf1c02fc75f579bcc76af370b0497b20be068 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:37:12 GMT
COPY file:0cfb36b89ea7e201c0cb92247b6a2a66bfa340811c384afdccafa204099bdb3e in /usr/local/bin/ 
# Thu, 11 May 2023 22:37:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:37:12 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:37:12 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:f3f60f415e9a03eed88bd5dd5268c841cde08dacf16911a3ef1e4e0fcdd76568`  
		Last Modified: Wed, 26 Apr 2023 02:08:37 GMT  
		Size: 28.4 MB (28389440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bfb87016de46ece16208cd39b5fa89740b8e8db147c2da2f6483551b3e8d521`  
		Last Modified: Thu, 04 May 2023 03:49:02 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8bd3f48f8f1fc94a1a143132ba91e005df50ee4327d0e209553cc89145a91f`  
		Last Modified: Thu, 04 May 2023 03:49:03 GMT  
		Size: 5.4 MB (5409831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ebb0502bf43d03d32f27b6cfa9ea349e89bccb62bd1ef3cf96a9a769e6c1fa`  
		Last Modified: Thu, 04 May 2023 03:49:00 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2781286fffdc0538506f5be1d6f1f14d737c66d7042a4c789ba3cd1d9c4c67e0`  
		Last Modified: Thu, 04 May 2023 03:49:00 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9436d24f9f9a4f77f8c5771fd454a56daa38a048ff78bcf8c908b9d4e9c4b6b4`  
		Last Modified: Thu, 04 May 2023 03:49:10 GMT  
		Size: 83.8 MB (83842223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed17c6611459f4902ac4ab4133d421b4b3055df090b0dfd458888a1038afe8a8`  
		Last Modified: Thu, 04 May 2023 03:49:00 GMT  
		Size: 3.5 KB (3524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59d01f0bdbb58bb671f458a3d2b0c2023d43b7b43469e169c9836740b860cd12`  
		Last Modified: Thu, 11 May 2023 22:41:19 GMT  
		Size: 7.5 KB (7509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:11.0.1-rc-jammy` - linux; ppc64le

```console
$ docker pull mariadb@sha256:c9885378c109b81e8051d8891c798457f76e3574c0eff74b319e765c161d3048
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131835507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b97d568e2c7b0ebdf0c4c35d67e1f0d7985964eb03bde2ec2a3787c439da969d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:17 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:18 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:21 GMT
ADD file:e75f08a67f0576b5441bb2fe454cad4b5b31a9d4efea23be791af62e1e0c712f in / 
# Tue, 25 Apr 2023 17:30:21 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 14:29:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 14:29:33 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 14:29:33 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 14:30:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 14:30:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 14:30:21 GMT
ENV LANG=C.UTF-8
# Thu, 04 May 2023 14:30:22 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.0.1 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 04 May 2023 14:30:22 GMT
ARG MARIADB_VERSION=1:11.0.1+maria~ubu2204
# Thu, 04 May 2023 14:30:22 GMT
ENV MARIADB_VERSION=1:11.0.1+maria~ubu2204
# Thu, 04 May 2023 14:30:23 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.0.1/repo/ubuntu/ jammy main
# Thu, 04 May 2023 14:30:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 04 May 2023 14:31:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.0.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 04 May 2023 14:31:37 GMT
VOLUME [/var/lib/mysql]
# Thu, 04 May 2023 14:31:38 GMT
COPY file:835b387376a8b7e7292ae71352abf1c02fc75f579bcc76af370b0497b20be068 in /usr/local/bin/healthcheck.sh 
# Thu, 04 May 2023 14:31:38 GMT
COPY file:81e2f110d5c7749483b612be77bb7deed9454bc875e251b8a1354a08473aaadb in /usr/local/bin/ 
# Thu, 04 May 2023 14:31:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 May 2023 14:31:39 GMT
EXPOSE 3306
# Thu, 04 May 2023 14:31:40 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:f6a63d8cd043e76933823b18cbb7057a55bb4d66d64639c81e15a4700c101582`  
		Last Modified: Wed, 03 May 2023 17:09:07 GMT  
		Size: 35.7 MB (35712706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df46cdfc9a45a40dd254c1a0f2ccb2b0020e6852a5fb101d44d79250da5ddc69`  
		Last Modified: Thu, 04 May 2023 14:38:11 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11d1aa00f5a23d7276d6c701876911c79820fef6401156510e68eecb03012091`  
		Last Modified: Thu, 04 May 2023 14:38:12 GMT  
		Size: 6.0 MB (6021655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ec0fb2f57daffaea6b67a61d9012d55d4fcef64766481235d00d0438513793b`  
		Last Modified: Thu, 04 May 2023 14:38:08 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a9a3df1d262b9ef8d4b687aed77dabc8d34b2f6ed59b470ad317891ab5fbfb`  
		Last Modified: Thu, 04 May 2023 14:38:08 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f17883769bd005b95135d09d695fce9357488323dff767b6a0bc532f47275827`  
		Last Modified: Thu, 04 May 2023 14:38:34 GMT  
		Size: 90.1 MB (90088429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16795b3e8f390730bc01666cd286a2e80748d891f5740c9b4b532c0ee0d4b7c3`  
		Last Modified: Thu, 04 May 2023 14:38:08 GMT  
		Size: 3.5 KB (3523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:074e2195362442b49218ef41ae40a0134e956b45d3f6400b054a8eee63bb4117`  
		Last Modified: Thu, 04 May 2023 14:38:08 GMT  
		Size: 7.0 KB (6968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:jammy`

```console
$ docker pull mariadb@sha256:5701c619e8f355f7d4d601f0007f1138f35d02882e206106e5d4a747a6805ed8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:jammy` - linux; amd64

```console
$ docker pull mariadb@sha256:f77c69a548d1a948f59d6b5eacf25903410cc156f84f33102cc4c662435dea72
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123112287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4af0c16be4b1af0799fd6f831b4fe63eab4ebe5e47d45bedac69b31d23c298e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 07:52:03 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 07:52:03 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 07:52:03 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 07:52:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 07:52:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 07:52:19 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:53:38 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.3 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:53:39 GMT
ARG MARIADB_VERSION=1:10.11.3+maria~ubu2204
# Thu, 11 May 2023 22:53:39 GMT
ENV MARIADB_VERSION=1:10.11.3+maria~ubu2204
# Thu, 11 May 2023 22:53:39 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
# Thu, 11 May 2023 22:53:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:54:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:54:06 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:54:06 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:54:06 GMT
COPY file:94a071210c811522ac7cb9cd9b6d33b1df5eb056971fbdeefa8e9bc2e8a2d629 in /usr/local/bin/ 
# Thu, 11 May 2023 22:54:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:54:06 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:54:07 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:1bc677758ad7fa4503417ae5be18809c5a8679b5b36fcd1464d5a8e41cb13305`  
		Last Modified: Tue, 25 Apr 2023 22:54:44 GMT  
		Size: 30.4 MB (30430220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196e1740aea41b9915498de02cc132de54583dad1a212d06c9f6eb4690e1e0cb`  
		Last Modified: Thu, 04 May 2023 07:54:52 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4df0997938e5fd755403145484e1253115d3739285c704f562cf3bd6d89ec8`  
		Last Modified: Thu, 04 May 2023 07:54:53 GMT  
		Size: 5.6 MB (5595975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa4e41848249471f699386db900347fa61b39622dfba140344d9c51b264e7db`  
		Last Modified: Thu, 04 May 2023 07:54:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a134c78ed13cbf2e6ac7f37c3ef851e65671664763a229e5460065d76e2ed7fa`  
		Last Modified: Thu, 11 May 2023 22:57:57 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7cd475067d8253d1d2cd28269770d3abf6eb40757983f4c92ae62f7a89b5535`  
		Last Modified: Thu, 11 May 2023 22:58:09 GMT  
		Size: 87.1 MB (87072824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348ae7ff2d74996bdc3e5da86e199b871eac8e2f86e7e15f7d03cbccc7231fa5`  
		Last Modified: Thu, 11 May 2023 22:57:57 GMT  
		Size: 3.5 KB (3528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e83ab58cb77ae0bded1f1bbd34ccc3c633547646227392d393af71e8b24a893`  
		Last Modified: Thu, 11 May 2023 22:57:57 GMT  
		Size: 7.5 KB (7516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:jammy` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:b180bb51094778a95fb835b429cfc2583d0f4e8e666cab652c221f3f03b6708b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117608447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ba3efd0815f87edbc030f0f8d50f783c1c9aa0c47ffec82ab94c6bad5822d7d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 03:46:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 03:46:08 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 03:46:08 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 03:46:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 03:46:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 03:46:28 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:37:14 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.3 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:37:14 GMT
ARG MARIADB_VERSION=1:10.11.3+maria~ubu2204
# Thu, 11 May 2023 22:37:14 GMT
ENV MARIADB_VERSION=1:10.11.3+maria~ubu2204
# Thu, 11 May 2023 22:37:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
# Thu, 11 May 2023 22:37:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:37:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:37:46 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:37:46 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:37:46 GMT
COPY file:94a071210c811522ac7cb9cd9b6d33b1df5eb056971fbdeefa8e9bc2e8a2d629 in /usr/local/bin/ 
# Thu, 11 May 2023 22:37:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:37:46 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:37:46 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:f3f60f415e9a03eed88bd5dd5268c841cde08dacf16911a3ef1e4e0fcdd76568`  
		Last Modified: Wed, 26 Apr 2023 02:08:37 GMT  
		Size: 28.4 MB (28389440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bfb87016de46ece16208cd39b5fa89740b8e8db147c2da2f6483551b3e8d521`  
		Last Modified: Thu, 04 May 2023 03:49:02 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8bd3f48f8f1fc94a1a143132ba91e005df50ee4327d0e209553cc89145a91f`  
		Last Modified: Thu, 04 May 2023 03:49:03 GMT  
		Size: 5.4 MB (5409831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ebb0502bf43d03d32f27b6cfa9ea349e89bccb62bd1ef3cf96a9a769e6c1fa`  
		Last Modified: Thu, 04 May 2023 03:49:00 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c39b9daac872cd7020c71e2bcfb8c097a1ea4c92c6e75f0fa1c5457a9793fabd`  
		Last Modified: Thu, 11 May 2023 22:41:30 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d0e97236e823170f83bde496cd664d5a354bdc0e3812e70d9e9dc434a067506`  
		Last Modified: Thu, 11 May 2023 22:41:40 GMT  
		Size: 83.8 MB (83795910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b5a4e92f3071fd8c0fcaba769b1d01c887847907025859069a695bebdfd2ca`  
		Last Modified: Thu, 11 May 2023 22:41:30 GMT  
		Size: 3.5 KB (3527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e100a9688501846d85a74ce52c2427d070849317340c48bdb06946ff8f89178`  
		Last Modified: Thu, 11 May 2023 22:41:30 GMT  
		Size: 7.5 KB (7515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:jammy` - linux; ppc64le

```console
$ docker pull mariadb@sha256:4d240e05dd2101a66ba61dd58ddc69e210df50aeefa05a74cbf242c6662dd584
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.9 MB (131883188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f8168152d1fd9b321f68df36d3f926ad414075ce59cb8a0b139cc40dc3a652c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:17 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:18 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:21 GMT
ADD file:e75f08a67f0576b5441bb2fe454cad4b5b31a9d4efea23be791af62e1e0c712f in / 
# Tue, 25 Apr 2023 17:30:21 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 14:29:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 14:29:33 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 14:29:33 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 14:30:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 14:30:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 14:30:21 GMT
ENV LANG=C.UTF-8
# Thu, 04 May 2023 14:31:55 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.2 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 04 May 2023 14:31:55 GMT
ARG MARIADB_VERSION=1:10.11.2+maria~ubu2204
# Thu, 04 May 2023 14:31:56 GMT
ENV MARIADB_VERSION=1:10.11.2+maria~ubu2204
# Thu, 04 May 2023 14:31:56 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.2/repo/ubuntu/ jammy main
# Thu, 04 May 2023 14:31:58 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 04 May 2023 14:32:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 04 May 2023 14:33:04 GMT
VOLUME [/var/lib/mysql]
# Thu, 04 May 2023 14:33:05 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 04 May 2023 14:33:05 GMT
COPY file:ebdfbcbc74dda1874f1c75d86e1c32733edb402d13440b2b7140a952010bc21f in /usr/local/bin/ 
# Thu, 04 May 2023 14:33:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 May 2023 14:33:07 GMT
EXPOSE 3306
# Thu, 04 May 2023 14:33:07 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:f6a63d8cd043e76933823b18cbb7057a55bb4d66d64639c81e15a4700c101582`  
		Last Modified: Wed, 03 May 2023 17:09:07 GMT  
		Size: 35.7 MB (35712706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df46cdfc9a45a40dd254c1a0f2ccb2b0020e6852a5fb101d44d79250da5ddc69`  
		Last Modified: Thu, 04 May 2023 14:38:11 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11d1aa00f5a23d7276d6c701876911c79820fef6401156510e68eecb03012091`  
		Last Modified: Thu, 04 May 2023 14:38:12 GMT  
		Size: 6.0 MB (6021655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ec0fb2f57daffaea6b67a61d9012d55d4fcef64766481235d00d0438513793b`  
		Last Modified: Thu, 04 May 2023 14:38:08 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5222456a7c2bfe3bf5175c63ee69047694ca04828ae27b736d3e365bb098e6`  
		Last Modified: Thu, 04 May 2023 14:38:49 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c483e4bc0a4a66eedb7d32ac48ebb035053d2581b308082f7f73aae65b5695`  
		Last Modified: Thu, 04 May 2023 14:39:13 GMT  
		Size: 90.1 MB (90136103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c20716d8d6a4a6fffb6a1a4433d2c519498b3245749451035f81128a7d9d6f5a`  
		Last Modified: Thu, 04 May 2023 14:38:49 GMT  
		Size: 3.5 KB (3526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92aecaeb58f118d19cc858ade38f52e5cc3f8fbd518c7cd5d71caecd07b49db`  
		Last Modified: Thu, 04 May 2023 14:38:49 GMT  
		Size: 7.0 KB (6970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:jammy` - linux; s390x

```console
$ docker pull mariadb@sha256:6776cef0f480be971c0746153bfc7d3c6a6ba04acb53448303d2ee7fd50b10d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121445424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5c39fb429a2411a98cc5e9ce78feeefc35cd3d0d3f948609f9d0d7162e091bf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 26 Jan 2023 05:08:35 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:08:35 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:08:36 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:08:36 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:08:37 GMT
ADD file:a9794efc1a102ab6a7160e660a63f4b267797b8b7e0b0bfd9c04ed62846cfb36 in / 
# Thu, 26 Jan 2023 05:08:38 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:42:50 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 31 Jan 2023 18:42:50 GMT
ENV GOSU_VERSION=1.14
# Tue, 31 Jan 2023 18:42:50 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 31 Jan 2023 18:43:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 31 Jan 2023 18:43:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 31 Jan 2023 18:43:06 GMT
ENV LANG=C.UTF-8
# Sat, 18 Feb 2023 00:39:43 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.2 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Sat, 18 Feb 2023 00:39:43 GMT
ARG MARIADB_VERSION=1:10.11.2+maria~ubu2204
# Sat, 18 Feb 2023 00:39:43 GMT
ENV MARIADB_VERSION=1:10.11.2+maria~ubu2204
# Sat, 18 Feb 2023 00:39:44 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.2/repo/ubuntu/ jammy main
# Sat, 18 Feb 2023 00:39:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 18 Feb 2023 00:40:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Sat, 18 Feb 2023 00:40:18 GMT
VOLUME [/var/lib/mysql]
# Sat, 25 Feb 2023 04:00:33 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Sat, 25 Feb 2023 04:00:33 GMT
COPY file:ebdfbcbc74dda1874f1c75d86e1c32733edb402d13440b2b7140a952010bc21f in /usr/local/bin/ 
# Sat, 25 Feb 2023 04:00:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 25 Feb 2023 04:00:33 GMT
EXPOSE 3306
# Sat, 25 Feb 2023 04:00:33 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:dd969ed9de43018fe5442c859bf66eabf23145b966b9338392ea707aed18b26f`  
		Last Modified: Tue, 31 Jan 2023 17:55:34 GMT  
		Size: 28.6 MB (28641926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b702438b56d7a6aaaad49e2be85e1bb2f3beb85406f6b9db1a232f798c558b3`  
		Last Modified: Tue, 31 Jan 2023 18:48:25 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60737998d0295bde808ca8856933482817ca605937f714f3cfca1ab0b4ca99ed`  
		Last Modified: Tue, 31 Jan 2023 18:48:26 GMT  
		Size: 5.4 MB (5401827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6e12a0288bb0803aeb23e581ca842e1fdf826fa28b4a730dd83585ea125ff8`  
		Last Modified: Tue, 31 Jan 2023 18:48:24 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36528da402899a29c65aec506cc3573ecd9edf046e710740371ea56b98466ce`  
		Last Modified: Sat, 18 Feb 2023 00:42:04 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c45532e045d6549e8a41f2b8cce4c9cc336de9d1dac3d929d2a7ea3fee6fcf`  
		Last Modified: Sat, 18 Feb 2023 00:42:16 GMT  
		Size: 87.4 MB (87388947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf76dfdfa839489a3b54c3eb3679f8718726a96a30cc2049089b7ac593b41ae`  
		Last Modified: Sat, 25 Feb 2023 04:02:18 GMT  
		Size: 3.5 KB (3526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f477561fbd237479df484d7fc122750ffa7b64e394c3ca9d2cc6e5072810967d`  
		Last Modified: Sat, 25 Feb 2023 04:02:18 GMT  
		Size: 7.0 KB (6971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:latest`

```console
$ docker pull mariadb@sha256:5701c619e8f355f7d4d601f0007f1138f35d02882e206106e5d4a747a6805ed8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:latest` - linux; amd64

```console
$ docker pull mariadb@sha256:f77c69a548d1a948f59d6b5eacf25903410cc156f84f33102cc4c662435dea72
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123112287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4af0c16be4b1af0799fd6f831b4fe63eab4ebe5e47d45bedac69b31d23c298e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 07:52:03 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 07:52:03 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 07:52:03 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 07:52:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 07:52:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 07:52:19 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:53:38 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.3 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:53:39 GMT
ARG MARIADB_VERSION=1:10.11.3+maria~ubu2204
# Thu, 11 May 2023 22:53:39 GMT
ENV MARIADB_VERSION=1:10.11.3+maria~ubu2204
# Thu, 11 May 2023 22:53:39 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
# Thu, 11 May 2023 22:53:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:54:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:54:06 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:54:06 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:54:06 GMT
COPY file:94a071210c811522ac7cb9cd9b6d33b1df5eb056971fbdeefa8e9bc2e8a2d629 in /usr/local/bin/ 
# Thu, 11 May 2023 22:54:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:54:06 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:54:07 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:1bc677758ad7fa4503417ae5be18809c5a8679b5b36fcd1464d5a8e41cb13305`  
		Last Modified: Tue, 25 Apr 2023 22:54:44 GMT  
		Size: 30.4 MB (30430220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196e1740aea41b9915498de02cc132de54583dad1a212d06c9f6eb4690e1e0cb`  
		Last Modified: Thu, 04 May 2023 07:54:52 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4df0997938e5fd755403145484e1253115d3739285c704f562cf3bd6d89ec8`  
		Last Modified: Thu, 04 May 2023 07:54:53 GMT  
		Size: 5.6 MB (5595975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa4e41848249471f699386db900347fa61b39622dfba140344d9c51b264e7db`  
		Last Modified: Thu, 04 May 2023 07:54:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a134c78ed13cbf2e6ac7f37c3ef851e65671664763a229e5460065d76e2ed7fa`  
		Last Modified: Thu, 11 May 2023 22:57:57 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7cd475067d8253d1d2cd28269770d3abf6eb40757983f4c92ae62f7a89b5535`  
		Last Modified: Thu, 11 May 2023 22:58:09 GMT  
		Size: 87.1 MB (87072824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348ae7ff2d74996bdc3e5da86e199b871eac8e2f86e7e15f7d03cbccc7231fa5`  
		Last Modified: Thu, 11 May 2023 22:57:57 GMT  
		Size: 3.5 KB (3528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e83ab58cb77ae0bded1f1bbd34ccc3c633547646227392d393af71e8b24a893`  
		Last Modified: Thu, 11 May 2023 22:57:57 GMT  
		Size: 7.5 KB (7516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:b180bb51094778a95fb835b429cfc2583d0f4e8e666cab652c221f3f03b6708b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117608447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ba3efd0815f87edbc030f0f8d50f783c1c9aa0c47ffec82ab94c6bad5822d7d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 03:46:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 03:46:08 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 03:46:08 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 03:46:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 03:46:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 03:46:28 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:37:14 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.3 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:37:14 GMT
ARG MARIADB_VERSION=1:10.11.3+maria~ubu2204
# Thu, 11 May 2023 22:37:14 GMT
ENV MARIADB_VERSION=1:10.11.3+maria~ubu2204
# Thu, 11 May 2023 22:37:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
# Thu, 11 May 2023 22:37:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:37:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:37:46 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:37:46 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:37:46 GMT
COPY file:94a071210c811522ac7cb9cd9b6d33b1df5eb056971fbdeefa8e9bc2e8a2d629 in /usr/local/bin/ 
# Thu, 11 May 2023 22:37:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:37:46 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:37:46 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:f3f60f415e9a03eed88bd5dd5268c841cde08dacf16911a3ef1e4e0fcdd76568`  
		Last Modified: Wed, 26 Apr 2023 02:08:37 GMT  
		Size: 28.4 MB (28389440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bfb87016de46ece16208cd39b5fa89740b8e8db147c2da2f6483551b3e8d521`  
		Last Modified: Thu, 04 May 2023 03:49:02 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8bd3f48f8f1fc94a1a143132ba91e005df50ee4327d0e209553cc89145a91f`  
		Last Modified: Thu, 04 May 2023 03:49:03 GMT  
		Size: 5.4 MB (5409831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ebb0502bf43d03d32f27b6cfa9ea349e89bccb62bd1ef3cf96a9a769e6c1fa`  
		Last Modified: Thu, 04 May 2023 03:49:00 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c39b9daac872cd7020c71e2bcfb8c097a1ea4c92c6e75f0fa1c5457a9793fabd`  
		Last Modified: Thu, 11 May 2023 22:41:30 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d0e97236e823170f83bde496cd664d5a354bdc0e3812e70d9e9dc434a067506`  
		Last Modified: Thu, 11 May 2023 22:41:40 GMT  
		Size: 83.8 MB (83795910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b5a4e92f3071fd8c0fcaba769b1d01c887847907025859069a695bebdfd2ca`  
		Last Modified: Thu, 11 May 2023 22:41:30 GMT  
		Size: 3.5 KB (3527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e100a9688501846d85a74ce52c2427d070849317340c48bdb06946ff8f89178`  
		Last Modified: Thu, 11 May 2023 22:41:30 GMT  
		Size: 7.5 KB (7515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; ppc64le

```console
$ docker pull mariadb@sha256:4d240e05dd2101a66ba61dd58ddc69e210df50aeefa05a74cbf242c6662dd584
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.9 MB (131883188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f8168152d1fd9b321f68df36d3f926ad414075ce59cb8a0b139cc40dc3a652c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:17 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:18 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:21 GMT
ADD file:e75f08a67f0576b5441bb2fe454cad4b5b31a9d4efea23be791af62e1e0c712f in / 
# Tue, 25 Apr 2023 17:30:21 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 14:29:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 14:29:33 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 14:29:33 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 14:30:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 14:30:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 14:30:21 GMT
ENV LANG=C.UTF-8
# Thu, 04 May 2023 14:31:55 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.2 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 04 May 2023 14:31:55 GMT
ARG MARIADB_VERSION=1:10.11.2+maria~ubu2204
# Thu, 04 May 2023 14:31:56 GMT
ENV MARIADB_VERSION=1:10.11.2+maria~ubu2204
# Thu, 04 May 2023 14:31:56 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.2/repo/ubuntu/ jammy main
# Thu, 04 May 2023 14:31:58 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 04 May 2023 14:32:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 04 May 2023 14:33:04 GMT
VOLUME [/var/lib/mysql]
# Thu, 04 May 2023 14:33:05 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 04 May 2023 14:33:05 GMT
COPY file:ebdfbcbc74dda1874f1c75d86e1c32733edb402d13440b2b7140a952010bc21f in /usr/local/bin/ 
# Thu, 04 May 2023 14:33:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 May 2023 14:33:07 GMT
EXPOSE 3306
# Thu, 04 May 2023 14:33:07 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:f6a63d8cd043e76933823b18cbb7057a55bb4d66d64639c81e15a4700c101582`  
		Last Modified: Wed, 03 May 2023 17:09:07 GMT  
		Size: 35.7 MB (35712706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df46cdfc9a45a40dd254c1a0f2ccb2b0020e6852a5fb101d44d79250da5ddc69`  
		Last Modified: Thu, 04 May 2023 14:38:11 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11d1aa00f5a23d7276d6c701876911c79820fef6401156510e68eecb03012091`  
		Last Modified: Thu, 04 May 2023 14:38:12 GMT  
		Size: 6.0 MB (6021655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ec0fb2f57daffaea6b67a61d9012d55d4fcef64766481235d00d0438513793b`  
		Last Modified: Thu, 04 May 2023 14:38:08 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5222456a7c2bfe3bf5175c63ee69047694ca04828ae27b736d3e365bb098e6`  
		Last Modified: Thu, 04 May 2023 14:38:49 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c483e4bc0a4a66eedb7d32ac48ebb035053d2581b308082f7f73aae65b5695`  
		Last Modified: Thu, 04 May 2023 14:39:13 GMT  
		Size: 90.1 MB (90136103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c20716d8d6a4a6fffb6a1a4433d2c519498b3245749451035f81128a7d9d6f5a`  
		Last Modified: Thu, 04 May 2023 14:38:49 GMT  
		Size: 3.5 KB (3526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92aecaeb58f118d19cc858ade38f52e5cc3f8fbd518c7cd5d71caecd07b49db`  
		Last Modified: Thu, 04 May 2023 14:38:49 GMT  
		Size: 7.0 KB (6970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; s390x

```console
$ docker pull mariadb@sha256:6776cef0f480be971c0746153bfc7d3c6a6ba04acb53448303d2ee7fd50b10d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121445424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5c39fb429a2411a98cc5e9ce78feeefc35cd3d0d3f948609f9d0d7162e091bf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 26 Jan 2023 05:08:35 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:08:35 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:08:36 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:08:36 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:08:37 GMT
ADD file:a9794efc1a102ab6a7160e660a63f4b267797b8b7e0b0bfd9c04ed62846cfb36 in / 
# Thu, 26 Jan 2023 05:08:38 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:42:50 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 31 Jan 2023 18:42:50 GMT
ENV GOSU_VERSION=1.14
# Tue, 31 Jan 2023 18:42:50 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 31 Jan 2023 18:43:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 31 Jan 2023 18:43:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 31 Jan 2023 18:43:06 GMT
ENV LANG=C.UTF-8
# Sat, 18 Feb 2023 00:39:43 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.2 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Sat, 18 Feb 2023 00:39:43 GMT
ARG MARIADB_VERSION=1:10.11.2+maria~ubu2204
# Sat, 18 Feb 2023 00:39:43 GMT
ENV MARIADB_VERSION=1:10.11.2+maria~ubu2204
# Sat, 18 Feb 2023 00:39:44 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.2/repo/ubuntu/ jammy main
# Sat, 18 Feb 2023 00:39:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 18 Feb 2023 00:40:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Sat, 18 Feb 2023 00:40:18 GMT
VOLUME [/var/lib/mysql]
# Sat, 25 Feb 2023 04:00:33 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Sat, 25 Feb 2023 04:00:33 GMT
COPY file:ebdfbcbc74dda1874f1c75d86e1c32733edb402d13440b2b7140a952010bc21f in /usr/local/bin/ 
# Sat, 25 Feb 2023 04:00:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 25 Feb 2023 04:00:33 GMT
EXPOSE 3306
# Sat, 25 Feb 2023 04:00:33 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:dd969ed9de43018fe5442c859bf66eabf23145b966b9338392ea707aed18b26f`  
		Last Modified: Tue, 31 Jan 2023 17:55:34 GMT  
		Size: 28.6 MB (28641926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b702438b56d7a6aaaad49e2be85e1bb2f3beb85406f6b9db1a232f798c558b3`  
		Last Modified: Tue, 31 Jan 2023 18:48:25 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60737998d0295bde808ca8856933482817ca605937f714f3cfca1ab0b4ca99ed`  
		Last Modified: Tue, 31 Jan 2023 18:48:26 GMT  
		Size: 5.4 MB (5401827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6e12a0288bb0803aeb23e581ca842e1fdf826fa28b4a730dd83585ea125ff8`  
		Last Modified: Tue, 31 Jan 2023 18:48:24 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36528da402899a29c65aec506cc3573ecd9edf046e710740371ea56b98466ce`  
		Last Modified: Sat, 18 Feb 2023 00:42:04 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c45532e045d6549e8a41f2b8cce4c9cc336de9d1dac3d929d2a7ea3fee6fcf`  
		Last Modified: Sat, 18 Feb 2023 00:42:16 GMT  
		Size: 87.4 MB (87388947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf76dfdfa839489a3b54c3eb3679f8718726a96a30cc2049089b7ac593b41ae`  
		Last Modified: Sat, 25 Feb 2023 04:02:18 GMT  
		Size: 3.5 KB (3526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f477561fbd237479df484d7fc122750ffa7b64e394c3ca9d2cc6e5072810967d`  
		Last Modified: Sat, 25 Feb 2023 04:02:18 GMT  
		Size: 7.0 KB (6971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:lts`

```console
$ docker pull mariadb@sha256:ab92bf22ba67bfd1f6b1f8c065e73613308dabb5e4abe00e1f42206100696f74
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mariadb:lts` - linux; amd64

```console
$ docker pull mariadb@sha256:f77c69a548d1a948f59d6b5eacf25903410cc156f84f33102cc4c662435dea72
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123112287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4af0c16be4b1af0799fd6f831b4fe63eab4ebe5e47d45bedac69b31d23c298e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 07:52:03 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 07:52:03 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 07:52:03 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 07:52:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 07:52:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 07:52:19 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:53:38 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.3 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:53:39 GMT
ARG MARIADB_VERSION=1:10.11.3+maria~ubu2204
# Thu, 11 May 2023 22:53:39 GMT
ENV MARIADB_VERSION=1:10.11.3+maria~ubu2204
# Thu, 11 May 2023 22:53:39 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
# Thu, 11 May 2023 22:53:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:54:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:54:06 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:54:06 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:54:06 GMT
COPY file:94a071210c811522ac7cb9cd9b6d33b1df5eb056971fbdeefa8e9bc2e8a2d629 in /usr/local/bin/ 
# Thu, 11 May 2023 22:54:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:54:06 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:54:07 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:1bc677758ad7fa4503417ae5be18809c5a8679b5b36fcd1464d5a8e41cb13305`  
		Last Modified: Tue, 25 Apr 2023 22:54:44 GMT  
		Size: 30.4 MB (30430220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196e1740aea41b9915498de02cc132de54583dad1a212d06c9f6eb4690e1e0cb`  
		Last Modified: Thu, 04 May 2023 07:54:52 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4df0997938e5fd755403145484e1253115d3739285c704f562cf3bd6d89ec8`  
		Last Modified: Thu, 04 May 2023 07:54:53 GMT  
		Size: 5.6 MB (5595975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa4e41848249471f699386db900347fa61b39622dfba140344d9c51b264e7db`  
		Last Modified: Thu, 04 May 2023 07:54:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a134c78ed13cbf2e6ac7f37c3ef851e65671664763a229e5460065d76e2ed7fa`  
		Last Modified: Thu, 11 May 2023 22:57:57 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7cd475067d8253d1d2cd28269770d3abf6eb40757983f4c92ae62f7a89b5535`  
		Last Modified: Thu, 11 May 2023 22:58:09 GMT  
		Size: 87.1 MB (87072824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348ae7ff2d74996bdc3e5da86e199b871eac8e2f86e7e15f7d03cbccc7231fa5`  
		Last Modified: Thu, 11 May 2023 22:57:57 GMT  
		Size: 3.5 KB (3528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e83ab58cb77ae0bded1f1bbd34ccc3c633547646227392d393af71e8b24a893`  
		Last Modified: Thu, 11 May 2023 22:57:57 GMT  
		Size: 7.5 KB (7516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:lts` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:b180bb51094778a95fb835b429cfc2583d0f4e8e666cab652c221f3f03b6708b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117608447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ba3efd0815f87edbc030f0f8d50f783c1c9aa0c47ffec82ab94c6bad5822d7d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 03:46:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 03:46:08 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 03:46:08 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 03:46:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 03:46:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 03:46:28 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:37:14 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.3 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:37:14 GMT
ARG MARIADB_VERSION=1:10.11.3+maria~ubu2204
# Thu, 11 May 2023 22:37:14 GMT
ENV MARIADB_VERSION=1:10.11.3+maria~ubu2204
# Thu, 11 May 2023 22:37:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
# Thu, 11 May 2023 22:37:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:37:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:37:46 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:37:46 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:37:46 GMT
COPY file:94a071210c811522ac7cb9cd9b6d33b1df5eb056971fbdeefa8e9bc2e8a2d629 in /usr/local/bin/ 
# Thu, 11 May 2023 22:37:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:37:46 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:37:46 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:f3f60f415e9a03eed88bd5dd5268c841cde08dacf16911a3ef1e4e0fcdd76568`  
		Last Modified: Wed, 26 Apr 2023 02:08:37 GMT  
		Size: 28.4 MB (28389440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bfb87016de46ece16208cd39b5fa89740b8e8db147c2da2f6483551b3e8d521`  
		Last Modified: Thu, 04 May 2023 03:49:02 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8bd3f48f8f1fc94a1a143132ba91e005df50ee4327d0e209553cc89145a91f`  
		Last Modified: Thu, 04 May 2023 03:49:03 GMT  
		Size: 5.4 MB (5409831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ebb0502bf43d03d32f27b6cfa9ea349e89bccb62bd1ef3cf96a9a769e6c1fa`  
		Last Modified: Thu, 04 May 2023 03:49:00 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c39b9daac872cd7020c71e2bcfb8c097a1ea4c92c6e75f0fa1c5457a9793fabd`  
		Last Modified: Thu, 11 May 2023 22:41:30 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d0e97236e823170f83bde496cd664d5a354bdc0e3812e70d9e9dc434a067506`  
		Last Modified: Thu, 11 May 2023 22:41:40 GMT  
		Size: 83.8 MB (83795910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b5a4e92f3071fd8c0fcaba769b1d01c887847907025859069a695bebdfd2ca`  
		Last Modified: Thu, 11 May 2023 22:41:30 GMT  
		Size: 3.5 KB (3527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e100a9688501846d85a74ce52c2427d070849317340c48bdb06946ff8f89178`  
		Last Modified: Thu, 11 May 2023 22:41:30 GMT  
		Size: 7.5 KB (7515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:lts-jammy`

```console
$ docker pull mariadb@sha256:ab92bf22ba67bfd1f6b1f8c065e73613308dabb5e4abe00e1f42206100696f74
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mariadb:lts-jammy` - linux; amd64

```console
$ docker pull mariadb@sha256:f77c69a548d1a948f59d6b5eacf25903410cc156f84f33102cc4c662435dea72
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123112287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4af0c16be4b1af0799fd6f831b4fe63eab4ebe5e47d45bedac69b31d23c298e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 07:52:03 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 07:52:03 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 07:52:03 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 07:52:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 07:52:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 07:52:19 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:53:38 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.3 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:53:39 GMT
ARG MARIADB_VERSION=1:10.11.3+maria~ubu2204
# Thu, 11 May 2023 22:53:39 GMT
ENV MARIADB_VERSION=1:10.11.3+maria~ubu2204
# Thu, 11 May 2023 22:53:39 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
# Thu, 11 May 2023 22:53:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:54:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:54:06 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:54:06 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:54:06 GMT
COPY file:94a071210c811522ac7cb9cd9b6d33b1df5eb056971fbdeefa8e9bc2e8a2d629 in /usr/local/bin/ 
# Thu, 11 May 2023 22:54:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:54:06 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:54:07 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:1bc677758ad7fa4503417ae5be18809c5a8679b5b36fcd1464d5a8e41cb13305`  
		Last Modified: Tue, 25 Apr 2023 22:54:44 GMT  
		Size: 30.4 MB (30430220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196e1740aea41b9915498de02cc132de54583dad1a212d06c9f6eb4690e1e0cb`  
		Last Modified: Thu, 04 May 2023 07:54:52 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4df0997938e5fd755403145484e1253115d3739285c704f562cf3bd6d89ec8`  
		Last Modified: Thu, 04 May 2023 07:54:53 GMT  
		Size: 5.6 MB (5595975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa4e41848249471f699386db900347fa61b39622dfba140344d9c51b264e7db`  
		Last Modified: Thu, 04 May 2023 07:54:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a134c78ed13cbf2e6ac7f37c3ef851e65671664763a229e5460065d76e2ed7fa`  
		Last Modified: Thu, 11 May 2023 22:57:57 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7cd475067d8253d1d2cd28269770d3abf6eb40757983f4c92ae62f7a89b5535`  
		Last Modified: Thu, 11 May 2023 22:58:09 GMT  
		Size: 87.1 MB (87072824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348ae7ff2d74996bdc3e5da86e199b871eac8e2f86e7e15f7d03cbccc7231fa5`  
		Last Modified: Thu, 11 May 2023 22:57:57 GMT  
		Size: 3.5 KB (3528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e83ab58cb77ae0bded1f1bbd34ccc3c633547646227392d393af71e8b24a893`  
		Last Modified: Thu, 11 May 2023 22:57:57 GMT  
		Size: 7.5 KB (7516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:lts-jammy` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:b180bb51094778a95fb835b429cfc2583d0f4e8e666cab652c221f3f03b6708b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117608447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ba3efd0815f87edbc030f0f8d50f783c1c9aa0c47ffec82ab94c6bad5822d7d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 03:46:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 04 May 2023 03:46:08 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 03:46:08 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 04 May 2023 03:46:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 03:46:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 May 2023 03:46:28 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:37:14 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.3 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 11 May 2023 22:37:14 GMT
ARG MARIADB_VERSION=1:10.11.3+maria~ubu2204
# Thu, 11 May 2023 22:37:14 GMT
ENV MARIADB_VERSION=1:10.11.3+maria~ubu2204
# Thu, 11 May 2023 22:37:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
# Thu, 11 May 2023 22:37:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 11 May 2023 22:37:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 11 May 2023 22:37:46 GMT
VOLUME [/var/lib/mysql]
# Thu, 11 May 2023 22:37:46 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 11 May 2023 22:37:46 GMT
COPY file:94a071210c811522ac7cb9cd9b6d33b1df5eb056971fbdeefa8e9bc2e8a2d629 in /usr/local/bin/ 
# Thu, 11 May 2023 22:37:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:37:46 GMT
EXPOSE 3306
# Thu, 11 May 2023 22:37:46 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:f3f60f415e9a03eed88bd5dd5268c841cde08dacf16911a3ef1e4e0fcdd76568`  
		Last Modified: Wed, 26 Apr 2023 02:08:37 GMT  
		Size: 28.4 MB (28389440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bfb87016de46ece16208cd39b5fa89740b8e8db147c2da2f6483551b3e8d521`  
		Last Modified: Thu, 04 May 2023 03:49:02 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8bd3f48f8f1fc94a1a143132ba91e005df50ee4327d0e209553cc89145a91f`  
		Last Modified: Thu, 04 May 2023 03:49:03 GMT  
		Size: 5.4 MB (5409831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ebb0502bf43d03d32f27b6cfa9ea349e89bccb62bd1ef3cf96a9a769e6c1fa`  
		Last Modified: Thu, 04 May 2023 03:49:00 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c39b9daac872cd7020c71e2bcfb8c097a1ea4c92c6e75f0fa1c5457a9793fabd`  
		Last Modified: Thu, 11 May 2023 22:41:30 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d0e97236e823170f83bde496cd664d5a354bdc0e3812e70d9e9dc434a067506`  
		Last Modified: Thu, 11 May 2023 22:41:40 GMT  
		Size: 83.8 MB (83795910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b5a4e92f3071fd8c0fcaba769b1d01c887847907025859069a695bebdfd2ca`  
		Last Modified: Thu, 11 May 2023 22:41:30 GMT  
		Size: 3.5 KB (3527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e100a9688501846d85a74ce52c2427d070849317340c48bdb06946ff8f89178`  
		Last Modified: Thu, 11 May 2023 22:41:30 GMT  
		Size: 7.5 KB (7515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
