## `mariadb:10-jammy`

```console
$ docker pull mariadb@sha256:323be150a4d341806195e7bf1e8e7156b867bd74b38e8cbc655bdbe9cc549c42
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10-jammy` - linux; amd64

```console
$ docker pull mariadb@sha256:4a3c597b5b79c50fd33d2e08054a5d8e76c54a2e8be6755048f7ba0cd32d7e17
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123105566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b960e1164e178ba7dad5c2c4d081c39b5f8c9f2401c45c9e6a083f738cdc8bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Mon, 05 Jun 2023 17:00:37 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:00:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:00:39 GMT
ADD file:0ad2ee2cfb186802f49c9bf4148674d1c6fc201f83478ec01ffaa7086d491323 in / 
# Mon, 05 Jun 2023 17:00:39 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:06:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 16 Jun 2023 03:06:33 GMT
ENV GOSU_VERSION=1.14
# Fri, 16 Jun 2023 03:06:33 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 16 Jun 2023 03:06:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 16 Jun 2023 03:06:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 16 Jun 2023 03:06:55 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 03:07:46 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 16 Jun 2023 03:07:46 GMT
ARG MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Fri, 16 Jun 2023 03:07:46 GMT
ENV MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Fri, 16 Jun 2023 03:07:46 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
# Fri, 16 Jun 2023 03:07:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 27 Jun 2023 01:04:49 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 27 Jun 2023 01:04:50 GMT
VOLUME [/var/lib/mysql]
# Tue, 27 Jun 2023 01:04:50 GMT
COPY file:60282e2c078282f09827dfb0926d431a7ad71f6de3495a21fc8a846430fc5fc9 in /usr/local/bin/healthcheck.sh 
# Tue, 27 Jun 2023 01:04:50 GMT
COPY file:704c6685e9d99f08306a2726e0468f5a764a4040cc2eb6138c1be72ac2529bbc in /usr/local/bin/ 
# Tue, 27 Jun 2023 01:04:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 27 Jun 2023 01:04:50 GMT
EXPOSE 3306
# Tue, 27 Jun 2023 01:04:50 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:3f94e4e483ea634d7ab0b63649b8f72f8b721d4c626297fd0edae0abea1df9e9`  
		Last Modified: Tue, 06 Jun 2023 11:46:33 GMT  
		Size: 30.4 MB (30431039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:302c1621580e19854b06603807eaa8c8a41dbf662e3b700c5d13304a7a04a0a7`  
		Last Modified: Fri, 16 Jun 2023 03:11:09 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ebb34cbdd06fb95713e4ea56452cdc40b779d51e634dc8a48e2caa7af17b64`  
		Last Modified: Fri, 16 Jun 2023 03:11:10 GMT  
		Size: 5.6 MB (5592601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58c98f01d4c3c8a4524ea4b0478504e2041caddcd5fa0c323b6c27b9ec6418d6`  
		Last Modified: Fri, 16 Jun 2023 03:11:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:330f6531cfa6ca3e1005445e93e623e980ec57785971a371bc3f123f1be51ccb`  
		Last Modified: Fri, 16 Jun 2023 03:12:05 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e47775cc79ee084d5dee1aca3d3f732bcf2a4c2fe21845f1376acc319c2b3d8`  
		Last Modified: Tue, 27 Jun 2023 01:08:48 GMT  
		Size: 87.1 MB (87068573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:401aa1d60c2be6bfc153a990811a7c4020d46bbc4ea18735781c593386c21089`  
		Last Modified: Tue, 27 Jun 2023 01:08:36 GMT  
		Size: 3.6 KB (3565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:849edda0d8a1b0721e596ee72dee15d428a9364841527eb4c14c96d02d348844`  
		Last Modified: Tue, 27 Jun 2023 01:08:36 GMT  
		Size: 7.6 KB (7569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-jammy` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:5fd6061badec786f9112fc509a0e7425ebba50a6b61a5b23b2098f3844b1eb74
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117614005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc1ac9f163ddf9c086f5ff38af41a821e6b4c566ed2fa47dbf4042cac3abc9fb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Mon, 05 Jun 2023 17:11:17 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:11:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:11:19 GMT
ADD file:1043594b482384e967c94378b65ec4bc7a38190649a94f0325b7fb00be0a623e in / 
# Mon, 05 Jun 2023 17:11:19 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:33:00 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 16 Jun 2023 03:33:00 GMT
ENV GOSU_VERSION=1.14
# Fri, 16 Jun 2023 03:33:00 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 16 Jun 2023 03:33:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 16 Jun 2023 03:33:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 16 Jun 2023 03:33:16 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 03:34:10 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 16 Jun 2023 03:34:10 GMT
ARG MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Fri, 16 Jun 2023 03:34:11 GMT
ENV MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Fri, 16 Jun 2023 03:34:11 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
# Fri, 16 Jun 2023 03:34:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 26 Jun 2023 21:40:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Mon, 26 Jun 2023 21:40:52 GMT
VOLUME [/var/lib/mysql]
# Mon, 26 Jun 2023 21:40:52 GMT
COPY file:60282e2c078282f09827dfb0926d431a7ad71f6de3495a21fc8a846430fc5fc9 in /usr/local/bin/healthcheck.sh 
# Mon, 26 Jun 2023 21:40:52 GMT
COPY file:704c6685e9d99f08306a2726e0468f5a764a4040cc2eb6138c1be72ac2529bbc in /usr/local/bin/ 
# Mon, 26 Jun 2023 21:40:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 26 Jun 2023 21:40:52 GMT
EXPOSE 3306
# Mon, 26 Jun 2023 21:40:52 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:a1df1d4a17c6a461a5967be8a40f1158e55e0ae4dc3b3b7ae64f57cae69eb7e7`  
		Last Modified: Wed, 07 Jun 2023 02:07:18 GMT  
		Size: 28.4 MB (28389201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05b290c6ac487f967a3cd823bafe1c30bb68bd232b9b2613d8bf1db248f40a7`  
		Last Modified: Fri, 16 Jun 2023 03:37:21 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ced3b974154dd666267c51016a4a0c17bb6e86daedea57be9d24f6ae0865081`  
		Last Modified: Fri, 16 Jun 2023 03:37:22 GMT  
		Size: 5.4 MB (5405771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d9fc3506927dcba1816f485bd214ec1b2135d27e7af0731bb320526b091a30`  
		Last Modified: Fri, 16 Jun 2023 03:37:19 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e1c6adef7b5c9168367b4c23ece8d3d07da6273f8ec16dc9c385cd3e7124858`  
		Last Modified: Fri, 16 Jun 2023 03:38:10 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:771ac932193ae00759bb3abebdfa99638b592769ff1f49ca1f1dc0afc28f9ec2`  
		Last Modified: Mon, 26 Jun 2023 21:44:29 GMT  
		Size: 83.8 MB (83805673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7279dc082fc8e1a2dfd7840251700f4c5c06594dd81994ae3958cc246e4ac74`  
		Last Modified: Mon, 26 Jun 2023 21:44:19 GMT  
		Size: 3.6 KB (3564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1942227a9fbdb8ea52795fc23928fc408fba31f7eb87a17300ca743c03891bc0`  
		Last Modified: Mon, 26 Jun 2023 21:44:19 GMT  
		Size: 7.6 KB (7567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-jammy` - linux; ppc64le

```console
$ docker pull mariadb@sha256:a1a6dd6fca61b3d83a63368f8539ffecd9b41960b1aa25db591db4269c765786
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131775290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4adb9411855e8a1791184cc8087ef31c3061842db9536bf29431bfebe46f67cb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Mon, 05 Jun 2023 17:01:00 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:01:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:01:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:01:01 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:01:03 GMT
ADD file:00c4f44b35b683caef54d5b8b0e0b1e68872f45eae17dd7543adaf6c54512447 in / 
# Mon, 05 Jun 2023 17:01:04 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:42:09 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 16 Jun 2023 01:42:09 GMT
ENV GOSU_VERSION=1.14
# Fri, 16 Jun 2023 01:42:10 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 16 Jun 2023 01:42:49 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 16 Jun 2023 01:42:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 16 Jun 2023 01:42:51 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 01:45:13 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 16 Jun 2023 01:45:14 GMT
ARG MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Fri, 16 Jun 2023 01:45:14 GMT
ENV MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Fri, 16 Jun 2023 01:45:15 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
# Fri, 16 Jun 2023 01:45:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 16 Jun 2023 01:46:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 16 Jun 2023 01:46:16 GMT
VOLUME [/var/lib/mysql]
# Fri, 16 Jun 2023 01:46:17 GMT
COPY file:cee75098a882f7d33ad2c4c4325b29adc56fc66450e6cee3711d5a1af1bda714 in /usr/local/bin/healthcheck.sh 
# Fri, 16 Jun 2023 01:46:18 GMT
COPY file:cb2b72015a5493e1348f12f52b387586b863bcc87072708862e1aa2af0493eb9 in /usr/local/bin/ 
# Fri, 16 Jun 2023 01:46:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 01:46:18 GMT
EXPOSE 3306
# Fri, 16 Jun 2023 01:46:19 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:a02dd69d9a8a1e6f4fc2ccb509fb8efd6014b00ff932a757d23b4b012a2bec49`  
		Last Modified: Fri, 16 Jun 2023 00:44:52 GMT  
		Size: 35.7 MB (35711397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ef2f0de58dc6b86ab230fc24fdea7663e7c4036eaecb5cfaa5ca13d0538e76`  
		Last Modified: Fri, 16 Jun 2023 01:55:23 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:527730925c9b9eea7a40aa0f642c5ecb732e3ffe1537b1481481e867ece7fc5b`  
		Last Modified: Fri, 16 Jun 2023 01:55:25 GMT  
		Size: 6.0 MB (6017949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68b6ffe59959eb8b4ce9b862df0bc5e9542904c81ae9b29b3bb640e9df667043`  
		Last Modified: Fri, 16 Jun 2023 01:55:21 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ee680c9d760e2a0bf4493724c809bd0e81a429896ce65611874b0a8b39e853`  
		Last Modified: Fri, 16 Jun 2023 01:56:45 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11cd199fcb1c775fc919204e95bc88912375d6ab259742f906c6d06cacc178d5`  
		Last Modified: Fri, 16 Jun 2023 01:57:09 GMT  
		Size: 90.0 MB (90032888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d440fd831e73daa38b45a4aefd5d60485a7f6746cd33789332dcadff57c85fd7`  
		Last Modified: Fri, 16 Jun 2023 01:56:44 GMT  
		Size: 3.5 KB (3526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf3e61d4bed37af7fee89779ed5e3da010ee9388a64be1a03bb1817070647b58`  
		Last Modified: Fri, 16 Jun 2023 01:56:44 GMT  
		Size: 7.3 KB (7308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-jammy` - linux; s390x

```console
$ docker pull mariadb@sha256:7cde1a4982a31df55977d56a55fe6eaf70cad4530f90b0a1d6226582ea90d6ec
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.6 MB (121578324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af29d11399eb80a82e67b74755906318a7078cf0e7f010072b42d848972a6fcb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Mon, 05 Jun 2023 17:01:02 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:01:02 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:01:02 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:01:02 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:01:04 GMT
ADD file:2d2f31ec110b9e7ec21a9d4824a430acdaabf0b4e9c1cdd337438992859b57ae in / 
# Mon, 05 Jun 2023 17:01:04 GMT
CMD ["/bin/bash"]
# Mon, 26 Jun 2023 23:52:51 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Mon, 26 Jun 2023 23:52:51 GMT
ENV GOSU_VERSION=1.14
# Mon, 26 Jun 2023 23:52:51 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Mon, 26 Jun 2023 23:53:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 26 Jun 2023 23:53:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 26 Jun 2023 23:53:04 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jun 2023 23:53:52 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.11.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Mon, 26 Jun 2023 23:53:52 GMT
ARG MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Mon, 26 Jun 2023 23:53:53 GMT
ENV MARIADB_VERSION=1:10.11.4+maria~ubu2204
# Mon, 26 Jun 2023 23:53:53 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
# Mon, 26 Jun 2023 23:53:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 26 Jun 2023 23:54:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.11.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Mon, 26 Jun 2023 23:54:11 GMT
VOLUME [/var/lib/mysql]
# Mon, 26 Jun 2023 23:54:11 GMT
COPY file:60282e2c078282f09827dfb0926d431a7ad71f6de3495a21fc8a846430fc5fc9 in /usr/local/bin/healthcheck.sh 
# Mon, 26 Jun 2023 23:54:11 GMT
COPY file:704c6685e9d99f08306a2726e0468f5a764a4040cc2eb6138c1be72ac2529bbc in /usr/local/bin/ 
# Mon, 26 Jun 2023 23:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 26 Jun 2023 23:54:11 GMT
EXPOSE 3306
# Mon, 26 Jun 2023 23:54:11 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:fab1a8aa44b00432834b7776a76fd4149ec2fee2336a3521bd5435428df7edc9`  
		Last Modified: Fri, 16 Jun 2023 18:23:35 GMT  
		Size: 28.6 MB (28644581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53df3d5922d3642cd5911e0c6423d017ddded67995449ff6bd062e3ab5648f74`  
		Last Modified: Mon, 26 Jun 2023 23:56:48 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a58eec09b2021ab0d6c9ee2294b48d5688afc031c589a5dd0b64980d6fc12256`  
		Last Modified: Mon, 26 Jun 2023 23:56:49 GMT  
		Size: 5.5 MB (5470702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9e045ee2a4f7d3a9c8d566a084299a0e3f69d1017f5e40dde421bdff8527fd`  
		Last Modified: Mon, 26 Jun 2023 23:56:47 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911ccd5e848648303594348bd05e76842123393d6a7320b8a8704d9c85ca6255`  
		Last Modified: Mon, 26 Jun 2023 23:57:34 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1687ea072ae1a6d440dd43b06396617f0269e2cd33b593ed6755a006c816abfa`  
		Last Modified: Mon, 26 Jun 2023 23:57:47 GMT  
		Size: 87.4 MB (87449677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47bafce622cccebb4be5d96ec5480f894a2683c5fabccd2fc5eaf8e20401cb48`  
		Last Modified: Mon, 26 Jun 2023 23:57:34 GMT  
		Size: 3.6 KB (3566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3d6f2805a5010e5457702c07deccba128f489716b4386cb285ccdd5198e65a`  
		Last Modified: Mon, 26 Jun 2023 23:57:34 GMT  
		Size: 7.6 KB (7568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
