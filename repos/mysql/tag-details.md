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
$ docker pull mysql@sha256:16e159331007eccc069822f7b731272043ed572a79a196a05ffa2ea127caaf67
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5` - linux; amd64

```console
$ docker pull mysql@sha256:368c1258fb7330eece5a0fbe2c9801d666bb0f26d7a82c78c431fbcb8f5fd191
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.5 MB (162456671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3d35804fa376a141b9a9dad8f5534c3179f4c328d6efc67c5c5145d257c291a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 11 May 2022 01:20:37 GMT
ADD file:76b454ddb7dfe4d22afae844a7e67e7e5fb4570dae2e21bbd259a1f2e5839f33 in / 
# Wed, 11 May 2022 01:20:37 GMT
CMD ["bash"]
# Wed, 11 May 2022 05:01:23 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 11 May 2022 05:01:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 05:01:29 GMT
ENV GOSU_VERSION=1.14
# Wed, 11 May 2022 05:01:38 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 11 May 2022 05:01:39 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 11 May 2022 05:01:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 05:01:46 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 11 May 2022 05:02:12 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 11 May 2022 05:02:12 GMT
ENV MYSQL_VERSION=5.7.38-1debian10
# Wed, 11 May 2022 05:02:13 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Wed, 11 May 2022 05:02:31 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 11 May 2022 05:02:32 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 May 2022 05:02:32 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Wed, 11 May 2022 05:02:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 05:02:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 05:02:32 GMT
EXPOSE 3306 33060
# Wed, 11 May 2022 05:02:33 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c32ce6654453d35d0b3dde45d195adeee586ffba0a683006ee06748c077c01fa`  
		Last Modified: Wed, 11 May 2022 01:25:58 GMT  
		Size: 27.1 MB (27140722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415d08ee031ab3bffe8c0db6b82f2cde88049eda62a50801eb6d8aa68bb0e12c`  
		Last Modified: Wed, 11 May 2022 05:03:03 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a38fec2542ffcfa6247f2992d1ec422b38e00ed5ca998bc5b890ca1a97ab1d5`  
		Last Modified: Wed, 11 May 2022 05:03:04 GMT  
		Size: 4.2 MB (4179283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352881ee8fe9b63edbd90eb3a1ffa035c72b7edfbcad6fda55db516c2a2b2cb9`  
		Last Modified: Wed, 11 May 2022 05:03:02 GMT  
		Size: 1.4 MB (1386677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8e20da291b6c92de4aa28a02fe8845045ec68d9b9ad1497e921fa42e8303650`  
		Last Modified: Wed, 11 May 2022 05:03:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66c2a8cc1999eedaa968d140339f25947e1faf8b3f2084c7eb5eee68455d6295`  
		Last Modified: Wed, 11 May 2022 05:03:03 GMT  
		Size: 14.1 MB (14064393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3a3a8e49878cc1f98a4927704e4fdc191bcc2cc80fbf7470b36fe1b44b7596d`  
		Last Modified: Wed, 11 May 2022 05:03:01 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:172aabfba65cfce5cfcc754b562da5a55e6328ca9c02b005fdf40d07b0e6cfcd`  
		Last Modified: Wed, 11 May 2022 05:03:45 GMT  
		Size: 254.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea17d0b1d1ec95b127efcb443db4ffe3c6bbc890efa5754602b9d49691a567d`  
		Last Modified: Wed, 11 May 2022 05:04:00 GMT  
		Size: 115.7 MB (115675657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fff7f5411ca9049d62e30c6a523c27a914994bcb1750bcef101daf61db3f42c4`  
		Last Modified: Wed, 11 May 2022 05:03:45 GMT  
		Size: 5.1 KB (5135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33d43428e07b9c9c4d69f30ad3287c01be6f5938dca2821207281bd6927d026`  
		Last Modified: Wed, 11 May 2022 05:03:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5-debian`

```console
$ docker pull mysql@sha256:16e159331007eccc069822f7b731272043ed572a79a196a05ffa2ea127caaf67
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5-debian` - linux; amd64

```console
$ docker pull mysql@sha256:368c1258fb7330eece5a0fbe2c9801d666bb0f26d7a82c78c431fbcb8f5fd191
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.5 MB (162456671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3d35804fa376a141b9a9dad8f5534c3179f4c328d6efc67c5c5145d257c291a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 11 May 2022 01:20:37 GMT
ADD file:76b454ddb7dfe4d22afae844a7e67e7e5fb4570dae2e21bbd259a1f2e5839f33 in / 
# Wed, 11 May 2022 01:20:37 GMT
CMD ["bash"]
# Wed, 11 May 2022 05:01:23 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 11 May 2022 05:01:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 05:01:29 GMT
ENV GOSU_VERSION=1.14
# Wed, 11 May 2022 05:01:38 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 11 May 2022 05:01:39 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 11 May 2022 05:01:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 05:01:46 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 11 May 2022 05:02:12 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 11 May 2022 05:02:12 GMT
ENV MYSQL_VERSION=5.7.38-1debian10
# Wed, 11 May 2022 05:02:13 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Wed, 11 May 2022 05:02:31 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 11 May 2022 05:02:32 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 May 2022 05:02:32 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Wed, 11 May 2022 05:02:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 05:02:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 05:02:32 GMT
EXPOSE 3306 33060
# Wed, 11 May 2022 05:02:33 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c32ce6654453d35d0b3dde45d195adeee586ffba0a683006ee06748c077c01fa`  
		Last Modified: Wed, 11 May 2022 01:25:58 GMT  
		Size: 27.1 MB (27140722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415d08ee031ab3bffe8c0db6b82f2cde88049eda62a50801eb6d8aa68bb0e12c`  
		Last Modified: Wed, 11 May 2022 05:03:03 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a38fec2542ffcfa6247f2992d1ec422b38e00ed5ca998bc5b890ca1a97ab1d5`  
		Last Modified: Wed, 11 May 2022 05:03:04 GMT  
		Size: 4.2 MB (4179283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352881ee8fe9b63edbd90eb3a1ffa035c72b7edfbcad6fda55db516c2a2b2cb9`  
		Last Modified: Wed, 11 May 2022 05:03:02 GMT  
		Size: 1.4 MB (1386677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8e20da291b6c92de4aa28a02fe8845045ec68d9b9ad1497e921fa42e8303650`  
		Last Modified: Wed, 11 May 2022 05:03:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66c2a8cc1999eedaa968d140339f25947e1faf8b3f2084c7eb5eee68455d6295`  
		Last Modified: Wed, 11 May 2022 05:03:03 GMT  
		Size: 14.1 MB (14064393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3a3a8e49878cc1f98a4927704e4fdc191bcc2cc80fbf7470b36fe1b44b7596d`  
		Last Modified: Wed, 11 May 2022 05:03:01 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:172aabfba65cfce5cfcc754b562da5a55e6328ca9c02b005fdf40d07b0e6cfcd`  
		Last Modified: Wed, 11 May 2022 05:03:45 GMT  
		Size: 254.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea17d0b1d1ec95b127efcb443db4ffe3c6bbc890efa5754602b9d49691a567d`  
		Last Modified: Wed, 11 May 2022 05:04:00 GMT  
		Size: 115.7 MB (115675657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fff7f5411ca9049d62e30c6a523c27a914994bcb1750bcef101daf61db3f42c4`  
		Last Modified: Wed, 11 May 2022 05:03:45 GMT  
		Size: 5.1 KB (5135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33d43428e07b9c9c4d69f30ad3287c01be6f5938dca2821207281bd6927d026`  
		Last Modified: Wed, 11 May 2022 05:03:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5-oracle`

```console
$ docker pull mysql@sha256:30a1708538c16b5487f559af0b223bd2d1391355c8e1d2d4bed39807ecb9bd2b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:1a41c43ec1d524c4b66c1901b27a438da21eadfbafe3616bda8ea75302098b8d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.9 MB (126893712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7619c1a0561f44994c5527d453687ac411749a02708aae7e966ce8407ad7a2b8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 29 Mar 2022 18:36:11 GMT
ADD file:b0df42f2bb614be48861be26e670ab6a81c1549d24e64b5e355980adcf0074be in / 
# Tue, 29 Mar 2022 18:36:11 GMT
CMD ["/bin/bash"]
# Thu, 31 Mar 2022 02:12:23 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Thu, 31 Mar 2022 02:12:23 GMT
ENV GOSU_VERSION=1.14
# Thu, 31 Mar 2022 02:12:26 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 31 Mar 2022 02:12:36 GMT
RUN set -eux; 	yum install -y 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Thu, 31 Mar 2022 02:12:37 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 31 Mar 2022 02:12:37 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 27 Apr 2022 22:19:48 GMT
ENV MYSQL_VERSION=5.7.38-1.el7
# Wed, 27 Apr 2022 22:19:48 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 27 Apr 2022 22:20:03 GMT
RUN set -eux; 	yum install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Wed, 27 Apr 2022 22:20:04 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 27 Apr 2022 22:20:04 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el7
# Wed, 27 Apr 2022 22:20:22 GMT
RUN set -eux; 	yum install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Wed, 27 Apr 2022 22:20:23 GMT
VOLUME [/var/lib/mysql]
# Wed, 27 Apr 2022 22:20:23 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Wed, 27 Apr 2022 22:20:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 27 Apr 2022 22:20:23 GMT
EXPOSE 3306 33060
# Wed, 27 Apr 2022 22:20:23 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:9347a8f0b30748522f1f50b679f9f2d0c3eea2bb49da98bb4f38a8c8619b7bf8`  
		Last Modified: Tue, 29 Mar 2022 18:37:31 GMT  
		Size: 48.8 MB (48757483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1268f9b69b4d2dfc0086f5426266fd97bb99c37e0dc2db707e3e7a5667bba3c`  
		Last Modified: Thu, 31 Mar 2022 02:14:13 GMT  
		Size: 1.1 KB (1060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1084d021338c13d9afc0d3fa5ab8ff753ddd7d97abc2a81074b6fff0807a96`  
		Last Modified: Thu, 31 Mar 2022 02:14:11 GMT  
		Size: 930.2 KB (930229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92ad34fb0ede94774c93b333cbdc752915f8d0b45eda981588615248b8fbad9e`  
		Last Modified: Thu, 31 Mar 2022 02:14:12 GMT  
		Size: 3.8 MB (3755164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e341499385aec2522efd754b4ba03c458add9de6802a7834b941209fb793dc0f`  
		Last Modified: Thu, 31 Mar 2022 02:14:11 GMT  
		Size: 2.7 KB (2658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f50a4a291c85ddcce0931530fad6656dbf111a0b9e320a939a69a55aedb3c6c8`  
		Last Modified: Wed, 27 Apr 2022 22:22:20 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:396321ba07427f51923e3a3dd9aae2ee975d943cd39407d5c1557dc5f457e5d0`  
		Last Modified: Wed, 27 Apr 2022 22:22:24 GMT  
		Size: 25.5 MB (25473337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3992ab4878ba76eec5124d91b386fd2e3c35db49932c8eec13e0511a1996e21`  
		Last Modified: Wed, 27 Apr 2022 22:22:20 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7881d745f09807de84ae1a7e0e09556a2c31831776461cc55e6b531d5e73bf3c`  
		Last Modified: Wed, 27 Apr 2022 22:22:29 GMT  
		Size: 48.0 MB (47967990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b17c44fe903a44a0e1f059dcb92b1bea5ce893982a0644e310ce3527cfd68f64`  
		Last Modified: Wed, 27 Apr 2022 22:22:20 GMT  
		Size: 5.1 KB (5141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7`

```console
$ docker pull mysql@sha256:16e159331007eccc069822f7b731272043ed572a79a196a05ffa2ea127caaf67
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7` - linux; amd64

```console
$ docker pull mysql@sha256:368c1258fb7330eece5a0fbe2c9801d666bb0f26d7a82c78c431fbcb8f5fd191
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.5 MB (162456671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3d35804fa376a141b9a9dad8f5534c3179f4c328d6efc67c5c5145d257c291a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 11 May 2022 01:20:37 GMT
ADD file:76b454ddb7dfe4d22afae844a7e67e7e5fb4570dae2e21bbd259a1f2e5839f33 in / 
# Wed, 11 May 2022 01:20:37 GMT
CMD ["bash"]
# Wed, 11 May 2022 05:01:23 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 11 May 2022 05:01:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 05:01:29 GMT
ENV GOSU_VERSION=1.14
# Wed, 11 May 2022 05:01:38 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 11 May 2022 05:01:39 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 11 May 2022 05:01:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 05:01:46 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 11 May 2022 05:02:12 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 11 May 2022 05:02:12 GMT
ENV MYSQL_VERSION=5.7.38-1debian10
# Wed, 11 May 2022 05:02:13 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Wed, 11 May 2022 05:02:31 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 11 May 2022 05:02:32 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 May 2022 05:02:32 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Wed, 11 May 2022 05:02:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 05:02:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 05:02:32 GMT
EXPOSE 3306 33060
# Wed, 11 May 2022 05:02:33 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c32ce6654453d35d0b3dde45d195adeee586ffba0a683006ee06748c077c01fa`  
		Last Modified: Wed, 11 May 2022 01:25:58 GMT  
		Size: 27.1 MB (27140722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415d08ee031ab3bffe8c0db6b82f2cde88049eda62a50801eb6d8aa68bb0e12c`  
		Last Modified: Wed, 11 May 2022 05:03:03 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a38fec2542ffcfa6247f2992d1ec422b38e00ed5ca998bc5b890ca1a97ab1d5`  
		Last Modified: Wed, 11 May 2022 05:03:04 GMT  
		Size: 4.2 MB (4179283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352881ee8fe9b63edbd90eb3a1ffa035c72b7edfbcad6fda55db516c2a2b2cb9`  
		Last Modified: Wed, 11 May 2022 05:03:02 GMT  
		Size: 1.4 MB (1386677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8e20da291b6c92de4aa28a02fe8845045ec68d9b9ad1497e921fa42e8303650`  
		Last Modified: Wed, 11 May 2022 05:03:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66c2a8cc1999eedaa968d140339f25947e1faf8b3f2084c7eb5eee68455d6295`  
		Last Modified: Wed, 11 May 2022 05:03:03 GMT  
		Size: 14.1 MB (14064393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3a3a8e49878cc1f98a4927704e4fdc191bcc2cc80fbf7470b36fe1b44b7596d`  
		Last Modified: Wed, 11 May 2022 05:03:01 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:172aabfba65cfce5cfcc754b562da5a55e6328ca9c02b005fdf40d07b0e6cfcd`  
		Last Modified: Wed, 11 May 2022 05:03:45 GMT  
		Size: 254.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea17d0b1d1ec95b127efcb443db4ffe3c6bbc890efa5754602b9d49691a567d`  
		Last Modified: Wed, 11 May 2022 05:04:00 GMT  
		Size: 115.7 MB (115675657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fff7f5411ca9049d62e30c6a523c27a914994bcb1750bcef101daf61db3f42c4`  
		Last Modified: Wed, 11 May 2022 05:03:45 GMT  
		Size: 5.1 KB (5135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33d43428e07b9c9c4d69f30ad3287c01be6f5938dca2821207281bd6927d026`  
		Last Modified: Wed, 11 May 2022 05:03:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7-debian`

```console
$ docker pull mysql@sha256:16e159331007eccc069822f7b731272043ed572a79a196a05ffa2ea127caaf67
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7-debian` - linux; amd64

```console
$ docker pull mysql@sha256:368c1258fb7330eece5a0fbe2c9801d666bb0f26d7a82c78c431fbcb8f5fd191
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.5 MB (162456671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3d35804fa376a141b9a9dad8f5534c3179f4c328d6efc67c5c5145d257c291a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 11 May 2022 01:20:37 GMT
ADD file:76b454ddb7dfe4d22afae844a7e67e7e5fb4570dae2e21bbd259a1f2e5839f33 in / 
# Wed, 11 May 2022 01:20:37 GMT
CMD ["bash"]
# Wed, 11 May 2022 05:01:23 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 11 May 2022 05:01:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 05:01:29 GMT
ENV GOSU_VERSION=1.14
# Wed, 11 May 2022 05:01:38 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 11 May 2022 05:01:39 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 11 May 2022 05:01:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 05:01:46 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 11 May 2022 05:02:12 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 11 May 2022 05:02:12 GMT
ENV MYSQL_VERSION=5.7.38-1debian10
# Wed, 11 May 2022 05:02:13 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Wed, 11 May 2022 05:02:31 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 11 May 2022 05:02:32 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 May 2022 05:02:32 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Wed, 11 May 2022 05:02:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 05:02:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 05:02:32 GMT
EXPOSE 3306 33060
# Wed, 11 May 2022 05:02:33 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c32ce6654453d35d0b3dde45d195adeee586ffba0a683006ee06748c077c01fa`  
		Last Modified: Wed, 11 May 2022 01:25:58 GMT  
		Size: 27.1 MB (27140722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415d08ee031ab3bffe8c0db6b82f2cde88049eda62a50801eb6d8aa68bb0e12c`  
		Last Modified: Wed, 11 May 2022 05:03:03 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a38fec2542ffcfa6247f2992d1ec422b38e00ed5ca998bc5b890ca1a97ab1d5`  
		Last Modified: Wed, 11 May 2022 05:03:04 GMT  
		Size: 4.2 MB (4179283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352881ee8fe9b63edbd90eb3a1ffa035c72b7edfbcad6fda55db516c2a2b2cb9`  
		Last Modified: Wed, 11 May 2022 05:03:02 GMT  
		Size: 1.4 MB (1386677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8e20da291b6c92de4aa28a02fe8845045ec68d9b9ad1497e921fa42e8303650`  
		Last Modified: Wed, 11 May 2022 05:03:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66c2a8cc1999eedaa968d140339f25947e1faf8b3f2084c7eb5eee68455d6295`  
		Last Modified: Wed, 11 May 2022 05:03:03 GMT  
		Size: 14.1 MB (14064393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3a3a8e49878cc1f98a4927704e4fdc191bcc2cc80fbf7470b36fe1b44b7596d`  
		Last Modified: Wed, 11 May 2022 05:03:01 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:172aabfba65cfce5cfcc754b562da5a55e6328ca9c02b005fdf40d07b0e6cfcd`  
		Last Modified: Wed, 11 May 2022 05:03:45 GMT  
		Size: 254.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea17d0b1d1ec95b127efcb443db4ffe3c6bbc890efa5754602b9d49691a567d`  
		Last Modified: Wed, 11 May 2022 05:04:00 GMT  
		Size: 115.7 MB (115675657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fff7f5411ca9049d62e30c6a523c27a914994bcb1750bcef101daf61db3f42c4`  
		Last Modified: Wed, 11 May 2022 05:03:45 GMT  
		Size: 5.1 KB (5135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33d43428e07b9c9c4d69f30ad3287c01be6f5938dca2821207281bd6927d026`  
		Last Modified: Wed, 11 May 2022 05:03:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7-oracle`

```console
$ docker pull mysql@sha256:30a1708538c16b5487f559af0b223bd2d1391355c8e1d2d4bed39807ecb9bd2b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:1a41c43ec1d524c4b66c1901b27a438da21eadfbafe3616bda8ea75302098b8d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.9 MB (126893712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7619c1a0561f44994c5527d453687ac411749a02708aae7e966ce8407ad7a2b8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 29 Mar 2022 18:36:11 GMT
ADD file:b0df42f2bb614be48861be26e670ab6a81c1549d24e64b5e355980adcf0074be in / 
# Tue, 29 Mar 2022 18:36:11 GMT
CMD ["/bin/bash"]
# Thu, 31 Mar 2022 02:12:23 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Thu, 31 Mar 2022 02:12:23 GMT
ENV GOSU_VERSION=1.14
# Thu, 31 Mar 2022 02:12:26 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 31 Mar 2022 02:12:36 GMT
RUN set -eux; 	yum install -y 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Thu, 31 Mar 2022 02:12:37 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 31 Mar 2022 02:12:37 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 27 Apr 2022 22:19:48 GMT
ENV MYSQL_VERSION=5.7.38-1.el7
# Wed, 27 Apr 2022 22:19:48 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 27 Apr 2022 22:20:03 GMT
RUN set -eux; 	yum install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Wed, 27 Apr 2022 22:20:04 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 27 Apr 2022 22:20:04 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el7
# Wed, 27 Apr 2022 22:20:22 GMT
RUN set -eux; 	yum install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Wed, 27 Apr 2022 22:20:23 GMT
VOLUME [/var/lib/mysql]
# Wed, 27 Apr 2022 22:20:23 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Wed, 27 Apr 2022 22:20:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 27 Apr 2022 22:20:23 GMT
EXPOSE 3306 33060
# Wed, 27 Apr 2022 22:20:23 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:9347a8f0b30748522f1f50b679f9f2d0c3eea2bb49da98bb4f38a8c8619b7bf8`  
		Last Modified: Tue, 29 Mar 2022 18:37:31 GMT  
		Size: 48.8 MB (48757483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1268f9b69b4d2dfc0086f5426266fd97bb99c37e0dc2db707e3e7a5667bba3c`  
		Last Modified: Thu, 31 Mar 2022 02:14:13 GMT  
		Size: 1.1 KB (1060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1084d021338c13d9afc0d3fa5ab8ff753ddd7d97abc2a81074b6fff0807a96`  
		Last Modified: Thu, 31 Mar 2022 02:14:11 GMT  
		Size: 930.2 KB (930229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92ad34fb0ede94774c93b333cbdc752915f8d0b45eda981588615248b8fbad9e`  
		Last Modified: Thu, 31 Mar 2022 02:14:12 GMT  
		Size: 3.8 MB (3755164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e341499385aec2522efd754b4ba03c458add9de6802a7834b941209fb793dc0f`  
		Last Modified: Thu, 31 Mar 2022 02:14:11 GMT  
		Size: 2.7 KB (2658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f50a4a291c85ddcce0931530fad6656dbf111a0b9e320a939a69a55aedb3c6c8`  
		Last Modified: Wed, 27 Apr 2022 22:22:20 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:396321ba07427f51923e3a3dd9aae2ee975d943cd39407d5c1557dc5f457e5d0`  
		Last Modified: Wed, 27 Apr 2022 22:22:24 GMT  
		Size: 25.5 MB (25473337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3992ab4878ba76eec5124d91b386fd2e3c35db49932c8eec13e0511a1996e21`  
		Last Modified: Wed, 27 Apr 2022 22:22:20 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7881d745f09807de84ae1a7e0e09556a2c31831776461cc55e6b531d5e73bf3c`  
		Last Modified: Wed, 27 Apr 2022 22:22:29 GMT  
		Size: 48.0 MB (47967990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b17c44fe903a44a0e1f059dcb92b1bea5ce893982a0644e310ce3527cfd68f64`  
		Last Modified: Wed, 27 Apr 2022 22:22:20 GMT  
		Size: 5.1 KB (5141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.38`

```console
$ docker pull mysql@sha256:16e159331007eccc069822f7b731272043ed572a79a196a05ffa2ea127caaf67
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.38` - linux; amd64

```console
$ docker pull mysql@sha256:368c1258fb7330eece5a0fbe2c9801d666bb0f26d7a82c78c431fbcb8f5fd191
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.5 MB (162456671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3d35804fa376a141b9a9dad8f5534c3179f4c328d6efc67c5c5145d257c291a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 11 May 2022 01:20:37 GMT
ADD file:76b454ddb7dfe4d22afae844a7e67e7e5fb4570dae2e21bbd259a1f2e5839f33 in / 
# Wed, 11 May 2022 01:20:37 GMT
CMD ["bash"]
# Wed, 11 May 2022 05:01:23 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 11 May 2022 05:01:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 05:01:29 GMT
ENV GOSU_VERSION=1.14
# Wed, 11 May 2022 05:01:38 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 11 May 2022 05:01:39 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 11 May 2022 05:01:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 05:01:46 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 11 May 2022 05:02:12 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 11 May 2022 05:02:12 GMT
ENV MYSQL_VERSION=5.7.38-1debian10
# Wed, 11 May 2022 05:02:13 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Wed, 11 May 2022 05:02:31 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 11 May 2022 05:02:32 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 May 2022 05:02:32 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Wed, 11 May 2022 05:02:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 05:02:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 05:02:32 GMT
EXPOSE 3306 33060
# Wed, 11 May 2022 05:02:33 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c32ce6654453d35d0b3dde45d195adeee586ffba0a683006ee06748c077c01fa`  
		Last Modified: Wed, 11 May 2022 01:25:58 GMT  
		Size: 27.1 MB (27140722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415d08ee031ab3bffe8c0db6b82f2cde88049eda62a50801eb6d8aa68bb0e12c`  
		Last Modified: Wed, 11 May 2022 05:03:03 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a38fec2542ffcfa6247f2992d1ec422b38e00ed5ca998bc5b890ca1a97ab1d5`  
		Last Modified: Wed, 11 May 2022 05:03:04 GMT  
		Size: 4.2 MB (4179283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352881ee8fe9b63edbd90eb3a1ffa035c72b7edfbcad6fda55db516c2a2b2cb9`  
		Last Modified: Wed, 11 May 2022 05:03:02 GMT  
		Size: 1.4 MB (1386677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8e20da291b6c92de4aa28a02fe8845045ec68d9b9ad1497e921fa42e8303650`  
		Last Modified: Wed, 11 May 2022 05:03:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66c2a8cc1999eedaa968d140339f25947e1faf8b3f2084c7eb5eee68455d6295`  
		Last Modified: Wed, 11 May 2022 05:03:03 GMT  
		Size: 14.1 MB (14064393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3a3a8e49878cc1f98a4927704e4fdc191bcc2cc80fbf7470b36fe1b44b7596d`  
		Last Modified: Wed, 11 May 2022 05:03:01 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:172aabfba65cfce5cfcc754b562da5a55e6328ca9c02b005fdf40d07b0e6cfcd`  
		Last Modified: Wed, 11 May 2022 05:03:45 GMT  
		Size: 254.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea17d0b1d1ec95b127efcb443db4ffe3c6bbc890efa5754602b9d49691a567d`  
		Last Modified: Wed, 11 May 2022 05:04:00 GMT  
		Size: 115.7 MB (115675657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fff7f5411ca9049d62e30c6a523c27a914994bcb1750bcef101daf61db3f42c4`  
		Last Modified: Wed, 11 May 2022 05:03:45 GMT  
		Size: 5.1 KB (5135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33d43428e07b9c9c4d69f30ad3287c01be6f5938dca2821207281bd6927d026`  
		Last Modified: Wed, 11 May 2022 05:03:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.38-debian`

```console
$ docker pull mysql@sha256:16e159331007eccc069822f7b731272043ed572a79a196a05ffa2ea127caaf67
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.38-debian` - linux; amd64

```console
$ docker pull mysql@sha256:368c1258fb7330eece5a0fbe2c9801d666bb0f26d7a82c78c431fbcb8f5fd191
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.5 MB (162456671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3d35804fa376a141b9a9dad8f5534c3179f4c328d6efc67c5c5145d257c291a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 11 May 2022 01:20:37 GMT
ADD file:76b454ddb7dfe4d22afae844a7e67e7e5fb4570dae2e21bbd259a1f2e5839f33 in / 
# Wed, 11 May 2022 01:20:37 GMT
CMD ["bash"]
# Wed, 11 May 2022 05:01:23 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 11 May 2022 05:01:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 05:01:29 GMT
ENV GOSU_VERSION=1.14
# Wed, 11 May 2022 05:01:38 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 11 May 2022 05:01:39 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 11 May 2022 05:01:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 05:01:46 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 11 May 2022 05:02:12 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 11 May 2022 05:02:12 GMT
ENV MYSQL_VERSION=5.7.38-1debian10
# Wed, 11 May 2022 05:02:13 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Wed, 11 May 2022 05:02:31 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 11 May 2022 05:02:32 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 May 2022 05:02:32 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Wed, 11 May 2022 05:02:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 05:02:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 05:02:32 GMT
EXPOSE 3306 33060
# Wed, 11 May 2022 05:02:33 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c32ce6654453d35d0b3dde45d195adeee586ffba0a683006ee06748c077c01fa`  
		Last Modified: Wed, 11 May 2022 01:25:58 GMT  
		Size: 27.1 MB (27140722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415d08ee031ab3bffe8c0db6b82f2cde88049eda62a50801eb6d8aa68bb0e12c`  
		Last Modified: Wed, 11 May 2022 05:03:03 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a38fec2542ffcfa6247f2992d1ec422b38e00ed5ca998bc5b890ca1a97ab1d5`  
		Last Modified: Wed, 11 May 2022 05:03:04 GMT  
		Size: 4.2 MB (4179283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352881ee8fe9b63edbd90eb3a1ffa035c72b7edfbcad6fda55db516c2a2b2cb9`  
		Last Modified: Wed, 11 May 2022 05:03:02 GMT  
		Size: 1.4 MB (1386677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8e20da291b6c92de4aa28a02fe8845045ec68d9b9ad1497e921fa42e8303650`  
		Last Modified: Wed, 11 May 2022 05:03:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66c2a8cc1999eedaa968d140339f25947e1faf8b3f2084c7eb5eee68455d6295`  
		Last Modified: Wed, 11 May 2022 05:03:03 GMT  
		Size: 14.1 MB (14064393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3a3a8e49878cc1f98a4927704e4fdc191bcc2cc80fbf7470b36fe1b44b7596d`  
		Last Modified: Wed, 11 May 2022 05:03:01 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:172aabfba65cfce5cfcc754b562da5a55e6328ca9c02b005fdf40d07b0e6cfcd`  
		Last Modified: Wed, 11 May 2022 05:03:45 GMT  
		Size: 254.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea17d0b1d1ec95b127efcb443db4ffe3c6bbc890efa5754602b9d49691a567d`  
		Last Modified: Wed, 11 May 2022 05:04:00 GMT  
		Size: 115.7 MB (115675657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fff7f5411ca9049d62e30c6a523c27a914994bcb1750bcef101daf61db3f42c4`  
		Last Modified: Wed, 11 May 2022 05:03:45 GMT  
		Size: 5.1 KB (5135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33d43428e07b9c9c4d69f30ad3287c01be6f5938dca2821207281bd6927d026`  
		Last Modified: Wed, 11 May 2022 05:03:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.38-oracle`

```console
$ docker pull mysql@sha256:30a1708538c16b5487f559af0b223bd2d1391355c8e1d2d4bed39807ecb9bd2b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.38-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:1a41c43ec1d524c4b66c1901b27a438da21eadfbafe3616bda8ea75302098b8d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.9 MB (126893712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7619c1a0561f44994c5527d453687ac411749a02708aae7e966ce8407ad7a2b8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 29 Mar 2022 18:36:11 GMT
ADD file:b0df42f2bb614be48861be26e670ab6a81c1549d24e64b5e355980adcf0074be in / 
# Tue, 29 Mar 2022 18:36:11 GMT
CMD ["/bin/bash"]
# Thu, 31 Mar 2022 02:12:23 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Thu, 31 Mar 2022 02:12:23 GMT
ENV GOSU_VERSION=1.14
# Thu, 31 Mar 2022 02:12:26 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 31 Mar 2022 02:12:36 GMT
RUN set -eux; 	yum install -y 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Thu, 31 Mar 2022 02:12:37 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 31 Mar 2022 02:12:37 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 27 Apr 2022 22:19:48 GMT
ENV MYSQL_VERSION=5.7.38-1.el7
# Wed, 27 Apr 2022 22:19:48 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 27 Apr 2022 22:20:03 GMT
RUN set -eux; 	yum install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Wed, 27 Apr 2022 22:20:04 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 27 Apr 2022 22:20:04 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el7
# Wed, 27 Apr 2022 22:20:22 GMT
RUN set -eux; 	yum install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Wed, 27 Apr 2022 22:20:23 GMT
VOLUME [/var/lib/mysql]
# Wed, 27 Apr 2022 22:20:23 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Wed, 27 Apr 2022 22:20:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 27 Apr 2022 22:20:23 GMT
EXPOSE 3306 33060
# Wed, 27 Apr 2022 22:20:23 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:9347a8f0b30748522f1f50b679f9f2d0c3eea2bb49da98bb4f38a8c8619b7bf8`  
		Last Modified: Tue, 29 Mar 2022 18:37:31 GMT  
		Size: 48.8 MB (48757483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1268f9b69b4d2dfc0086f5426266fd97bb99c37e0dc2db707e3e7a5667bba3c`  
		Last Modified: Thu, 31 Mar 2022 02:14:13 GMT  
		Size: 1.1 KB (1060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1084d021338c13d9afc0d3fa5ab8ff753ddd7d97abc2a81074b6fff0807a96`  
		Last Modified: Thu, 31 Mar 2022 02:14:11 GMT  
		Size: 930.2 KB (930229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92ad34fb0ede94774c93b333cbdc752915f8d0b45eda981588615248b8fbad9e`  
		Last Modified: Thu, 31 Mar 2022 02:14:12 GMT  
		Size: 3.8 MB (3755164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e341499385aec2522efd754b4ba03c458add9de6802a7834b941209fb793dc0f`  
		Last Modified: Thu, 31 Mar 2022 02:14:11 GMT  
		Size: 2.7 KB (2658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f50a4a291c85ddcce0931530fad6656dbf111a0b9e320a939a69a55aedb3c6c8`  
		Last Modified: Wed, 27 Apr 2022 22:22:20 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:396321ba07427f51923e3a3dd9aae2ee975d943cd39407d5c1557dc5f457e5d0`  
		Last Modified: Wed, 27 Apr 2022 22:22:24 GMT  
		Size: 25.5 MB (25473337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3992ab4878ba76eec5124d91b386fd2e3c35db49932c8eec13e0511a1996e21`  
		Last Modified: Wed, 27 Apr 2022 22:22:20 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7881d745f09807de84ae1a7e0e09556a2c31831776461cc55e6b531d5e73bf3c`  
		Last Modified: Wed, 27 Apr 2022 22:22:29 GMT  
		Size: 48.0 MB (47967990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b17c44fe903a44a0e1f059dcb92b1bea5ce893982a0644e310ce3527cfd68f64`  
		Last Modified: Wed, 27 Apr 2022 22:22:20 GMT  
		Size: 5.1 KB (5141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8`

```console
$ docker pull mysql@sha256:a0805d37d4d298bd61e0dfa61f0ddf6f4680b453fa25d7aad420485a62417eab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8` - linux; amd64

```console
$ docker pull mysql@sha256:f8c1d78c6f134d3a99d451cd983399087de0faf376f350ebb47886c3d3a343e6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.9 MB (155885550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76152be684492598eb4fb366674a85c7ae222025d783525d548e607d0c0030f4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 11 May 2022 01:20:37 GMT
ADD file:76b454ddb7dfe4d22afae844a7e67e7e5fb4570dae2e21bbd259a1f2e5839f33 in / 
# Wed, 11 May 2022 01:20:37 GMT
CMD ["bash"]
# Wed, 11 May 2022 05:01:23 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 11 May 2022 05:01:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 05:01:29 GMT
ENV GOSU_VERSION=1.14
# Wed, 11 May 2022 05:01:38 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 11 May 2022 05:01:39 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 11 May 2022 05:01:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 05:01:46 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 11 May 2022 05:01:46 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 11 May 2022 05:01:46 GMT
ENV MYSQL_VERSION=8.0.29-1debian10
# Wed, 11 May 2022 05:01:47 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Wed, 11 May 2022 05:02:01 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 11 May 2022 05:02:02 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 May 2022 05:02:02 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Wed, 11 May 2022 05:02:02 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Wed, 11 May 2022 05:02:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 05:02:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 05:02:03 GMT
EXPOSE 3306 33060
# Wed, 11 May 2022 05:02:03 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c32ce6654453d35d0b3dde45d195adeee586ffba0a683006ee06748c077c01fa`  
		Last Modified: Wed, 11 May 2022 01:25:58 GMT  
		Size: 27.1 MB (27140722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415d08ee031ab3bffe8c0db6b82f2cde88049eda62a50801eb6d8aa68bb0e12c`  
		Last Modified: Wed, 11 May 2022 05:03:03 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a38fec2542ffcfa6247f2992d1ec422b38e00ed5ca998bc5b890ca1a97ab1d5`  
		Last Modified: Wed, 11 May 2022 05:03:04 GMT  
		Size: 4.2 MB (4179283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352881ee8fe9b63edbd90eb3a1ffa035c72b7edfbcad6fda55db516c2a2b2cb9`  
		Last Modified: Wed, 11 May 2022 05:03:02 GMT  
		Size: 1.4 MB (1386677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8e20da291b6c92de4aa28a02fe8845045ec68d9b9ad1497e921fa42e8303650`  
		Last Modified: Wed, 11 May 2022 05:03:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66c2a8cc1999eedaa968d140339f25947e1faf8b3f2084c7eb5eee68455d6295`  
		Last Modified: Wed, 11 May 2022 05:03:03 GMT  
		Size: 14.1 MB (14064393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3a3a8e49878cc1f98a4927704e4fdc191bcc2cc80fbf7470b36fe1b44b7596d`  
		Last Modified: Wed, 11 May 2022 05:03:01 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e33a48832bec0e74023cbd16a908bc440f32f292f7db67c91de8114199145984`  
		Last Modified: Wed, 11 May 2022 05:02:58 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410b942b8b28385f3aa8f160e5cfa770f39b81c059e6842d17ac37a75aa573c5`  
		Last Modified: Wed, 11 May 2022 05:03:15 GMT  
		Size: 109.1 MB (109103697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5323c9dd265c14ee05d2fef4d1a2116eeb2199a40af1ffbd3895f282b7aac05`  
		Last Modified: Wed, 11 May 2022 05:02:59 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3212737f31c01d2dba54855d882345d6a94318af0d57906a89b76af8fd6e2463`  
		Last Modified: Wed, 11 May 2022 05:02:58 GMT  
		Size: 5.1 KB (5136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0032d4b0dc5586f10e64a531c0f7d2671ec571b3ad0fdfb200ad6ea974db9ae`  
		Last Modified: Wed, 11 May 2022 05:02:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8-debian`

```console
$ docker pull mysql@sha256:a0805d37d4d298bd61e0dfa61f0ddf6f4680b453fa25d7aad420485a62417eab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8-debian` - linux; amd64

```console
$ docker pull mysql@sha256:f8c1d78c6f134d3a99d451cd983399087de0faf376f350ebb47886c3d3a343e6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.9 MB (155885550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76152be684492598eb4fb366674a85c7ae222025d783525d548e607d0c0030f4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 11 May 2022 01:20:37 GMT
ADD file:76b454ddb7dfe4d22afae844a7e67e7e5fb4570dae2e21bbd259a1f2e5839f33 in / 
# Wed, 11 May 2022 01:20:37 GMT
CMD ["bash"]
# Wed, 11 May 2022 05:01:23 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 11 May 2022 05:01:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 05:01:29 GMT
ENV GOSU_VERSION=1.14
# Wed, 11 May 2022 05:01:38 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 11 May 2022 05:01:39 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 11 May 2022 05:01:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 05:01:46 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 11 May 2022 05:01:46 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 11 May 2022 05:01:46 GMT
ENV MYSQL_VERSION=8.0.29-1debian10
# Wed, 11 May 2022 05:01:47 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Wed, 11 May 2022 05:02:01 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 11 May 2022 05:02:02 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 May 2022 05:02:02 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Wed, 11 May 2022 05:02:02 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Wed, 11 May 2022 05:02:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 05:02:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 05:02:03 GMT
EXPOSE 3306 33060
# Wed, 11 May 2022 05:02:03 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c32ce6654453d35d0b3dde45d195adeee586ffba0a683006ee06748c077c01fa`  
		Last Modified: Wed, 11 May 2022 01:25:58 GMT  
		Size: 27.1 MB (27140722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415d08ee031ab3bffe8c0db6b82f2cde88049eda62a50801eb6d8aa68bb0e12c`  
		Last Modified: Wed, 11 May 2022 05:03:03 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a38fec2542ffcfa6247f2992d1ec422b38e00ed5ca998bc5b890ca1a97ab1d5`  
		Last Modified: Wed, 11 May 2022 05:03:04 GMT  
		Size: 4.2 MB (4179283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352881ee8fe9b63edbd90eb3a1ffa035c72b7edfbcad6fda55db516c2a2b2cb9`  
		Last Modified: Wed, 11 May 2022 05:03:02 GMT  
		Size: 1.4 MB (1386677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8e20da291b6c92de4aa28a02fe8845045ec68d9b9ad1497e921fa42e8303650`  
		Last Modified: Wed, 11 May 2022 05:03:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66c2a8cc1999eedaa968d140339f25947e1faf8b3f2084c7eb5eee68455d6295`  
		Last Modified: Wed, 11 May 2022 05:03:03 GMT  
		Size: 14.1 MB (14064393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3a3a8e49878cc1f98a4927704e4fdc191bcc2cc80fbf7470b36fe1b44b7596d`  
		Last Modified: Wed, 11 May 2022 05:03:01 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e33a48832bec0e74023cbd16a908bc440f32f292f7db67c91de8114199145984`  
		Last Modified: Wed, 11 May 2022 05:02:58 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410b942b8b28385f3aa8f160e5cfa770f39b81c059e6842d17ac37a75aa573c5`  
		Last Modified: Wed, 11 May 2022 05:03:15 GMT  
		Size: 109.1 MB (109103697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5323c9dd265c14ee05d2fef4d1a2116eeb2199a40af1ffbd3895f282b7aac05`  
		Last Modified: Wed, 11 May 2022 05:02:59 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3212737f31c01d2dba54855d882345d6a94318af0d57906a89b76af8fd6e2463`  
		Last Modified: Wed, 11 May 2022 05:02:58 GMT  
		Size: 5.1 KB (5136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0032d4b0dc5586f10e64a531c0f7d2671ec571b3ad0fdfb200ad6ea974db9ae`  
		Last Modified: Wed, 11 May 2022 05:02:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8-oracle`

```console
$ docker pull mysql@sha256:fc7cc18cbd47405471f57a6cf3ae44883fc3aecff8248c5318f18e1bbbf4c7d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:4029b0a406ed7ffbad0fc873f6395cd62642cc7e5d6ea3ce308829017d0a2208
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.8 MB (134822098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a7183f6f3be655d9b8f7f738edd3f499f504e2f3152dae2ca46e96a6f01fd98`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 02 May 2022 20:51:06 GMT
ADD file:b2c3e9f338a70507ba6d9ec21f28c7023f4120a45f234ff9a28188119091c60b in / 
# Mon, 02 May 2022 20:51:06 GMT
CMD ["/bin/bash"]
# Mon, 02 May 2022 21:25:41 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Mon, 02 May 2022 21:25:41 GMT
ENV GOSU_VERSION=1.14
# Mon, 02 May 2022 21:25:44 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 02 May 2022 21:26:03 GMT
RUN set -eux; 	microdnf install -y 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Mon, 02 May 2022 21:26:05 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Mon, 02 May 2022 21:26:05 GMT
ENV MYSQL_MAJOR=8.0
# Mon, 02 May 2022 21:26:05 GMT
ENV MYSQL_VERSION=8.0.29-1.el8
# Mon, 02 May 2022 21:26:05 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Mon, 02 May 2022 21:26:30 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Mon, 02 May 2022 21:26:31 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Mon, 02 May 2022 21:26:31 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el8
# Mon, 02 May 2022 21:26:59 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Mon, 02 May 2022 21:26:59 GMT
VOLUME [/var/lib/mysql]
# Mon, 02 May 2022 21:26:59 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Mon, 02 May 2022 21:26:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 May 2022 21:27:00 GMT
EXPOSE 3306 33060
# Mon, 02 May 2022 21:27:00 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:121b730bab02bd12143950d97a621f2d2dcf4723433bbadc2777d594c871ee71`  
		Last Modified: Mon, 02 May 2022 20:51:57 GMT  
		Size: 42.1 MB (42114330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e9e2a78afa6df23c55a53b92caf896d4fec5432a3c8d498bb39e295b44e5b67`  
		Last Modified: Mon, 02 May 2022 21:27:36 GMT  
		Size: 1.1 KB (1077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cffb51c633f075cebe9be73f4974c0b4a6185e655edb307b442048489f875f2`  
		Last Modified: Mon, 02 May 2022 21:27:34 GMT  
		Size: 928.8 KB (928833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b30efc1d40585868336a1299ad6aaae07a5cac0908f7dbb5436fdc3cbd4e83af`  
		Last Modified: Mon, 02 May 2022 21:27:34 GMT  
		Size: 4.6 MB (4557313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a4885b222a344a3de7796a9584ddf75df420828e2d2670dedff2dc1f4028c2`  
		Last Modified: Mon, 02 May 2022 21:27:33 GMT  
		Size: 2.6 KB (2627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de448cfca2e8ff2d6f4c8d6b5ee49cdfa1ae265f1f4edfa9bc833e3b44ee802d`  
		Last Modified: Mon, 02 May 2022 21:27:31 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3034ce8f4c19e81398b7257a015575b819a81cd0c3b7c68a4af9107ebb9602b8`  
		Last Modified: Mon, 02 May 2022 21:27:39 GMT  
		Size: 47.3 MB (47270489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2dbcaeba54f8c5b40833db3461dae5c1fa6e9b5237333280fdfc305b820899`  
		Last Modified: Mon, 02 May 2022 21:27:31 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a293a2607ec5d7c611e24d0257aa234870901ba5aa3bbf68c497675c143505a`  
		Last Modified: Mon, 02 May 2022 21:27:39 GMT  
		Size: 39.9 MB (39941638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:793ce953acec2a92a68b4677562f8db94d2079acd81c75404ae2457a707988cf`  
		Last Modified: Mon, 02 May 2022 21:27:31 GMT  
		Size: 5.1 KB (5143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:2bd5e5638a6669e3311baf198d538bf536e1f1b53af094442fa874e8997125ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.8 MB (142803022 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1eb4ca7381432c79f18435a1c7e727d3b25b210ffb12df85f595cb7a0510753`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 02 May 2022 21:46:34 GMT
ADD file:e59d0ab85f777209561c628874489b9544223a23fed0755bedd408a55452b4af in / 
# Mon, 02 May 2022 21:46:35 GMT
CMD ["/bin/bash"]
# Mon, 02 May 2022 22:02:55 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Mon, 02 May 2022 22:02:56 GMT
ENV GOSU_VERSION=1.14
# Mon, 02 May 2022 22:03:00 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 02 May 2022 22:03:20 GMT
RUN set -eux; 	microdnf install -y 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Mon, 02 May 2022 22:03:21 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Mon, 02 May 2022 22:03:22 GMT
ENV MYSQL_MAJOR=8.0
# Mon, 02 May 2022 22:03:23 GMT
ENV MYSQL_VERSION=8.0.29-1.el8
# Mon, 02 May 2022 22:03:24 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Mon, 02 May 2022 22:03:47 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Mon, 02 May 2022 22:03:47 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Mon, 02 May 2022 22:03:48 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el8
# Mon, 02 May 2022 22:04:20 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Mon, 02 May 2022 22:04:21 GMT
VOLUME [/var/lib/mysql]
# Mon, 02 May 2022 22:04:22 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Mon, 02 May 2022 22:04:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 May 2022 22:04:23 GMT
EXPOSE 3306 33060
# Mon, 02 May 2022 22:04:24 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2d35f3f87cf615a8684aa1b866b03a7078bce1beea91489effc1e6c03c83124c`  
		Last Modified: Mon, 02 May 2022 21:47:34 GMT  
		Size: 42.0 MB (42016620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08c104e7e4b73e841253b097a9d2ecf3b6b4052d0d5c6a0adb4cf9e075d429c`  
		Last Modified: Mon, 02 May 2022 22:04:53 GMT  
		Size: 1.0 KB (1014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a34eb48fc75c9042fd1b298591193aef6abe1011bf6d4f3459a86228e083bb3`  
		Last Modified: Mon, 02 May 2022 22:04:51 GMT  
		Size: 857.1 KB (857148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bb6dedbc752a6eb91186e7f395298b217e72267bef00a0cf60dc06556ea57c5`  
		Last Modified: Mon, 02 May 2022 22:04:51 GMT  
		Size: 4.4 MB (4360273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a4f2fda7b80e523ec1e635a622494eeced432bfffe325a8bd9a747ed266540`  
		Last Modified: Mon, 02 May 2022 22:04:50 GMT  
		Size: 2.6 KB (2607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff080c7a5faf34b8eb671ee5bd3aee9db12a10cefe82fdd2a5a39bff3520219`  
		Last Modified: Mon, 02 May 2022 22:04:48 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c984e7fd2f692c899aa76f205ff4762eed31a48b5bae4dabcac638f90de2ca0`  
		Last Modified: Mon, 02 May 2022 22:04:55 GMT  
		Size: 53.3 MB (53310133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57b567fb3d572dbb33f0e8b12befb868eddc7534fc74b7f541f2bd993c208c09`  
		Last Modified: Mon, 02 May 2022 22:04:48 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbbd9d96c94e0c08c62e3372a5222046e9f4dc76a8177e4215baf7fae03c6a43`  
		Last Modified: Mon, 02 May 2022 22:04:56 GMT  
		Size: 42.2 MB (42249442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71907ccd70c599d8fb39b045c89bd656550ac92c63b42e1969e88743570a7ecd`  
		Last Modified: Mon, 02 May 2022 22:04:48 GMT  
		Size: 5.1 KB (5134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0`

```console
$ docker pull mysql@sha256:a0805d37d4d298bd61e0dfa61f0ddf6f4680b453fa25d7aad420485a62417eab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0` - linux; amd64

```console
$ docker pull mysql@sha256:f8c1d78c6f134d3a99d451cd983399087de0faf376f350ebb47886c3d3a343e6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.9 MB (155885550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76152be684492598eb4fb366674a85c7ae222025d783525d548e607d0c0030f4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 11 May 2022 01:20:37 GMT
ADD file:76b454ddb7dfe4d22afae844a7e67e7e5fb4570dae2e21bbd259a1f2e5839f33 in / 
# Wed, 11 May 2022 01:20:37 GMT
CMD ["bash"]
# Wed, 11 May 2022 05:01:23 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 11 May 2022 05:01:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 05:01:29 GMT
ENV GOSU_VERSION=1.14
# Wed, 11 May 2022 05:01:38 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 11 May 2022 05:01:39 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 11 May 2022 05:01:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 05:01:46 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 11 May 2022 05:01:46 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 11 May 2022 05:01:46 GMT
ENV MYSQL_VERSION=8.0.29-1debian10
# Wed, 11 May 2022 05:01:47 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Wed, 11 May 2022 05:02:01 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 11 May 2022 05:02:02 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 May 2022 05:02:02 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Wed, 11 May 2022 05:02:02 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Wed, 11 May 2022 05:02:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 05:02:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 05:02:03 GMT
EXPOSE 3306 33060
# Wed, 11 May 2022 05:02:03 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c32ce6654453d35d0b3dde45d195adeee586ffba0a683006ee06748c077c01fa`  
		Last Modified: Wed, 11 May 2022 01:25:58 GMT  
		Size: 27.1 MB (27140722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415d08ee031ab3bffe8c0db6b82f2cde88049eda62a50801eb6d8aa68bb0e12c`  
		Last Modified: Wed, 11 May 2022 05:03:03 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a38fec2542ffcfa6247f2992d1ec422b38e00ed5ca998bc5b890ca1a97ab1d5`  
		Last Modified: Wed, 11 May 2022 05:03:04 GMT  
		Size: 4.2 MB (4179283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352881ee8fe9b63edbd90eb3a1ffa035c72b7edfbcad6fda55db516c2a2b2cb9`  
		Last Modified: Wed, 11 May 2022 05:03:02 GMT  
		Size: 1.4 MB (1386677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8e20da291b6c92de4aa28a02fe8845045ec68d9b9ad1497e921fa42e8303650`  
		Last Modified: Wed, 11 May 2022 05:03:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66c2a8cc1999eedaa968d140339f25947e1faf8b3f2084c7eb5eee68455d6295`  
		Last Modified: Wed, 11 May 2022 05:03:03 GMT  
		Size: 14.1 MB (14064393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3a3a8e49878cc1f98a4927704e4fdc191bcc2cc80fbf7470b36fe1b44b7596d`  
		Last Modified: Wed, 11 May 2022 05:03:01 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e33a48832bec0e74023cbd16a908bc440f32f292f7db67c91de8114199145984`  
		Last Modified: Wed, 11 May 2022 05:02:58 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410b942b8b28385f3aa8f160e5cfa770f39b81c059e6842d17ac37a75aa573c5`  
		Last Modified: Wed, 11 May 2022 05:03:15 GMT  
		Size: 109.1 MB (109103697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5323c9dd265c14ee05d2fef4d1a2116eeb2199a40af1ffbd3895f282b7aac05`  
		Last Modified: Wed, 11 May 2022 05:02:59 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3212737f31c01d2dba54855d882345d6a94318af0d57906a89b76af8fd6e2463`  
		Last Modified: Wed, 11 May 2022 05:02:58 GMT  
		Size: 5.1 KB (5136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0032d4b0dc5586f10e64a531c0f7d2671ec571b3ad0fdfb200ad6ea974db9ae`  
		Last Modified: Wed, 11 May 2022 05:02:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0-debian`

```console
$ docker pull mysql@sha256:a0805d37d4d298bd61e0dfa61f0ddf6f4680b453fa25d7aad420485a62417eab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0-debian` - linux; amd64

```console
$ docker pull mysql@sha256:f8c1d78c6f134d3a99d451cd983399087de0faf376f350ebb47886c3d3a343e6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.9 MB (155885550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76152be684492598eb4fb366674a85c7ae222025d783525d548e607d0c0030f4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 11 May 2022 01:20:37 GMT
ADD file:76b454ddb7dfe4d22afae844a7e67e7e5fb4570dae2e21bbd259a1f2e5839f33 in / 
# Wed, 11 May 2022 01:20:37 GMT
CMD ["bash"]
# Wed, 11 May 2022 05:01:23 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 11 May 2022 05:01:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 05:01:29 GMT
ENV GOSU_VERSION=1.14
# Wed, 11 May 2022 05:01:38 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 11 May 2022 05:01:39 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 11 May 2022 05:01:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 05:01:46 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 11 May 2022 05:01:46 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 11 May 2022 05:01:46 GMT
ENV MYSQL_VERSION=8.0.29-1debian10
# Wed, 11 May 2022 05:01:47 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Wed, 11 May 2022 05:02:01 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 11 May 2022 05:02:02 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 May 2022 05:02:02 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Wed, 11 May 2022 05:02:02 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Wed, 11 May 2022 05:02:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 05:02:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 05:02:03 GMT
EXPOSE 3306 33060
# Wed, 11 May 2022 05:02:03 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c32ce6654453d35d0b3dde45d195adeee586ffba0a683006ee06748c077c01fa`  
		Last Modified: Wed, 11 May 2022 01:25:58 GMT  
		Size: 27.1 MB (27140722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415d08ee031ab3bffe8c0db6b82f2cde88049eda62a50801eb6d8aa68bb0e12c`  
		Last Modified: Wed, 11 May 2022 05:03:03 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a38fec2542ffcfa6247f2992d1ec422b38e00ed5ca998bc5b890ca1a97ab1d5`  
		Last Modified: Wed, 11 May 2022 05:03:04 GMT  
		Size: 4.2 MB (4179283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352881ee8fe9b63edbd90eb3a1ffa035c72b7edfbcad6fda55db516c2a2b2cb9`  
		Last Modified: Wed, 11 May 2022 05:03:02 GMT  
		Size: 1.4 MB (1386677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8e20da291b6c92de4aa28a02fe8845045ec68d9b9ad1497e921fa42e8303650`  
		Last Modified: Wed, 11 May 2022 05:03:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66c2a8cc1999eedaa968d140339f25947e1faf8b3f2084c7eb5eee68455d6295`  
		Last Modified: Wed, 11 May 2022 05:03:03 GMT  
		Size: 14.1 MB (14064393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3a3a8e49878cc1f98a4927704e4fdc191bcc2cc80fbf7470b36fe1b44b7596d`  
		Last Modified: Wed, 11 May 2022 05:03:01 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e33a48832bec0e74023cbd16a908bc440f32f292f7db67c91de8114199145984`  
		Last Modified: Wed, 11 May 2022 05:02:58 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410b942b8b28385f3aa8f160e5cfa770f39b81c059e6842d17ac37a75aa573c5`  
		Last Modified: Wed, 11 May 2022 05:03:15 GMT  
		Size: 109.1 MB (109103697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5323c9dd265c14ee05d2fef4d1a2116eeb2199a40af1ffbd3895f282b7aac05`  
		Last Modified: Wed, 11 May 2022 05:02:59 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3212737f31c01d2dba54855d882345d6a94318af0d57906a89b76af8fd6e2463`  
		Last Modified: Wed, 11 May 2022 05:02:58 GMT  
		Size: 5.1 KB (5136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0032d4b0dc5586f10e64a531c0f7d2671ec571b3ad0fdfb200ad6ea974db9ae`  
		Last Modified: Wed, 11 May 2022 05:02:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0-oracle`

```console
$ docker pull mysql@sha256:fc7cc18cbd47405471f57a6cf3ae44883fc3aecff8248c5318f18e1bbbf4c7d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:4029b0a406ed7ffbad0fc873f6395cd62642cc7e5d6ea3ce308829017d0a2208
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.8 MB (134822098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a7183f6f3be655d9b8f7f738edd3f499f504e2f3152dae2ca46e96a6f01fd98`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 02 May 2022 20:51:06 GMT
ADD file:b2c3e9f338a70507ba6d9ec21f28c7023f4120a45f234ff9a28188119091c60b in / 
# Mon, 02 May 2022 20:51:06 GMT
CMD ["/bin/bash"]
# Mon, 02 May 2022 21:25:41 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Mon, 02 May 2022 21:25:41 GMT
ENV GOSU_VERSION=1.14
# Mon, 02 May 2022 21:25:44 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 02 May 2022 21:26:03 GMT
RUN set -eux; 	microdnf install -y 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Mon, 02 May 2022 21:26:05 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Mon, 02 May 2022 21:26:05 GMT
ENV MYSQL_MAJOR=8.0
# Mon, 02 May 2022 21:26:05 GMT
ENV MYSQL_VERSION=8.0.29-1.el8
# Mon, 02 May 2022 21:26:05 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Mon, 02 May 2022 21:26:30 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Mon, 02 May 2022 21:26:31 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Mon, 02 May 2022 21:26:31 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el8
# Mon, 02 May 2022 21:26:59 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Mon, 02 May 2022 21:26:59 GMT
VOLUME [/var/lib/mysql]
# Mon, 02 May 2022 21:26:59 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Mon, 02 May 2022 21:26:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 May 2022 21:27:00 GMT
EXPOSE 3306 33060
# Mon, 02 May 2022 21:27:00 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:121b730bab02bd12143950d97a621f2d2dcf4723433bbadc2777d594c871ee71`  
		Last Modified: Mon, 02 May 2022 20:51:57 GMT  
		Size: 42.1 MB (42114330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e9e2a78afa6df23c55a53b92caf896d4fec5432a3c8d498bb39e295b44e5b67`  
		Last Modified: Mon, 02 May 2022 21:27:36 GMT  
		Size: 1.1 KB (1077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cffb51c633f075cebe9be73f4974c0b4a6185e655edb307b442048489f875f2`  
		Last Modified: Mon, 02 May 2022 21:27:34 GMT  
		Size: 928.8 KB (928833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b30efc1d40585868336a1299ad6aaae07a5cac0908f7dbb5436fdc3cbd4e83af`  
		Last Modified: Mon, 02 May 2022 21:27:34 GMT  
		Size: 4.6 MB (4557313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a4885b222a344a3de7796a9584ddf75df420828e2d2670dedff2dc1f4028c2`  
		Last Modified: Mon, 02 May 2022 21:27:33 GMT  
		Size: 2.6 KB (2627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de448cfca2e8ff2d6f4c8d6b5ee49cdfa1ae265f1f4edfa9bc833e3b44ee802d`  
		Last Modified: Mon, 02 May 2022 21:27:31 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3034ce8f4c19e81398b7257a015575b819a81cd0c3b7c68a4af9107ebb9602b8`  
		Last Modified: Mon, 02 May 2022 21:27:39 GMT  
		Size: 47.3 MB (47270489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2dbcaeba54f8c5b40833db3461dae5c1fa6e9b5237333280fdfc305b820899`  
		Last Modified: Mon, 02 May 2022 21:27:31 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a293a2607ec5d7c611e24d0257aa234870901ba5aa3bbf68c497675c143505a`  
		Last Modified: Mon, 02 May 2022 21:27:39 GMT  
		Size: 39.9 MB (39941638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:793ce953acec2a92a68b4677562f8db94d2079acd81c75404ae2457a707988cf`  
		Last Modified: Mon, 02 May 2022 21:27:31 GMT  
		Size: 5.1 KB (5143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:2bd5e5638a6669e3311baf198d538bf536e1f1b53af094442fa874e8997125ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.8 MB (142803022 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1eb4ca7381432c79f18435a1c7e727d3b25b210ffb12df85f595cb7a0510753`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 02 May 2022 21:46:34 GMT
ADD file:e59d0ab85f777209561c628874489b9544223a23fed0755bedd408a55452b4af in / 
# Mon, 02 May 2022 21:46:35 GMT
CMD ["/bin/bash"]
# Mon, 02 May 2022 22:02:55 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Mon, 02 May 2022 22:02:56 GMT
ENV GOSU_VERSION=1.14
# Mon, 02 May 2022 22:03:00 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 02 May 2022 22:03:20 GMT
RUN set -eux; 	microdnf install -y 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Mon, 02 May 2022 22:03:21 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Mon, 02 May 2022 22:03:22 GMT
ENV MYSQL_MAJOR=8.0
# Mon, 02 May 2022 22:03:23 GMT
ENV MYSQL_VERSION=8.0.29-1.el8
# Mon, 02 May 2022 22:03:24 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Mon, 02 May 2022 22:03:47 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Mon, 02 May 2022 22:03:47 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Mon, 02 May 2022 22:03:48 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el8
# Mon, 02 May 2022 22:04:20 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Mon, 02 May 2022 22:04:21 GMT
VOLUME [/var/lib/mysql]
# Mon, 02 May 2022 22:04:22 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Mon, 02 May 2022 22:04:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 May 2022 22:04:23 GMT
EXPOSE 3306 33060
# Mon, 02 May 2022 22:04:24 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2d35f3f87cf615a8684aa1b866b03a7078bce1beea91489effc1e6c03c83124c`  
		Last Modified: Mon, 02 May 2022 21:47:34 GMT  
		Size: 42.0 MB (42016620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08c104e7e4b73e841253b097a9d2ecf3b6b4052d0d5c6a0adb4cf9e075d429c`  
		Last Modified: Mon, 02 May 2022 22:04:53 GMT  
		Size: 1.0 KB (1014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a34eb48fc75c9042fd1b298591193aef6abe1011bf6d4f3459a86228e083bb3`  
		Last Modified: Mon, 02 May 2022 22:04:51 GMT  
		Size: 857.1 KB (857148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bb6dedbc752a6eb91186e7f395298b217e72267bef00a0cf60dc06556ea57c5`  
		Last Modified: Mon, 02 May 2022 22:04:51 GMT  
		Size: 4.4 MB (4360273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a4f2fda7b80e523ec1e635a622494eeced432bfffe325a8bd9a747ed266540`  
		Last Modified: Mon, 02 May 2022 22:04:50 GMT  
		Size: 2.6 KB (2607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff080c7a5faf34b8eb671ee5bd3aee9db12a10cefe82fdd2a5a39bff3520219`  
		Last Modified: Mon, 02 May 2022 22:04:48 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c984e7fd2f692c899aa76f205ff4762eed31a48b5bae4dabcac638f90de2ca0`  
		Last Modified: Mon, 02 May 2022 22:04:55 GMT  
		Size: 53.3 MB (53310133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57b567fb3d572dbb33f0e8b12befb868eddc7534fc74b7f541f2bd993c208c09`  
		Last Modified: Mon, 02 May 2022 22:04:48 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbbd9d96c94e0c08c62e3372a5222046e9f4dc76a8177e4215baf7fae03c6a43`  
		Last Modified: Mon, 02 May 2022 22:04:56 GMT  
		Size: 42.2 MB (42249442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71907ccd70c599d8fb39b045c89bd656550ac92c63b42e1969e88743570a7ecd`  
		Last Modified: Mon, 02 May 2022 22:04:48 GMT  
		Size: 5.1 KB (5134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.29`

```console
$ docker pull mysql@sha256:a0805d37d4d298bd61e0dfa61f0ddf6f4680b453fa25d7aad420485a62417eab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0.29` - linux; amd64

```console
$ docker pull mysql@sha256:f8c1d78c6f134d3a99d451cd983399087de0faf376f350ebb47886c3d3a343e6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.9 MB (155885550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76152be684492598eb4fb366674a85c7ae222025d783525d548e607d0c0030f4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 11 May 2022 01:20:37 GMT
ADD file:76b454ddb7dfe4d22afae844a7e67e7e5fb4570dae2e21bbd259a1f2e5839f33 in / 
# Wed, 11 May 2022 01:20:37 GMT
CMD ["bash"]
# Wed, 11 May 2022 05:01:23 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 11 May 2022 05:01:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 05:01:29 GMT
ENV GOSU_VERSION=1.14
# Wed, 11 May 2022 05:01:38 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 11 May 2022 05:01:39 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 11 May 2022 05:01:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 05:01:46 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 11 May 2022 05:01:46 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 11 May 2022 05:01:46 GMT
ENV MYSQL_VERSION=8.0.29-1debian10
# Wed, 11 May 2022 05:01:47 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Wed, 11 May 2022 05:02:01 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 11 May 2022 05:02:02 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 May 2022 05:02:02 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Wed, 11 May 2022 05:02:02 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Wed, 11 May 2022 05:02:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 05:02:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 05:02:03 GMT
EXPOSE 3306 33060
# Wed, 11 May 2022 05:02:03 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c32ce6654453d35d0b3dde45d195adeee586ffba0a683006ee06748c077c01fa`  
		Last Modified: Wed, 11 May 2022 01:25:58 GMT  
		Size: 27.1 MB (27140722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415d08ee031ab3bffe8c0db6b82f2cde88049eda62a50801eb6d8aa68bb0e12c`  
		Last Modified: Wed, 11 May 2022 05:03:03 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a38fec2542ffcfa6247f2992d1ec422b38e00ed5ca998bc5b890ca1a97ab1d5`  
		Last Modified: Wed, 11 May 2022 05:03:04 GMT  
		Size: 4.2 MB (4179283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352881ee8fe9b63edbd90eb3a1ffa035c72b7edfbcad6fda55db516c2a2b2cb9`  
		Last Modified: Wed, 11 May 2022 05:03:02 GMT  
		Size: 1.4 MB (1386677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8e20da291b6c92de4aa28a02fe8845045ec68d9b9ad1497e921fa42e8303650`  
		Last Modified: Wed, 11 May 2022 05:03:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66c2a8cc1999eedaa968d140339f25947e1faf8b3f2084c7eb5eee68455d6295`  
		Last Modified: Wed, 11 May 2022 05:03:03 GMT  
		Size: 14.1 MB (14064393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3a3a8e49878cc1f98a4927704e4fdc191bcc2cc80fbf7470b36fe1b44b7596d`  
		Last Modified: Wed, 11 May 2022 05:03:01 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e33a48832bec0e74023cbd16a908bc440f32f292f7db67c91de8114199145984`  
		Last Modified: Wed, 11 May 2022 05:02:58 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410b942b8b28385f3aa8f160e5cfa770f39b81c059e6842d17ac37a75aa573c5`  
		Last Modified: Wed, 11 May 2022 05:03:15 GMT  
		Size: 109.1 MB (109103697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5323c9dd265c14ee05d2fef4d1a2116eeb2199a40af1ffbd3895f282b7aac05`  
		Last Modified: Wed, 11 May 2022 05:02:59 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3212737f31c01d2dba54855d882345d6a94318af0d57906a89b76af8fd6e2463`  
		Last Modified: Wed, 11 May 2022 05:02:58 GMT  
		Size: 5.1 KB (5136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0032d4b0dc5586f10e64a531c0f7d2671ec571b3ad0fdfb200ad6ea974db9ae`  
		Last Modified: Wed, 11 May 2022 05:02:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.29-debian`

```console
$ docker pull mysql@sha256:a0805d37d4d298bd61e0dfa61f0ddf6f4680b453fa25d7aad420485a62417eab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0.29-debian` - linux; amd64

```console
$ docker pull mysql@sha256:f8c1d78c6f134d3a99d451cd983399087de0faf376f350ebb47886c3d3a343e6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.9 MB (155885550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76152be684492598eb4fb366674a85c7ae222025d783525d548e607d0c0030f4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 11 May 2022 01:20:37 GMT
ADD file:76b454ddb7dfe4d22afae844a7e67e7e5fb4570dae2e21bbd259a1f2e5839f33 in / 
# Wed, 11 May 2022 01:20:37 GMT
CMD ["bash"]
# Wed, 11 May 2022 05:01:23 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 11 May 2022 05:01:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 05:01:29 GMT
ENV GOSU_VERSION=1.14
# Wed, 11 May 2022 05:01:38 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 11 May 2022 05:01:39 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 11 May 2022 05:01:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 05:01:46 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 11 May 2022 05:01:46 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 11 May 2022 05:01:46 GMT
ENV MYSQL_VERSION=8.0.29-1debian10
# Wed, 11 May 2022 05:01:47 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Wed, 11 May 2022 05:02:01 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 11 May 2022 05:02:02 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 May 2022 05:02:02 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Wed, 11 May 2022 05:02:02 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Wed, 11 May 2022 05:02:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 05:02:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 05:02:03 GMT
EXPOSE 3306 33060
# Wed, 11 May 2022 05:02:03 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c32ce6654453d35d0b3dde45d195adeee586ffba0a683006ee06748c077c01fa`  
		Last Modified: Wed, 11 May 2022 01:25:58 GMT  
		Size: 27.1 MB (27140722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415d08ee031ab3bffe8c0db6b82f2cde88049eda62a50801eb6d8aa68bb0e12c`  
		Last Modified: Wed, 11 May 2022 05:03:03 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a38fec2542ffcfa6247f2992d1ec422b38e00ed5ca998bc5b890ca1a97ab1d5`  
		Last Modified: Wed, 11 May 2022 05:03:04 GMT  
		Size: 4.2 MB (4179283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352881ee8fe9b63edbd90eb3a1ffa035c72b7edfbcad6fda55db516c2a2b2cb9`  
		Last Modified: Wed, 11 May 2022 05:03:02 GMT  
		Size: 1.4 MB (1386677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8e20da291b6c92de4aa28a02fe8845045ec68d9b9ad1497e921fa42e8303650`  
		Last Modified: Wed, 11 May 2022 05:03:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66c2a8cc1999eedaa968d140339f25947e1faf8b3f2084c7eb5eee68455d6295`  
		Last Modified: Wed, 11 May 2022 05:03:03 GMT  
		Size: 14.1 MB (14064393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3a3a8e49878cc1f98a4927704e4fdc191bcc2cc80fbf7470b36fe1b44b7596d`  
		Last Modified: Wed, 11 May 2022 05:03:01 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e33a48832bec0e74023cbd16a908bc440f32f292f7db67c91de8114199145984`  
		Last Modified: Wed, 11 May 2022 05:02:58 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410b942b8b28385f3aa8f160e5cfa770f39b81c059e6842d17ac37a75aa573c5`  
		Last Modified: Wed, 11 May 2022 05:03:15 GMT  
		Size: 109.1 MB (109103697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5323c9dd265c14ee05d2fef4d1a2116eeb2199a40af1ffbd3895f282b7aac05`  
		Last Modified: Wed, 11 May 2022 05:02:59 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3212737f31c01d2dba54855d882345d6a94318af0d57906a89b76af8fd6e2463`  
		Last Modified: Wed, 11 May 2022 05:02:58 GMT  
		Size: 5.1 KB (5136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0032d4b0dc5586f10e64a531c0f7d2671ec571b3ad0fdfb200ad6ea974db9ae`  
		Last Modified: Wed, 11 May 2022 05:02:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.29-oracle`

```console
$ docker pull mysql@sha256:fc7cc18cbd47405471f57a6cf3ae44883fc3aecff8248c5318f18e1bbbf4c7d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0.29-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:4029b0a406ed7ffbad0fc873f6395cd62642cc7e5d6ea3ce308829017d0a2208
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.8 MB (134822098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a7183f6f3be655d9b8f7f738edd3f499f504e2f3152dae2ca46e96a6f01fd98`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 02 May 2022 20:51:06 GMT
ADD file:b2c3e9f338a70507ba6d9ec21f28c7023f4120a45f234ff9a28188119091c60b in / 
# Mon, 02 May 2022 20:51:06 GMT
CMD ["/bin/bash"]
# Mon, 02 May 2022 21:25:41 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Mon, 02 May 2022 21:25:41 GMT
ENV GOSU_VERSION=1.14
# Mon, 02 May 2022 21:25:44 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 02 May 2022 21:26:03 GMT
RUN set -eux; 	microdnf install -y 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Mon, 02 May 2022 21:26:05 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Mon, 02 May 2022 21:26:05 GMT
ENV MYSQL_MAJOR=8.0
# Mon, 02 May 2022 21:26:05 GMT
ENV MYSQL_VERSION=8.0.29-1.el8
# Mon, 02 May 2022 21:26:05 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Mon, 02 May 2022 21:26:30 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Mon, 02 May 2022 21:26:31 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Mon, 02 May 2022 21:26:31 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el8
# Mon, 02 May 2022 21:26:59 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Mon, 02 May 2022 21:26:59 GMT
VOLUME [/var/lib/mysql]
# Mon, 02 May 2022 21:26:59 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Mon, 02 May 2022 21:26:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 May 2022 21:27:00 GMT
EXPOSE 3306 33060
# Mon, 02 May 2022 21:27:00 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:121b730bab02bd12143950d97a621f2d2dcf4723433bbadc2777d594c871ee71`  
		Last Modified: Mon, 02 May 2022 20:51:57 GMT  
		Size: 42.1 MB (42114330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e9e2a78afa6df23c55a53b92caf896d4fec5432a3c8d498bb39e295b44e5b67`  
		Last Modified: Mon, 02 May 2022 21:27:36 GMT  
		Size: 1.1 KB (1077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cffb51c633f075cebe9be73f4974c0b4a6185e655edb307b442048489f875f2`  
		Last Modified: Mon, 02 May 2022 21:27:34 GMT  
		Size: 928.8 KB (928833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b30efc1d40585868336a1299ad6aaae07a5cac0908f7dbb5436fdc3cbd4e83af`  
		Last Modified: Mon, 02 May 2022 21:27:34 GMT  
		Size: 4.6 MB (4557313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a4885b222a344a3de7796a9584ddf75df420828e2d2670dedff2dc1f4028c2`  
		Last Modified: Mon, 02 May 2022 21:27:33 GMT  
		Size: 2.6 KB (2627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de448cfca2e8ff2d6f4c8d6b5ee49cdfa1ae265f1f4edfa9bc833e3b44ee802d`  
		Last Modified: Mon, 02 May 2022 21:27:31 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3034ce8f4c19e81398b7257a015575b819a81cd0c3b7c68a4af9107ebb9602b8`  
		Last Modified: Mon, 02 May 2022 21:27:39 GMT  
		Size: 47.3 MB (47270489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2dbcaeba54f8c5b40833db3461dae5c1fa6e9b5237333280fdfc305b820899`  
		Last Modified: Mon, 02 May 2022 21:27:31 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a293a2607ec5d7c611e24d0257aa234870901ba5aa3bbf68c497675c143505a`  
		Last Modified: Mon, 02 May 2022 21:27:39 GMT  
		Size: 39.9 MB (39941638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:793ce953acec2a92a68b4677562f8db94d2079acd81c75404ae2457a707988cf`  
		Last Modified: Mon, 02 May 2022 21:27:31 GMT  
		Size: 5.1 KB (5143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0.29-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:2bd5e5638a6669e3311baf198d538bf536e1f1b53af094442fa874e8997125ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.8 MB (142803022 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1eb4ca7381432c79f18435a1c7e727d3b25b210ffb12df85f595cb7a0510753`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 02 May 2022 21:46:34 GMT
ADD file:e59d0ab85f777209561c628874489b9544223a23fed0755bedd408a55452b4af in / 
# Mon, 02 May 2022 21:46:35 GMT
CMD ["/bin/bash"]
# Mon, 02 May 2022 22:02:55 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Mon, 02 May 2022 22:02:56 GMT
ENV GOSU_VERSION=1.14
# Mon, 02 May 2022 22:03:00 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 02 May 2022 22:03:20 GMT
RUN set -eux; 	microdnf install -y 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Mon, 02 May 2022 22:03:21 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Mon, 02 May 2022 22:03:22 GMT
ENV MYSQL_MAJOR=8.0
# Mon, 02 May 2022 22:03:23 GMT
ENV MYSQL_VERSION=8.0.29-1.el8
# Mon, 02 May 2022 22:03:24 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Mon, 02 May 2022 22:03:47 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Mon, 02 May 2022 22:03:47 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Mon, 02 May 2022 22:03:48 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el8
# Mon, 02 May 2022 22:04:20 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Mon, 02 May 2022 22:04:21 GMT
VOLUME [/var/lib/mysql]
# Mon, 02 May 2022 22:04:22 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Mon, 02 May 2022 22:04:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 May 2022 22:04:23 GMT
EXPOSE 3306 33060
# Mon, 02 May 2022 22:04:24 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2d35f3f87cf615a8684aa1b866b03a7078bce1beea91489effc1e6c03c83124c`  
		Last Modified: Mon, 02 May 2022 21:47:34 GMT  
		Size: 42.0 MB (42016620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08c104e7e4b73e841253b097a9d2ecf3b6b4052d0d5c6a0adb4cf9e075d429c`  
		Last Modified: Mon, 02 May 2022 22:04:53 GMT  
		Size: 1.0 KB (1014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a34eb48fc75c9042fd1b298591193aef6abe1011bf6d4f3459a86228e083bb3`  
		Last Modified: Mon, 02 May 2022 22:04:51 GMT  
		Size: 857.1 KB (857148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bb6dedbc752a6eb91186e7f395298b217e72267bef00a0cf60dc06556ea57c5`  
		Last Modified: Mon, 02 May 2022 22:04:51 GMT  
		Size: 4.4 MB (4360273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a4f2fda7b80e523ec1e635a622494eeced432bfffe325a8bd9a747ed266540`  
		Last Modified: Mon, 02 May 2022 22:04:50 GMT  
		Size: 2.6 KB (2607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff080c7a5faf34b8eb671ee5bd3aee9db12a10cefe82fdd2a5a39bff3520219`  
		Last Modified: Mon, 02 May 2022 22:04:48 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c984e7fd2f692c899aa76f205ff4762eed31a48b5bae4dabcac638f90de2ca0`  
		Last Modified: Mon, 02 May 2022 22:04:55 GMT  
		Size: 53.3 MB (53310133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57b567fb3d572dbb33f0e8b12befb868eddc7534fc74b7f541f2bd993c208c09`  
		Last Modified: Mon, 02 May 2022 22:04:48 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbbd9d96c94e0c08c62e3372a5222046e9f4dc76a8177e4215baf7fae03c6a43`  
		Last Modified: Mon, 02 May 2022 22:04:56 GMT  
		Size: 42.2 MB (42249442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71907ccd70c599d8fb39b045c89bd656550ac92c63b42e1969e88743570a7ecd`  
		Last Modified: Mon, 02 May 2022 22:04:48 GMT  
		Size: 5.1 KB (5134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:debian`

```console
$ docker pull mysql@sha256:a0805d37d4d298bd61e0dfa61f0ddf6f4680b453fa25d7aad420485a62417eab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:debian` - linux; amd64

```console
$ docker pull mysql@sha256:f8c1d78c6f134d3a99d451cd983399087de0faf376f350ebb47886c3d3a343e6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.9 MB (155885550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76152be684492598eb4fb366674a85c7ae222025d783525d548e607d0c0030f4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 11 May 2022 01:20:37 GMT
ADD file:76b454ddb7dfe4d22afae844a7e67e7e5fb4570dae2e21bbd259a1f2e5839f33 in / 
# Wed, 11 May 2022 01:20:37 GMT
CMD ["bash"]
# Wed, 11 May 2022 05:01:23 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 11 May 2022 05:01:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 05:01:29 GMT
ENV GOSU_VERSION=1.14
# Wed, 11 May 2022 05:01:38 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 11 May 2022 05:01:39 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 11 May 2022 05:01:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 05:01:46 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 11 May 2022 05:01:46 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 11 May 2022 05:01:46 GMT
ENV MYSQL_VERSION=8.0.29-1debian10
# Wed, 11 May 2022 05:01:47 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Wed, 11 May 2022 05:02:01 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 11 May 2022 05:02:02 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 May 2022 05:02:02 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Wed, 11 May 2022 05:02:02 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Wed, 11 May 2022 05:02:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 05:02:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 05:02:03 GMT
EXPOSE 3306 33060
# Wed, 11 May 2022 05:02:03 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c32ce6654453d35d0b3dde45d195adeee586ffba0a683006ee06748c077c01fa`  
		Last Modified: Wed, 11 May 2022 01:25:58 GMT  
		Size: 27.1 MB (27140722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415d08ee031ab3bffe8c0db6b82f2cde88049eda62a50801eb6d8aa68bb0e12c`  
		Last Modified: Wed, 11 May 2022 05:03:03 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a38fec2542ffcfa6247f2992d1ec422b38e00ed5ca998bc5b890ca1a97ab1d5`  
		Last Modified: Wed, 11 May 2022 05:03:04 GMT  
		Size: 4.2 MB (4179283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352881ee8fe9b63edbd90eb3a1ffa035c72b7edfbcad6fda55db516c2a2b2cb9`  
		Last Modified: Wed, 11 May 2022 05:03:02 GMT  
		Size: 1.4 MB (1386677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8e20da291b6c92de4aa28a02fe8845045ec68d9b9ad1497e921fa42e8303650`  
		Last Modified: Wed, 11 May 2022 05:03:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66c2a8cc1999eedaa968d140339f25947e1faf8b3f2084c7eb5eee68455d6295`  
		Last Modified: Wed, 11 May 2022 05:03:03 GMT  
		Size: 14.1 MB (14064393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3a3a8e49878cc1f98a4927704e4fdc191bcc2cc80fbf7470b36fe1b44b7596d`  
		Last Modified: Wed, 11 May 2022 05:03:01 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e33a48832bec0e74023cbd16a908bc440f32f292f7db67c91de8114199145984`  
		Last Modified: Wed, 11 May 2022 05:02:58 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410b942b8b28385f3aa8f160e5cfa770f39b81c059e6842d17ac37a75aa573c5`  
		Last Modified: Wed, 11 May 2022 05:03:15 GMT  
		Size: 109.1 MB (109103697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5323c9dd265c14ee05d2fef4d1a2116eeb2199a40af1ffbd3895f282b7aac05`  
		Last Modified: Wed, 11 May 2022 05:02:59 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3212737f31c01d2dba54855d882345d6a94318af0d57906a89b76af8fd6e2463`  
		Last Modified: Wed, 11 May 2022 05:02:58 GMT  
		Size: 5.1 KB (5136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0032d4b0dc5586f10e64a531c0f7d2671ec571b3ad0fdfb200ad6ea974db9ae`  
		Last Modified: Wed, 11 May 2022 05:02:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:latest`

```console
$ docker pull mysql@sha256:a0805d37d4d298bd61e0dfa61f0ddf6f4680b453fa25d7aad420485a62417eab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:latest` - linux; amd64

```console
$ docker pull mysql@sha256:f8c1d78c6f134d3a99d451cd983399087de0faf376f350ebb47886c3d3a343e6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.9 MB (155885550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76152be684492598eb4fb366674a85c7ae222025d783525d548e607d0c0030f4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 11 May 2022 01:20:37 GMT
ADD file:76b454ddb7dfe4d22afae844a7e67e7e5fb4570dae2e21bbd259a1f2e5839f33 in / 
# Wed, 11 May 2022 01:20:37 GMT
CMD ["bash"]
# Wed, 11 May 2022 05:01:23 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 11 May 2022 05:01:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 05:01:29 GMT
ENV GOSU_VERSION=1.14
# Wed, 11 May 2022 05:01:38 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 11 May 2022 05:01:39 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 11 May 2022 05:01:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 05:01:46 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 11 May 2022 05:01:46 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 11 May 2022 05:01:46 GMT
ENV MYSQL_VERSION=8.0.29-1debian10
# Wed, 11 May 2022 05:01:47 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Wed, 11 May 2022 05:02:01 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 11 May 2022 05:02:02 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 May 2022 05:02:02 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Wed, 11 May 2022 05:02:02 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Wed, 11 May 2022 05:02:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 05:02:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 05:02:03 GMT
EXPOSE 3306 33060
# Wed, 11 May 2022 05:02:03 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c32ce6654453d35d0b3dde45d195adeee586ffba0a683006ee06748c077c01fa`  
		Last Modified: Wed, 11 May 2022 01:25:58 GMT  
		Size: 27.1 MB (27140722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415d08ee031ab3bffe8c0db6b82f2cde88049eda62a50801eb6d8aa68bb0e12c`  
		Last Modified: Wed, 11 May 2022 05:03:03 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a38fec2542ffcfa6247f2992d1ec422b38e00ed5ca998bc5b890ca1a97ab1d5`  
		Last Modified: Wed, 11 May 2022 05:03:04 GMT  
		Size: 4.2 MB (4179283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352881ee8fe9b63edbd90eb3a1ffa035c72b7edfbcad6fda55db516c2a2b2cb9`  
		Last Modified: Wed, 11 May 2022 05:03:02 GMT  
		Size: 1.4 MB (1386677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8e20da291b6c92de4aa28a02fe8845045ec68d9b9ad1497e921fa42e8303650`  
		Last Modified: Wed, 11 May 2022 05:03:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66c2a8cc1999eedaa968d140339f25947e1faf8b3f2084c7eb5eee68455d6295`  
		Last Modified: Wed, 11 May 2022 05:03:03 GMT  
		Size: 14.1 MB (14064393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3a3a8e49878cc1f98a4927704e4fdc191bcc2cc80fbf7470b36fe1b44b7596d`  
		Last Modified: Wed, 11 May 2022 05:03:01 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e33a48832bec0e74023cbd16a908bc440f32f292f7db67c91de8114199145984`  
		Last Modified: Wed, 11 May 2022 05:02:58 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410b942b8b28385f3aa8f160e5cfa770f39b81c059e6842d17ac37a75aa573c5`  
		Last Modified: Wed, 11 May 2022 05:03:15 GMT  
		Size: 109.1 MB (109103697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5323c9dd265c14ee05d2fef4d1a2116eeb2199a40af1ffbd3895f282b7aac05`  
		Last Modified: Wed, 11 May 2022 05:02:59 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3212737f31c01d2dba54855d882345d6a94318af0d57906a89b76af8fd6e2463`  
		Last Modified: Wed, 11 May 2022 05:02:58 GMT  
		Size: 5.1 KB (5136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0032d4b0dc5586f10e64a531c0f7d2671ec571b3ad0fdfb200ad6ea974db9ae`  
		Last Modified: Wed, 11 May 2022 05:02:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:oracle`

```console
$ docker pull mysql@sha256:fc7cc18cbd47405471f57a6cf3ae44883fc3aecff8248c5318f18e1bbbf4c7d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:oracle` - linux; amd64

```console
$ docker pull mysql@sha256:4029b0a406ed7ffbad0fc873f6395cd62642cc7e5d6ea3ce308829017d0a2208
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.8 MB (134822098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a7183f6f3be655d9b8f7f738edd3f499f504e2f3152dae2ca46e96a6f01fd98`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 02 May 2022 20:51:06 GMT
ADD file:b2c3e9f338a70507ba6d9ec21f28c7023f4120a45f234ff9a28188119091c60b in / 
# Mon, 02 May 2022 20:51:06 GMT
CMD ["/bin/bash"]
# Mon, 02 May 2022 21:25:41 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Mon, 02 May 2022 21:25:41 GMT
ENV GOSU_VERSION=1.14
# Mon, 02 May 2022 21:25:44 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 02 May 2022 21:26:03 GMT
RUN set -eux; 	microdnf install -y 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Mon, 02 May 2022 21:26:05 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Mon, 02 May 2022 21:26:05 GMT
ENV MYSQL_MAJOR=8.0
# Mon, 02 May 2022 21:26:05 GMT
ENV MYSQL_VERSION=8.0.29-1.el8
# Mon, 02 May 2022 21:26:05 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Mon, 02 May 2022 21:26:30 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Mon, 02 May 2022 21:26:31 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Mon, 02 May 2022 21:26:31 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el8
# Mon, 02 May 2022 21:26:59 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Mon, 02 May 2022 21:26:59 GMT
VOLUME [/var/lib/mysql]
# Mon, 02 May 2022 21:26:59 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Mon, 02 May 2022 21:26:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 May 2022 21:27:00 GMT
EXPOSE 3306 33060
# Mon, 02 May 2022 21:27:00 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:121b730bab02bd12143950d97a621f2d2dcf4723433bbadc2777d594c871ee71`  
		Last Modified: Mon, 02 May 2022 20:51:57 GMT  
		Size: 42.1 MB (42114330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e9e2a78afa6df23c55a53b92caf896d4fec5432a3c8d498bb39e295b44e5b67`  
		Last Modified: Mon, 02 May 2022 21:27:36 GMT  
		Size: 1.1 KB (1077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cffb51c633f075cebe9be73f4974c0b4a6185e655edb307b442048489f875f2`  
		Last Modified: Mon, 02 May 2022 21:27:34 GMT  
		Size: 928.8 KB (928833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b30efc1d40585868336a1299ad6aaae07a5cac0908f7dbb5436fdc3cbd4e83af`  
		Last Modified: Mon, 02 May 2022 21:27:34 GMT  
		Size: 4.6 MB (4557313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a4885b222a344a3de7796a9584ddf75df420828e2d2670dedff2dc1f4028c2`  
		Last Modified: Mon, 02 May 2022 21:27:33 GMT  
		Size: 2.6 KB (2627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de448cfca2e8ff2d6f4c8d6b5ee49cdfa1ae265f1f4edfa9bc833e3b44ee802d`  
		Last Modified: Mon, 02 May 2022 21:27:31 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3034ce8f4c19e81398b7257a015575b819a81cd0c3b7c68a4af9107ebb9602b8`  
		Last Modified: Mon, 02 May 2022 21:27:39 GMT  
		Size: 47.3 MB (47270489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2dbcaeba54f8c5b40833db3461dae5c1fa6e9b5237333280fdfc305b820899`  
		Last Modified: Mon, 02 May 2022 21:27:31 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a293a2607ec5d7c611e24d0257aa234870901ba5aa3bbf68c497675c143505a`  
		Last Modified: Mon, 02 May 2022 21:27:39 GMT  
		Size: 39.9 MB (39941638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:793ce953acec2a92a68b4677562f8db94d2079acd81c75404ae2457a707988cf`  
		Last Modified: Mon, 02 May 2022 21:27:31 GMT  
		Size: 5.1 KB (5143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:2bd5e5638a6669e3311baf198d538bf536e1f1b53af094442fa874e8997125ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.8 MB (142803022 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1eb4ca7381432c79f18435a1c7e727d3b25b210ffb12df85f595cb7a0510753`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 02 May 2022 21:46:34 GMT
ADD file:e59d0ab85f777209561c628874489b9544223a23fed0755bedd408a55452b4af in / 
# Mon, 02 May 2022 21:46:35 GMT
CMD ["/bin/bash"]
# Mon, 02 May 2022 22:02:55 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Mon, 02 May 2022 22:02:56 GMT
ENV GOSU_VERSION=1.14
# Mon, 02 May 2022 22:03:00 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 02 May 2022 22:03:20 GMT
RUN set -eux; 	microdnf install -y 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Mon, 02 May 2022 22:03:21 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Mon, 02 May 2022 22:03:22 GMT
ENV MYSQL_MAJOR=8.0
# Mon, 02 May 2022 22:03:23 GMT
ENV MYSQL_VERSION=8.0.29-1.el8
# Mon, 02 May 2022 22:03:24 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Mon, 02 May 2022 22:03:47 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Mon, 02 May 2022 22:03:47 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Mon, 02 May 2022 22:03:48 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el8
# Mon, 02 May 2022 22:04:20 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Mon, 02 May 2022 22:04:21 GMT
VOLUME [/var/lib/mysql]
# Mon, 02 May 2022 22:04:22 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Mon, 02 May 2022 22:04:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 May 2022 22:04:23 GMT
EXPOSE 3306 33060
# Mon, 02 May 2022 22:04:24 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2d35f3f87cf615a8684aa1b866b03a7078bce1beea91489effc1e6c03c83124c`  
		Last Modified: Mon, 02 May 2022 21:47:34 GMT  
		Size: 42.0 MB (42016620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08c104e7e4b73e841253b097a9d2ecf3b6b4052d0d5c6a0adb4cf9e075d429c`  
		Last Modified: Mon, 02 May 2022 22:04:53 GMT  
		Size: 1.0 KB (1014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a34eb48fc75c9042fd1b298591193aef6abe1011bf6d4f3459a86228e083bb3`  
		Last Modified: Mon, 02 May 2022 22:04:51 GMT  
		Size: 857.1 KB (857148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bb6dedbc752a6eb91186e7f395298b217e72267bef00a0cf60dc06556ea57c5`  
		Last Modified: Mon, 02 May 2022 22:04:51 GMT  
		Size: 4.4 MB (4360273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a4f2fda7b80e523ec1e635a622494eeced432bfffe325a8bd9a747ed266540`  
		Last Modified: Mon, 02 May 2022 22:04:50 GMT  
		Size: 2.6 KB (2607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff080c7a5faf34b8eb671ee5bd3aee9db12a10cefe82fdd2a5a39bff3520219`  
		Last Modified: Mon, 02 May 2022 22:04:48 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c984e7fd2f692c899aa76f205ff4762eed31a48b5bae4dabcac638f90de2ca0`  
		Last Modified: Mon, 02 May 2022 22:04:55 GMT  
		Size: 53.3 MB (53310133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57b567fb3d572dbb33f0e8b12befb868eddc7534fc74b7f541f2bd993c208c09`  
		Last Modified: Mon, 02 May 2022 22:04:48 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbbd9d96c94e0c08c62e3372a5222046e9f4dc76a8177e4215baf7fae03c6a43`  
		Last Modified: Mon, 02 May 2022 22:04:56 GMT  
		Size: 42.2 MB (42249442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71907ccd70c599d8fb39b045c89bd656550ac92c63b42e1969e88743570a7ecd`  
		Last Modified: Mon, 02 May 2022 22:04:48 GMT  
		Size: 5.1 KB (5134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
