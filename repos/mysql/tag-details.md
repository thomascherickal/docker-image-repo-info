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
$ docker pull mysql@sha256:0e5a4f3064c00a4b0a5ca90ad1aa805837f52633242b8c168d67607d207165b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:4d5e8763440bd8c7af3c68132796e201a8297d4d77df2c978e96c51678cb2c4f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.9 MB (126910013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23eb9a154db6b6e6b0ba7c0a0f656d5741f848b3d2ac66af2bf6113d5ba1d209`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 12 May 2022 20:58:56 GMT
ADD file:8ac79c33c3bdf8a0a1c23cc009fabc3ead9d97891d701ad21090a6bc542521e2 in / 
# Thu, 12 May 2022 20:58:56 GMT
CMD ["/bin/bash"]
# Thu, 12 May 2022 22:39:33 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Thu, 12 May 2022 22:39:33 GMT
ENV GOSU_VERSION=1.14
# Thu, 12 May 2022 22:39:36 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 12 May 2022 22:39:46 GMT
RUN set -eux; 	yum install -y 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Thu, 12 May 2022 22:39:48 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 12 May 2022 22:39:48 GMT
ENV MYSQL_MAJOR=5.7
# Thu, 12 May 2022 22:39:48 GMT
ENV MYSQL_VERSION=5.7.38-1.el7
# Thu, 12 May 2022 22:39:48 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Thu, 12 May 2022 22:40:02 GMT
RUN set -eux; 	yum install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Thu, 12 May 2022 22:40:03 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Thu, 12 May 2022 22:40:03 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el7
# Thu, 12 May 2022 22:40:21 GMT
RUN set -eux; 	yum install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Thu, 12 May 2022 22:40:21 GMT
VOLUME [/var/lib/mysql]
# Thu, 12 May 2022 22:40:22 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Thu, 12 May 2022 22:40:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 May 2022 22:40:22 GMT
EXPOSE 3306 33060
# Thu, 12 May 2022 22:40:22 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:cd32cd816e68367704ec22e6e4d27af6a08b27e32aca3d0bd7a47424e37d0b91`  
		Last Modified: Thu, 12 May 2022 20:59:41 GMT  
		Size: 48.8 MB (48758049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac1cac655dec3bbc6c5dd2efa9156e4798ca4cbb99f1311853f490d7092ba3ad`  
		Last Modified: Thu, 12 May 2022 22:41:03 GMT  
		Size: 1.1 KB (1061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882efd5b0b9e419c5b8707b94c9916f62f166a427c37954da0aefc0f7c744ca0`  
		Last Modified: Thu, 12 May 2022 22:41:00 GMT  
		Size: 930.2 KB (930225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8424ed51a7a3d46b24a5876e22e1d42a033170139757b9b003be5da80d6c33a8`  
		Last Modified: Thu, 12 May 2022 22:41:01 GMT  
		Size: 3.8 MB (3761150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edd7d8c8b2c6eb0293ce188c4627a483f57d6c6cd1409bee035ee58fbcd39f41`  
		Last Modified: Thu, 12 May 2022 22:40:59 GMT  
		Size: 2.7 KB (2658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d485f7c40504fc4261d3b5cb62305b4f41a0507cb46e11c2c54b65a2ca6d39`  
		Last Modified: Thu, 12 May 2022 22:40:57 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15656ef8b782ab3e6234de4f2c4854115373be8ab28b59f9f014dbff120037af`  
		Last Modified: Thu, 12 May 2022 22:41:01 GMT  
		Size: 25.5 MB (25476162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3786d73cb960fecd724e6bcf500defd0e02cf03a7869863adb65266d025b909e`  
		Last Modified: Thu, 12 May 2022 22:40:57 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a3f7291494d2e057d61cfdeff9c32d944d87bcc349fe31f2a79bf85be661461`  
		Last Modified: Thu, 12 May 2022 22:41:06 GMT  
		Size: 48.0 MB (47974917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2399c35146d1646f6f535235dfce69c437e13576fa19a283fdb340323b36fdfe`  
		Last Modified: Thu, 12 May 2022 22:40:57 GMT  
		Size: 5.1 KB (5139 bytes)  
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
$ docker pull mysql@sha256:0e5a4f3064c00a4b0a5ca90ad1aa805837f52633242b8c168d67607d207165b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:4d5e8763440bd8c7af3c68132796e201a8297d4d77df2c978e96c51678cb2c4f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.9 MB (126910013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23eb9a154db6b6e6b0ba7c0a0f656d5741f848b3d2ac66af2bf6113d5ba1d209`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 12 May 2022 20:58:56 GMT
ADD file:8ac79c33c3bdf8a0a1c23cc009fabc3ead9d97891d701ad21090a6bc542521e2 in / 
# Thu, 12 May 2022 20:58:56 GMT
CMD ["/bin/bash"]
# Thu, 12 May 2022 22:39:33 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Thu, 12 May 2022 22:39:33 GMT
ENV GOSU_VERSION=1.14
# Thu, 12 May 2022 22:39:36 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 12 May 2022 22:39:46 GMT
RUN set -eux; 	yum install -y 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Thu, 12 May 2022 22:39:48 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 12 May 2022 22:39:48 GMT
ENV MYSQL_MAJOR=5.7
# Thu, 12 May 2022 22:39:48 GMT
ENV MYSQL_VERSION=5.7.38-1.el7
# Thu, 12 May 2022 22:39:48 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Thu, 12 May 2022 22:40:02 GMT
RUN set -eux; 	yum install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Thu, 12 May 2022 22:40:03 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Thu, 12 May 2022 22:40:03 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el7
# Thu, 12 May 2022 22:40:21 GMT
RUN set -eux; 	yum install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Thu, 12 May 2022 22:40:21 GMT
VOLUME [/var/lib/mysql]
# Thu, 12 May 2022 22:40:22 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Thu, 12 May 2022 22:40:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 May 2022 22:40:22 GMT
EXPOSE 3306 33060
# Thu, 12 May 2022 22:40:22 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:cd32cd816e68367704ec22e6e4d27af6a08b27e32aca3d0bd7a47424e37d0b91`  
		Last Modified: Thu, 12 May 2022 20:59:41 GMT  
		Size: 48.8 MB (48758049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac1cac655dec3bbc6c5dd2efa9156e4798ca4cbb99f1311853f490d7092ba3ad`  
		Last Modified: Thu, 12 May 2022 22:41:03 GMT  
		Size: 1.1 KB (1061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882efd5b0b9e419c5b8707b94c9916f62f166a427c37954da0aefc0f7c744ca0`  
		Last Modified: Thu, 12 May 2022 22:41:00 GMT  
		Size: 930.2 KB (930225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8424ed51a7a3d46b24a5876e22e1d42a033170139757b9b003be5da80d6c33a8`  
		Last Modified: Thu, 12 May 2022 22:41:01 GMT  
		Size: 3.8 MB (3761150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edd7d8c8b2c6eb0293ce188c4627a483f57d6c6cd1409bee035ee58fbcd39f41`  
		Last Modified: Thu, 12 May 2022 22:40:59 GMT  
		Size: 2.7 KB (2658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d485f7c40504fc4261d3b5cb62305b4f41a0507cb46e11c2c54b65a2ca6d39`  
		Last Modified: Thu, 12 May 2022 22:40:57 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15656ef8b782ab3e6234de4f2c4854115373be8ab28b59f9f014dbff120037af`  
		Last Modified: Thu, 12 May 2022 22:41:01 GMT  
		Size: 25.5 MB (25476162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3786d73cb960fecd724e6bcf500defd0e02cf03a7869863adb65266d025b909e`  
		Last Modified: Thu, 12 May 2022 22:40:57 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a3f7291494d2e057d61cfdeff9c32d944d87bcc349fe31f2a79bf85be661461`  
		Last Modified: Thu, 12 May 2022 22:41:06 GMT  
		Size: 48.0 MB (47974917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2399c35146d1646f6f535235dfce69c437e13576fa19a283fdb340323b36fdfe`  
		Last Modified: Thu, 12 May 2022 22:40:57 GMT  
		Size: 5.1 KB (5139 bytes)  
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
$ docker pull mysql@sha256:0e5a4f3064c00a4b0a5ca90ad1aa805837f52633242b8c168d67607d207165b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.38-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:4d5e8763440bd8c7af3c68132796e201a8297d4d77df2c978e96c51678cb2c4f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.9 MB (126910013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23eb9a154db6b6e6b0ba7c0a0f656d5741f848b3d2ac66af2bf6113d5ba1d209`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 12 May 2022 20:58:56 GMT
ADD file:8ac79c33c3bdf8a0a1c23cc009fabc3ead9d97891d701ad21090a6bc542521e2 in / 
# Thu, 12 May 2022 20:58:56 GMT
CMD ["/bin/bash"]
# Thu, 12 May 2022 22:39:33 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Thu, 12 May 2022 22:39:33 GMT
ENV GOSU_VERSION=1.14
# Thu, 12 May 2022 22:39:36 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 12 May 2022 22:39:46 GMT
RUN set -eux; 	yum install -y 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Thu, 12 May 2022 22:39:48 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 12 May 2022 22:39:48 GMT
ENV MYSQL_MAJOR=5.7
# Thu, 12 May 2022 22:39:48 GMT
ENV MYSQL_VERSION=5.7.38-1.el7
# Thu, 12 May 2022 22:39:48 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Thu, 12 May 2022 22:40:02 GMT
RUN set -eux; 	yum install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Thu, 12 May 2022 22:40:03 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Thu, 12 May 2022 22:40:03 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el7
# Thu, 12 May 2022 22:40:21 GMT
RUN set -eux; 	yum install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Thu, 12 May 2022 22:40:21 GMT
VOLUME [/var/lib/mysql]
# Thu, 12 May 2022 22:40:22 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Thu, 12 May 2022 22:40:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 May 2022 22:40:22 GMT
EXPOSE 3306 33060
# Thu, 12 May 2022 22:40:22 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:cd32cd816e68367704ec22e6e4d27af6a08b27e32aca3d0bd7a47424e37d0b91`  
		Last Modified: Thu, 12 May 2022 20:59:41 GMT  
		Size: 48.8 MB (48758049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac1cac655dec3bbc6c5dd2efa9156e4798ca4cbb99f1311853f490d7092ba3ad`  
		Last Modified: Thu, 12 May 2022 22:41:03 GMT  
		Size: 1.1 KB (1061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882efd5b0b9e419c5b8707b94c9916f62f166a427c37954da0aefc0f7c744ca0`  
		Last Modified: Thu, 12 May 2022 22:41:00 GMT  
		Size: 930.2 KB (930225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8424ed51a7a3d46b24a5876e22e1d42a033170139757b9b003be5da80d6c33a8`  
		Last Modified: Thu, 12 May 2022 22:41:01 GMT  
		Size: 3.8 MB (3761150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edd7d8c8b2c6eb0293ce188c4627a483f57d6c6cd1409bee035ee58fbcd39f41`  
		Last Modified: Thu, 12 May 2022 22:40:59 GMT  
		Size: 2.7 KB (2658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d485f7c40504fc4261d3b5cb62305b4f41a0507cb46e11c2c54b65a2ca6d39`  
		Last Modified: Thu, 12 May 2022 22:40:57 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15656ef8b782ab3e6234de4f2c4854115373be8ab28b59f9f014dbff120037af`  
		Last Modified: Thu, 12 May 2022 22:41:01 GMT  
		Size: 25.5 MB (25476162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3786d73cb960fecd724e6bcf500defd0e02cf03a7869863adb65266d025b909e`  
		Last Modified: Thu, 12 May 2022 22:40:57 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a3f7291494d2e057d61cfdeff9c32d944d87bcc349fe31f2a79bf85be661461`  
		Last Modified: Thu, 12 May 2022 22:41:06 GMT  
		Size: 48.0 MB (47974917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2399c35146d1646f6f535235dfce69c437e13576fa19a283fdb340323b36fdfe`  
		Last Modified: Thu, 12 May 2022 22:40:57 GMT  
		Size: 5.1 KB (5139 bytes)  
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
$ docker pull mysql@sha256:2befebef0265220c2d6caed2599cd4fe6497c90408fc9f9925684ae26e92d769
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:8141c03377ac2ad7853c98833d620015590d76caa5c17d1d7599ef26baf44da4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.6 MB (131645641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28bb00bfe52a2aae96a7ab476f324e2c37fab25dd52dd86ff436331e067b4696`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 17 May 2022 22:41:42 GMT
ADD file:bbaf69bdffd0f506e447fbc52dca450a8966d950b8fa9aebd3a1bd5bd98f8b28 in / 
# Tue, 17 May 2022 22:41:42 GMT
CMD ["/bin/bash"]
# Tue, 17 May 2022 23:10:18 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Tue, 17 May 2022 23:10:18 GMT
ENV GOSU_VERSION=1.14
# Tue, 17 May 2022 23:10:22 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 17 May 2022 23:10:42 GMT
RUN set -eux; 	microdnf install -y 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Tue, 17 May 2022 23:10:43 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Tue, 17 May 2022 23:10:43 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 17 May 2022 23:10:43 GMT
ENV MYSQL_VERSION=8.0.29-1.el8
# Tue, 17 May 2022 23:10:44 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 17 May 2022 23:11:10 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Tue, 17 May 2022 23:11:11 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 17 May 2022 23:11:11 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el8
# Tue, 17 May 2022 23:11:40 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 17 May 2022 23:11:40 GMT
VOLUME [/var/lib/mysql]
# Tue, 17 May 2022 23:11:40 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Tue, 17 May 2022 23:11:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 May 2022 23:11:41 GMT
EXPOSE 3306 33060
# Tue, 17 May 2022 23:11:41 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:90a00d516db16c568d3da8e0a7a5a78fa6fef5a39f3d688f831d254b77791565`  
		Last Modified: Tue, 17 May 2022 22:42:38 GMT  
		Size: 39.2 MB (39220501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec380701a2aab4173cf5a055f74c99227ae7c4fddf87803362ac984b3cbfa8ef`  
		Last Modified: Tue, 17 May 2022 23:12:28 GMT  
		Size: 1.1 KB (1080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c639d40d7782dd181799bc0e030b8269850fa3ad5bb3bbdeb511ea1c782e33c6`  
		Last Modified: Tue, 17 May 2022 23:12:26 GMT  
		Size: 928.8 KB (928834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba2e5b74a30bdb2c55f39992bb2ae64d81e0b737541ad217123841bd41bda53`  
		Last Modified: Tue, 17 May 2022 23:12:26 GMT  
		Size: 4.5 MB (4536235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bce381d3796288927fc508cdc11bdca5a6c3d0dca64c13c2fc51035851ab296`  
		Last Modified: Tue, 17 May 2022 23:12:25 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5e5b79d5c8e16d050f0a02cf0d1214f77e2a4e272b88299488b054d7c95f711`  
		Last Modified: Tue, 17 May 2022 23:12:23 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:858b3b51a1f97d5a72794a4cde78e9130b00620b922db41c2bc3ac79a55e8f58`  
		Last Modified: Tue, 17 May 2022 23:12:30 GMT  
		Size: 47.2 MB (47242274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2171f9f10a16c77335db5f61043051469c24c5080d9f80f87d5778f96b2bbc1c`  
		Last Modified: Tue, 17 May 2022 23:12:23 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0fa78a73ac6ced6b681d9255b9345f3f8ab04aec0f08aa1fa0533dc37f055e`  
		Last Modified: Tue, 17 May 2022 23:12:31 GMT  
		Size: 39.7 MB (39708291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c240edbdbe67409f4ac9e83c9fc86c0cebf506ad3ebfd9d1ccdd29baa7a9e889`  
		Last Modified: Tue, 17 May 2022 23:12:23 GMT  
		Size: 5.1 KB (5142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:32019f5c8959fb725787a9873aeee9c28c8a4a054413e89263f37aa2007901c1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.6 MB (138552501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e001f62601a11aea9a86873c2edf17d733c7a26cbd6d4ea0e05e0a73e9140e6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 17 May 2022 22:52:38 GMT
ADD file:263fe8ce0663428b324fa2909814084a77bf17118d772058d41546b804a4b968 in / 
# Tue, 17 May 2022 22:52:39 GMT
CMD ["/bin/bash"]
# Tue, 17 May 2022 23:09:01 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Tue, 17 May 2022 23:09:02 GMT
ENV GOSU_VERSION=1.14
# Tue, 17 May 2022 23:09:05 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 17 May 2022 23:09:26 GMT
RUN set -eux; 	microdnf install -y 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Tue, 17 May 2022 23:09:28 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Tue, 17 May 2022 23:09:29 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 17 May 2022 23:09:30 GMT
ENV MYSQL_VERSION=8.0.29-1.el8
# Tue, 17 May 2022 23:09:31 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 17 May 2022 23:09:55 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Tue, 17 May 2022 23:09:55 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 17 May 2022 23:09:56 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el8
# Tue, 17 May 2022 23:10:23 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 17 May 2022 23:10:24 GMT
VOLUME [/var/lib/mysql]
# Tue, 17 May 2022 23:10:26 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Tue, 17 May 2022 23:10:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 May 2022 23:10:27 GMT
EXPOSE 3306 33060
# Tue, 17 May 2022 23:10:28 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:0dbddf5847a3e154a061766ddebe6a3cae471c97cabb3be2871f6d91f265d137`  
		Last Modified: Tue, 17 May 2022 22:53:43 GMT  
		Size: 38.0 MB (38012703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db29b0b5a771d422a5f85337ad705ae13b90861da7c4ae8a2d3020b42d0d4892`  
		Last Modified: Tue, 17 May 2022 23:10:58 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3855c850e40abd0de4601587237af854d07522e10e3bb9ee0e8c66b40ae49911`  
		Last Modified: Tue, 17 May 2022 23:10:56 GMT  
		Size: 857.2 KB (857152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a57b88152cf6fe699baa66b60fd8c2f07daef18b1931fae4dfc7c92d5d48ae5`  
		Last Modified: Tue, 17 May 2022 23:10:56 GMT  
		Size: 4.3 MB (4342967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ac9375febdd7998b9cc129e95d554b5b9d024f9ecf3053d3e7156a31279923f`  
		Last Modified: Tue, 17 May 2022 23:10:55 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a199a4e720f0e82bafd1852cdf3a57870a449bcb60c197daf349869c4d332bb3`  
		Last Modified: Tue, 17 May 2022 23:10:53 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebac76248d98ab600a56814d6569f0e4f4799aceb8bc8d8999f1b88938873e6`  
		Last Modified: Tue, 17 May 2022 23:11:00 GMT  
		Size: 53.3 MB (53299522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b6eb52402d98a9e93f419ca2bc248862a3b2b7e0c0fc6800cadd1622dc46e9`  
		Last Modified: Tue, 17 May 2022 23:10:53 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef5d943dd79edceeeeb858d6e3e80aa85a14a1f402e70156d2fd61d6e5f60a4`  
		Last Modified: Tue, 17 May 2022 23:11:01 GMT  
		Size: 42.0 MB (42030739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cd2e0c049de23bde6eb2d74d0ccebd69780e107d88608b72e6e229ea7c8bdf3`  
		Last Modified: Tue, 17 May 2022 23:10:53 GMT  
		Size: 5.1 KB (5142 bytes)  
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
$ docker pull mysql@sha256:2befebef0265220c2d6caed2599cd4fe6497c90408fc9f9925684ae26e92d769
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:8141c03377ac2ad7853c98833d620015590d76caa5c17d1d7599ef26baf44da4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.6 MB (131645641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28bb00bfe52a2aae96a7ab476f324e2c37fab25dd52dd86ff436331e067b4696`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 17 May 2022 22:41:42 GMT
ADD file:bbaf69bdffd0f506e447fbc52dca450a8966d950b8fa9aebd3a1bd5bd98f8b28 in / 
# Tue, 17 May 2022 22:41:42 GMT
CMD ["/bin/bash"]
# Tue, 17 May 2022 23:10:18 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Tue, 17 May 2022 23:10:18 GMT
ENV GOSU_VERSION=1.14
# Tue, 17 May 2022 23:10:22 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 17 May 2022 23:10:42 GMT
RUN set -eux; 	microdnf install -y 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Tue, 17 May 2022 23:10:43 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Tue, 17 May 2022 23:10:43 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 17 May 2022 23:10:43 GMT
ENV MYSQL_VERSION=8.0.29-1.el8
# Tue, 17 May 2022 23:10:44 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 17 May 2022 23:11:10 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Tue, 17 May 2022 23:11:11 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 17 May 2022 23:11:11 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el8
# Tue, 17 May 2022 23:11:40 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 17 May 2022 23:11:40 GMT
VOLUME [/var/lib/mysql]
# Tue, 17 May 2022 23:11:40 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Tue, 17 May 2022 23:11:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 May 2022 23:11:41 GMT
EXPOSE 3306 33060
# Tue, 17 May 2022 23:11:41 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:90a00d516db16c568d3da8e0a7a5a78fa6fef5a39f3d688f831d254b77791565`  
		Last Modified: Tue, 17 May 2022 22:42:38 GMT  
		Size: 39.2 MB (39220501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec380701a2aab4173cf5a055f74c99227ae7c4fddf87803362ac984b3cbfa8ef`  
		Last Modified: Tue, 17 May 2022 23:12:28 GMT  
		Size: 1.1 KB (1080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c639d40d7782dd181799bc0e030b8269850fa3ad5bb3bbdeb511ea1c782e33c6`  
		Last Modified: Tue, 17 May 2022 23:12:26 GMT  
		Size: 928.8 KB (928834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba2e5b74a30bdb2c55f39992bb2ae64d81e0b737541ad217123841bd41bda53`  
		Last Modified: Tue, 17 May 2022 23:12:26 GMT  
		Size: 4.5 MB (4536235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bce381d3796288927fc508cdc11bdca5a6c3d0dca64c13c2fc51035851ab296`  
		Last Modified: Tue, 17 May 2022 23:12:25 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5e5b79d5c8e16d050f0a02cf0d1214f77e2a4e272b88299488b054d7c95f711`  
		Last Modified: Tue, 17 May 2022 23:12:23 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:858b3b51a1f97d5a72794a4cde78e9130b00620b922db41c2bc3ac79a55e8f58`  
		Last Modified: Tue, 17 May 2022 23:12:30 GMT  
		Size: 47.2 MB (47242274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2171f9f10a16c77335db5f61043051469c24c5080d9f80f87d5778f96b2bbc1c`  
		Last Modified: Tue, 17 May 2022 23:12:23 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0fa78a73ac6ced6b681d9255b9345f3f8ab04aec0f08aa1fa0533dc37f055e`  
		Last Modified: Tue, 17 May 2022 23:12:31 GMT  
		Size: 39.7 MB (39708291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c240edbdbe67409f4ac9e83c9fc86c0cebf506ad3ebfd9d1ccdd29baa7a9e889`  
		Last Modified: Tue, 17 May 2022 23:12:23 GMT  
		Size: 5.1 KB (5142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:32019f5c8959fb725787a9873aeee9c28c8a4a054413e89263f37aa2007901c1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.6 MB (138552501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e001f62601a11aea9a86873c2edf17d733c7a26cbd6d4ea0e05e0a73e9140e6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 17 May 2022 22:52:38 GMT
ADD file:263fe8ce0663428b324fa2909814084a77bf17118d772058d41546b804a4b968 in / 
# Tue, 17 May 2022 22:52:39 GMT
CMD ["/bin/bash"]
# Tue, 17 May 2022 23:09:01 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Tue, 17 May 2022 23:09:02 GMT
ENV GOSU_VERSION=1.14
# Tue, 17 May 2022 23:09:05 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 17 May 2022 23:09:26 GMT
RUN set -eux; 	microdnf install -y 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Tue, 17 May 2022 23:09:28 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Tue, 17 May 2022 23:09:29 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 17 May 2022 23:09:30 GMT
ENV MYSQL_VERSION=8.0.29-1.el8
# Tue, 17 May 2022 23:09:31 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 17 May 2022 23:09:55 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Tue, 17 May 2022 23:09:55 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 17 May 2022 23:09:56 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el8
# Tue, 17 May 2022 23:10:23 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 17 May 2022 23:10:24 GMT
VOLUME [/var/lib/mysql]
# Tue, 17 May 2022 23:10:26 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Tue, 17 May 2022 23:10:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 May 2022 23:10:27 GMT
EXPOSE 3306 33060
# Tue, 17 May 2022 23:10:28 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:0dbddf5847a3e154a061766ddebe6a3cae471c97cabb3be2871f6d91f265d137`  
		Last Modified: Tue, 17 May 2022 22:53:43 GMT  
		Size: 38.0 MB (38012703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db29b0b5a771d422a5f85337ad705ae13b90861da7c4ae8a2d3020b42d0d4892`  
		Last Modified: Tue, 17 May 2022 23:10:58 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3855c850e40abd0de4601587237af854d07522e10e3bb9ee0e8c66b40ae49911`  
		Last Modified: Tue, 17 May 2022 23:10:56 GMT  
		Size: 857.2 KB (857152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a57b88152cf6fe699baa66b60fd8c2f07daef18b1931fae4dfc7c92d5d48ae5`  
		Last Modified: Tue, 17 May 2022 23:10:56 GMT  
		Size: 4.3 MB (4342967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ac9375febdd7998b9cc129e95d554b5b9d024f9ecf3053d3e7156a31279923f`  
		Last Modified: Tue, 17 May 2022 23:10:55 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a199a4e720f0e82bafd1852cdf3a57870a449bcb60c197daf349869c4d332bb3`  
		Last Modified: Tue, 17 May 2022 23:10:53 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebac76248d98ab600a56814d6569f0e4f4799aceb8bc8d8999f1b88938873e6`  
		Last Modified: Tue, 17 May 2022 23:11:00 GMT  
		Size: 53.3 MB (53299522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b6eb52402d98a9e93f419ca2bc248862a3b2b7e0c0fc6800cadd1622dc46e9`  
		Last Modified: Tue, 17 May 2022 23:10:53 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef5d943dd79edceeeeb858d6e3e80aa85a14a1f402e70156d2fd61d6e5f60a4`  
		Last Modified: Tue, 17 May 2022 23:11:01 GMT  
		Size: 42.0 MB (42030739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cd2e0c049de23bde6eb2d74d0ccebd69780e107d88608b72e6e229ea7c8bdf3`  
		Last Modified: Tue, 17 May 2022 23:10:53 GMT  
		Size: 5.1 KB (5142 bytes)  
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
$ docker pull mysql@sha256:2befebef0265220c2d6caed2599cd4fe6497c90408fc9f9925684ae26e92d769
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0.29-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:8141c03377ac2ad7853c98833d620015590d76caa5c17d1d7599ef26baf44da4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.6 MB (131645641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28bb00bfe52a2aae96a7ab476f324e2c37fab25dd52dd86ff436331e067b4696`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 17 May 2022 22:41:42 GMT
ADD file:bbaf69bdffd0f506e447fbc52dca450a8966d950b8fa9aebd3a1bd5bd98f8b28 in / 
# Tue, 17 May 2022 22:41:42 GMT
CMD ["/bin/bash"]
# Tue, 17 May 2022 23:10:18 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Tue, 17 May 2022 23:10:18 GMT
ENV GOSU_VERSION=1.14
# Tue, 17 May 2022 23:10:22 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 17 May 2022 23:10:42 GMT
RUN set -eux; 	microdnf install -y 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Tue, 17 May 2022 23:10:43 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Tue, 17 May 2022 23:10:43 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 17 May 2022 23:10:43 GMT
ENV MYSQL_VERSION=8.0.29-1.el8
# Tue, 17 May 2022 23:10:44 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 17 May 2022 23:11:10 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Tue, 17 May 2022 23:11:11 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 17 May 2022 23:11:11 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el8
# Tue, 17 May 2022 23:11:40 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 17 May 2022 23:11:40 GMT
VOLUME [/var/lib/mysql]
# Tue, 17 May 2022 23:11:40 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Tue, 17 May 2022 23:11:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 May 2022 23:11:41 GMT
EXPOSE 3306 33060
# Tue, 17 May 2022 23:11:41 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:90a00d516db16c568d3da8e0a7a5a78fa6fef5a39f3d688f831d254b77791565`  
		Last Modified: Tue, 17 May 2022 22:42:38 GMT  
		Size: 39.2 MB (39220501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec380701a2aab4173cf5a055f74c99227ae7c4fddf87803362ac984b3cbfa8ef`  
		Last Modified: Tue, 17 May 2022 23:12:28 GMT  
		Size: 1.1 KB (1080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c639d40d7782dd181799bc0e030b8269850fa3ad5bb3bbdeb511ea1c782e33c6`  
		Last Modified: Tue, 17 May 2022 23:12:26 GMT  
		Size: 928.8 KB (928834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba2e5b74a30bdb2c55f39992bb2ae64d81e0b737541ad217123841bd41bda53`  
		Last Modified: Tue, 17 May 2022 23:12:26 GMT  
		Size: 4.5 MB (4536235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bce381d3796288927fc508cdc11bdca5a6c3d0dca64c13c2fc51035851ab296`  
		Last Modified: Tue, 17 May 2022 23:12:25 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5e5b79d5c8e16d050f0a02cf0d1214f77e2a4e272b88299488b054d7c95f711`  
		Last Modified: Tue, 17 May 2022 23:12:23 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:858b3b51a1f97d5a72794a4cde78e9130b00620b922db41c2bc3ac79a55e8f58`  
		Last Modified: Tue, 17 May 2022 23:12:30 GMT  
		Size: 47.2 MB (47242274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2171f9f10a16c77335db5f61043051469c24c5080d9f80f87d5778f96b2bbc1c`  
		Last Modified: Tue, 17 May 2022 23:12:23 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0fa78a73ac6ced6b681d9255b9345f3f8ab04aec0f08aa1fa0533dc37f055e`  
		Last Modified: Tue, 17 May 2022 23:12:31 GMT  
		Size: 39.7 MB (39708291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c240edbdbe67409f4ac9e83c9fc86c0cebf506ad3ebfd9d1ccdd29baa7a9e889`  
		Last Modified: Tue, 17 May 2022 23:12:23 GMT  
		Size: 5.1 KB (5142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0.29-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:32019f5c8959fb725787a9873aeee9c28c8a4a054413e89263f37aa2007901c1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.6 MB (138552501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e001f62601a11aea9a86873c2edf17d733c7a26cbd6d4ea0e05e0a73e9140e6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 17 May 2022 22:52:38 GMT
ADD file:263fe8ce0663428b324fa2909814084a77bf17118d772058d41546b804a4b968 in / 
# Tue, 17 May 2022 22:52:39 GMT
CMD ["/bin/bash"]
# Tue, 17 May 2022 23:09:01 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Tue, 17 May 2022 23:09:02 GMT
ENV GOSU_VERSION=1.14
# Tue, 17 May 2022 23:09:05 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 17 May 2022 23:09:26 GMT
RUN set -eux; 	microdnf install -y 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Tue, 17 May 2022 23:09:28 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Tue, 17 May 2022 23:09:29 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 17 May 2022 23:09:30 GMT
ENV MYSQL_VERSION=8.0.29-1.el8
# Tue, 17 May 2022 23:09:31 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 17 May 2022 23:09:55 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Tue, 17 May 2022 23:09:55 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 17 May 2022 23:09:56 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el8
# Tue, 17 May 2022 23:10:23 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 17 May 2022 23:10:24 GMT
VOLUME [/var/lib/mysql]
# Tue, 17 May 2022 23:10:26 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Tue, 17 May 2022 23:10:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 May 2022 23:10:27 GMT
EXPOSE 3306 33060
# Tue, 17 May 2022 23:10:28 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:0dbddf5847a3e154a061766ddebe6a3cae471c97cabb3be2871f6d91f265d137`  
		Last Modified: Tue, 17 May 2022 22:53:43 GMT  
		Size: 38.0 MB (38012703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db29b0b5a771d422a5f85337ad705ae13b90861da7c4ae8a2d3020b42d0d4892`  
		Last Modified: Tue, 17 May 2022 23:10:58 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3855c850e40abd0de4601587237af854d07522e10e3bb9ee0e8c66b40ae49911`  
		Last Modified: Tue, 17 May 2022 23:10:56 GMT  
		Size: 857.2 KB (857152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a57b88152cf6fe699baa66b60fd8c2f07daef18b1931fae4dfc7c92d5d48ae5`  
		Last Modified: Tue, 17 May 2022 23:10:56 GMT  
		Size: 4.3 MB (4342967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ac9375febdd7998b9cc129e95d554b5b9d024f9ecf3053d3e7156a31279923f`  
		Last Modified: Tue, 17 May 2022 23:10:55 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a199a4e720f0e82bafd1852cdf3a57870a449bcb60c197daf349869c4d332bb3`  
		Last Modified: Tue, 17 May 2022 23:10:53 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebac76248d98ab600a56814d6569f0e4f4799aceb8bc8d8999f1b88938873e6`  
		Last Modified: Tue, 17 May 2022 23:11:00 GMT  
		Size: 53.3 MB (53299522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b6eb52402d98a9e93f419ca2bc248862a3b2b7e0c0fc6800cadd1622dc46e9`  
		Last Modified: Tue, 17 May 2022 23:10:53 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef5d943dd79edceeeeb858d6e3e80aa85a14a1f402e70156d2fd61d6e5f60a4`  
		Last Modified: Tue, 17 May 2022 23:11:01 GMT  
		Size: 42.0 MB (42030739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cd2e0c049de23bde6eb2d74d0ccebd69780e107d88608b72e6e229ea7c8bdf3`  
		Last Modified: Tue, 17 May 2022 23:10:53 GMT  
		Size: 5.1 KB (5142 bytes)  
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
$ docker pull mysql@sha256:2befebef0265220c2d6caed2599cd4fe6497c90408fc9f9925684ae26e92d769
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:oracle` - linux; amd64

```console
$ docker pull mysql@sha256:8141c03377ac2ad7853c98833d620015590d76caa5c17d1d7599ef26baf44da4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.6 MB (131645641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28bb00bfe52a2aae96a7ab476f324e2c37fab25dd52dd86ff436331e067b4696`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 17 May 2022 22:41:42 GMT
ADD file:bbaf69bdffd0f506e447fbc52dca450a8966d950b8fa9aebd3a1bd5bd98f8b28 in / 
# Tue, 17 May 2022 22:41:42 GMT
CMD ["/bin/bash"]
# Tue, 17 May 2022 23:10:18 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Tue, 17 May 2022 23:10:18 GMT
ENV GOSU_VERSION=1.14
# Tue, 17 May 2022 23:10:22 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 17 May 2022 23:10:42 GMT
RUN set -eux; 	microdnf install -y 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Tue, 17 May 2022 23:10:43 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Tue, 17 May 2022 23:10:43 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 17 May 2022 23:10:43 GMT
ENV MYSQL_VERSION=8.0.29-1.el8
# Tue, 17 May 2022 23:10:44 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 17 May 2022 23:11:10 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Tue, 17 May 2022 23:11:11 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 17 May 2022 23:11:11 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el8
# Tue, 17 May 2022 23:11:40 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 17 May 2022 23:11:40 GMT
VOLUME [/var/lib/mysql]
# Tue, 17 May 2022 23:11:40 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Tue, 17 May 2022 23:11:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 May 2022 23:11:41 GMT
EXPOSE 3306 33060
# Tue, 17 May 2022 23:11:41 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:90a00d516db16c568d3da8e0a7a5a78fa6fef5a39f3d688f831d254b77791565`  
		Last Modified: Tue, 17 May 2022 22:42:38 GMT  
		Size: 39.2 MB (39220501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec380701a2aab4173cf5a055f74c99227ae7c4fddf87803362ac984b3cbfa8ef`  
		Last Modified: Tue, 17 May 2022 23:12:28 GMT  
		Size: 1.1 KB (1080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c639d40d7782dd181799bc0e030b8269850fa3ad5bb3bbdeb511ea1c782e33c6`  
		Last Modified: Tue, 17 May 2022 23:12:26 GMT  
		Size: 928.8 KB (928834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba2e5b74a30bdb2c55f39992bb2ae64d81e0b737541ad217123841bd41bda53`  
		Last Modified: Tue, 17 May 2022 23:12:26 GMT  
		Size: 4.5 MB (4536235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bce381d3796288927fc508cdc11bdca5a6c3d0dca64c13c2fc51035851ab296`  
		Last Modified: Tue, 17 May 2022 23:12:25 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5e5b79d5c8e16d050f0a02cf0d1214f77e2a4e272b88299488b054d7c95f711`  
		Last Modified: Tue, 17 May 2022 23:12:23 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:858b3b51a1f97d5a72794a4cde78e9130b00620b922db41c2bc3ac79a55e8f58`  
		Last Modified: Tue, 17 May 2022 23:12:30 GMT  
		Size: 47.2 MB (47242274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2171f9f10a16c77335db5f61043051469c24c5080d9f80f87d5778f96b2bbc1c`  
		Last Modified: Tue, 17 May 2022 23:12:23 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0fa78a73ac6ced6b681d9255b9345f3f8ab04aec0f08aa1fa0533dc37f055e`  
		Last Modified: Tue, 17 May 2022 23:12:31 GMT  
		Size: 39.7 MB (39708291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c240edbdbe67409f4ac9e83c9fc86c0cebf506ad3ebfd9d1ccdd29baa7a9e889`  
		Last Modified: Tue, 17 May 2022 23:12:23 GMT  
		Size: 5.1 KB (5142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:32019f5c8959fb725787a9873aeee9c28c8a4a054413e89263f37aa2007901c1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.6 MB (138552501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e001f62601a11aea9a86873c2edf17d733c7a26cbd6d4ea0e05e0a73e9140e6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 17 May 2022 22:52:38 GMT
ADD file:263fe8ce0663428b324fa2909814084a77bf17118d772058d41546b804a4b968 in / 
# Tue, 17 May 2022 22:52:39 GMT
CMD ["/bin/bash"]
# Tue, 17 May 2022 23:09:01 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Tue, 17 May 2022 23:09:02 GMT
ENV GOSU_VERSION=1.14
# Tue, 17 May 2022 23:09:05 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 17 May 2022 23:09:26 GMT
RUN set -eux; 	microdnf install -y 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Tue, 17 May 2022 23:09:28 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Tue, 17 May 2022 23:09:29 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 17 May 2022 23:09:30 GMT
ENV MYSQL_VERSION=8.0.29-1.el8
# Tue, 17 May 2022 23:09:31 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 17 May 2022 23:09:55 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Tue, 17 May 2022 23:09:55 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 17 May 2022 23:09:56 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el8
# Tue, 17 May 2022 23:10:23 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 17 May 2022 23:10:24 GMT
VOLUME [/var/lib/mysql]
# Tue, 17 May 2022 23:10:26 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Tue, 17 May 2022 23:10:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 May 2022 23:10:27 GMT
EXPOSE 3306 33060
# Tue, 17 May 2022 23:10:28 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:0dbddf5847a3e154a061766ddebe6a3cae471c97cabb3be2871f6d91f265d137`  
		Last Modified: Tue, 17 May 2022 22:53:43 GMT  
		Size: 38.0 MB (38012703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db29b0b5a771d422a5f85337ad705ae13b90861da7c4ae8a2d3020b42d0d4892`  
		Last Modified: Tue, 17 May 2022 23:10:58 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3855c850e40abd0de4601587237af854d07522e10e3bb9ee0e8c66b40ae49911`  
		Last Modified: Tue, 17 May 2022 23:10:56 GMT  
		Size: 857.2 KB (857152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a57b88152cf6fe699baa66b60fd8c2f07daef18b1931fae4dfc7c92d5d48ae5`  
		Last Modified: Tue, 17 May 2022 23:10:56 GMT  
		Size: 4.3 MB (4342967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ac9375febdd7998b9cc129e95d554b5b9d024f9ecf3053d3e7156a31279923f`  
		Last Modified: Tue, 17 May 2022 23:10:55 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a199a4e720f0e82bafd1852cdf3a57870a449bcb60c197daf349869c4d332bb3`  
		Last Modified: Tue, 17 May 2022 23:10:53 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebac76248d98ab600a56814d6569f0e4f4799aceb8bc8d8999f1b88938873e6`  
		Last Modified: Tue, 17 May 2022 23:11:00 GMT  
		Size: 53.3 MB (53299522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b6eb52402d98a9e93f419ca2bc248862a3b2b7e0c0fc6800cadd1622dc46e9`  
		Last Modified: Tue, 17 May 2022 23:10:53 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef5d943dd79edceeeeb858d6e3e80aa85a14a1f402e70156d2fd61d6e5f60a4`  
		Last Modified: Tue, 17 May 2022 23:11:01 GMT  
		Size: 42.0 MB (42030739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cd2e0c049de23bde6eb2d74d0ccebd69780e107d88608b72e6e229ea7c8bdf3`  
		Last Modified: Tue, 17 May 2022 23:10:53 GMT  
		Size: 5.1 KB (5142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
