<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mysql`

-	[`mysql:5`](#mysql5)
-	[`mysql:5-debian`](#mysql5-debian)
-	[`mysql:5-oracle`](#mysql5-oracle)
-	[`mysql:5.7`](#mysql57)
-	[`mysql:5.7-debian`](#mysql57-debian)
-	[`mysql:5.7-oracle`](#mysql57-oracle)
-	[`mysql:5.7.38`](#mysql5738)
-	[`mysql:5.7.38-debian`](#mysql5738-debian)
-	[`mysql:5.7.38-oracle`](#mysql5738-oracle)
-	[`mysql:8`](#mysql8)
-	[`mysql:8-debian`](#mysql8-debian)
-	[`mysql:8-oracle`](#mysql8-oracle)
-	[`mysql:8.0`](#mysql80)
-	[`mysql:8.0-debian`](#mysql80-debian)
-	[`mysql:8.0-oracle`](#mysql80-oracle)
-	[`mysql:8.0.29`](#mysql8029)
-	[`mysql:8.0.29-debian`](#mysql8029-debian)
-	[`mysql:8.0.29-oracle`](#mysql8029-oracle)
-	[`mysql:debian`](#mysqldebian)
-	[`mysql:latest`](#mysqllatest)
-	[`mysql:oracle`](#mysqloracle)

## `mysql:5`

```console
$ docker pull mysql@sha256:7e99b2b8d5bca914ef31059858210f57b009c40375d647f0d4d65ecd01d6b1d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5` - linux; amd64

```console
$ docker pull mysql@sha256:06c614dfc9720ccc0177acf700d0e0794f0efe3a032e78ea5318c30886ce62c1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.5 MB (162456143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a0961b7de03c7b11afd13fec09d0d30992b6e0b4f947a4aba4273723778ed95`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 28 May 2022 01:20:43 GMT
ADD file:0513eda9512e010cb9459591b62e0c9d9319750923df091b64250ad6e98c2878 in / 
# Sat, 28 May 2022 01:20:43 GMT
CMD ["bash"]
# Sat, 28 May 2022 05:33:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 28 May 2022 05:33:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:33:14 GMT
ENV GOSU_VERSION=1.14
# Sat, 28 May 2022 05:33:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 28 May 2022 05:33:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 28 May 2022 05:33:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:33:31 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Sat, 28 May 2022 05:33:57 GMT
ENV MYSQL_MAJOR=5.7
# Sat, 28 May 2022 05:33:57 GMT
ENV MYSQL_VERSION=5.7.38-1debian10
# Sat, 28 May 2022 05:33:58 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Sat, 28 May 2022 05:34:16 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Sat, 28 May 2022 05:34:17 GMT
VOLUME [/var/lib/mysql]
# Sat, 28 May 2022 05:34:17 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Sat, 28 May 2022 05:34:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 28 May 2022 05:34:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 May 2022 05:34:17 GMT
EXPOSE 3306 33060
# Sat, 28 May 2022 05:34:18 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c1ad9731b2c7bf7fddea67f2f3f553515179a375c489e591e2372700fcaca766`  
		Last Modified: Sat, 28 May 2022 01:26:05 GMT  
		Size: 27.1 MB (27140144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f6eb0ee84d0c793cbd8456f03775cc5d88f72c576ec455596dca4ad465df07`  
		Last Modified: Sat, 28 May 2022 05:34:47 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cffcf8691bc5ddfc0c45d837fef9c77c7e264f7a69faf37073d0c4b31fb87156`  
		Last Modified: Sat, 28 May 2022 05:34:48 GMT  
		Size: 4.2 MB (4179298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89a783b5ac8a82c6355c62896648cb37efdc387f41b31b5c1d09418ce1808e81`  
		Last Modified: Sat, 28 May 2022 05:34:45 GMT  
		Size: 1.4 MB (1386680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8393c7be5fa5ff5d50fba15ce47f16cb29d3363d3885632e7892c0854a4d9c`  
		Last Modified: Sat, 28 May 2022 05:34:45 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af768d0b181edf1d8a35699d64f8e71d05d7648a28c37a5ab6fe2e36ffddc5e0`  
		Last Modified: Sat, 28 May 2022 05:34:48 GMT  
		Size: 14.1 MB (14064399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:810d6aaaf54a9c0c9d817fd1615f43aaf0194bcc1fca1574a90e90d8f6d66c6a`  
		Last Modified: Sat, 28 May 2022 05:34:45 GMT  
		Size: 2.5 KB (2547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fe6daf23954caa3d837bbd8317dcde57ad466ad3ca6e0c4b8f0f3c61ee451b`  
		Last Modified: Sat, 28 May 2022 05:35:29 GMT  
		Size: 254.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ccf426818fd53d690090f3e6029160dec25694793d6b77a52e80ff70d7651e2`  
		Last Modified: Sat, 28 May 2022 05:35:45 GMT  
		Size: 115.7 MB (115675662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68b838b06054d3f3b54fea8f73531a1908182330b6571c08f5453c78aa879901`  
		Last Modified: Sat, 28 May 2022 05:35:29 GMT  
		Size: 5.2 KB (5155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b606c4f93dfd881271b87ffd349ff0467a9fe1354d461f8d1a54934a1457c37`  
		Last Modified: Sat, 28 May 2022 05:35:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5-debian`

```console
$ docker pull mysql@sha256:7e99b2b8d5bca914ef31059858210f57b009c40375d647f0d4d65ecd01d6b1d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5-debian` - linux; amd64

```console
$ docker pull mysql@sha256:06c614dfc9720ccc0177acf700d0e0794f0efe3a032e78ea5318c30886ce62c1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.5 MB (162456143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a0961b7de03c7b11afd13fec09d0d30992b6e0b4f947a4aba4273723778ed95`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 28 May 2022 01:20:43 GMT
ADD file:0513eda9512e010cb9459591b62e0c9d9319750923df091b64250ad6e98c2878 in / 
# Sat, 28 May 2022 01:20:43 GMT
CMD ["bash"]
# Sat, 28 May 2022 05:33:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 28 May 2022 05:33:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:33:14 GMT
ENV GOSU_VERSION=1.14
# Sat, 28 May 2022 05:33:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 28 May 2022 05:33:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 28 May 2022 05:33:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:33:31 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Sat, 28 May 2022 05:33:57 GMT
ENV MYSQL_MAJOR=5.7
# Sat, 28 May 2022 05:33:57 GMT
ENV MYSQL_VERSION=5.7.38-1debian10
# Sat, 28 May 2022 05:33:58 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Sat, 28 May 2022 05:34:16 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Sat, 28 May 2022 05:34:17 GMT
VOLUME [/var/lib/mysql]
# Sat, 28 May 2022 05:34:17 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Sat, 28 May 2022 05:34:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 28 May 2022 05:34:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 May 2022 05:34:17 GMT
EXPOSE 3306 33060
# Sat, 28 May 2022 05:34:18 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c1ad9731b2c7bf7fddea67f2f3f553515179a375c489e591e2372700fcaca766`  
		Last Modified: Sat, 28 May 2022 01:26:05 GMT  
		Size: 27.1 MB (27140144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f6eb0ee84d0c793cbd8456f03775cc5d88f72c576ec455596dca4ad465df07`  
		Last Modified: Sat, 28 May 2022 05:34:47 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cffcf8691bc5ddfc0c45d837fef9c77c7e264f7a69faf37073d0c4b31fb87156`  
		Last Modified: Sat, 28 May 2022 05:34:48 GMT  
		Size: 4.2 MB (4179298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89a783b5ac8a82c6355c62896648cb37efdc387f41b31b5c1d09418ce1808e81`  
		Last Modified: Sat, 28 May 2022 05:34:45 GMT  
		Size: 1.4 MB (1386680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8393c7be5fa5ff5d50fba15ce47f16cb29d3363d3885632e7892c0854a4d9c`  
		Last Modified: Sat, 28 May 2022 05:34:45 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af768d0b181edf1d8a35699d64f8e71d05d7648a28c37a5ab6fe2e36ffddc5e0`  
		Last Modified: Sat, 28 May 2022 05:34:48 GMT  
		Size: 14.1 MB (14064399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:810d6aaaf54a9c0c9d817fd1615f43aaf0194bcc1fca1574a90e90d8f6d66c6a`  
		Last Modified: Sat, 28 May 2022 05:34:45 GMT  
		Size: 2.5 KB (2547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fe6daf23954caa3d837bbd8317dcde57ad466ad3ca6e0c4b8f0f3c61ee451b`  
		Last Modified: Sat, 28 May 2022 05:35:29 GMT  
		Size: 254.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ccf426818fd53d690090f3e6029160dec25694793d6b77a52e80ff70d7651e2`  
		Last Modified: Sat, 28 May 2022 05:35:45 GMT  
		Size: 115.7 MB (115675662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68b838b06054d3f3b54fea8f73531a1908182330b6571c08f5453c78aa879901`  
		Last Modified: Sat, 28 May 2022 05:35:29 GMT  
		Size: 5.2 KB (5155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b606c4f93dfd881271b87ffd349ff0467a9fe1354d461f8d1a54934a1457c37`  
		Last Modified: Sat, 28 May 2022 05:35:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5-oracle`

```console
$ docker pull mysql@sha256:c67e9e97879305e0c7a4934372f35bdb7d79d4a0914d7304d0ee6836be0127a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:3030fdb1154e62ed44c2e2dbbc7dee2643ee27fb6dd201b06b19a87682498e8b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.9 MB (126873058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f19b3d18c4a01f69bdb995e46233fcdcc66c1ef84bc8d28396e981c020e395ee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 16 Jun 2022 01:20:22 GMT
ADD file:5e615d6d49ec50cba937fa86f5fb7d6a4a7e680b2b4f5b659e879b95304c0417 in / 
# Thu, 16 Jun 2022 01:20:22 GMT
CMD ["/bin/bash"]
# Thu, 16 Jun 2022 01:38:41 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Thu, 16 Jun 2022 01:38:41 GMT
ENV GOSU_VERSION=1.14
# Thu, 16 Jun 2022 01:38:45 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 16 Jun 2022 01:38:55 GMT
RUN set -eux; 	yum install -y 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Thu, 16 Jun 2022 01:38:56 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 16 Jun 2022 01:38:56 GMT
ENV MYSQL_MAJOR=5.7
# Thu, 16 Jun 2022 01:38:56 GMT
ENV MYSQL_VERSION=5.7.38-1.el7
# Thu, 16 Jun 2022 01:38:57 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Thu, 16 Jun 2022 01:39:11 GMT
RUN set -eux; 	yum install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Thu, 16 Jun 2022 01:39:11 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Thu, 16 Jun 2022 01:39:12 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el7
# Thu, 16 Jun 2022 01:39:29 GMT
RUN set -eux; 	yum install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Thu, 16 Jun 2022 01:39:30 GMT
VOLUME [/var/lib/mysql]
# Thu, 16 Jun 2022 01:39:30 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Thu, 16 Jun 2022 01:39:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Jun 2022 01:39:31 GMT
EXPOSE 3306 33060
# Thu, 16 Jun 2022 01:39:31 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:63183c9b4598e16c4cef95f706d50ff6c928de41f391cd513495b27eaa27bf89`  
		Last Modified: Thu, 16 Jun 2022 01:21:08 GMT  
		Size: 48.8 MB (48757931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:921fb508f1d1aecc5558b119c43c60ca99e2803d417ea98b5a55f94975ac5440`  
		Last Modified: Thu, 16 Jun 2022 01:40:10 GMT  
		Size: 1.1 KB (1059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c722a284ecb6bbcc3803b2a9fb3df9e58ebd491e421507db7c73d8f4255cf0f4`  
		Last Modified: Thu, 16 Jun 2022 01:40:09 GMT  
		Size: 930.2 KB (930225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e1ea46ae00991c24638c08d268652beb0ce5b878c83d34964f12345618c8941`  
		Last Modified: Thu, 16 Jun 2022 01:40:11 GMT  
		Size: 3.8 MB (3750823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15dccdcd437d9fe54d225731d32bb52246dc75794a5d49e7f12010322dd06c1`  
		Last Modified: Thu, 16 Jun 2022 01:40:08 GMT  
		Size: 2.7 KB (2659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1050fbf8b84448d369e5743034ffd13580e9313a7e5092eace10220aa687f9b`  
		Last Modified: Thu, 16 Jun 2022 01:40:06 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848d1501cd8fc9f77a4e51a2e6dc077dcc0e468191ffaf2f433a4ffb4f7f63c1`  
		Last Modified: Thu, 16 Jun 2022 01:40:10 GMT  
		Size: 25.5 MB (25466694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98f50b8fa8c9ba100ca41212bdb8cb892fa707fb9395959c967bcc9355b3ddea`  
		Last Modified: Thu, 16 Jun 2022 01:40:06 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8b3d4a8dbcebd64c0cd3dcde292b97e52335441dac4d3c0e8e010d1197578b`  
		Last Modified: Thu, 16 Jun 2022 01:40:15 GMT  
		Size: 48.0 MB (47957859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4284667ffa5966a13950eda5dee3eb23bc10e60d2dee427c9e7c18c789099568`  
		Last Modified: Thu, 16 Jun 2022 01:40:06 GMT  
		Size: 5.2 KB (5159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7`

```console
$ docker pull mysql@sha256:7e99b2b8d5bca914ef31059858210f57b009c40375d647f0d4d65ecd01d6b1d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7` - linux; amd64

```console
$ docker pull mysql@sha256:06c614dfc9720ccc0177acf700d0e0794f0efe3a032e78ea5318c30886ce62c1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.5 MB (162456143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a0961b7de03c7b11afd13fec09d0d30992b6e0b4f947a4aba4273723778ed95`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 28 May 2022 01:20:43 GMT
ADD file:0513eda9512e010cb9459591b62e0c9d9319750923df091b64250ad6e98c2878 in / 
# Sat, 28 May 2022 01:20:43 GMT
CMD ["bash"]
# Sat, 28 May 2022 05:33:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 28 May 2022 05:33:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:33:14 GMT
ENV GOSU_VERSION=1.14
# Sat, 28 May 2022 05:33:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 28 May 2022 05:33:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 28 May 2022 05:33:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:33:31 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Sat, 28 May 2022 05:33:57 GMT
ENV MYSQL_MAJOR=5.7
# Sat, 28 May 2022 05:33:57 GMT
ENV MYSQL_VERSION=5.7.38-1debian10
# Sat, 28 May 2022 05:33:58 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Sat, 28 May 2022 05:34:16 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Sat, 28 May 2022 05:34:17 GMT
VOLUME [/var/lib/mysql]
# Sat, 28 May 2022 05:34:17 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Sat, 28 May 2022 05:34:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 28 May 2022 05:34:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 May 2022 05:34:17 GMT
EXPOSE 3306 33060
# Sat, 28 May 2022 05:34:18 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c1ad9731b2c7bf7fddea67f2f3f553515179a375c489e591e2372700fcaca766`  
		Last Modified: Sat, 28 May 2022 01:26:05 GMT  
		Size: 27.1 MB (27140144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f6eb0ee84d0c793cbd8456f03775cc5d88f72c576ec455596dca4ad465df07`  
		Last Modified: Sat, 28 May 2022 05:34:47 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cffcf8691bc5ddfc0c45d837fef9c77c7e264f7a69faf37073d0c4b31fb87156`  
		Last Modified: Sat, 28 May 2022 05:34:48 GMT  
		Size: 4.2 MB (4179298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89a783b5ac8a82c6355c62896648cb37efdc387f41b31b5c1d09418ce1808e81`  
		Last Modified: Sat, 28 May 2022 05:34:45 GMT  
		Size: 1.4 MB (1386680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8393c7be5fa5ff5d50fba15ce47f16cb29d3363d3885632e7892c0854a4d9c`  
		Last Modified: Sat, 28 May 2022 05:34:45 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af768d0b181edf1d8a35699d64f8e71d05d7648a28c37a5ab6fe2e36ffddc5e0`  
		Last Modified: Sat, 28 May 2022 05:34:48 GMT  
		Size: 14.1 MB (14064399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:810d6aaaf54a9c0c9d817fd1615f43aaf0194bcc1fca1574a90e90d8f6d66c6a`  
		Last Modified: Sat, 28 May 2022 05:34:45 GMT  
		Size: 2.5 KB (2547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fe6daf23954caa3d837bbd8317dcde57ad466ad3ca6e0c4b8f0f3c61ee451b`  
		Last Modified: Sat, 28 May 2022 05:35:29 GMT  
		Size: 254.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ccf426818fd53d690090f3e6029160dec25694793d6b77a52e80ff70d7651e2`  
		Last Modified: Sat, 28 May 2022 05:35:45 GMT  
		Size: 115.7 MB (115675662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68b838b06054d3f3b54fea8f73531a1908182330b6571c08f5453c78aa879901`  
		Last Modified: Sat, 28 May 2022 05:35:29 GMT  
		Size: 5.2 KB (5155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b606c4f93dfd881271b87ffd349ff0467a9fe1354d461f8d1a54934a1457c37`  
		Last Modified: Sat, 28 May 2022 05:35:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7-debian`

```console
$ docker pull mysql@sha256:7e99b2b8d5bca914ef31059858210f57b009c40375d647f0d4d65ecd01d6b1d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7-debian` - linux; amd64

```console
$ docker pull mysql@sha256:06c614dfc9720ccc0177acf700d0e0794f0efe3a032e78ea5318c30886ce62c1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.5 MB (162456143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a0961b7de03c7b11afd13fec09d0d30992b6e0b4f947a4aba4273723778ed95`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 28 May 2022 01:20:43 GMT
ADD file:0513eda9512e010cb9459591b62e0c9d9319750923df091b64250ad6e98c2878 in / 
# Sat, 28 May 2022 01:20:43 GMT
CMD ["bash"]
# Sat, 28 May 2022 05:33:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 28 May 2022 05:33:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:33:14 GMT
ENV GOSU_VERSION=1.14
# Sat, 28 May 2022 05:33:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 28 May 2022 05:33:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 28 May 2022 05:33:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:33:31 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Sat, 28 May 2022 05:33:57 GMT
ENV MYSQL_MAJOR=5.7
# Sat, 28 May 2022 05:33:57 GMT
ENV MYSQL_VERSION=5.7.38-1debian10
# Sat, 28 May 2022 05:33:58 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Sat, 28 May 2022 05:34:16 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Sat, 28 May 2022 05:34:17 GMT
VOLUME [/var/lib/mysql]
# Sat, 28 May 2022 05:34:17 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Sat, 28 May 2022 05:34:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 28 May 2022 05:34:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 May 2022 05:34:17 GMT
EXPOSE 3306 33060
# Sat, 28 May 2022 05:34:18 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c1ad9731b2c7bf7fddea67f2f3f553515179a375c489e591e2372700fcaca766`  
		Last Modified: Sat, 28 May 2022 01:26:05 GMT  
		Size: 27.1 MB (27140144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f6eb0ee84d0c793cbd8456f03775cc5d88f72c576ec455596dca4ad465df07`  
		Last Modified: Sat, 28 May 2022 05:34:47 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cffcf8691bc5ddfc0c45d837fef9c77c7e264f7a69faf37073d0c4b31fb87156`  
		Last Modified: Sat, 28 May 2022 05:34:48 GMT  
		Size: 4.2 MB (4179298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89a783b5ac8a82c6355c62896648cb37efdc387f41b31b5c1d09418ce1808e81`  
		Last Modified: Sat, 28 May 2022 05:34:45 GMT  
		Size: 1.4 MB (1386680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8393c7be5fa5ff5d50fba15ce47f16cb29d3363d3885632e7892c0854a4d9c`  
		Last Modified: Sat, 28 May 2022 05:34:45 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af768d0b181edf1d8a35699d64f8e71d05d7648a28c37a5ab6fe2e36ffddc5e0`  
		Last Modified: Sat, 28 May 2022 05:34:48 GMT  
		Size: 14.1 MB (14064399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:810d6aaaf54a9c0c9d817fd1615f43aaf0194bcc1fca1574a90e90d8f6d66c6a`  
		Last Modified: Sat, 28 May 2022 05:34:45 GMT  
		Size: 2.5 KB (2547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fe6daf23954caa3d837bbd8317dcde57ad466ad3ca6e0c4b8f0f3c61ee451b`  
		Last Modified: Sat, 28 May 2022 05:35:29 GMT  
		Size: 254.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ccf426818fd53d690090f3e6029160dec25694793d6b77a52e80ff70d7651e2`  
		Last Modified: Sat, 28 May 2022 05:35:45 GMT  
		Size: 115.7 MB (115675662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68b838b06054d3f3b54fea8f73531a1908182330b6571c08f5453c78aa879901`  
		Last Modified: Sat, 28 May 2022 05:35:29 GMT  
		Size: 5.2 KB (5155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b606c4f93dfd881271b87ffd349ff0467a9fe1354d461f8d1a54934a1457c37`  
		Last Modified: Sat, 28 May 2022 05:35:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7-oracle`

```console
$ docker pull mysql@sha256:c67e9e97879305e0c7a4934372f35bdb7d79d4a0914d7304d0ee6836be0127a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:3030fdb1154e62ed44c2e2dbbc7dee2643ee27fb6dd201b06b19a87682498e8b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.9 MB (126873058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f19b3d18c4a01f69bdb995e46233fcdcc66c1ef84bc8d28396e981c020e395ee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 16 Jun 2022 01:20:22 GMT
ADD file:5e615d6d49ec50cba937fa86f5fb7d6a4a7e680b2b4f5b659e879b95304c0417 in / 
# Thu, 16 Jun 2022 01:20:22 GMT
CMD ["/bin/bash"]
# Thu, 16 Jun 2022 01:38:41 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Thu, 16 Jun 2022 01:38:41 GMT
ENV GOSU_VERSION=1.14
# Thu, 16 Jun 2022 01:38:45 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 16 Jun 2022 01:38:55 GMT
RUN set -eux; 	yum install -y 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Thu, 16 Jun 2022 01:38:56 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 16 Jun 2022 01:38:56 GMT
ENV MYSQL_MAJOR=5.7
# Thu, 16 Jun 2022 01:38:56 GMT
ENV MYSQL_VERSION=5.7.38-1.el7
# Thu, 16 Jun 2022 01:38:57 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Thu, 16 Jun 2022 01:39:11 GMT
RUN set -eux; 	yum install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Thu, 16 Jun 2022 01:39:11 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Thu, 16 Jun 2022 01:39:12 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el7
# Thu, 16 Jun 2022 01:39:29 GMT
RUN set -eux; 	yum install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Thu, 16 Jun 2022 01:39:30 GMT
VOLUME [/var/lib/mysql]
# Thu, 16 Jun 2022 01:39:30 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Thu, 16 Jun 2022 01:39:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Jun 2022 01:39:31 GMT
EXPOSE 3306 33060
# Thu, 16 Jun 2022 01:39:31 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:63183c9b4598e16c4cef95f706d50ff6c928de41f391cd513495b27eaa27bf89`  
		Last Modified: Thu, 16 Jun 2022 01:21:08 GMT  
		Size: 48.8 MB (48757931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:921fb508f1d1aecc5558b119c43c60ca99e2803d417ea98b5a55f94975ac5440`  
		Last Modified: Thu, 16 Jun 2022 01:40:10 GMT  
		Size: 1.1 KB (1059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c722a284ecb6bbcc3803b2a9fb3df9e58ebd491e421507db7c73d8f4255cf0f4`  
		Last Modified: Thu, 16 Jun 2022 01:40:09 GMT  
		Size: 930.2 KB (930225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e1ea46ae00991c24638c08d268652beb0ce5b878c83d34964f12345618c8941`  
		Last Modified: Thu, 16 Jun 2022 01:40:11 GMT  
		Size: 3.8 MB (3750823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15dccdcd437d9fe54d225731d32bb52246dc75794a5d49e7f12010322dd06c1`  
		Last Modified: Thu, 16 Jun 2022 01:40:08 GMT  
		Size: 2.7 KB (2659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1050fbf8b84448d369e5743034ffd13580e9313a7e5092eace10220aa687f9b`  
		Last Modified: Thu, 16 Jun 2022 01:40:06 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848d1501cd8fc9f77a4e51a2e6dc077dcc0e468191ffaf2f433a4ffb4f7f63c1`  
		Last Modified: Thu, 16 Jun 2022 01:40:10 GMT  
		Size: 25.5 MB (25466694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98f50b8fa8c9ba100ca41212bdb8cb892fa707fb9395959c967bcc9355b3ddea`  
		Last Modified: Thu, 16 Jun 2022 01:40:06 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8b3d4a8dbcebd64c0cd3dcde292b97e52335441dac4d3c0e8e010d1197578b`  
		Last Modified: Thu, 16 Jun 2022 01:40:15 GMT  
		Size: 48.0 MB (47957859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4284667ffa5966a13950eda5dee3eb23bc10e60d2dee427c9e7c18c789099568`  
		Last Modified: Thu, 16 Jun 2022 01:40:06 GMT  
		Size: 5.2 KB (5159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.38`

```console
$ docker pull mysql@sha256:7e99b2b8d5bca914ef31059858210f57b009c40375d647f0d4d65ecd01d6b1d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.38` - linux; amd64

```console
$ docker pull mysql@sha256:06c614dfc9720ccc0177acf700d0e0794f0efe3a032e78ea5318c30886ce62c1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.5 MB (162456143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a0961b7de03c7b11afd13fec09d0d30992b6e0b4f947a4aba4273723778ed95`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 28 May 2022 01:20:43 GMT
ADD file:0513eda9512e010cb9459591b62e0c9d9319750923df091b64250ad6e98c2878 in / 
# Sat, 28 May 2022 01:20:43 GMT
CMD ["bash"]
# Sat, 28 May 2022 05:33:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 28 May 2022 05:33:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:33:14 GMT
ENV GOSU_VERSION=1.14
# Sat, 28 May 2022 05:33:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 28 May 2022 05:33:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 28 May 2022 05:33:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:33:31 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Sat, 28 May 2022 05:33:57 GMT
ENV MYSQL_MAJOR=5.7
# Sat, 28 May 2022 05:33:57 GMT
ENV MYSQL_VERSION=5.7.38-1debian10
# Sat, 28 May 2022 05:33:58 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Sat, 28 May 2022 05:34:16 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Sat, 28 May 2022 05:34:17 GMT
VOLUME [/var/lib/mysql]
# Sat, 28 May 2022 05:34:17 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Sat, 28 May 2022 05:34:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 28 May 2022 05:34:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 May 2022 05:34:17 GMT
EXPOSE 3306 33060
# Sat, 28 May 2022 05:34:18 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c1ad9731b2c7bf7fddea67f2f3f553515179a375c489e591e2372700fcaca766`  
		Last Modified: Sat, 28 May 2022 01:26:05 GMT  
		Size: 27.1 MB (27140144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f6eb0ee84d0c793cbd8456f03775cc5d88f72c576ec455596dca4ad465df07`  
		Last Modified: Sat, 28 May 2022 05:34:47 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cffcf8691bc5ddfc0c45d837fef9c77c7e264f7a69faf37073d0c4b31fb87156`  
		Last Modified: Sat, 28 May 2022 05:34:48 GMT  
		Size: 4.2 MB (4179298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89a783b5ac8a82c6355c62896648cb37efdc387f41b31b5c1d09418ce1808e81`  
		Last Modified: Sat, 28 May 2022 05:34:45 GMT  
		Size: 1.4 MB (1386680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8393c7be5fa5ff5d50fba15ce47f16cb29d3363d3885632e7892c0854a4d9c`  
		Last Modified: Sat, 28 May 2022 05:34:45 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af768d0b181edf1d8a35699d64f8e71d05d7648a28c37a5ab6fe2e36ffddc5e0`  
		Last Modified: Sat, 28 May 2022 05:34:48 GMT  
		Size: 14.1 MB (14064399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:810d6aaaf54a9c0c9d817fd1615f43aaf0194bcc1fca1574a90e90d8f6d66c6a`  
		Last Modified: Sat, 28 May 2022 05:34:45 GMT  
		Size: 2.5 KB (2547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fe6daf23954caa3d837bbd8317dcde57ad466ad3ca6e0c4b8f0f3c61ee451b`  
		Last Modified: Sat, 28 May 2022 05:35:29 GMT  
		Size: 254.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ccf426818fd53d690090f3e6029160dec25694793d6b77a52e80ff70d7651e2`  
		Last Modified: Sat, 28 May 2022 05:35:45 GMT  
		Size: 115.7 MB (115675662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68b838b06054d3f3b54fea8f73531a1908182330b6571c08f5453c78aa879901`  
		Last Modified: Sat, 28 May 2022 05:35:29 GMT  
		Size: 5.2 KB (5155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b606c4f93dfd881271b87ffd349ff0467a9fe1354d461f8d1a54934a1457c37`  
		Last Modified: Sat, 28 May 2022 05:35:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.38-debian`

```console
$ docker pull mysql@sha256:7e99b2b8d5bca914ef31059858210f57b009c40375d647f0d4d65ecd01d6b1d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.38-debian` - linux; amd64

```console
$ docker pull mysql@sha256:06c614dfc9720ccc0177acf700d0e0794f0efe3a032e78ea5318c30886ce62c1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.5 MB (162456143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a0961b7de03c7b11afd13fec09d0d30992b6e0b4f947a4aba4273723778ed95`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 28 May 2022 01:20:43 GMT
ADD file:0513eda9512e010cb9459591b62e0c9d9319750923df091b64250ad6e98c2878 in / 
# Sat, 28 May 2022 01:20:43 GMT
CMD ["bash"]
# Sat, 28 May 2022 05:33:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 28 May 2022 05:33:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:33:14 GMT
ENV GOSU_VERSION=1.14
# Sat, 28 May 2022 05:33:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 28 May 2022 05:33:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 28 May 2022 05:33:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:33:31 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Sat, 28 May 2022 05:33:57 GMT
ENV MYSQL_MAJOR=5.7
# Sat, 28 May 2022 05:33:57 GMT
ENV MYSQL_VERSION=5.7.38-1debian10
# Sat, 28 May 2022 05:33:58 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Sat, 28 May 2022 05:34:16 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Sat, 28 May 2022 05:34:17 GMT
VOLUME [/var/lib/mysql]
# Sat, 28 May 2022 05:34:17 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Sat, 28 May 2022 05:34:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 28 May 2022 05:34:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 May 2022 05:34:17 GMT
EXPOSE 3306 33060
# Sat, 28 May 2022 05:34:18 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c1ad9731b2c7bf7fddea67f2f3f553515179a375c489e591e2372700fcaca766`  
		Last Modified: Sat, 28 May 2022 01:26:05 GMT  
		Size: 27.1 MB (27140144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f6eb0ee84d0c793cbd8456f03775cc5d88f72c576ec455596dca4ad465df07`  
		Last Modified: Sat, 28 May 2022 05:34:47 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cffcf8691bc5ddfc0c45d837fef9c77c7e264f7a69faf37073d0c4b31fb87156`  
		Last Modified: Sat, 28 May 2022 05:34:48 GMT  
		Size: 4.2 MB (4179298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89a783b5ac8a82c6355c62896648cb37efdc387f41b31b5c1d09418ce1808e81`  
		Last Modified: Sat, 28 May 2022 05:34:45 GMT  
		Size: 1.4 MB (1386680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8393c7be5fa5ff5d50fba15ce47f16cb29d3363d3885632e7892c0854a4d9c`  
		Last Modified: Sat, 28 May 2022 05:34:45 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af768d0b181edf1d8a35699d64f8e71d05d7648a28c37a5ab6fe2e36ffddc5e0`  
		Last Modified: Sat, 28 May 2022 05:34:48 GMT  
		Size: 14.1 MB (14064399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:810d6aaaf54a9c0c9d817fd1615f43aaf0194bcc1fca1574a90e90d8f6d66c6a`  
		Last Modified: Sat, 28 May 2022 05:34:45 GMT  
		Size: 2.5 KB (2547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fe6daf23954caa3d837bbd8317dcde57ad466ad3ca6e0c4b8f0f3c61ee451b`  
		Last Modified: Sat, 28 May 2022 05:35:29 GMT  
		Size: 254.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ccf426818fd53d690090f3e6029160dec25694793d6b77a52e80ff70d7651e2`  
		Last Modified: Sat, 28 May 2022 05:35:45 GMT  
		Size: 115.7 MB (115675662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68b838b06054d3f3b54fea8f73531a1908182330b6571c08f5453c78aa879901`  
		Last Modified: Sat, 28 May 2022 05:35:29 GMT  
		Size: 5.2 KB (5155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b606c4f93dfd881271b87ffd349ff0467a9fe1354d461f8d1a54934a1457c37`  
		Last Modified: Sat, 28 May 2022 05:35:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.38-oracle`

```console
$ docker pull mysql@sha256:c67e9e97879305e0c7a4934372f35bdb7d79d4a0914d7304d0ee6836be0127a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.38-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:3030fdb1154e62ed44c2e2dbbc7dee2643ee27fb6dd201b06b19a87682498e8b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.9 MB (126873058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f19b3d18c4a01f69bdb995e46233fcdcc66c1ef84bc8d28396e981c020e395ee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 16 Jun 2022 01:20:22 GMT
ADD file:5e615d6d49ec50cba937fa86f5fb7d6a4a7e680b2b4f5b659e879b95304c0417 in / 
# Thu, 16 Jun 2022 01:20:22 GMT
CMD ["/bin/bash"]
# Thu, 16 Jun 2022 01:38:41 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Thu, 16 Jun 2022 01:38:41 GMT
ENV GOSU_VERSION=1.14
# Thu, 16 Jun 2022 01:38:45 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 16 Jun 2022 01:38:55 GMT
RUN set -eux; 	yum install -y 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Thu, 16 Jun 2022 01:38:56 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 16 Jun 2022 01:38:56 GMT
ENV MYSQL_MAJOR=5.7
# Thu, 16 Jun 2022 01:38:56 GMT
ENV MYSQL_VERSION=5.7.38-1.el7
# Thu, 16 Jun 2022 01:38:57 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Thu, 16 Jun 2022 01:39:11 GMT
RUN set -eux; 	yum install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Thu, 16 Jun 2022 01:39:11 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Thu, 16 Jun 2022 01:39:12 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el7
# Thu, 16 Jun 2022 01:39:29 GMT
RUN set -eux; 	yum install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Thu, 16 Jun 2022 01:39:30 GMT
VOLUME [/var/lib/mysql]
# Thu, 16 Jun 2022 01:39:30 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Thu, 16 Jun 2022 01:39:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Jun 2022 01:39:31 GMT
EXPOSE 3306 33060
# Thu, 16 Jun 2022 01:39:31 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:63183c9b4598e16c4cef95f706d50ff6c928de41f391cd513495b27eaa27bf89`  
		Last Modified: Thu, 16 Jun 2022 01:21:08 GMT  
		Size: 48.8 MB (48757931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:921fb508f1d1aecc5558b119c43c60ca99e2803d417ea98b5a55f94975ac5440`  
		Last Modified: Thu, 16 Jun 2022 01:40:10 GMT  
		Size: 1.1 KB (1059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c722a284ecb6bbcc3803b2a9fb3df9e58ebd491e421507db7c73d8f4255cf0f4`  
		Last Modified: Thu, 16 Jun 2022 01:40:09 GMT  
		Size: 930.2 KB (930225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e1ea46ae00991c24638c08d268652beb0ce5b878c83d34964f12345618c8941`  
		Last Modified: Thu, 16 Jun 2022 01:40:11 GMT  
		Size: 3.8 MB (3750823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15dccdcd437d9fe54d225731d32bb52246dc75794a5d49e7f12010322dd06c1`  
		Last Modified: Thu, 16 Jun 2022 01:40:08 GMT  
		Size: 2.7 KB (2659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1050fbf8b84448d369e5743034ffd13580e9313a7e5092eace10220aa687f9b`  
		Last Modified: Thu, 16 Jun 2022 01:40:06 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848d1501cd8fc9f77a4e51a2e6dc077dcc0e468191ffaf2f433a4ffb4f7f63c1`  
		Last Modified: Thu, 16 Jun 2022 01:40:10 GMT  
		Size: 25.5 MB (25466694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98f50b8fa8c9ba100ca41212bdb8cb892fa707fb9395959c967bcc9355b3ddea`  
		Last Modified: Thu, 16 Jun 2022 01:40:06 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8b3d4a8dbcebd64c0cd3dcde292b97e52335441dac4d3c0e8e010d1197578b`  
		Last Modified: Thu, 16 Jun 2022 01:40:15 GMT  
		Size: 48.0 MB (47957859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4284667ffa5966a13950eda5dee3eb23bc10e60d2dee427c9e7c18c789099568`  
		Last Modified: Thu, 16 Jun 2022 01:40:06 GMT  
		Size: 5.2 KB (5159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8`

```console
$ docker pull mysql@sha256:548da4c67fd8a71908f17c308b8ddb098acf5191d3d7694e56801c6a8b2072cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8` - linux; amd64

```console
$ docker pull mysql@sha256:0c0beeac7ca1937d60f54e1fb0c4a5c0b0ffee2aae37488fbc9f5ea301425551
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.9 MB (155884977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65b636d5542b73254ce90cc4b895597dc1adc2c661ca553c38eda159979dded1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 28 May 2022 01:20:43 GMT
ADD file:0513eda9512e010cb9459591b62e0c9d9319750923df091b64250ad6e98c2878 in / 
# Sat, 28 May 2022 01:20:43 GMT
CMD ["bash"]
# Sat, 28 May 2022 05:33:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 28 May 2022 05:33:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:33:14 GMT
ENV GOSU_VERSION=1.14
# Sat, 28 May 2022 05:33:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 28 May 2022 05:33:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 28 May 2022 05:33:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:33:31 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Sat, 28 May 2022 05:33:31 GMT
ENV MYSQL_MAJOR=8.0
# Sat, 28 May 2022 05:33:32 GMT
ENV MYSQL_VERSION=8.0.29-1debian10
# Sat, 28 May 2022 05:33:32 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Sat, 28 May 2022 05:33:46 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Sat, 28 May 2022 05:33:47 GMT
VOLUME [/var/lib/mysql]
# Sat, 28 May 2022 05:33:47 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Sat, 28 May 2022 05:33:47 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Sat, 28 May 2022 05:33:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 28 May 2022 05:33:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 May 2022 05:33:48 GMT
EXPOSE 3306 33060
# Sat, 28 May 2022 05:33:48 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c1ad9731b2c7bf7fddea67f2f3f553515179a375c489e591e2372700fcaca766`  
		Last Modified: Sat, 28 May 2022 01:26:05 GMT  
		Size: 27.1 MB (27140144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f6eb0ee84d0c793cbd8456f03775cc5d88f72c576ec455596dca4ad465df07`  
		Last Modified: Sat, 28 May 2022 05:34:47 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cffcf8691bc5ddfc0c45d837fef9c77c7e264f7a69faf37073d0c4b31fb87156`  
		Last Modified: Sat, 28 May 2022 05:34:48 GMT  
		Size: 4.2 MB (4179298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89a783b5ac8a82c6355c62896648cb37efdc387f41b31b5c1d09418ce1808e81`  
		Last Modified: Sat, 28 May 2022 05:34:45 GMT  
		Size: 1.4 MB (1386680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8393c7be5fa5ff5d50fba15ce47f16cb29d3363d3885632e7892c0854a4d9c`  
		Last Modified: Sat, 28 May 2022 05:34:45 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af768d0b181edf1d8a35699d64f8e71d05d7648a28c37a5ab6fe2e36ffddc5e0`  
		Last Modified: Sat, 28 May 2022 05:34:48 GMT  
		Size: 14.1 MB (14064399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:810d6aaaf54a9c0c9d817fd1615f43aaf0194bcc1fca1574a90e90d8f6d66c6a`  
		Last Modified: Sat, 28 May 2022 05:34:45 GMT  
		Size: 2.5 KB (2547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e014a8ae4c97230ff31778e48cc8801fe3d3b141b8e0a878270d1e2ddc4b4f3`  
		Last Modified: Sat, 28 May 2022 05:34:43 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a821425a33418d8b2e6373a86d9bdca37a6a4d7315ca23302665c2556269fd64`  
		Last Modified: Sat, 28 May 2022 05:35:00 GMT  
		Size: 109.1 MB (109103661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a10c2652132a5609dcf19779c0bebde64ef5f5d9e7d8a50f3127c274d56c894`  
		Last Modified: Sat, 28 May 2022 05:34:43 GMT  
		Size: 842.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4419638feac46fa0870175acf37fdb6aea243ba43de9dea79a31fc9afbff395b`  
		Last Modified: Sat, 28 May 2022 05:34:43 GMT  
		Size: 5.2 KB (5152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:681aeed97dfe0d4bc23a8411287a322f495b790026a8b476b956f90355c9aae0`  
		Last Modified: Sat, 28 May 2022 05:34:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8-debian`

```console
$ docker pull mysql@sha256:548da4c67fd8a71908f17c308b8ddb098acf5191d3d7694e56801c6a8b2072cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8-debian` - linux; amd64

```console
$ docker pull mysql@sha256:0c0beeac7ca1937d60f54e1fb0c4a5c0b0ffee2aae37488fbc9f5ea301425551
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.9 MB (155884977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65b636d5542b73254ce90cc4b895597dc1adc2c661ca553c38eda159979dded1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 28 May 2022 01:20:43 GMT
ADD file:0513eda9512e010cb9459591b62e0c9d9319750923df091b64250ad6e98c2878 in / 
# Sat, 28 May 2022 01:20:43 GMT
CMD ["bash"]
# Sat, 28 May 2022 05:33:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 28 May 2022 05:33:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:33:14 GMT
ENV GOSU_VERSION=1.14
# Sat, 28 May 2022 05:33:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 28 May 2022 05:33:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 28 May 2022 05:33:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:33:31 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Sat, 28 May 2022 05:33:31 GMT
ENV MYSQL_MAJOR=8.0
# Sat, 28 May 2022 05:33:32 GMT
ENV MYSQL_VERSION=8.0.29-1debian10
# Sat, 28 May 2022 05:33:32 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Sat, 28 May 2022 05:33:46 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Sat, 28 May 2022 05:33:47 GMT
VOLUME [/var/lib/mysql]
# Sat, 28 May 2022 05:33:47 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Sat, 28 May 2022 05:33:47 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Sat, 28 May 2022 05:33:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 28 May 2022 05:33:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 May 2022 05:33:48 GMT
EXPOSE 3306 33060
# Sat, 28 May 2022 05:33:48 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c1ad9731b2c7bf7fddea67f2f3f553515179a375c489e591e2372700fcaca766`  
		Last Modified: Sat, 28 May 2022 01:26:05 GMT  
		Size: 27.1 MB (27140144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f6eb0ee84d0c793cbd8456f03775cc5d88f72c576ec455596dca4ad465df07`  
		Last Modified: Sat, 28 May 2022 05:34:47 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cffcf8691bc5ddfc0c45d837fef9c77c7e264f7a69faf37073d0c4b31fb87156`  
		Last Modified: Sat, 28 May 2022 05:34:48 GMT  
		Size: 4.2 MB (4179298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89a783b5ac8a82c6355c62896648cb37efdc387f41b31b5c1d09418ce1808e81`  
		Last Modified: Sat, 28 May 2022 05:34:45 GMT  
		Size: 1.4 MB (1386680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8393c7be5fa5ff5d50fba15ce47f16cb29d3363d3885632e7892c0854a4d9c`  
		Last Modified: Sat, 28 May 2022 05:34:45 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af768d0b181edf1d8a35699d64f8e71d05d7648a28c37a5ab6fe2e36ffddc5e0`  
		Last Modified: Sat, 28 May 2022 05:34:48 GMT  
		Size: 14.1 MB (14064399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:810d6aaaf54a9c0c9d817fd1615f43aaf0194bcc1fca1574a90e90d8f6d66c6a`  
		Last Modified: Sat, 28 May 2022 05:34:45 GMT  
		Size: 2.5 KB (2547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e014a8ae4c97230ff31778e48cc8801fe3d3b141b8e0a878270d1e2ddc4b4f3`  
		Last Modified: Sat, 28 May 2022 05:34:43 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a821425a33418d8b2e6373a86d9bdca37a6a4d7315ca23302665c2556269fd64`  
		Last Modified: Sat, 28 May 2022 05:35:00 GMT  
		Size: 109.1 MB (109103661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a10c2652132a5609dcf19779c0bebde64ef5f5d9e7d8a50f3127c274d56c894`  
		Last Modified: Sat, 28 May 2022 05:34:43 GMT  
		Size: 842.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4419638feac46fa0870175acf37fdb6aea243ba43de9dea79a31fc9afbff395b`  
		Last Modified: Sat, 28 May 2022 05:34:43 GMT  
		Size: 5.2 KB (5152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:681aeed97dfe0d4bc23a8411287a322f495b790026a8b476b956f90355c9aae0`  
		Last Modified: Sat, 28 May 2022 05:34:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8-oracle`

```console
$ docker pull mysql@sha256:da035e352c785da143a1c02408b1895f95a5ef1c8aafa6555a7c6a386d49026c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:940fdfa3dc408fb792a8cceb21cafda4b7cd56ce4fbc32833766bdd2a57d6a4f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.6 MB (131636256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebcfb2bcbf716a71cdb2dd51277575869547854e0c57519c03cd5d5cec58a9a0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 14 Jun 2022 18:23:26 GMT
ADD file:837f6c6e7e20067b92edb72e78a8399e6cbbd72dab23db7b5b5a301c58d2a0de in / 
# Tue, 14 Jun 2022 18:23:26 GMT
CMD ["/bin/bash"]
# Tue, 14 Jun 2022 18:39:39 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Tue, 14 Jun 2022 18:39:39 GMT
ENV GOSU_VERSION=1.14
# Tue, 14 Jun 2022 18:39:43 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 14 Jun 2022 18:40:04 GMT
RUN set -eux; 	microdnf install -y 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Tue, 14 Jun 2022 18:40:05 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Tue, 14 Jun 2022 18:40:06 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 14 Jun 2022 18:40:06 GMT
ENV MYSQL_VERSION=8.0.29-1.el8
# Tue, 14 Jun 2022 18:40:06 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 14 Jun 2022 18:40:34 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Tue, 14 Jun 2022 18:40:35 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 14 Jun 2022 18:40:35 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el8
# Tue, 14 Jun 2022 18:41:10 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 14 Jun 2022 18:41:10 GMT
VOLUME [/var/lib/mysql]
# Tue, 14 Jun 2022 18:41:10 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 14 Jun 2022 18:41:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Jun 2022 18:41:11 GMT
EXPOSE 3306 33060
# Tue, 14 Jun 2022 18:41:11 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5f160c0f6cac587a73883b48a8857f5cce0930112792cef25c62510e256e93dc`  
		Last Modified: Tue, 14 Jun 2022 18:24:18 GMT  
		Size: 39.2 MB (39219730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d86c3d841d1984f858257755bdf734554725af4f926f3b1d1b22f119cce8bda9`  
		Last Modified: Tue, 14 Jun 2022 18:41:49 GMT  
		Size: 1.1 KB (1079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f026b3ec1ed102cfe531d812e2063669bad08ac3a0ac68a31e44083d9b9a5f5d`  
		Last Modified: Tue, 14 Jun 2022 18:41:47 GMT  
		Size: 928.8 KB (928831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80b2ddd662a38dbb423dbaa2be04afd41904253b436138b52f2a73aa46a5547`  
		Last Modified: Tue, 14 Jun 2022 18:41:48 GMT  
		Size: 4.5 MB (4535169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a7724a6d28d1e789da86c89f0010caa7de0e4747dfcd360fa981a194850951f`  
		Last Modified: Tue, 14 Jun 2022 18:41:47 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8122570b85fec5c1d3bc0c08a48be2657da195b764c9a13b1a791a086c007368`  
		Last Modified: Tue, 14 Jun 2022 18:41:45 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea018df6cdc3d2aa821feb43a3035926c0c296b3c363e64ab0fa95f144f2e7b`  
		Last Modified: Tue, 14 Jun 2022 18:41:52 GMT  
		Size: 47.2 MB (47244178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8066c16abd2efdd49dd1fe3fab6fec9d250b699d9c0227f69c779c8da2c2acd6`  
		Last Modified: Tue, 14 Jun 2022 18:41:44 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd480e7da7ced7cfb1fb54d07fc5eb08057151be162150bd053f4eb89d9ba85f`  
		Last Modified: Tue, 14 Jun 2022 18:41:52 GMT  
		Size: 39.7 MB (39698832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b680e02f092e5330cf0200abf3ba02bddc3d440d02ebb11ec6ed8bf2ba3155`  
		Last Modified: Tue, 14 Jun 2022 18:41:45 GMT  
		Size: 5.2 KB (5158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:72ada8284e4c164a799b2a97058fdbf3a12883704b0505b15c61c136cd67e4d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.6 MB (138588260 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55ca64bef8c56fe87faa7cc81e738b003c0d59448a15740d822fb0666bf26fd0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 14 Jun 2022 18:41:36 GMT
ADD file:4a6ee90ad73353bfb87b2f121e06bddaed6104536e485baa83fadbe7facc774c in / 
# Tue, 14 Jun 2022 18:41:37 GMT
CMD ["/bin/bash"]
# Tue, 14 Jun 2022 19:17:17 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Tue, 14 Jun 2022 19:17:17 GMT
ENV GOSU_VERSION=1.14
# Tue, 14 Jun 2022 19:17:21 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 14 Jun 2022 19:17:44 GMT
RUN set -eux; 	microdnf install -y 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Tue, 14 Jun 2022 19:17:45 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Tue, 14 Jun 2022 19:17:46 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 14 Jun 2022 19:17:47 GMT
ENV MYSQL_VERSION=8.0.29-1.el8
# Tue, 14 Jun 2022 19:17:48 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 14 Jun 2022 19:18:15 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Tue, 14 Jun 2022 19:18:16 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 14 Jun 2022 19:18:17 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el8
# Tue, 14 Jun 2022 19:18:47 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 14 Jun 2022 19:18:48 GMT
VOLUME [/var/lib/mysql]
# Tue, 14 Jun 2022 19:18:49 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 14 Jun 2022 19:18:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Jun 2022 19:18:50 GMT
EXPOSE 3306 33060
# Tue, 14 Jun 2022 19:18:51 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2bbc1bf883bd601c0da5735b538963308bcc17f90d36525ecc93456ffad79064`  
		Last Modified: Tue, 14 Jun 2022 18:42:39 GMT  
		Size: 38.0 MB (38012371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8428f9d18fc319262a774f75a5849d4819b5b44cbf07fbb5e3c262e5cf30c22d`  
		Last Modified: Tue, 14 Jun 2022 19:19:14 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69cba94044003680a99c76f187ea817c71b843de38bb7f28faf8ca6508efd45e`  
		Last Modified: Tue, 14 Jun 2022 19:19:12 GMT  
		Size: 857.2 KB (857152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eac2db801a3647077263a37064e93b70b92541bf4ca7ff49164ebd26b5909df1`  
		Last Modified: Tue, 14 Jun 2022 19:19:13 GMT  
		Size: 4.4 MB (4361254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8bdbcb57725745140238f0807a9980dfccc7901a59788bdd8e8673b9dfc9e4`  
		Last Modified: Tue, 14 Jun 2022 19:19:12 GMT  
		Size: 2.6 KB (2603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25a4fad67d68ae03439e555e68701ab4ee3ea16f2e2f90c1b202ba894b9c4d37`  
		Last Modified: Tue, 14 Jun 2022 19:19:09 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab136e2e0f6c6851a5804d1310ceaad035c500537f8208705649f4b35402829`  
		Last Modified: Tue, 14 Jun 2022 19:19:17 GMT  
		Size: 53.3 MB (53307019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee6421b3efe2970642254e83d78cea1cb6f54a77db5a9b1c4c5c6be95df2532`  
		Last Modified: Tue, 14 Jun 2022 19:19:09 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1620f6ea4d62464f9ce80ceafbcf9b7fea1f93be1355e6eadd5fee9eaf35bf6f`  
		Last Modified: Tue, 14 Jun 2022 19:19:17 GMT  
		Size: 42.0 MB (42041038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b288f89c74171bb779509de10b16a7756d2694417c2d960dc3d2b3a534245992`  
		Last Modified: Tue, 14 Jun 2022 19:19:09 GMT  
		Size: 5.2 KB (5160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0`

```console
$ docker pull mysql@sha256:548da4c67fd8a71908f17c308b8ddb098acf5191d3d7694e56801c6a8b2072cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0` - linux; amd64

```console
$ docker pull mysql@sha256:0c0beeac7ca1937d60f54e1fb0c4a5c0b0ffee2aae37488fbc9f5ea301425551
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.9 MB (155884977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65b636d5542b73254ce90cc4b895597dc1adc2c661ca553c38eda159979dded1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 28 May 2022 01:20:43 GMT
ADD file:0513eda9512e010cb9459591b62e0c9d9319750923df091b64250ad6e98c2878 in / 
# Sat, 28 May 2022 01:20:43 GMT
CMD ["bash"]
# Sat, 28 May 2022 05:33:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 28 May 2022 05:33:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:33:14 GMT
ENV GOSU_VERSION=1.14
# Sat, 28 May 2022 05:33:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 28 May 2022 05:33:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 28 May 2022 05:33:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:33:31 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Sat, 28 May 2022 05:33:31 GMT
ENV MYSQL_MAJOR=8.0
# Sat, 28 May 2022 05:33:32 GMT
ENV MYSQL_VERSION=8.0.29-1debian10
# Sat, 28 May 2022 05:33:32 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Sat, 28 May 2022 05:33:46 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Sat, 28 May 2022 05:33:47 GMT
VOLUME [/var/lib/mysql]
# Sat, 28 May 2022 05:33:47 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Sat, 28 May 2022 05:33:47 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Sat, 28 May 2022 05:33:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 28 May 2022 05:33:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 May 2022 05:33:48 GMT
EXPOSE 3306 33060
# Sat, 28 May 2022 05:33:48 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c1ad9731b2c7bf7fddea67f2f3f553515179a375c489e591e2372700fcaca766`  
		Last Modified: Sat, 28 May 2022 01:26:05 GMT  
		Size: 27.1 MB (27140144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f6eb0ee84d0c793cbd8456f03775cc5d88f72c576ec455596dca4ad465df07`  
		Last Modified: Sat, 28 May 2022 05:34:47 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cffcf8691bc5ddfc0c45d837fef9c77c7e264f7a69faf37073d0c4b31fb87156`  
		Last Modified: Sat, 28 May 2022 05:34:48 GMT  
		Size: 4.2 MB (4179298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89a783b5ac8a82c6355c62896648cb37efdc387f41b31b5c1d09418ce1808e81`  
		Last Modified: Sat, 28 May 2022 05:34:45 GMT  
		Size: 1.4 MB (1386680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8393c7be5fa5ff5d50fba15ce47f16cb29d3363d3885632e7892c0854a4d9c`  
		Last Modified: Sat, 28 May 2022 05:34:45 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af768d0b181edf1d8a35699d64f8e71d05d7648a28c37a5ab6fe2e36ffddc5e0`  
		Last Modified: Sat, 28 May 2022 05:34:48 GMT  
		Size: 14.1 MB (14064399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:810d6aaaf54a9c0c9d817fd1615f43aaf0194bcc1fca1574a90e90d8f6d66c6a`  
		Last Modified: Sat, 28 May 2022 05:34:45 GMT  
		Size: 2.5 KB (2547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e014a8ae4c97230ff31778e48cc8801fe3d3b141b8e0a878270d1e2ddc4b4f3`  
		Last Modified: Sat, 28 May 2022 05:34:43 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a821425a33418d8b2e6373a86d9bdca37a6a4d7315ca23302665c2556269fd64`  
		Last Modified: Sat, 28 May 2022 05:35:00 GMT  
		Size: 109.1 MB (109103661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a10c2652132a5609dcf19779c0bebde64ef5f5d9e7d8a50f3127c274d56c894`  
		Last Modified: Sat, 28 May 2022 05:34:43 GMT  
		Size: 842.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4419638feac46fa0870175acf37fdb6aea243ba43de9dea79a31fc9afbff395b`  
		Last Modified: Sat, 28 May 2022 05:34:43 GMT  
		Size: 5.2 KB (5152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:681aeed97dfe0d4bc23a8411287a322f495b790026a8b476b956f90355c9aae0`  
		Last Modified: Sat, 28 May 2022 05:34:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0-debian`

```console
$ docker pull mysql@sha256:548da4c67fd8a71908f17c308b8ddb098acf5191d3d7694e56801c6a8b2072cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0-debian` - linux; amd64

```console
$ docker pull mysql@sha256:0c0beeac7ca1937d60f54e1fb0c4a5c0b0ffee2aae37488fbc9f5ea301425551
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.9 MB (155884977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65b636d5542b73254ce90cc4b895597dc1adc2c661ca553c38eda159979dded1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 28 May 2022 01:20:43 GMT
ADD file:0513eda9512e010cb9459591b62e0c9d9319750923df091b64250ad6e98c2878 in / 
# Sat, 28 May 2022 01:20:43 GMT
CMD ["bash"]
# Sat, 28 May 2022 05:33:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 28 May 2022 05:33:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:33:14 GMT
ENV GOSU_VERSION=1.14
# Sat, 28 May 2022 05:33:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 28 May 2022 05:33:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 28 May 2022 05:33:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:33:31 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Sat, 28 May 2022 05:33:31 GMT
ENV MYSQL_MAJOR=8.0
# Sat, 28 May 2022 05:33:32 GMT
ENV MYSQL_VERSION=8.0.29-1debian10
# Sat, 28 May 2022 05:33:32 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Sat, 28 May 2022 05:33:46 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Sat, 28 May 2022 05:33:47 GMT
VOLUME [/var/lib/mysql]
# Sat, 28 May 2022 05:33:47 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Sat, 28 May 2022 05:33:47 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Sat, 28 May 2022 05:33:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 28 May 2022 05:33:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 May 2022 05:33:48 GMT
EXPOSE 3306 33060
# Sat, 28 May 2022 05:33:48 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c1ad9731b2c7bf7fddea67f2f3f553515179a375c489e591e2372700fcaca766`  
		Last Modified: Sat, 28 May 2022 01:26:05 GMT  
		Size: 27.1 MB (27140144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f6eb0ee84d0c793cbd8456f03775cc5d88f72c576ec455596dca4ad465df07`  
		Last Modified: Sat, 28 May 2022 05:34:47 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cffcf8691bc5ddfc0c45d837fef9c77c7e264f7a69faf37073d0c4b31fb87156`  
		Last Modified: Sat, 28 May 2022 05:34:48 GMT  
		Size: 4.2 MB (4179298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89a783b5ac8a82c6355c62896648cb37efdc387f41b31b5c1d09418ce1808e81`  
		Last Modified: Sat, 28 May 2022 05:34:45 GMT  
		Size: 1.4 MB (1386680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8393c7be5fa5ff5d50fba15ce47f16cb29d3363d3885632e7892c0854a4d9c`  
		Last Modified: Sat, 28 May 2022 05:34:45 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af768d0b181edf1d8a35699d64f8e71d05d7648a28c37a5ab6fe2e36ffddc5e0`  
		Last Modified: Sat, 28 May 2022 05:34:48 GMT  
		Size: 14.1 MB (14064399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:810d6aaaf54a9c0c9d817fd1615f43aaf0194bcc1fca1574a90e90d8f6d66c6a`  
		Last Modified: Sat, 28 May 2022 05:34:45 GMT  
		Size: 2.5 KB (2547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e014a8ae4c97230ff31778e48cc8801fe3d3b141b8e0a878270d1e2ddc4b4f3`  
		Last Modified: Sat, 28 May 2022 05:34:43 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a821425a33418d8b2e6373a86d9bdca37a6a4d7315ca23302665c2556269fd64`  
		Last Modified: Sat, 28 May 2022 05:35:00 GMT  
		Size: 109.1 MB (109103661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a10c2652132a5609dcf19779c0bebde64ef5f5d9e7d8a50f3127c274d56c894`  
		Last Modified: Sat, 28 May 2022 05:34:43 GMT  
		Size: 842.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4419638feac46fa0870175acf37fdb6aea243ba43de9dea79a31fc9afbff395b`  
		Last Modified: Sat, 28 May 2022 05:34:43 GMT  
		Size: 5.2 KB (5152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:681aeed97dfe0d4bc23a8411287a322f495b790026a8b476b956f90355c9aae0`  
		Last Modified: Sat, 28 May 2022 05:34:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0-oracle`

```console
$ docker pull mysql@sha256:da035e352c785da143a1c02408b1895f95a5ef1c8aafa6555a7c6a386d49026c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:940fdfa3dc408fb792a8cceb21cafda4b7cd56ce4fbc32833766bdd2a57d6a4f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.6 MB (131636256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebcfb2bcbf716a71cdb2dd51277575869547854e0c57519c03cd5d5cec58a9a0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 14 Jun 2022 18:23:26 GMT
ADD file:837f6c6e7e20067b92edb72e78a8399e6cbbd72dab23db7b5b5a301c58d2a0de in / 
# Tue, 14 Jun 2022 18:23:26 GMT
CMD ["/bin/bash"]
# Tue, 14 Jun 2022 18:39:39 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Tue, 14 Jun 2022 18:39:39 GMT
ENV GOSU_VERSION=1.14
# Tue, 14 Jun 2022 18:39:43 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 14 Jun 2022 18:40:04 GMT
RUN set -eux; 	microdnf install -y 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Tue, 14 Jun 2022 18:40:05 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Tue, 14 Jun 2022 18:40:06 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 14 Jun 2022 18:40:06 GMT
ENV MYSQL_VERSION=8.0.29-1.el8
# Tue, 14 Jun 2022 18:40:06 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 14 Jun 2022 18:40:34 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Tue, 14 Jun 2022 18:40:35 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 14 Jun 2022 18:40:35 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el8
# Tue, 14 Jun 2022 18:41:10 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 14 Jun 2022 18:41:10 GMT
VOLUME [/var/lib/mysql]
# Tue, 14 Jun 2022 18:41:10 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 14 Jun 2022 18:41:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Jun 2022 18:41:11 GMT
EXPOSE 3306 33060
# Tue, 14 Jun 2022 18:41:11 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5f160c0f6cac587a73883b48a8857f5cce0930112792cef25c62510e256e93dc`  
		Last Modified: Tue, 14 Jun 2022 18:24:18 GMT  
		Size: 39.2 MB (39219730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d86c3d841d1984f858257755bdf734554725af4f926f3b1d1b22f119cce8bda9`  
		Last Modified: Tue, 14 Jun 2022 18:41:49 GMT  
		Size: 1.1 KB (1079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f026b3ec1ed102cfe531d812e2063669bad08ac3a0ac68a31e44083d9b9a5f5d`  
		Last Modified: Tue, 14 Jun 2022 18:41:47 GMT  
		Size: 928.8 KB (928831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80b2ddd662a38dbb423dbaa2be04afd41904253b436138b52f2a73aa46a5547`  
		Last Modified: Tue, 14 Jun 2022 18:41:48 GMT  
		Size: 4.5 MB (4535169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a7724a6d28d1e789da86c89f0010caa7de0e4747dfcd360fa981a194850951f`  
		Last Modified: Tue, 14 Jun 2022 18:41:47 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8122570b85fec5c1d3bc0c08a48be2657da195b764c9a13b1a791a086c007368`  
		Last Modified: Tue, 14 Jun 2022 18:41:45 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea018df6cdc3d2aa821feb43a3035926c0c296b3c363e64ab0fa95f144f2e7b`  
		Last Modified: Tue, 14 Jun 2022 18:41:52 GMT  
		Size: 47.2 MB (47244178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8066c16abd2efdd49dd1fe3fab6fec9d250b699d9c0227f69c779c8da2c2acd6`  
		Last Modified: Tue, 14 Jun 2022 18:41:44 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd480e7da7ced7cfb1fb54d07fc5eb08057151be162150bd053f4eb89d9ba85f`  
		Last Modified: Tue, 14 Jun 2022 18:41:52 GMT  
		Size: 39.7 MB (39698832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b680e02f092e5330cf0200abf3ba02bddc3d440d02ebb11ec6ed8bf2ba3155`  
		Last Modified: Tue, 14 Jun 2022 18:41:45 GMT  
		Size: 5.2 KB (5158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:72ada8284e4c164a799b2a97058fdbf3a12883704b0505b15c61c136cd67e4d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.6 MB (138588260 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55ca64bef8c56fe87faa7cc81e738b003c0d59448a15740d822fb0666bf26fd0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 14 Jun 2022 18:41:36 GMT
ADD file:4a6ee90ad73353bfb87b2f121e06bddaed6104536e485baa83fadbe7facc774c in / 
# Tue, 14 Jun 2022 18:41:37 GMT
CMD ["/bin/bash"]
# Tue, 14 Jun 2022 19:17:17 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Tue, 14 Jun 2022 19:17:17 GMT
ENV GOSU_VERSION=1.14
# Tue, 14 Jun 2022 19:17:21 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 14 Jun 2022 19:17:44 GMT
RUN set -eux; 	microdnf install -y 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Tue, 14 Jun 2022 19:17:45 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Tue, 14 Jun 2022 19:17:46 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 14 Jun 2022 19:17:47 GMT
ENV MYSQL_VERSION=8.0.29-1.el8
# Tue, 14 Jun 2022 19:17:48 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 14 Jun 2022 19:18:15 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Tue, 14 Jun 2022 19:18:16 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 14 Jun 2022 19:18:17 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el8
# Tue, 14 Jun 2022 19:18:47 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 14 Jun 2022 19:18:48 GMT
VOLUME [/var/lib/mysql]
# Tue, 14 Jun 2022 19:18:49 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 14 Jun 2022 19:18:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Jun 2022 19:18:50 GMT
EXPOSE 3306 33060
# Tue, 14 Jun 2022 19:18:51 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2bbc1bf883bd601c0da5735b538963308bcc17f90d36525ecc93456ffad79064`  
		Last Modified: Tue, 14 Jun 2022 18:42:39 GMT  
		Size: 38.0 MB (38012371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8428f9d18fc319262a774f75a5849d4819b5b44cbf07fbb5e3c262e5cf30c22d`  
		Last Modified: Tue, 14 Jun 2022 19:19:14 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69cba94044003680a99c76f187ea817c71b843de38bb7f28faf8ca6508efd45e`  
		Last Modified: Tue, 14 Jun 2022 19:19:12 GMT  
		Size: 857.2 KB (857152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eac2db801a3647077263a37064e93b70b92541bf4ca7ff49164ebd26b5909df1`  
		Last Modified: Tue, 14 Jun 2022 19:19:13 GMT  
		Size: 4.4 MB (4361254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8bdbcb57725745140238f0807a9980dfccc7901a59788bdd8e8673b9dfc9e4`  
		Last Modified: Tue, 14 Jun 2022 19:19:12 GMT  
		Size: 2.6 KB (2603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25a4fad67d68ae03439e555e68701ab4ee3ea16f2e2f90c1b202ba894b9c4d37`  
		Last Modified: Tue, 14 Jun 2022 19:19:09 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab136e2e0f6c6851a5804d1310ceaad035c500537f8208705649f4b35402829`  
		Last Modified: Tue, 14 Jun 2022 19:19:17 GMT  
		Size: 53.3 MB (53307019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee6421b3efe2970642254e83d78cea1cb6f54a77db5a9b1c4c5c6be95df2532`  
		Last Modified: Tue, 14 Jun 2022 19:19:09 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1620f6ea4d62464f9ce80ceafbcf9b7fea1f93be1355e6eadd5fee9eaf35bf6f`  
		Last Modified: Tue, 14 Jun 2022 19:19:17 GMT  
		Size: 42.0 MB (42041038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b288f89c74171bb779509de10b16a7756d2694417c2d960dc3d2b3a534245992`  
		Last Modified: Tue, 14 Jun 2022 19:19:09 GMT  
		Size: 5.2 KB (5160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.29`

```console
$ docker pull mysql@sha256:548da4c67fd8a71908f17c308b8ddb098acf5191d3d7694e56801c6a8b2072cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0.29` - linux; amd64

```console
$ docker pull mysql@sha256:0c0beeac7ca1937d60f54e1fb0c4a5c0b0ffee2aae37488fbc9f5ea301425551
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.9 MB (155884977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65b636d5542b73254ce90cc4b895597dc1adc2c661ca553c38eda159979dded1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 28 May 2022 01:20:43 GMT
ADD file:0513eda9512e010cb9459591b62e0c9d9319750923df091b64250ad6e98c2878 in / 
# Sat, 28 May 2022 01:20:43 GMT
CMD ["bash"]
# Sat, 28 May 2022 05:33:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 28 May 2022 05:33:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:33:14 GMT
ENV GOSU_VERSION=1.14
# Sat, 28 May 2022 05:33:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 28 May 2022 05:33:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 28 May 2022 05:33:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:33:31 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Sat, 28 May 2022 05:33:31 GMT
ENV MYSQL_MAJOR=8.0
# Sat, 28 May 2022 05:33:32 GMT
ENV MYSQL_VERSION=8.0.29-1debian10
# Sat, 28 May 2022 05:33:32 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Sat, 28 May 2022 05:33:46 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Sat, 28 May 2022 05:33:47 GMT
VOLUME [/var/lib/mysql]
# Sat, 28 May 2022 05:33:47 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Sat, 28 May 2022 05:33:47 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Sat, 28 May 2022 05:33:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 28 May 2022 05:33:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 May 2022 05:33:48 GMT
EXPOSE 3306 33060
# Sat, 28 May 2022 05:33:48 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c1ad9731b2c7bf7fddea67f2f3f553515179a375c489e591e2372700fcaca766`  
		Last Modified: Sat, 28 May 2022 01:26:05 GMT  
		Size: 27.1 MB (27140144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f6eb0ee84d0c793cbd8456f03775cc5d88f72c576ec455596dca4ad465df07`  
		Last Modified: Sat, 28 May 2022 05:34:47 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cffcf8691bc5ddfc0c45d837fef9c77c7e264f7a69faf37073d0c4b31fb87156`  
		Last Modified: Sat, 28 May 2022 05:34:48 GMT  
		Size: 4.2 MB (4179298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89a783b5ac8a82c6355c62896648cb37efdc387f41b31b5c1d09418ce1808e81`  
		Last Modified: Sat, 28 May 2022 05:34:45 GMT  
		Size: 1.4 MB (1386680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8393c7be5fa5ff5d50fba15ce47f16cb29d3363d3885632e7892c0854a4d9c`  
		Last Modified: Sat, 28 May 2022 05:34:45 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af768d0b181edf1d8a35699d64f8e71d05d7648a28c37a5ab6fe2e36ffddc5e0`  
		Last Modified: Sat, 28 May 2022 05:34:48 GMT  
		Size: 14.1 MB (14064399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:810d6aaaf54a9c0c9d817fd1615f43aaf0194bcc1fca1574a90e90d8f6d66c6a`  
		Last Modified: Sat, 28 May 2022 05:34:45 GMT  
		Size: 2.5 KB (2547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e014a8ae4c97230ff31778e48cc8801fe3d3b141b8e0a878270d1e2ddc4b4f3`  
		Last Modified: Sat, 28 May 2022 05:34:43 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a821425a33418d8b2e6373a86d9bdca37a6a4d7315ca23302665c2556269fd64`  
		Last Modified: Sat, 28 May 2022 05:35:00 GMT  
		Size: 109.1 MB (109103661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a10c2652132a5609dcf19779c0bebde64ef5f5d9e7d8a50f3127c274d56c894`  
		Last Modified: Sat, 28 May 2022 05:34:43 GMT  
		Size: 842.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4419638feac46fa0870175acf37fdb6aea243ba43de9dea79a31fc9afbff395b`  
		Last Modified: Sat, 28 May 2022 05:34:43 GMT  
		Size: 5.2 KB (5152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:681aeed97dfe0d4bc23a8411287a322f495b790026a8b476b956f90355c9aae0`  
		Last Modified: Sat, 28 May 2022 05:34:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.29-debian`

```console
$ docker pull mysql@sha256:548da4c67fd8a71908f17c308b8ddb098acf5191d3d7694e56801c6a8b2072cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0.29-debian` - linux; amd64

```console
$ docker pull mysql@sha256:0c0beeac7ca1937d60f54e1fb0c4a5c0b0ffee2aae37488fbc9f5ea301425551
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.9 MB (155884977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65b636d5542b73254ce90cc4b895597dc1adc2c661ca553c38eda159979dded1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 28 May 2022 01:20:43 GMT
ADD file:0513eda9512e010cb9459591b62e0c9d9319750923df091b64250ad6e98c2878 in / 
# Sat, 28 May 2022 01:20:43 GMT
CMD ["bash"]
# Sat, 28 May 2022 05:33:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 28 May 2022 05:33:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:33:14 GMT
ENV GOSU_VERSION=1.14
# Sat, 28 May 2022 05:33:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 28 May 2022 05:33:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 28 May 2022 05:33:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:33:31 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Sat, 28 May 2022 05:33:31 GMT
ENV MYSQL_MAJOR=8.0
# Sat, 28 May 2022 05:33:32 GMT
ENV MYSQL_VERSION=8.0.29-1debian10
# Sat, 28 May 2022 05:33:32 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Sat, 28 May 2022 05:33:46 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Sat, 28 May 2022 05:33:47 GMT
VOLUME [/var/lib/mysql]
# Sat, 28 May 2022 05:33:47 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Sat, 28 May 2022 05:33:47 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Sat, 28 May 2022 05:33:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 28 May 2022 05:33:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 May 2022 05:33:48 GMT
EXPOSE 3306 33060
# Sat, 28 May 2022 05:33:48 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c1ad9731b2c7bf7fddea67f2f3f553515179a375c489e591e2372700fcaca766`  
		Last Modified: Sat, 28 May 2022 01:26:05 GMT  
		Size: 27.1 MB (27140144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f6eb0ee84d0c793cbd8456f03775cc5d88f72c576ec455596dca4ad465df07`  
		Last Modified: Sat, 28 May 2022 05:34:47 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cffcf8691bc5ddfc0c45d837fef9c77c7e264f7a69faf37073d0c4b31fb87156`  
		Last Modified: Sat, 28 May 2022 05:34:48 GMT  
		Size: 4.2 MB (4179298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89a783b5ac8a82c6355c62896648cb37efdc387f41b31b5c1d09418ce1808e81`  
		Last Modified: Sat, 28 May 2022 05:34:45 GMT  
		Size: 1.4 MB (1386680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8393c7be5fa5ff5d50fba15ce47f16cb29d3363d3885632e7892c0854a4d9c`  
		Last Modified: Sat, 28 May 2022 05:34:45 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af768d0b181edf1d8a35699d64f8e71d05d7648a28c37a5ab6fe2e36ffddc5e0`  
		Last Modified: Sat, 28 May 2022 05:34:48 GMT  
		Size: 14.1 MB (14064399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:810d6aaaf54a9c0c9d817fd1615f43aaf0194bcc1fca1574a90e90d8f6d66c6a`  
		Last Modified: Sat, 28 May 2022 05:34:45 GMT  
		Size: 2.5 KB (2547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e014a8ae4c97230ff31778e48cc8801fe3d3b141b8e0a878270d1e2ddc4b4f3`  
		Last Modified: Sat, 28 May 2022 05:34:43 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a821425a33418d8b2e6373a86d9bdca37a6a4d7315ca23302665c2556269fd64`  
		Last Modified: Sat, 28 May 2022 05:35:00 GMT  
		Size: 109.1 MB (109103661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a10c2652132a5609dcf19779c0bebde64ef5f5d9e7d8a50f3127c274d56c894`  
		Last Modified: Sat, 28 May 2022 05:34:43 GMT  
		Size: 842.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4419638feac46fa0870175acf37fdb6aea243ba43de9dea79a31fc9afbff395b`  
		Last Modified: Sat, 28 May 2022 05:34:43 GMT  
		Size: 5.2 KB (5152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:681aeed97dfe0d4bc23a8411287a322f495b790026a8b476b956f90355c9aae0`  
		Last Modified: Sat, 28 May 2022 05:34:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.29-oracle`

```console
$ docker pull mysql@sha256:da035e352c785da143a1c02408b1895f95a5ef1c8aafa6555a7c6a386d49026c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0.29-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:940fdfa3dc408fb792a8cceb21cafda4b7cd56ce4fbc32833766bdd2a57d6a4f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.6 MB (131636256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebcfb2bcbf716a71cdb2dd51277575869547854e0c57519c03cd5d5cec58a9a0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 14 Jun 2022 18:23:26 GMT
ADD file:837f6c6e7e20067b92edb72e78a8399e6cbbd72dab23db7b5b5a301c58d2a0de in / 
# Tue, 14 Jun 2022 18:23:26 GMT
CMD ["/bin/bash"]
# Tue, 14 Jun 2022 18:39:39 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Tue, 14 Jun 2022 18:39:39 GMT
ENV GOSU_VERSION=1.14
# Tue, 14 Jun 2022 18:39:43 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 14 Jun 2022 18:40:04 GMT
RUN set -eux; 	microdnf install -y 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Tue, 14 Jun 2022 18:40:05 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Tue, 14 Jun 2022 18:40:06 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 14 Jun 2022 18:40:06 GMT
ENV MYSQL_VERSION=8.0.29-1.el8
# Tue, 14 Jun 2022 18:40:06 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 14 Jun 2022 18:40:34 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Tue, 14 Jun 2022 18:40:35 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 14 Jun 2022 18:40:35 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el8
# Tue, 14 Jun 2022 18:41:10 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 14 Jun 2022 18:41:10 GMT
VOLUME [/var/lib/mysql]
# Tue, 14 Jun 2022 18:41:10 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 14 Jun 2022 18:41:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Jun 2022 18:41:11 GMT
EXPOSE 3306 33060
# Tue, 14 Jun 2022 18:41:11 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5f160c0f6cac587a73883b48a8857f5cce0930112792cef25c62510e256e93dc`  
		Last Modified: Tue, 14 Jun 2022 18:24:18 GMT  
		Size: 39.2 MB (39219730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d86c3d841d1984f858257755bdf734554725af4f926f3b1d1b22f119cce8bda9`  
		Last Modified: Tue, 14 Jun 2022 18:41:49 GMT  
		Size: 1.1 KB (1079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f026b3ec1ed102cfe531d812e2063669bad08ac3a0ac68a31e44083d9b9a5f5d`  
		Last Modified: Tue, 14 Jun 2022 18:41:47 GMT  
		Size: 928.8 KB (928831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80b2ddd662a38dbb423dbaa2be04afd41904253b436138b52f2a73aa46a5547`  
		Last Modified: Tue, 14 Jun 2022 18:41:48 GMT  
		Size: 4.5 MB (4535169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a7724a6d28d1e789da86c89f0010caa7de0e4747dfcd360fa981a194850951f`  
		Last Modified: Tue, 14 Jun 2022 18:41:47 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8122570b85fec5c1d3bc0c08a48be2657da195b764c9a13b1a791a086c007368`  
		Last Modified: Tue, 14 Jun 2022 18:41:45 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea018df6cdc3d2aa821feb43a3035926c0c296b3c363e64ab0fa95f144f2e7b`  
		Last Modified: Tue, 14 Jun 2022 18:41:52 GMT  
		Size: 47.2 MB (47244178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8066c16abd2efdd49dd1fe3fab6fec9d250b699d9c0227f69c779c8da2c2acd6`  
		Last Modified: Tue, 14 Jun 2022 18:41:44 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd480e7da7ced7cfb1fb54d07fc5eb08057151be162150bd053f4eb89d9ba85f`  
		Last Modified: Tue, 14 Jun 2022 18:41:52 GMT  
		Size: 39.7 MB (39698832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b680e02f092e5330cf0200abf3ba02bddc3d440d02ebb11ec6ed8bf2ba3155`  
		Last Modified: Tue, 14 Jun 2022 18:41:45 GMT  
		Size: 5.2 KB (5158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0.29-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:72ada8284e4c164a799b2a97058fdbf3a12883704b0505b15c61c136cd67e4d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.6 MB (138588260 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55ca64bef8c56fe87faa7cc81e738b003c0d59448a15740d822fb0666bf26fd0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 14 Jun 2022 18:41:36 GMT
ADD file:4a6ee90ad73353bfb87b2f121e06bddaed6104536e485baa83fadbe7facc774c in / 
# Tue, 14 Jun 2022 18:41:37 GMT
CMD ["/bin/bash"]
# Tue, 14 Jun 2022 19:17:17 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Tue, 14 Jun 2022 19:17:17 GMT
ENV GOSU_VERSION=1.14
# Tue, 14 Jun 2022 19:17:21 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 14 Jun 2022 19:17:44 GMT
RUN set -eux; 	microdnf install -y 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Tue, 14 Jun 2022 19:17:45 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Tue, 14 Jun 2022 19:17:46 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 14 Jun 2022 19:17:47 GMT
ENV MYSQL_VERSION=8.0.29-1.el8
# Tue, 14 Jun 2022 19:17:48 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 14 Jun 2022 19:18:15 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Tue, 14 Jun 2022 19:18:16 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 14 Jun 2022 19:18:17 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el8
# Tue, 14 Jun 2022 19:18:47 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 14 Jun 2022 19:18:48 GMT
VOLUME [/var/lib/mysql]
# Tue, 14 Jun 2022 19:18:49 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 14 Jun 2022 19:18:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Jun 2022 19:18:50 GMT
EXPOSE 3306 33060
# Tue, 14 Jun 2022 19:18:51 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2bbc1bf883bd601c0da5735b538963308bcc17f90d36525ecc93456ffad79064`  
		Last Modified: Tue, 14 Jun 2022 18:42:39 GMT  
		Size: 38.0 MB (38012371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8428f9d18fc319262a774f75a5849d4819b5b44cbf07fbb5e3c262e5cf30c22d`  
		Last Modified: Tue, 14 Jun 2022 19:19:14 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69cba94044003680a99c76f187ea817c71b843de38bb7f28faf8ca6508efd45e`  
		Last Modified: Tue, 14 Jun 2022 19:19:12 GMT  
		Size: 857.2 KB (857152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eac2db801a3647077263a37064e93b70b92541bf4ca7ff49164ebd26b5909df1`  
		Last Modified: Tue, 14 Jun 2022 19:19:13 GMT  
		Size: 4.4 MB (4361254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8bdbcb57725745140238f0807a9980dfccc7901a59788bdd8e8673b9dfc9e4`  
		Last Modified: Tue, 14 Jun 2022 19:19:12 GMT  
		Size: 2.6 KB (2603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25a4fad67d68ae03439e555e68701ab4ee3ea16f2e2f90c1b202ba894b9c4d37`  
		Last Modified: Tue, 14 Jun 2022 19:19:09 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab136e2e0f6c6851a5804d1310ceaad035c500537f8208705649f4b35402829`  
		Last Modified: Tue, 14 Jun 2022 19:19:17 GMT  
		Size: 53.3 MB (53307019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee6421b3efe2970642254e83d78cea1cb6f54a77db5a9b1c4c5c6be95df2532`  
		Last Modified: Tue, 14 Jun 2022 19:19:09 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1620f6ea4d62464f9ce80ceafbcf9b7fea1f93be1355e6eadd5fee9eaf35bf6f`  
		Last Modified: Tue, 14 Jun 2022 19:19:17 GMT  
		Size: 42.0 MB (42041038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b288f89c74171bb779509de10b16a7756d2694417c2d960dc3d2b3a534245992`  
		Last Modified: Tue, 14 Jun 2022 19:19:09 GMT  
		Size: 5.2 KB (5160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:debian`

```console
$ docker pull mysql@sha256:548da4c67fd8a71908f17c308b8ddb098acf5191d3d7694e56801c6a8b2072cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:debian` - linux; amd64

```console
$ docker pull mysql@sha256:0c0beeac7ca1937d60f54e1fb0c4a5c0b0ffee2aae37488fbc9f5ea301425551
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.9 MB (155884977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65b636d5542b73254ce90cc4b895597dc1adc2c661ca553c38eda159979dded1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 28 May 2022 01:20:43 GMT
ADD file:0513eda9512e010cb9459591b62e0c9d9319750923df091b64250ad6e98c2878 in / 
# Sat, 28 May 2022 01:20:43 GMT
CMD ["bash"]
# Sat, 28 May 2022 05:33:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 28 May 2022 05:33:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:33:14 GMT
ENV GOSU_VERSION=1.14
# Sat, 28 May 2022 05:33:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 28 May 2022 05:33:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 28 May 2022 05:33:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:33:31 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Sat, 28 May 2022 05:33:31 GMT
ENV MYSQL_MAJOR=8.0
# Sat, 28 May 2022 05:33:32 GMT
ENV MYSQL_VERSION=8.0.29-1debian10
# Sat, 28 May 2022 05:33:32 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Sat, 28 May 2022 05:33:46 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Sat, 28 May 2022 05:33:47 GMT
VOLUME [/var/lib/mysql]
# Sat, 28 May 2022 05:33:47 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Sat, 28 May 2022 05:33:47 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Sat, 28 May 2022 05:33:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 28 May 2022 05:33:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 May 2022 05:33:48 GMT
EXPOSE 3306 33060
# Sat, 28 May 2022 05:33:48 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c1ad9731b2c7bf7fddea67f2f3f553515179a375c489e591e2372700fcaca766`  
		Last Modified: Sat, 28 May 2022 01:26:05 GMT  
		Size: 27.1 MB (27140144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f6eb0ee84d0c793cbd8456f03775cc5d88f72c576ec455596dca4ad465df07`  
		Last Modified: Sat, 28 May 2022 05:34:47 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cffcf8691bc5ddfc0c45d837fef9c77c7e264f7a69faf37073d0c4b31fb87156`  
		Last Modified: Sat, 28 May 2022 05:34:48 GMT  
		Size: 4.2 MB (4179298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89a783b5ac8a82c6355c62896648cb37efdc387f41b31b5c1d09418ce1808e81`  
		Last Modified: Sat, 28 May 2022 05:34:45 GMT  
		Size: 1.4 MB (1386680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8393c7be5fa5ff5d50fba15ce47f16cb29d3363d3885632e7892c0854a4d9c`  
		Last Modified: Sat, 28 May 2022 05:34:45 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af768d0b181edf1d8a35699d64f8e71d05d7648a28c37a5ab6fe2e36ffddc5e0`  
		Last Modified: Sat, 28 May 2022 05:34:48 GMT  
		Size: 14.1 MB (14064399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:810d6aaaf54a9c0c9d817fd1615f43aaf0194bcc1fca1574a90e90d8f6d66c6a`  
		Last Modified: Sat, 28 May 2022 05:34:45 GMT  
		Size: 2.5 KB (2547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e014a8ae4c97230ff31778e48cc8801fe3d3b141b8e0a878270d1e2ddc4b4f3`  
		Last Modified: Sat, 28 May 2022 05:34:43 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a821425a33418d8b2e6373a86d9bdca37a6a4d7315ca23302665c2556269fd64`  
		Last Modified: Sat, 28 May 2022 05:35:00 GMT  
		Size: 109.1 MB (109103661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a10c2652132a5609dcf19779c0bebde64ef5f5d9e7d8a50f3127c274d56c894`  
		Last Modified: Sat, 28 May 2022 05:34:43 GMT  
		Size: 842.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4419638feac46fa0870175acf37fdb6aea243ba43de9dea79a31fc9afbff395b`  
		Last Modified: Sat, 28 May 2022 05:34:43 GMT  
		Size: 5.2 KB (5152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:681aeed97dfe0d4bc23a8411287a322f495b790026a8b476b956f90355c9aae0`  
		Last Modified: Sat, 28 May 2022 05:34:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:latest`

```console
$ docker pull mysql@sha256:548da4c67fd8a71908f17c308b8ddb098acf5191d3d7694e56801c6a8b2072cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:latest` - linux; amd64

```console
$ docker pull mysql@sha256:0c0beeac7ca1937d60f54e1fb0c4a5c0b0ffee2aae37488fbc9f5ea301425551
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.9 MB (155884977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65b636d5542b73254ce90cc4b895597dc1adc2c661ca553c38eda159979dded1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 28 May 2022 01:20:43 GMT
ADD file:0513eda9512e010cb9459591b62e0c9d9319750923df091b64250ad6e98c2878 in / 
# Sat, 28 May 2022 01:20:43 GMT
CMD ["bash"]
# Sat, 28 May 2022 05:33:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 28 May 2022 05:33:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:33:14 GMT
ENV GOSU_VERSION=1.14
# Sat, 28 May 2022 05:33:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 28 May 2022 05:33:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 28 May 2022 05:33:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:33:31 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Sat, 28 May 2022 05:33:31 GMT
ENV MYSQL_MAJOR=8.0
# Sat, 28 May 2022 05:33:32 GMT
ENV MYSQL_VERSION=8.0.29-1debian10
# Sat, 28 May 2022 05:33:32 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Sat, 28 May 2022 05:33:46 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Sat, 28 May 2022 05:33:47 GMT
VOLUME [/var/lib/mysql]
# Sat, 28 May 2022 05:33:47 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Sat, 28 May 2022 05:33:47 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Sat, 28 May 2022 05:33:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 28 May 2022 05:33:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 May 2022 05:33:48 GMT
EXPOSE 3306 33060
# Sat, 28 May 2022 05:33:48 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c1ad9731b2c7bf7fddea67f2f3f553515179a375c489e591e2372700fcaca766`  
		Last Modified: Sat, 28 May 2022 01:26:05 GMT  
		Size: 27.1 MB (27140144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f6eb0ee84d0c793cbd8456f03775cc5d88f72c576ec455596dca4ad465df07`  
		Last Modified: Sat, 28 May 2022 05:34:47 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cffcf8691bc5ddfc0c45d837fef9c77c7e264f7a69faf37073d0c4b31fb87156`  
		Last Modified: Sat, 28 May 2022 05:34:48 GMT  
		Size: 4.2 MB (4179298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89a783b5ac8a82c6355c62896648cb37efdc387f41b31b5c1d09418ce1808e81`  
		Last Modified: Sat, 28 May 2022 05:34:45 GMT  
		Size: 1.4 MB (1386680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8393c7be5fa5ff5d50fba15ce47f16cb29d3363d3885632e7892c0854a4d9c`  
		Last Modified: Sat, 28 May 2022 05:34:45 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af768d0b181edf1d8a35699d64f8e71d05d7648a28c37a5ab6fe2e36ffddc5e0`  
		Last Modified: Sat, 28 May 2022 05:34:48 GMT  
		Size: 14.1 MB (14064399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:810d6aaaf54a9c0c9d817fd1615f43aaf0194bcc1fca1574a90e90d8f6d66c6a`  
		Last Modified: Sat, 28 May 2022 05:34:45 GMT  
		Size: 2.5 KB (2547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e014a8ae4c97230ff31778e48cc8801fe3d3b141b8e0a878270d1e2ddc4b4f3`  
		Last Modified: Sat, 28 May 2022 05:34:43 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a821425a33418d8b2e6373a86d9bdca37a6a4d7315ca23302665c2556269fd64`  
		Last Modified: Sat, 28 May 2022 05:35:00 GMT  
		Size: 109.1 MB (109103661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a10c2652132a5609dcf19779c0bebde64ef5f5d9e7d8a50f3127c274d56c894`  
		Last Modified: Sat, 28 May 2022 05:34:43 GMT  
		Size: 842.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4419638feac46fa0870175acf37fdb6aea243ba43de9dea79a31fc9afbff395b`  
		Last Modified: Sat, 28 May 2022 05:34:43 GMT  
		Size: 5.2 KB (5152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:681aeed97dfe0d4bc23a8411287a322f495b790026a8b476b956f90355c9aae0`  
		Last Modified: Sat, 28 May 2022 05:34:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:oracle`

```console
$ docker pull mysql@sha256:da035e352c785da143a1c02408b1895f95a5ef1c8aafa6555a7c6a386d49026c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:oracle` - linux; amd64

```console
$ docker pull mysql@sha256:940fdfa3dc408fb792a8cceb21cafda4b7cd56ce4fbc32833766bdd2a57d6a4f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.6 MB (131636256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebcfb2bcbf716a71cdb2dd51277575869547854e0c57519c03cd5d5cec58a9a0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 14 Jun 2022 18:23:26 GMT
ADD file:837f6c6e7e20067b92edb72e78a8399e6cbbd72dab23db7b5b5a301c58d2a0de in / 
# Tue, 14 Jun 2022 18:23:26 GMT
CMD ["/bin/bash"]
# Tue, 14 Jun 2022 18:39:39 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Tue, 14 Jun 2022 18:39:39 GMT
ENV GOSU_VERSION=1.14
# Tue, 14 Jun 2022 18:39:43 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 14 Jun 2022 18:40:04 GMT
RUN set -eux; 	microdnf install -y 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Tue, 14 Jun 2022 18:40:05 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Tue, 14 Jun 2022 18:40:06 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 14 Jun 2022 18:40:06 GMT
ENV MYSQL_VERSION=8.0.29-1.el8
# Tue, 14 Jun 2022 18:40:06 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 14 Jun 2022 18:40:34 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Tue, 14 Jun 2022 18:40:35 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 14 Jun 2022 18:40:35 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el8
# Tue, 14 Jun 2022 18:41:10 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 14 Jun 2022 18:41:10 GMT
VOLUME [/var/lib/mysql]
# Tue, 14 Jun 2022 18:41:10 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 14 Jun 2022 18:41:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Jun 2022 18:41:11 GMT
EXPOSE 3306 33060
# Tue, 14 Jun 2022 18:41:11 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5f160c0f6cac587a73883b48a8857f5cce0930112792cef25c62510e256e93dc`  
		Last Modified: Tue, 14 Jun 2022 18:24:18 GMT  
		Size: 39.2 MB (39219730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d86c3d841d1984f858257755bdf734554725af4f926f3b1d1b22f119cce8bda9`  
		Last Modified: Tue, 14 Jun 2022 18:41:49 GMT  
		Size: 1.1 KB (1079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f026b3ec1ed102cfe531d812e2063669bad08ac3a0ac68a31e44083d9b9a5f5d`  
		Last Modified: Tue, 14 Jun 2022 18:41:47 GMT  
		Size: 928.8 KB (928831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80b2ddd662a38dbb423dbaa2be04afd41904253b436138b52f2a73aa46a5547`  
		Last Modified: Tue, 14 Jun 2022 18:41:48 GMT  
		Size: 4.5 MB (4535169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a7724a6d28d1e789da86c89f0010caa7de0e4747dfcd360fa981a194850951f`  
		Last Modified: Tue, 14 Jun 2022 18:41:47 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8122570b85fec5c1d3bc0c08a48be2657da195b764c9a13b1a791a086c007368`  
		Last Modified: Tue, 14 Jun 2022 18:41:45 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea018df6cdc3d2aa821feb43a3035926c0c296b3c363e64ab0fa95f144f2e7b`  
		Last Modified: Tue, 14 Jun 2022 18:41:52 GMT  
		Size: 47.2 MB (47244178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8066c16abd2efdd49dd1fe3fab6fec9d250b699d9c0227f69c779c8da2c2acd6`  
		Last Modified: Tue, 14 Jun 2022 18:41:44 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd480e7da7ced7cfb1fb54d07fc5eb08057151be162150bd053f4eb89d9ba85f`  
		Last Modified: Tue, 14 Jun 2022 18:41:52 GMT  
		Size: 39.7 MB (39698832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b680e02f092e5330cf0200abf3ba02bddc3d440d02ebb11ec6ed8bf2ba3155`  
		Last Modified: Tue, 14 Jun 2022 18:41:45 GMT  
		Size: 5.2 KB (5158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:72ada8284e4c164a799b2a97058fdbf3a12883704b0505b15c61c136cd67e4d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.6 MB (138588260 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55ca64bef8c56fe87faa7cc81e738b003c0d59448a15740d822fb0666bf26fd0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 14 Jun 2022 18:41:36 GMT
ADD file:4a6ee90ad73353bfb87b2f121e06bddaed6104536e485baa83fadbe7facc774c in / 
# Tue, 14 Jun 2022 18:41:37 GMT
CMD ["/bin/bash"]
# Tue, 14 Jun 2022 19:17:17 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Tue, 14 Jun 2022 19:17:17 GMT
ENV GOSU_VERSION=1.14
# Tue, 14 Jun 2022 19:17:21 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 14 Jun 2022 19:17:44 GMT
RUN set -eux; 	microdnf install -y 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Tue, 14 Jun 2022 19:17:45 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Tue, 14 Jun 2022 19:17:46 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 14 Jun 2022 19:17:47 GMT
ENV MYSQL_VERSION=8.0.29-1.el8
# Tue, 14 Jun 2022 19:17:48 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 14 Jun 2022 19:18:15 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Tue, 14 Jun 2022 19:18:16 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 14 Jun 2022 19:18:17 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el8
# Tue, 14 Jun 2022 19:18:47 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 14 Jun 2022 19:18:48 GMT
VOLUME [/var/lib/mysql]
# Tue, 14 Jun 2022 19:18:49 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 14 Jun 2022 19:18:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Jun 2022 19:18:50 GMT
EXPOSE 3306 33060
# Tue, 14 Jun 2022 19:18:51 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2bbc1bf883bd601c0da5735b538963308bcc17f90d36525ecc93456ffad79064`  
		Last Modified: Tue, 14 Jun 2022 18:42:39 GMT  
		Size: 38.0 MB (38012371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8428f9d18fc319262a774f75a5849d4819b5b44cbf07fbb5e3c262e5cf30c22d`  
		Last Modified: Tue, 14 Jun 2022 19:19:14 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69cba94044003680a99c76f187ea817c71b843de38bb7f28faf8ca6508efd45e`  
		Last Modified: Tue, 14 Jun 2022 19:19:12 GMT  
		Size: 857.2 KB (857152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eac2db801a3647077263a37064e93b70b92541bf4ca7ff49164ebd26b5909df1`  
		Last Modified: Tue, 14 Jun 2022 19:19:13 GMT  
		Size: 4.4 MB (4361254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8bdbcb57725745140238f0807a9980dfccc7901a59788bdd8e8673b9dfc9e4`  
		Last Modified: Tue, 14 Jun 2022 19:19:12 GMT  
		Size: 2.6 KB (2603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25a4fad67d68ae03439e555e68701ab4ee3ea16f2e2f90c1b202ba894b9c4d37`  
		Last Modified: Tue, 14 Jun 2022 19:19:09 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab136e2e0f6c6851a5804d1310ceaad035c500537f8208705649f4b35402829`  
		Last Modified: Tue, 14 Jun 2022 19:19:17 GMT  
		Size: 53.3 MB (53307019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee6421b3efe2970642254e83d78cea1cb6f54a77db5a9b1c4c5c6be95df2532`  
		Last Modified: Tue, 14 Jun 2022 19:19:09 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1620f6ea4d62464f9ce80ceafbcf9b7fea1f93be1355e6eadd5fee9eaf35bf6f`  
		Last Modified: Tue, 14 Jun 2022 19:19:17 GMT  
		Size: 42.0 MB (42041038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b288f89c74171bb779509de10b16a7756d2694417c2d960dc3d2b3a534245992`  
		Last Modified: Tue, 14 Jun 2022 19:19:09 GMT  
		Size: 5.2 KB (5160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
