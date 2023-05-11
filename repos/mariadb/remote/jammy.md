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
