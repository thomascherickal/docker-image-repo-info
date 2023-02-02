## `mariadb:10-jammy`

```console
$ docker pull mariadb@sha256:bfc25a68e113de43d0d112f5a7126df8e278579c3224e3923359e1c1d8d5ce6e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10-jammy` - linux; amd64

```console
$ docker pull mariadb@sha256:569cda3a16fbd0235d20a0f895c9a906e022a75eeeb836da6c29f9a542cccf75
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125686970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:039bd724508bee8d3247e2219a9019b57eb788e1f6dac6cefa9906ce80e433e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 26 Jan 2023 04:57:59 GMT
ARG RELEASE
# Thu, 26 Jan 2023 04:57:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 04:58:02 GMT
ADD file:18e71f049606f6339ce7a995839623f50e6ec6474bfd0a3a7ca799db726f47f6 in / 
# Thu, 26 Jan 2023 04:58:02 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:41:49 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 31 Jan 2023 18:41:49 GMT
ENV GOSU_VERSION=1.14
# Tue, 31 Jan 2023 18:41:49 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 31 Jan 2023 18:42:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 31 Jan 2023 18:42:07 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 31 Jan 2023 18:42:07 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 18:42:46 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.10.2 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 31 Jan 2023 18:42:47 GMT
ARG MARIADB_VERSION=1:10.10.2+maria~ubu2204
# Tue, 31 Jan 2023 18:42:47 GMT
ENV MARIADB_VERSION=1:10.10.2+maria~ubu2204
# Tue, 31 Jan 2023 18:42:47 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.2/repo/ubuntu/ jammy main
# Tue, 31 Jan 2023 18:42:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 31 Jan 2023 18:43:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 31 Jan 2023 18:43:09 GMT
VOLUME [/var/lib/mysql]
# Tue, 31 Jan 2023 18:43:09 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Tue, 31 Jan 2023 18:43:09 GMT
COPY file:ebdfbcbc74dda1874f1c75d86e1c32733edb402d13440b2b7140a952010bc21f in /usr/local/bin/ 
# Tue, 31 Jan 2023 18:43:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Jan 2023 18:43:09 GMT
EXPOSE 3306
# Tue, 31 Jan 2023 18:43:09 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:10ac4908093d4325f2c94b2c9a571fa1071a17a72dd9c21c1ffb2c86f68ca028`  
		Last Modified: Thu, 26 Jan 2023 08:46:26 GMT  
		Size: 30.4 MB (30429004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44779101e748f75ed5c15e71623718a3a0da88462d3300331a0deb1fc2012dec`  
		Last Modified: Tue, 31 Jan 2023 18:48:21 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a721db3e3f3d1be16602fce85cd2feff91a9104107efce1d51f0ee623f397024`  
		Last Modified: Tue, 31 Jan 2023 18:48:22 GMT  
		Size: 5.5 MB (5525584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1850a929b84ae3d753f63aa0155a580c8c638f888b87d8c8c9c2ff9e6a4c2f21`  
		Last Modified: Tue, 31 Jan 2023 18:48:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:397a918c7da3c28902e77179cc9a1d31ca5eb9e48cb73745a4824ff022ec598b`  
		Last Modified: Tue, 31 Jan 2023 18:48:45 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:806be17e856df1962f97221cf9f8ad6ee74f3f60d42945b1d16722f24d5257fd`  
		Last Modified: Tue, 31 Jan 2023 18:48:59 GMT  
		Size: 89.7 MB (89719701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634de6c90876c763e80e6030370c0a397f1cf9b2cbbcd0d42fb053b36f4b37f9`  
		Last Modified: Tue, 31 Jan 2023 18:48:45 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd00854cfb1a76890930090bcbbd5c59b3c873353b907dfef16c182978df10e7`  
		Last Modified: Tue, 31 Jan 2023 18:48:45 GMT  
		Size: 7.0 KB (6971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-jammy` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:315e03c1fbeb013c732d84656c419ced4487d41da6dccef31ccf4772820994de
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.2 MB (120198334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a252ec6f0e4abc72c9e00ef48697d7e1c827e636f60d5586b67a8e74e1ef9f75`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 26 Jan 2023 05:05:49 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:05:49 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:05:49 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:05:50 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:05:51 GMT
ADD file:55486a91f732042dd4e81ecfd8457d23e04dcd7dd80a0bb06cc7c44873fac838 in / 
# Thu, 26 Jan 2023 05:05:51 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:58:49 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 31 Jan 2023 18:58:49 GMT
ENV GOSU_VERSION=1.14
# Tue, 31 Jan 2023 18:58:49 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 31 Jan 2023 18:59:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 31 Jan 2023 18:59:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 31 Jan 2023 18:59:06 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 18:59:46 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.10.2 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 31 Jan 2023 18:59:46 GMT
ARG MARIADB_VERSION=1:10.10.2+maria~ubu2204
# Tue, 31 Jan 2023 18:59:47 GMT
ENV MARIADB_VERSION=1:10.10.2+maria~ubu2204
# Tue, 31 Jan 2023 18:59:47 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.2/repo/ubuntu/ jammy main
# Tue, 31 Jan 2023 18:59:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 31 Jan 2023 19:00:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 31 Jan 2023 19:00:07 GMT
VOLUME [/var/lib/mysql]
# Tue, 31 Jan 2023 19:00:07 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Tue, 31 Jan 2023 19:00:07 GMT
COPY file:ebdfbcbc74dda1874f1c75d86e1c32733edb402d13440b2b7140a952010bc21f in /usr/local/bin/ 
# Tue, 31 Jan 2023 19:00:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Jan 2023 19:00:07 GMT
EXPOSE 3306
# Tue, 31 Jan 2023 19:00:07 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:565cb979c5c01279efcd69c4457a9954801b6be6da65894374260ec92d993891`  
		Last Modified: Thu, 26 Jan 2023 16:22:40 GMT  
		Size: 28.4 MB (28384974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69f4258cab38852673e53c594c585f87577f69776492968b4e19c7daebb15fdf`  
		Last Modified: Tue, 31 Jan 2023 19:04:34 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75aa640c13b12193dc224bc9f5b4910fbc69b99a150826e3128a9c1b19a0ae49`  
		Last Modified: Tue, 31 Jan 2023 19:04:35 GMT  
		Size: 5.3 MB (5339546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:158ff8362680c557055e043bda03294414a00c3cd19b1e92fe7b6e1c221e4cc5`  
		Last Modified: Tue, 31 Jan 2023 19:04:32 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6af53dbcc52b70eeb59a058fc9f806f44d5f16804f0f842c01fcfde93ab0ade`  
		Last Modified: Tue, 31 Jan 2023 19:04:57 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee0542ebe9297e1f697b31c168edc86855279babe84e89565af21c93f0b0aa3`  
		Last Modified: Tue, 31 Jan 2023 19:05:07 GMT  
		Size: 86.5 MB (86461124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10afc8d4c5a207bf1ad3c45247fb775336de89f7ad40fae357d7eddf0d6893ec`  
		Last Modified: Tue, 31 Jan 2023 19:04:57 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0c228ae19c23cb9054079d139dcae5addba0c1d423b3d780e4c282e1cd96d6`  
		Last Modified: Tue, 31 Jan 2023 19:04:56 GMT  
		Size: 7.0 KB (6971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-jammy` - linux; ppc64le

```console
$ docker pull mariadb@sha256:f2ef89a82602a7f48dd37c7960e823b840a88e76c0290557a2c8eccb126dbbe5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.5 MB (134534888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d71c25ab70361039151ab147fb387290b965c89a5598eeda987b66eeb6b8844a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 26 Jan 2023 04:58:24 GMT
ARG RELEASE
# Thu, 26 Jan 2023 04:58:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 04:58:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 04:58:24 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 04:58:28 GMT
ADD file:f0400001a50847feb579e66e804ec9daaaaeb9a414b4b5cca8bb0c8e9c7fa8f9 in / 
# Thu, 26 Jan 2023 04:58:28 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:09:57 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 31 Jan 2023 19:09:57 GMT
ENV GOSU_VERSION=1.14
# Tue, 31 Jan 2023 19:09:58 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 31 Jan 2023 19:10:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 31 Jan 2023 19:10:35 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 31 Jan 2023 19:10:36 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:11:51 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.10.2 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 31 Jan 2023 19:11:51 GMT
ARG MARIADB_VERSION=1:10.10.2+maria~ubu2204
# Tue, 31 Jan 2023 19:11:52 GMT
ENV MARIADB_VERSION=1:10.10.2+maria~ubu2204
# Tue, 31 Jan 2023 19:11:52 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.2/repo/ubuntu/ jammy main
# Tue, 31 Jan 2023 19:11:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 31 Jan 2023 19:12:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 31 Jan 2023 19:12:40 GMT
VOLUME [/var/lib/mysql]
# Tue, 31 Jan 2023 19:12:40 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Tue, 31 Jan 2023 19:12:40 GMT
COPY file:ebdfbcbc74dda1874f1c75d86e1c32733edb402d13440b2b7140a952010bc21f in /usr/local/bin/ 
# Tue, 31 Jan 2023 19:12:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Jan 2023 19:12:41 GMT
EXPOSE 3306
# Tue, 31 Jan 2023 19:12:41 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:b919bd9d6c8a596b3ac4fb9ee1cc6727efdd1f1b05e5c130efec5deaae53ae60`  
		Last Modified: Tue, 31 Jan 2023 17:52:01 GMT  
		Size: 35.7 MB (35708930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34925dcc400f2a1b514093e0e4de02d73abcf3ee0f349a1cbb3c0e3b52d3e5d5`  
		Last Modified: Tue, 31 Jan 2023 19:22:46 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:864dbb2cdeef8067c1d6080aa272db95e8b2722ee45171da9994b7d9538573b3`  
		Last Modified: Tue, 31 Jan 2023 19:22:47 GMT  
		Size: 6.0 MB (5952082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b679f99da80d64217bbc8bdd99da752f0a09d997d590717a04303c9485e8643`  
		Last Modified: Tue, 31 Jan 2023 19:22:43 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1994a7aa1cfc51046540b48560bc9ab8cc69aa1157c2cff9416ae639643d680`  
		Last Modified: Tue, 31 Jan 2023 19:23:26 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec4debae2676f9e8952e5edf466d42ff10a5ae9424c5d1a6e66aad4cfad4cc12`  
		Last Modified: Tue, 31 Jan 2023 19:23:51 GMT  
		Size: 92.9 MB (92861184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d75ce9ceedaf276d7fb7ef5393b0acfba3d0325735219445a28d7f30bf73222`  
		Last Modified: Tue, 31 Jan 2023 19:23:26 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:979c33fde596d89eebf2fcaf238828094a3cd8c3e164cf92bfad1bbd68bf4480`  
		Last Modified: Tue, 31 Jan 2023 19:23:26 GMT  
		Size: 7.0 KB (6973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-jammy` - linux; s390x

```console
$ docker pull mariadb@sha256:46a236dec65334d197810c16fb4be6b9f50fee6b972751176c664dc1479f9277
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.1 MB (124109851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a821d22da5ba91606e436d1e56d04f9821e0f1f2f4951181be05c395f6c13938`
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
# Tue, 31 Jan 2023 18:43:47 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.10.2 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 31 Jan 2023 18:43:47 GMT
ARG MARIADB_VERSION=1:10.10.2+maria~ubu2204
# Tue, 31 Jan 2023 18:43:48 GMT
ENV MARIADB_VERSION=1:10.10.2+maria~ubu2204
# Tue, 31 Jan 2023 18:43:48 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.2/repo/ubuntu/ jammy main
# Tue, 31 Jan 2023 18:43:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 31 Jan 2023 18:44:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 31 Jan 2023 18:44:08 GMT
VOLUME [/var/lib/mysql]
# Tue, 31 Jan 2023 18:44:08 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Tue, 31 Jan 2023 18:44:08 GMT
COPY file:ebdfbcbc74dda1874f1c75d86e1c32733edb402d13440b2b7140a952010bc21f in /usr/local/bin/ 
# Tue, 31 Jan 2023 18:44:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Jan 2023 18:44:08 GMT
EXPOSE 3306
# Tue, 31 Jan 2023 18:44:08 GMT
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
	-	`sha256:63a110c3a8f2e88448d7dfc51834d374e406a420acfa7f7f21074b2b00503851`  
		Last Modified: Tue, 31 Jan 2023 18:48:48 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27753964f61234df97e812193e77b4b2a9cdd89bed2c4fa4aae6c4949d591ab`  
		Last Modified: Tue, 31 Jan 2023 18:49:00 GMT  
		Size: 90.1 MB (90053410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91ad2ebd988291e9a388e3b51b27a0ef3b2d53513b62ef1d91facc8e26ae1f2f`  
		Last Modified: Tue, 31 Jan 2023 18:48:48 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d6e4de547f3a491667babed2f5ebbdd1a3696d5738a8a0e6bb1a40fd4f3519`  
		Last Modified: Tue, 31 Jan 2023 18:48:48 GMT  
		Size: 7.0 KB (6971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
