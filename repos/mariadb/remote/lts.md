## `mariadb:lts`

```console
$ docker pull mariadb@sha256:828b4dac595a4898b95f74373b90be3a9fcd3f3088331974fafe05cce506d35a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

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
$ docker pull mariadb@sha256:886bd9c1e252885703993768b93073e88ff816889ede2daff07a64d87c8dda8d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117603176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:030ee12b5b896fbc3be3321ca4671ebc7c5c51273ff20d7ed324df379de68154`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Mon, 22 May 2023 17:53:00 GMT
ARG RELEASE
# Mon, 22 May 2023 17:53:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 22 May 2023 17:53:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 22 May 2023 17:53:01 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 22 May 2023 17:53:07 GMT
ADD file:f0435ed8dcf91cc69ec63b6b16d9efac56e5a6a7ec518e1fcc3df7457d3113ed in / 
# Mon, 22 May 2023 17:53:08 GMT
CMD ["/bin/bash"]
# Thu, 01 Jun 2023 23:40:52 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 01 Jun 2023 23:40:52 GMT
ENV GOSU_VERSION=1.14
# Thu, 01 Jun 2023 23:40:52 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 01 Jun 2023 23:41:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 01 Jun 2023 23:41:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 01 Jun 2023 23:41:08 GMT
ENV LANG=C.UTF-8
# Thu, 01 Jun 2023 23:41:39 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.3 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Thu, 01 Jun 2023 23:41:39 GMT
ARG MARIADB_VERSION=1:10.11.3+maria~ubu2204
# Thu, 01 Jun 2023 23:41:39 GMT
ENV MARIADB_VERSION=1:10.11.3+maria~ubu2204
# Thu, 01 Jun 2023 23:41:39 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
# Thu, 01 Jun 2023 23:41:40 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 01 Jun 2023 23:41:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Thu, 01 Jun 2023 23:41:59 GMT
VOLUME [/var/lib/mysql]
# Thu, 01 Jun 2023 23:41:59 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Thu, 01 Jun 2023 23:41:59 GMT
COPY file:94a071210c811522ac7cb9cd9b6d33b1df5eb056971fbdeefa8e9bc2e8a2d629 in /usr/local/bin/ 
# Thu, 01 Jun 2023 23:41:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Jun 2023 23:41:59 GMT
EXPOSE 3306
# Thu, 01 Jun 2023 23:41:59 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:6c7698a779f6d8c45a39a6721fb5cce267d66ff8ab5181c55aa6d02c8ddacd01`  
		Last Modified: Tue, 23 May 2023 02:05:13 GMT  
		Size: 28.4 MB (28389044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3beef926275df9bcc0f302dcc80b1df1778597e3762c0bcba4aba7cb6640680`  
		Last Modified: Thu, 01 Jun 2023 23:43:36 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd40ffbb6cb3906cf4feaa019e5002505b5aa18f7fc6fc78552fe0499d3b56b0`  
		Last Modified: Thu, 01 Jun 2023 23:43:37 GMT  
		Size: 5.4 MB (5405164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31691bc52e3b474eb0509035feef6f06782d2807ad942714f4d3830b8c5aa1b0`  
		Last Modified: Thu, 01 Jun 2023 23:43:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49840160095fb7b855e6cb7131cfc8b9fe0fbb7a6ab0548f457396e1e41ba786`  
		Last Modified: Thu, 01 Jun 2023 23:43:56 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:390c12b9e644ce89f8619c194ac28a2009720c223817f96e1d85f3d4e6b19c87`  
		Last Modified: Thu, 01 Jun 2023 23:44:06 GMT  
		Size: 83.8 MB (83795698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b1d471f4b5ac9b9cd0f057fd85748f08c3ab2323e7cf2654d3aa6f3917b999`  
		Last Modified: Thu, 01 Jun 2023 23:43:56 GMT  
		Size: 3.5 KB (3525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c803e18c0cb9843d9df011baedca9e93d836f7290b615987fabcd871007b8f7`  
		Last Modified: Thu, 01 Jun 2023 23:43:56 GMT  
		Size: 7.5 KB (7515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:lts` - linux; ppc64le

```console
$ docker pull mariadb@sha256:4e1012010879de84fbb42aca83353a0566666e9aded4ab4829d26f90f2767dcf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131778071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a85f74ad3cb30cdb96091760626c669badeca09c22371e610df9434d4009fc6`
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
# Fri, 12 May 2023 00:11:33 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.3 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 12 May 2023 00:11:34 GMT
ARG MARIADB_VERSION=1:10.11.3+maria~ubu2204
# Fri, 12 May 2023 00:11:34 GMT
ENV MARIADB_VERSION=1:10.11.3+maria~ubu2204
# Fri, 12 May 2023 00:11:35 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
# Fri, 12 May 2023 00:11:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 12 May 2023 00:13:07 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 12 May 2023 00:13:12 GMT
VOLUME [/var/lib/mysql]
# Fri, 12 May 2023 00:13:13 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Fri, 12 May 2023 00:13:13 GMT
COPY file:94a071210c811522ac7cb9cd9b6d33b1df5eb056971fbdeefa8e9bc2e8a2d629 in /usr/local/bin/ 
# Fri, 12 May 2023 00:13:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 May 2023 00:13:14 GMT
EXPOSE 3306
# Fri, 12 May 2023 00:13:14 GMT
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
	-	`sha256:8b9e3a656db00d10f138f8b8fc2c2b73a7aaeccf3c1a7dbb33ee8d4ed74c8c71`  
		Last Modified: Fri, 12 May 2023 00:27:08 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c82780e8d87431789bc1e19cc60f76673562df9f918c2bfc111a36e4ab69bc2`  
		Last Modified: Fri, 12 May 2023 00:27:33 GMT  
		Size: 90.0 MB (90030442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7132acf535f21b86ef9489710e7cc0bae905e94205595566e7c3de8a2daaec7b`  
		Last Modified: Fri, 12 May 2023 00:27:08 GMT  
		Size: 3.5 KB (3527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be82f8f5e0b7ab4863e1d243afe4a12b6128ff93673c9f95bb4a315590f9a27c`  
		Last Modified: Fri, 12 May 2023 00:27:08 GMT  
		Size: 7.5 KB (7515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
