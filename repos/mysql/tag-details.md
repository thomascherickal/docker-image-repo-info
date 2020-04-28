<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mysql`

-	[`mysql:5`](#mysql5)
-	[`mysql:5.6`](#mysql56)
-	[`mysql:5.6.48`](#mysql5648)
-	[`mysql:5.7`](#mysql57)
-	[`mysql:5.7.30`](#mysql5730)
-	[`mysql:8`](#mysql8)
-	[`mysql:8.0`](#mysql80)
-	[`mysql:8.0.20`](#mysql8020)
-	[`mysql:latest`](#mysqllatest)

## `mysql:5`

```console
$ docker pull mysql@sha256:95b4bc7c1b111906fdb7a39cd990dd99f21c594722735d059769b80312eb57a7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:5` - linux; amd64

```console
$ docker pull mysql@sha256:8044616c01e46c6bc826d205103a2b650a1679be2f34beab9bbf6c6f642df673
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.4 MB (158351512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d9483f9a7b21c87e0f5b9776c3e06567603c28c0062013eda127c968175f5e8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 23 Apr 2020 00:20:32 GMT
ADD file:9b8be2b52ee0fa31da1b6256099030b73546253a57e94cccb24605cd888bb74d in / 
# Thu, 23 Apr 2020 00:20:32 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 04:13:52 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 23 Apr 2020 04:13:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 04:13:59 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 04:14:08 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 04:14:09 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 23 Apr 2020 04:14:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 04:14:20 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Thu, 23 Apr 2020 04:15:08 GMT
ENV MYSQL_MAJOR=5.7
# Thu, 23 Apr 2020 04:15:09 GMT
ENV MYSQL_VERSION=5.7.29-1debian10
# Thu, 23 Apr 2020 04:15:10 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ buster mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Thu, 23 Apr 2020 04:15:49 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-server="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 777 /var/run/mysqld 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 23 Apr 2020 04:15:49 GMT
VOLUME [/var/lib/mysql]
# Thu, 23 Apr 2020 04:15:50 GMT
COPY file:b09451ebd8fb98d90335352b9649da1b3336a789513bb4ae725c9eadafd519b6 in /usr/local/bin/ 
# Thu, 23 Apr 2020 04:15:51 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Apr 2020 04:15:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 04:15:52 GMT
EXPOSE 3306 33060
# Thu, 23 Apr 2020 04:15:52 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:54fec2fa59d0a0de9cd2dec9850b36c43de451f1fd1c0a5bf8f1cf26a61a5da4`  
		Last Modified: Thu, 23 Apr 2020 00:25:10 GMT  
		Size: 27.1 MB (27098254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc6c614591231a51a8abf93a762208fd1aed3f72f3e3fd0b8907904e3c9a38b`  
		Last Modified: Thu, 23 Apr 2020 04:17:30 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:951c3d959c9d9548b3c320af7856e6e16c967daf7d280ac2607e49aa2b3816dd`  
		Last Modified: Thu, 23 Apr 2020 04:17:32 GMT  
		Size: 4.2 MB (4178101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05de4d0e206e076ed00d1b32a5104bcd7246484f51de192ba7d5b5c75fe215d0`  
		Last Modified: Thu, 23 Apr 2020 04:17:30 GMT  
		Size: 1.4 MB (1419225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:319f0394ef4231f3e9f43809855fba117032c697e51c94defda703f34a527b43`  
		Last Modified: Thu, 23 Apr 2020 04:17:29 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9185034607beae95fac5ee5b684c0182fa10a66b51ba65a7e81345e860b91c2`  
		Last Modified: Thu, 23 Apr 2020 04:17:35 GMT  
		Size: 13.4 MB (13443052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013a9c64dadc90a7aef7354825e9668f7b7667ad915df865cb4d05142a76938e`  
		Last Modified: Thu, 23 Apr 2020 04:17:28 GMT  
		Size: 2.4 KB (2395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58b7b840ebff81e42f4ba9bc82fe6da1012d22753693561022c1cadce29bf98e`  
		Last Modified: Thu, 23 Apr 2020 04:18:07 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b85c0abc43d54e9d83638b7ac1bdeca8c38dab7cda795c45541b52fd0fcda5e`  
		Last Modified: Thu, 23 Apr 2020 04:18:31 GMT  
		Size: 112.2 MB (112203157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf022f63e85cdffd7cfea4a44248b378f34553171463eaee142ef09aefa1f33`  
		Last Modified: Thu, 23 Apr 2020 04:18:07 GMT  
		Size: 5.1 KB (5135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35f7f707ce83e3b72c259b3e9e813cc5c10f2bd0f723193f3f58ef277c58ddd5`  
		Last Modified: Thu, 23 Apr 2020 04:18:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.6`

```console
$ docker pull mysql@sha256:852b5dee257c9c23ce410b7d005f9d8f04efa9998059780cd5a358d866c53dea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:5.6` - linux; amd64

```console
$ docker pull mysql@sha256:7d4df6c491e9b844b8c594c5607cea7465b42bd3d51db3d93359b3e8d06f1518
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.9 MB (102875758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43f75a12e7bae4f49a91d5c5c39bae41e0492f42eab91a54a4ba437b7093dcbf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 23 Apr 2020 00:23:03 GMT
ADD file:08ea1ff3fcd4efc24ab4f262cfa24e55e65844f6858e41a46fe0635d247f174d in / 
# Thu, 23 Apr 2020 00:23:03 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 04:16:04 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 23 Apr 2020 04:16:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 04:16:13 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 04:16:29 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 04:16:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 23 Apr 2020 04:16:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 04:16:44 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Thu, 23 Apr 2020 04:16:44 GMT
ENV MYSQL_MAJOR=5.6
# Thu, 23 Apr 2020 04:16:45 GMT
ENV MYSQL_VERSION=5.6.47-1debian9
# Thu, 23 Apr 2020 04:16:46 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ stretch mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Thu, 23 Apr 2020 04:17:10 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-server="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 777 /var/run/mysqld 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 23 Apr 2020 04:17:10 GMT
VOLUME [/var/lib/mysql]
# Thu, 23 Apr 2020 04:17:11 GMT
COPY file:b09451ebd8fb98d90335352b9649da1b3336a789513bb4ae725c9eadafd519b6 in /usr/local/bin/ 
# Thu, 23 Apr 2020 04:17:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Apr 2020 04:17:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 04:17:13 GMT
EXPOSE 3306
# Thu, 23 Apr 2020 04:17:13 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:b248fa9f6d2ae427ad7f00de3537ab256ae7eb413565f8be0773ee9b86ef57d4`  
		Last Modified: Thu, 23 Apr 2020 00:27:46 GMT  
		Size: 22.5 MB (22513488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0058702edba7456c09cc65fc8215cdb4de22e5b5619657b3429b4612e0782492`  
		Last Modified: Thu, 23 Apr 2020 04:18:41 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84e63f6f229769b34b9dc42ef242e26827f4ef62dc068b8cfb3978896d1f400f`  
		Last Modified: Thu, 23 Apr 2020 04:18:41 GMT  
		Size: 4.5 MB (4501274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ad333a340332086ec5356c921af17ee104cf83bc65316ebb8eba19e53baa07`  
		Last Modified: Thu, 23 Apr 2020 04:18:40 GMT  
		Size: 1.4 MB (1412350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3708a6b9545b82d874821a4e519265431f64c59be326f3a8d634c588abec0673`  
		Last Modified: Thu, 23 Apr 2020 04:18:39 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:442342ef4996aa063f2752b7f40a8814f35f583fccb430f62f58087db31d6431`  
		Last Modified: Thu, 23 Apr 2020 04:18:44 GMT  
		Size: 10.2 MB (10222752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecf24ffdea0f6a9b3a7ec50870603c50b164d3f65730cea120f246f1421a6952`  
		Last Modified: Thu, 23 Apr 2020 04:18:38 GMT  
		Size: 28.3 KB (28326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a02b8b4c83b0d89fe614d24955d1fe5bde1692e29caacdf6558a7e0ea178e95e`  
		Last Modified: Thu, 23 Apr 2020 04:18:38 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b1a4d0969f1da6a112e69c003bfbaa6cffe42a77ea2fad695dd76eedb91c460`  
		Last Modified: Thu, 23 Apr 2020 04:18:55 GMT  
		Size: 64.2 MB (64190215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d715f261d93c70db80a4699fad768e6c3bf49b306947440afd7176bf42e550d`  
		Last Modified: Thu, 23 Apr 2020 04:18:38 GMT  
		Size: 5.2 KB (5151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:140640d3c0e36c983a0e10500aa2a751e67a1a5c896cc9fb8a306168dc7af7fa`  
		Last Modified: Thu, 23 Apr 2020 04:18:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.6.48`

```console
$ docker pull mysql@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `mysql:5.7`

```console
$ docker pull mysql@sha256:95b4bc7c1b111906fdb7a39cd990dd99f21c594722735d059769b80312eb57a7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:5.7` - linux; amd64

```console
$ docker pull mysql@sha256:8044616c01e46c6bc826d205103a2b650a1679be2f34beab9bbf6c6f642df673
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.4 MB (158351512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d9483f9a7b21c87e0f5b9776c3e06567603c28c0062013eda127c968175f5e8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 23 Apr 2020 00:20:32 GMT
ADD file:9b8be2b52ee0fa31da1b6256099030b73546253a57e94cccb24605cd888bb74d in / 
# Thu, 23 Apr 2020 00:20:32 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 04:13:52 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 23 Apr 2020 04:13:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 04:13:59 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 04:14:08 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 04:14:09 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 23 Apr 2020 04:14:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 04:14:20 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Thu, 23 Apr 2020 04:15:08 GMT
ENV MYSQL_MAJOR=5.7
# Thu, 23 Apr 2020 04:15:09 GMT
ENV MYSQL_VERSION=5.7.29-1debian10
# Thu, 23 Apr 2020 04:15:10 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ buster mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Thu, 23 Apr 2020 04:15:49 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-server="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 777 /var/run/mysqld 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 23 Apr 2020 04:15:49 GMT
VOLUME [/var/lib/mysql]
# Thu, 23 Apr 2020 04:15:50 GMT
COPY file:b09451ebd8fb98d90335352b9649da1b3336a789513bb4ae725c9eadafd519b6 in /usr/local/bin/ 
# Thu, 23 Apr 2020 04:15:51 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Apr 2020 04:15:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 04:15:52 GMT
EXPOSE 3306 33060
# Thu, 23 Apr 2020 04:15:52 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:54fec2fa59d0a0de9cd2dec9850b36c43de451f1fd1c0a5bf8f1cf26a61a5da4`  
		Last Modified: Thu, 23 Apr 2020 00:25:10 GMT  
		Size: 27.1 MB (27098254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc6c614591231a51a8abf93a762208fd1aed3f72f3e3fd0b8907904e3c9a38b`  
		Last Modified: Thu, 23 Apr 2020 04:17:30 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:951c3d959c9d9548b3c320af7856e6e16c967daf7d280ac2607e49aa2b3816dd`  
		Last Modified: Thu, 23 Apr 2020 04:17:32 GMT  
		Size: 4.2 MB (4178101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05de4d0e206e076ed00d1b32a5104bcd7246484f51de192ba7d5b5c75fe215d0`  
		Last Modified: Thu, 23 Apr 2020 04:17:30 GMT  
		Size: 1.4 MB (1419225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:319f0394ef4231f3e9f43809855fba117032c697e51c94defda703f34a527b43`  
		Last Modified: Thu, 23 Apr 2020 04:17:29 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9185034607beae95fac5ee5b684c0182fa10a66b51ba65a7e81345e860b91c2`  
		Last Modified: Thu, 23 Apr 2020 04:17:35 GMT  
		Size: 13.4 MB (13443052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013a9c64dadc90a7aef7354825e9668f7b7667ad915df865cb4d05142a76938e`  
		Last Modified: Thu, 23 Apr 2020 04:17:28 GMT  
		Size: 2.4 KB (2395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58b7b840ebff81e42f4ba9bc82fe6da1012d22753693561022c1cadce29bf98e`  
		Last Modified: Thu, 23 Apr 2020 04:18:07 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b85c0abc43d54e9d83638b7ac1bdeca8c38dab7cda795c45541b52fd0fcda5e`  
		Last Modified: Thu, 23 Apr 2020 04:18:31 GMT  
		Size: 112.2 MB (112203157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf022f63e85cdffd7cfea4a44248b378f34553171463eaee142ef09aefa1f33`  
		Last Modified: Thu, 23 Apr 2020 04:18:07 GMT  
		Size: 5.1 KB (5135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35f7f707ce83e3b72c259b3e9e813cc5c10f2bd0f723193f3f58ef277c58ddd5`  
		Last Modified: Thu, 23 Apr 2020 04:18:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.30`

```console
$ docker pull mysql@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `mysql:8`

```console
$ docker pull mysql@sha256:9643e9fbd6330d10686f8922292dcb20995e7b792c17d4e94ddf95255f1d5449
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:8` - linux; amd64

```console
$ docker pull mysql@sha256:09de7b17af0c17d397e6b69ff841756b80074aed00c1e91d7bc0f3caa5512113
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.1 MB (159104807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c27e8e5fcfab7805cfed996b55e5e98f43fd7ee76e1516f20cba139c6a299c5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 23 Apr 2020 00:20:32 GMT
ADD file:9b8be2b52ee0fa31da1b6256099030b73546253a57e94cccb24605cd888bb74d in / 
# Thu, 23 Apr 2020 00:20:32 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 04:13:52 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 23 Apr 2020 04:13:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 04:13:59 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 04:14:08 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 04:14:09 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 23 Apr 2020 04:14:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 04:14:20 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Thu, 23 Apr 2020 04:14:20 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 23 Apr 2020 04:14:20 GMT
ENV MYSQL_VERSION=8.0.19-1debian10
# Thu, 23 Apr 2020 04:14:22 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ buster mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Thu, 23 Apr 2020 04:14:51 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-community-client="${MYSQL_VERSION}" mysql-community-server-core="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 777 /var/run/mysqld
# Thu, 23 Apr 2020 04:14:52 GMT
VOLUME [/var/lib/mysql]
# Thu, 23 Apr 2020 04:14:52 GMT
COPY dir:478f098f3681084f7493af1f04cbcd3eeda6f10e0dd2f5c740acd25328a73455 in /etc/mysql/ 
# Thu, 23 Apr 2020 04:14:53 GMT
COPY file:b09451ebd8fb98d90335352b9649da1b3336a789513bb4ae725c9eadafd519b6 in /usr/local/bin/ 
# Thu, 23 Apr 2020 04:14:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Apr 2020 04:14:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 04:14:55 GMT
EXPOSE 3306 33060
# Thu, 23 Apr 2020 04:14:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:54fec2fa59d0a0de9cd2dec9850b36c43de451f1fd1c0a5bf8f1cf26a61a5da4`  
		Last Modified: Thu, 23 Apr 2020 00:25:10 GMT  
		Size: 27.1 MB (27098254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc6c614591231a51a8abf93a762208fd1aed3f72f3e3fd0b8907904e3c9a38b`  
		Last Modified: Thu, 23 Apr 2020 04:17:30 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:951c3d959c9d9548b3c320af7856e6e16c967daf7d280ac2607e49aa2b3816dd`  
		Last Modified: Thu, 23 Apr 2020 04:17:32 GMT  
		Size: 4.2 MB (4178101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05de4d0e206e076ed00d1b32a5104bcd7246484f51de192ba7d5b5c75fe215d0`  
		Last Modified: Thu, 23 Apr 2020 04:17:30 GMT  
		Size: 1.4 MB (1419225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:319f0394ef4231f3e9f43809855fba117032c697e51c94defda703f34a527b43`  
		Last Modified: Thu, 23 Apr 2020 04:17:29 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9185034607beae95fac5ee5b684c0182fa10a66b51ba65a7e81345e860b91c2`  
		Last Modified: Thu, 23 Apr 2020 04:17:35 GMT  
		Size: 13.4 MB (13443052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013a9c64dadc90a7aef7354825e9668f7b7667ad915df865cb4d05142a76938e`  
		Last Modified: Thu, 23 Apr 2020 04:17:28 GMT  
		Size: 2.4 KB (2395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96d4c3d31f9fc0ab35d93dc1903fbc323bffa08916d6e36bb1ff94daf7cfdaae`  
		Last Modified: Thu, 23 Apr 2020 04:17:27 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785bc90808da2b19e21a428ac3175392a1c8305895f511d5a0ab33860e449f0e`  
		Last Modified: Thu, 23 Apr 2020 04:17:58 GMT  
		Size: 113.0 MB (112955549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1339cf094729be360a598b68a79a4e7f4161e8f36cf3ae03c483be2c6e92edd5`  
		Last Modified: Thu, 23 Apr 2020 04:17:27 GMT  
		Size: 901.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beb8f531cc379f34be8e909cb6ee7d80b4421550fef6eaf6f63e084870901b7f`  
		Last Modified: Thu, 23 Apr 2020 04:17:27 GMT  
		Size: 5.1 KB (5137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b40c9f6a9184482286ab917d42eae90352f951adbebef03fcd100d9a3b55dff`  
		Last Modified: Thu, 23 Apr 2020 04:17:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0`

```console
$ docker pull mysql@sha256:9643e9fbd6330d10686f8922292dcb20995e7b792c17d4e94ddf95255f1d5449
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:8.0` - linux; amd64

```console
$ docker pull mysql@sha256:09de7b17af0c17d397e6b69ff841756b80074aed00c1e91d7bc0f3caa5512113
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.1 MB (159104807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c27e8e5fcfab7805cfed996b55e5e98f43fd7ee76e1516f20cba139c6a299c5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 23 Apr 2020 00:20:32 GMT
ADD file:9b8be2b52ee0fa31da1b6256099030b73546253a57e94cccb24605cd888bb74d in / 
# Thu, 23 Apr 2020 00:20:32 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 04:13:52 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 23 Apr 2020 04:13:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 04:13:59 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 04:14:08 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 04:14:09 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 23 Apr 2020 04:14:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 04:14:20 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Thu, 23 Apr 2020 04:14:20 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 23 Apr 2020 04:14:20 GMT
ENV MYSQL_VERSION=8.0.19-1debian10
# Thu, 23 Apr 2020 04:14:22 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ buster mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Thu, 23 Apr 2020 04:14:51 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-community-client="${MYSQL_VERSION}" mysql-community-server-core="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 777 /var/run/mysqld
# Thu, 23 Apr 2020 04:14:52 GMT
VOLUME [/var/lib/mysql]
# Thu, 23 Apr 2020 04:14:52 GMT
COPY dir:478f098f3681084f7493af1f04cbcd3eeda6f10e0dd2f5c740acd25328a73455 in /etc/mysql/ 
# Thu, 23 Apr 2020 04:14:53 GMT
COPY file:b09451ebd8fb98d90335352b9649da1b3336a789513bb4ae725c9eadafd519b6 in /usr/local/bin/ 
# Thu, 23 Apr 2020 04:14:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Apr 2020 04:14:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 04:14:55 GMT
EXPOSE 3306 33060
# Thu, 23 Apr 2020 04:14:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:54fec2fa59d0a0de9cd2dec9850b36c43de451f1fd1c0a5bf8f1cf26a61a5da4`  
		Last Modified: Thu, 23 Apr 2020 00:25:10 GMT  
		Size: 27.1 MB (27098254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc6c614591231a51a8abf93a762208fd1aed3f72f3e3fd0b8907904e3c9a38b`  
		Last Modified: Thu, 23 Apr 2020 04:17:30 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:951c3d959c9d9548b3c320af7856e6e16c967daf7d280ac2607e49aa2b3816dd`  
		Last Modified: Thu, 23 Apr 2020 04:17:32 GMT  
		Size: 4.2 MB (4178101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05de4d0e206e076ed00d1b32a5104bcd7246484f51de192ba7d5b5c75fe215d0`  
		Last Modified: Thu, 23 Apr 2020 04:17:30 GMT  
		Size: 1.4 MB (1419225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:319f0394ef4231f3e9f43809855fba117032c697e51c94defda703f34a527b43`  
		Last Modified: Thu, 23 Apr 2020 04:17:29 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9185034607beae95fac5ee5b684c0182fa10a66b51ba65a7e81345e860b91c2`  
		Last Modified: Thu, 23 Apr 2020 04:17:35 GMT  
		Size: 13.4 MB (13443052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013a9c64dadc90a7aef7354825e9668f7b7667ad915df865cb4d05142a76938e`  
		Last Modified: Thu, 23 Apr 2020 04:17:28 GMT  
		Size: 2.4 KB (2395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96d4c3d31f9fc0ab35d93dc1903fbc323bffa08916d6e36bb1ff94daf7cfdaae`  
		Last Modified: Thu, 23 Apr 2020 04:17:27 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785bc90808da2b19e21a428ac3175392a1c8305895f511d5a0ab33860e449f0e`  
		Last Modified: Thu, 23 Apr 2020 04:17:58 GMT  
		Size: 113.0 MB (112955549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1339cf094729be360a598b68a79a4e7f4161e8f36cf3ae03c483be2c6e92edd5`  
		Last Modified: Thu, 23 Apr 2020 04:17:27 GMT  
		Size: 901.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beb8f531cc379f34be8e909cb6ee7d80b4421550fef6eaf6f63e084870901b7f`  
		Last Modified: Thu, 23 Apr 2020 04:17:27 GMT  
		Size: 5.1 KB (5137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b40c9f6a9184482286ab917d42eae90352f951adbebef03fcd100d9a3b55dff`  
		Last Modified: Thu, 23 Apr 2020 04:17:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.20`

```console
$ docker pull mysql@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `mysql:latest`

```console
$ docker pull mysql@sha256:9643e9fbd6330d10686f8922292dcb20995e7b792c17d4e94ddf95255f1d5449
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:latest` - linux; amd64

```console
$ docker pull mysql@sha256:09de7b17af0c17d397e6b69ff841756b80074aed00c1e91d7bc0f3caa5512113
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.1 MB (159104807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c27e8e5fcfab7805cfed996b55e5e98f43fd7ee76e1516f20cba139c6a299c5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 23 Apr 2020 00:20:32 GMT
ADD file:9b8be2b52ee0fa31da1b6256099030b73546253a57e94cccb24605cd888bb74d in / 
# Thu, 23 Apr 2020 00:20:32 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 04:13:52 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 23 Apr 2020 04:13:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 04:13:59 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 04:14:08 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 04:14:09 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 23 Apr 2020 04:14:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 04:14:20 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Thu, 23 Apr 2020 04:14:20 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 23 Apr 2020 04:14:20 GMT
ENV MYSQL_VERSION=8.0.19-1debian10
# Thu, 23 Apr 2020 04:14:22 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ buster mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Thu, 23 Apr 2020 04:14:51 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-community-client="${MYSQL_VERSION}" mysql-community-server-core="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 777 /var/run/mysqld
# Thu, 23 Apr 2020 04:14:52 GMT
VOLUME [/var/lib/mysql]
# Thu, 23 Apr 2020 04:14:52 GMT
COPY dir:478f098f3681084f7493af1f04cbcd3eeda6f10e0dd2f5c740acd25328a73455 in /etc/mysql/ 
# Thu, 23 Apr 2020 04:14:53 GMT
COPY file:b09451ebd8fb98d90335352b9649da1b3336a789513bb4ae725c9eadafd519b6 in /usr/local/bin/ 
# Thu, 23 Apr 2020 04:14:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Apr 2020 04:14:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 04:14:55 GMT
EXPOSE 3306 33060
# Thu, 23 Apr 2020 04:14:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:54fec2fa59d0a0de9cd2dec9850b36c43de451f1fd1c0a5bf8f1cf26a61a5da4`  
		Last Modified: Thu, 23 Apr 2020 00:25:10 GMT  
		Size: 27.1 MB (27098254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc6c614591231a51a8abf93a762208fd1aed3f72f3e3fd0b8907904e3c9a38b`  
		Last Modified: Thu, 23 Apr 2020 04:17:30 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:951c3d959c9d9548b3c320af7856e6e16c967daf7d280ac2607e49aa2b3816dd`  
		Last Modified: Thu, 23 Apr 2020 04:17:32 GMT  
		Size: 4.2 MB (4178101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05de4d0e206e076ed00d1b32a5104bcd7246484f51de192ba7d5b5c75fe215d0`  
		Last Modified: Thu, 23 Apr 2020 04:17:30 GMT  
		Size: 1.4 MB (1419225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:319f0394ef4231f3e9f43809855fba117032c697e51c94defda703f34a527b43`  
		Last Modified: Thu, 23 Apr 2020 04:17:29 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9185034607beae95fac5ee5b684c0182fa10a66b51ba65a7e81345e860b91c2`  
		Last Modified: Thu, 23 Apr 2020 04:17:35 GMT  
		Size: 13.4 MB (13443052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013a9c64dadc90a7aef7354825e9668f7b7667ad915df865cb4d05142a76938e`  
		Last Modified: Thu, 23 Apr 2020 04:17:28 GMT  
		Size: 2.4 KB (2395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96d4c3d31f9fc0ab35d93dc1903fbc323bffa08916d6e36bb1ff94daf7cfdaae`  
		Last Modified: Thu, 23 Apr 2020 04:17:27 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785bc90808da2b19e21a428ac3175392a1c8305895f511d5a0ab33860e449f0e`  
		Last Modified: Thu, 23 Apr 2020 04:17:58 GMT  
		Size: 113.0 MB (112955549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1339cf094729be360a598b68a79a4e7f4161e8f36cf3ae03c483be2c6e92edd5`  
		Last Modified: Thu, 23 Apr 2020 04:17:27 GMT  
		Size: 901.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beb8f531cc379f34be8e909cb6ee7d80b4421550fef6eaf6f63e084870901b7f`  
		Last Modified: Thu, 23 Apr 2020 04:17:27 GMT  
		Size: 5.1 KB (5137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b40c9f6a9184482286ab917d42eae90352f951adbebef03fcd100d9a3b55dff`  
		Last Modified: Thu, 23 Apr 2020 04:17:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
