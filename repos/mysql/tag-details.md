<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mysql`

-	[`mysql:5`](#mysql5)
-	[`mysql:5.6`](#mysql56)
-	[`mysql:5.6.49`](#mysql5649)
-	[`mysql:5.7`](#mysql57)
-	[`mysql:5.7.31`](#mysql5731)
-	[`mysql:8`](#mysql8)
-	[`mysql:8.0`](#mysql80)
-	[`mysql:8.0.21`](#mysql8021)
-	[`mysql:latest`](#mysqllatest)

## `mysql:5`

```console
$ docker pull mysql@sha256:32f9d9a069f7a735e28fd44ea944d53c61f990ba71460c5c183e610854ca4854
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:5` - linux; amd64

```console
$ docker pull mysql@sha256:0563b36ec2d1a262f79e1d8562e61f642a0f64f93306d8a709047cdea0444d0a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.4 MB (154404894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cfcce23593a93135ca6dbf3ed544d1db9324d4c40b5c0d56958165bfaa2d46a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 09 Jun 2020 01:20:56 GMT
ADD file:4d35f6c8bbbe6801cc5f44989730fb6d349a644ecb36eca481e7df25842d6321 in / 
# Tue, 09 Jun 2020 01:20:56 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 07:20:09 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 09 Jun 2020 07:20:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 07:20:15 GMT
ENV GOSU_VERSION=1.12
# Tue, 09 Jun 2020 07:20:24 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 09 Jun 2020 07:20:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 09 Jun 2020 07:20:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 07:20:32 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Tue, 09 Jun 2020 07:20:55 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 09 Jun 2020 07:20:55 GMT
ENV MYSQL_VERSION=5.7.30-1debian10
# Tue, 09 Jun 2020 07:20:56 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ buster mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Tue, 09 Jun 2020 07:21:17 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-server="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 777 /var/run/mysqld 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Tue, 09 Jun 2020 07:21:17 GMT
VOLUME [/var/lib/mysql]
# Tue, 09 Jun 2020 07:21:17 GMT
COPY file:7cbb26bbdb8e71b36aafda38dbac08caa641714a19991b86cde77daf3286ec11 in /usr/local/bin/ 
# Tue, 09 Jun 2020 07:21:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 09 Jun 2020 07:21:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Jun 2020 07:21:18 GMT
EXPOSE 3306 33060
# Tue, 09 Jun 2020 07:21:19 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8559a31e96f442f2c7b6da49d6c84705f98a39d8be10b3f5f14821d0ee8417df`  
		Last Modified: Tue, 09 Jun 2020 01:25:50 GMT  
		Size: 27.1 MB (27098265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d51ce1c2e5758ad66758028c37b3224bff94ee2cdb716215a91dde7b754443f3`  
		Last Modified: Tue, 09 Jun 2020 07:22:27 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2344adc4858d61b5c9424d49320703bec8d5e1044378a83cae39dbdc49acba7`  
		Last Modified: Tue, 09 Jun 2020 07:22:28 GMT  
		Size: 4.2 MB (4178032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf3ceff18fca19f16c7108d4c0dfcacc194f1762f80712e854c16ec164733aa`  
		Last Modified: Tue, 09 Jun 2020 07:22:26 GMT  
		Size: 1.4 MB (1419203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16da0c38dc5bad1047f9912514e8232bf9d4d40c3790e94e9c25d5f48ac39ffd`  
		Last Modified: Tue, 09 Jun 2020 07:22:26 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b905d1797e97cbecb5a12655cab5c3df92736805574af0f96477c98d7a27411c`  
		Last Modified: Tue, 09 Jun 2020 07:22:30 GMT  
		Size: 13.4 MB (13442691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b50d1c6b05cfc51651f145028c85c8eb3a5c8c02b0c4537aad065ad3083150d`  
		Last Modified: Tue, 09 Jun 2020 07:22:25 GMT  
		Size: 2.4 KB (2393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d85174a871441e82995f5577b3bbd247e53ed25d5a75a709b3b63a638c07457f`  
		Last Modified: Tue, 09 Jun 2020 07:22:52 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ad33703fa83c968fe06b3576f6a202630ad251f8ff729384d32b15e1fa5344`  
		Last Modified: Tue, 09 Jun 2020 07:23:10 GMT  
		Size: 108.3 MB (108256979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a5433ce20d474c9cb1b3ae428f1b804c7ae866ca4c34e01af1bfc9201ae51a`  
		Last Modified: Tue, 09 Jun 2020 07:22:52 GMT  
		Size: 5.1 KB (5144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dcd2a278b4adab247dd447b0d8fd2b284dbcaffbf9914a2b1da2c9f3f98e887`  
		Last Modified: Tue, 09 Jun 2020 07:22:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.6`

```console
$ docker pull mysql@sha256:2bf1a0a05a6ad437dcac6689e48a9c33774ac92c6213fce2c4196343210592f3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:5.6` - linux; amd64

```console
$ docker pull mysql@sha256:77c18189a775dac4c281de075e46a3c910dcca3775244667d7b8b93e251dbea6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.9 MB (102886725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8de95e6026c348c1206d35a9ba7a043ff71885573dace41b14e4236c44cba593`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 09 Jun 2020 01:23:35 GMT
ADD file:57b431451a292755d0f13673f5f3bea9f62aea36c7a1b59d34d7d200ba134fea in / 
# Tue, 09 Jun 2020 01:23:35 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 07:21:25 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 09 Jun 2020 07:21:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 07:21:31 GMT
ENV GOSU_VERSION=1.12
# Tue, 09 Jun 2020 07:21:42 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 09 Jun 2020 07:21:43 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 09 Jun 2020 07:21:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 07:21:52 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Tue, 09 Jun 2020 07:21:52 GMT
ENV MYSQL_MAJOR=5.6
# Tue, 09 Jun 2020 07:21:52 GMT
ENV MYSQL_VERSION=5.6.48-1debian9
# Tue, 09 Jun 2020 07:21:53 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ stretch mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Tue, 09 Jun 2020 07:22:11 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-server="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 777 /var/run/mysqld 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Tue, 09 Jun 2020 07:22:11 GMT
VOLUME [/var/lib/mysql]
# Tue, 09 Jun 2020 07:22:11 GMT
COPY file:7cbb26bbdb8e71b36aafda38dbac08caa641714a19991b86cde77daf3286ec11 in /usr/local/bin/ 
# Tue, 09 Jun 2020 07:22:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 09 Jun 2020 07:22:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Jun 2020 07:22:12 GMT
EXPOSE 3306
# Tue, 09 Jun 2020 07:22:12 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7d2977b12acb33f192e3f20b7e15a467cc8f3f5124a15d975a6d4afe5fa3d258`  
		Last Modified: Tue, 09 Jun 2020 01:28:13 GMT  
		Size: 22.5 MB (22519600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb8400e7f070d8f49a4948426702454922382a6643db2a8547614258185eb47`  
		Last Modified: Tue, 09 Jun 2020 07:23:18 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:234877fbb165b4219127d8d8c5a36c89533f0fd8496fedea46d3be950993dc1f`  
		Last Modified: Tue, 09 Jun 2020 07:23:19 GMT  
		Size: 4.5 MB (4501264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fe1021f12f383728116c00d312032068542e5e5b39d014efaea58a52fa3714f`  
		Last Modified: Tue, 09 Jun 2020 07:23:19 GMT  
		Size: 1.4 MB (1412012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e36fe6b53f00d381bd369862bec14d84d57c10743ebb876c61c7689ae8699eb`  
		Last Modified: Tue, 09 Jun 2020 07:23:17 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:996ec709c11ba48cf0d54a4283187f9ba9ec04ca24cb1265261d344705d7fd8a`  
		Last Modified: Tue, 09 Jun 2020 07:23:20 GMT  
		Size: 10.2 MB (10222890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5198b7523387a277c164ae93f3d4d6c81f8b363fa3d9a0a7b99e031e49d3b328`  
		Last Modified: Tue, 09 Jun 2020 07:23:16 GMT  
		Size: 28.3 KB (28323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc9bdad4dcc02e0727b48128a3a1aeb20097d5a19c8cbaa118fbde668ef540c4`  
		Last Modified: Tue, 09 Jun 2020 07:23:16 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:380cd37ad979bf6d7b7994d45391fadae80e3d980f2677da5147a2021e50abc0`  
		Last Modified: Tue, 09 Jun 2020 07:23:28 GMT  
		Size: 64.2 MB (64195285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d64465acf034b5bfaf5ec5d105bed9415c1756e5aa7eb6bbb552c67dbd64d2f1`  
		Last Modified: Tue, 09 Jun 2020 07:23:17 GMT  
		Size: 5.2 KB (5158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4ee6606b3ab33681e4d218a127f8a44580c71b7cc137c56f6dc513acf4a8612`  
		Last Modified: Tue, 09 Jun 2020 07:23:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.6.49`

**does not exist** (yet?)

## `mysql:5.7`

```console
$ docker pull mysql@sha256:32f9d9a069f7a735e28fd44ea944d53c61f990ba71460c5c183e610854ca4854
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:5.7` - linux; amd64

```console
$ docker pull mysql@sha256:0563b36ec2d1a262f79e1d8562e61f642a0f64f93306d8a709047cdea0444d0a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.4 MB (154404894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cfcce23593a93135ca6dbf3ed544d1db9324d4c40b5c0d56958165bfaa2d46a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 09 Jun 2020 01:20:56 GMT
ADD file:4d35f6c8bbbe6801cc5f44989730fb6d349a644ecb36eca481e7df25842d6321 in / 
# Tue, 09 Jun 2020 01:20:56 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 07:20:09 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 09 Jun 2020 07:20:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 07:20:15 GMT
ENV GOSU_VERSION=1.12
# Tue, 09 Jun 2020 07:20:24 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 09 Jun 2020 07:20:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 09 Jun 2020 07:20:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 07:20:32 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Tue, 09 Jun 2020 07:20:55 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 09 Jun 2020 07:20:55 GMT
ENV MYSQL_VERSION=5.7.30-1debian10
# Tue, 09 Jun 2020 07:20:56 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ buster mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Tue, 09 Jun 2020 07:21:17 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-server="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 777 /var/run/mysqld 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Tue, 09 Jun 2020 07:21:17 GMT
VOLUME [/var/lib/mysql]
# Tue, 09 Jun 2020 07:21:17 GMT
COPY file:7cbb26bbdb8e71b36aafda38dbac08caa641714a19991b86cde77daf3286ec11 in /usr/local/bin/ 
# Tue, 09 Jun 2020 07:21:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 09 Jun 2020 07:21:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Jun 2020 07:21:18 GMT
EXPOSE 3306 33060
# Tue, 09 Jun 2020 07:21:19 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8559a31e96f442f2c7b6da49d6c84705f98a39d8be10b3f5f14821d0ee8417df`  
		Last Modified: Tue, 09 Jun 2020 01:25:50 GMT  
		Size: 27.1 MB (27098265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d51ce1c2e5758ad66758028c37b3224bff94ee2cdb716215a91dde7b754443f3`  
		Last Modified: Tue, 09 Jun 2020 07:22:27 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2344adc4858d61b5c9424d49320703bec8d5e1044378a83cae39dbdc49acba7`  
		Last Modified: Tue, 09 Jun 2020 07:22:28 GMT  
		Size: 4.2 MB (4178032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf3ceff18fca19f16c7108d4c0dfcacc194f1762f80712e854c16ec164733aa`  
		Last Modified: Tue, 09 Jun 2020 07:22:26 GMT  
		Size: 1.4 MB (1419203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16da0c38dc5bad1047f9912514e8232bf9d4d40c3790e94e9c25d5f48ac39ffd`  
		Last Modified: Tue, 09 Jun 2020 07:22:26 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b905d1797e97cbecb5a12655cab5c3df92736805574af0f96477c98d7a27411c`  
		Last Modified: Tue, 09 Jun 2020 07:22:30 GMT  
		Size: 13.4 MB (13442691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b50d1c6b05cfc51651f145028c85c8eb3a5c8c02b0c4537aad065ad3083150d`  
		Last Modified: Tue, 09 Jun 2020 07:22:25 GMT  
		Size: 2.4 KB (2393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d85174a871441e82995f5577b3bbd247e53ed25d5a75a709b3b63a638c07457f`  
		Last Modified: Tue, 09 Jun 2020 07:22:52 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ad33703fa83c968fe06b3576f6a202630ad251f8ff729384d32b15e1fa5344`  
		Last Modified: Tue, 09 Jun 2020 07:23:10 GMT  
		Size: 108.3 MB (108256979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a5433ce20d474c9cb1b3ae428f1b804c7ae866ca4c34e01af1bfc9201ae51a`  
		Last Modified: Tue, 09 Jun 2020 07:22:52 GMT  
		Size: 5.1 KB (5144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dcd2a278b4adab247dd447b0d8fd2b284dbcaffbf9914a2b1da2c9f3f98e887`  
		Last Modified: Tue, 09 Jun 2020 07:22:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.31`

**does not exist** (yet?)

## `mysql:8`

```console
$ docker pull mysql@sha256:8b7b328a7ff6de46ef96bcf83af048cb00a1c86282bfca0cb119c84568b4caf6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:8` - linux; amd64

```console
$ docker pull mysql@sha256:0ba38ea9c478d1e98b2f0bc0cee5a62345c9f06f78c4b48123bdc70d8d224686
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.6 MB (157635446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be0dbf01a0f3f46fc8c88b67696e74e7005c3e16d9071032fa0cd89773771576`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 09 Jun 2020 01:20:56 GMT
ADD file:4d35f6c8bbbe6801cc5f44989730fb6d349a644ecb36eca481e7df25842d6321 in / 
# Tue, 09 Jun 2020 01:20:56 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 07:20:09 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 09 Jun 2020 07:20:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 07:20:15 GMT
ENV GOSU_VERSION=1.12
# Tue, 09 Jun 2020 07:20:24 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 09 Jun 2020 07:20:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 09 Jun 2020 07:20:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 07:20:32 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Tue, 09 Jun 2020 07:20:32 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 09 Jun 2020 07:20:32 GMT
ENV MYSQL_VERSION=8.0.20-1debian10
# Tue, 09 Jun 2020 07:20:33 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ buster mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Tue, 09 Jun 2020 07:20:49 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-community-client="${MYSQL_VERSION}" mysql-community-server-core="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 777 /var/run/mysqld
# Tue, 09 Jun 2020 07:20:49 GMT
VOLUME [/var/lib/mysql]
# Tue, 09 Jun 2020 07:20:50 GMT
COPY dir:478f098f3681084f7493af1f04cbcd3eeda6f10e0dd2f5c740acd25328a73455 in /etc/mysql/ 
# Tue, 09 Jun 2020 07:20:50 GMT
COPY file:7cbb26bbdb8e71b36aafda38dbac08caa641714a19991b86cde77daf3286ec11 in /usr/local/bin/ 
# Tue, 09 Jun 2020 07:20:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 09 Jun 2020 07:20:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Jun 2020 07:20:51 GMT
EXPOSE 3306 33060
# Tue, 09 Jun 2020 07:20:51 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8559a31e96f442f2c7b6da49d6c84705f98a39d8be10b3f5f14821d0ee8417df`  
		Last Modified: Tue, 09 Jun 2020 01:25:50 GMT  
		Size: 27.1 MB (27098265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d51ce1c2e5758ad66758028c37b3224bff94ee2cdb716215a91dde7b754443f3`  
		Last Modified: Tue, 09 Jun 2020 07:22:27 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2344adc4858d61b5c9424d49320703bec8d5e1044378a83cae39dbdc49acba7`  
		Last Modified: Tue, 09 Jun 2020 07:22:28 GMT  
		Size: 4.2 MB (4178032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf3ceff18fca19f16c7108d4c0dfcacc194f1762f80712e854c16ec164733aa`  
		Last Modified: Tue, 09 Jun 2020 07:22:26 GMT  
		Size: 1.4 MB (1419203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16da0c38dc5bad1047f9912514e8232bf9d4d40c3790e94e9c25d5f48ac39ffd`  
		Last Modified: Tue, 09 Jun 2020 07:22:26 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b905d1797e97cbecb5a12655cab5c3df92736805574af0f96477c98d7a27411c`  
		Last Modified: Tue, 09 Jun 2020 07:22:30 GMT  
		Size: 13.4 MB (13442691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b50d1c6b05cfc51651f145028c85c8eb3a5c8c02b0c4537aad065ad3083150d`  
		Last Modified: Tue, 09 Jun 2020 07:22:25 GMT  
		Size: 2.4 KB (2393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c75914a65ca227bf8a305dcc9e91a46cf9ac85098e6136f052121370d2ba02c2`  
		Last Modified: Tue, 09 Jun 2020 07:22:24 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae8042bdd096b7a5e2e85ca88e744eb2d61896749e1643411ff1af2b1929aef`  
		Last Modified: Tue, 09 Jun 2020 07:22:45 GMT  
		Size: 111.5 MB (111486634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:453ac13c00a353d3106bf14a375cab7f6661ec7c4854528091ff3cc20184c3bd`  
		Last Modified: Tue, 09 Jun 2020 07:22:24 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e680cd72f08cd6cb9db395c62485983f6892234f83bbf35a27f5f80f1f6e568`  
		Last Modified: Tue, 09 Jun 2020 07:22:24 GMT  
		Size: 5.1 KB (5143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b5dc864b6c283cb3dc29c66714099ef6103a1f5de7923a5c1ea63e6d597279`  
		Last Modified: Tue, 09 Jun 2020 07:22:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0`

```console
$ docker pull mysql@sha256:8b7b328a7ff6de46ef96bcf83af048cb00a1c86282bfca0cb119c84568b4caf6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:8.0` - linux; amd64

```console
$ docker pull mysql@sha256:0ba38ea9c478d1e98b2f0bc0cee5a62345c9f06f78c4b48123bdc70d8d224686
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.6 MB (157635446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be0dbf01a0f3f46fc8c88b67696e74e7005c3e16d9071032fa0cd89773771576`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 09 Jun 2020 01:20:56 GMT
ADD file:4d35f6c8bbbe6801cc5f44989730fb6d349a644ecb36eca481e7df25842d6321 in / 
# Tue, 09 Jun 2020 01:20:56 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 07:20:09 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 09 Jun 2020 07:20:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 07:20:15 GMT
ENV GOSU_VERSION=1.12
# Tue, 09 Jun 2020 07:20:24 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 09 Jun 2020 07:20:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 09 Jun 2020 07:20:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 07:20:32 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Tue, 09 Jun 2020 07:20:32 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 09 Jun 2020 07:20:32 GMT
ENV MYSQL_VERSION=8.0.20-1debian10
# Tue, 09 Jun 2020 07:20:33 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ buster mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Tue, 09 Jun 2020 07:20:49 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-community-client="${MYSQL_VERSION}" mysql-community-server-core="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 777 /var/run/mysqld
# Tue, 09 Jun 2020 07:20:49 GMT
VOLUME [/var/lib/mysql]
# Tue, 09 Jun 2020 07:20:50 GMT
COPY dir:478f098f3681084f7493af1f04cbcd3eeda6f10e0dd2f5c740acd25328a73455 in /etc/mysql/ 
# Tue, 09 Jun 2020 07:20:50 GMT
COPY file:7cbb26bbdb8e71b36aafda38dbac08caa641714a19991b86cde77daf3286ec11 in /usr/local/bin/ 
# Tue, 09 Jun 2020 07:20:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 09 Jun 2020 07:20:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Jun 2020 07:20:51 GMT
EXPOSE 3306 33060
# Tue, 09 Jun 2020 07:20:51 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8559a31e96f442f2c7b6da49d6c84705f98a39d8be10b3f5f14821d0ee8417df`  
		Last Modified: Tue, 09 Jun 2020 01:25:50 GMT  
		Size: 27.1 MB (27098265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d51ce1c2e5758ad66758028c37b3224bff94ee2cdb716215a91dde7b754443f3`  
		Last Modified: Tue, 09 Jun 2020 07:22:27 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2344adc4858d61b5c9424d49320703bec8d5e1044378a83cae39dbdc49acba7`  
		Last Modified: Tue, 09 Jun 2020 07:22:28 GMT  
		Size: 4.2 MB (4178032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf3ceff18fca19f16c7108d4c0dfcacc194f1762f80712e854c16ec164733aa`  
		Last Modified: Tue, 09 Jun 2020 07:22:26 GMT  
		Size: 1.4 MB (1419203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16da0c38dc5bad1047f9912514e8232bf9d4d40c3790e94e9c25d5f48ac39ffd`  
		Last Modified: Tue, 09 Jun 2020 07:22:26 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b905d1797e97cbecb5a12655cab5c3df92736805574af0f96477c98d7a27411c`  
		Last Modified: Tue, 09 Jun 2020 07:22:30 GMT  
		Size: 13.4 MB (13442691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b50d1c6b05cfc51651f145028c85c8eb3a5c8c02b0c4537aad065ad3083150d`  
		Last Modified: Tue, 09 Jun 2020 07:22:25 GMT  
		Size: 2.4 KB (2393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c75914a65ca227bf8a305dcc9e91a46cf9ac85098e6136f052121370d2ba02c2`  
		Last Modified: Tue, 09 Jun 2020 07:22:24 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae8042bdd096b7a5e2e85ca88e744eb2d61896749e1643411ff1af2b1929aef`  
		Last Modified: Tue, 09 Jun 2020 07:22:45 GMT  
		Size: 111.5 MB (111486634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:453ac13c00a353d3106bf14a375cab7f6661ec7c4854528091ff3cc20184c3bd`  
		Last Modified: Tue, 09 Jun 2020 07:22:24 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e680cd72f08cd6cb9db395c62485983f6892234f83bbf35a27f5f80f1f6e568`  
		Last Modified: Tue, 09 Jun 2020 07:22:24 GMT  
		Size: 5.1 KB (5143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b5dc864b6c283cb3dc29c66714099ef6103a1f5de7923a5c1ea63e6d597279`  
		Last Modified: Tue, 09 Jun 2020 07:22:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.21`

**does not exist** (yet?)

## `mysql:latest`

```console
$ docker pull mysql@sha256:8b7b328a7ff6de46ef96bcf83af048cb00a1c86282bfca0cb119c84568b4caf6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:latest` - linux; amd64

```console
$ docker pull mysql@sha256:0ba38ea9c478d1e98b2f0bc0cee5a62345c9f06f78c4b48123bdc70d8d224686
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.6 MB (157635446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be0dbf01a0f3f46fc8c88b67696e74e7005c3e16d9071032fa0cd89773771576`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 09 Jun 2020 01:20:56 GMT
ADD file:4d35f6c8bbbe6801cc5f44989730fb6d349a644ecb36eca481e7df25842d6321 in / 
# Tue, 09 Jun 2020 01:20:56 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 07:20:09 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 09 Jun 2020 07:20:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 07:20:15 GMT
ENV GOSU_VERSION=1.12
# Tue, 09 Jun 2020 07:20:24 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 09 Jun 2020 07:20:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 09 Jun 2020 07:20:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 07:20:32 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Tue, 09 Jun 2020 07:20:32 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 09 Jun 2020 07:20:32 GMT
ENV MYSQL_VERSION=8.0.20-1debian10
# Tue, 09 Jun 2020 07:20:33 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ buster mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Tue, 09 Jun 2020 07:20:49 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-community-client="${MYSQL_VERSION}" mysql-community-server-core="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 777 /var/run/mysqld
# Tue, 09 Jun 2020 07:20:49 GMT
VOLUME [/var/lib/mysql]
# Tue, 09 Jun 2020 07:20:50 GMT
COPY dir:478f098f3681084f7493af1f04cbcd3eeda6f10e0dd2f5c740acd25328a73455 in /etc/mysql/ 
# Tue, 09 Jun 2020 07:20:50 GMT
COPY file:7cbb26bbdb8e71b36aafda38dbac08caa641714a19991b86cde77daf3286ec11 in /usr/local/bin/ 
# Tue, 09 Jun 2020 07:20:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 09 Jun 2020 07:20:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Jun 2020 07:20:51 GMT
EXPOSE 3306 33060
# Tue, 09 Jun 2020 07:20:51 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8559a31e96f442f2c7b6da49d6c84705f98a39d8be10b3f5f14821d0ee8417df`  
		Last Modified: Tue, 09 Jun 2020 01:25:50 GMT  
		Size: 27.1 MB (27098265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d51ce1c2e5758ad66758028c37b3224bff94ee2cdb716215a91dde7b754443f3`  
		Last Modified: Tue, 09 Jun 2020 07:22:27 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2344adc4858d61b5c9424d49320703bec8d5e1044378a83cae39dbdc49acba7`  
		Last Modified: Tue, 09 Jun 2020 07:22:28 GMT  
		Size: 4.2 MB (4178032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf3ceff18fca19f16c7108d4c0dfcacc194f1762f80712e854c16ec164733aa`  
		Last Modified: Tue, 09 Jun 2020 07:22:26 GMT  
		Size: 1.4 MB (1419203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16da0c38dc5bad1047f9912514e8232bf9d4d40c3790e94e9c25d5f48ac39ffd`  
		Last Modified: Tue, 09 Jun 2020 07:22:26 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b905d1797e97cbecb5a12655cab5c3df92736805574af0f96477c98d7a27411c`  
		Last Modified: Tue, 09 Jun 2020 07:22:30 GMT  
		Size: 13.4 MB (13442691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b50d1c6b05cfc51651f145028c85c8eb3a5c8c02b0c4537aad065ad3083150d`  
		Last Modified: Tue, 09 Jun 2020 07:22:25 GMT  
		Size: 2.4 KB (2393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c75914a65ca227bf8a305dcc9e91a46cf9ac85098e6136f052121370d2ba02c2`  
		Last Modified: Tue, 09 Jun 2020 07:22:24 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae8042bdd096b7a5e2e85ca88e744eb2d61896749e1643411ff1af2b1929aef`  
		Last Modified: Tue, 09 Jun 2020 07:22:45 GMT  
		Size: 111.5 MB (111486634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:453ac13c00a353d3106bf14a375cab7f6661ec7c4854528091ff3cc20184c3bd`  
		Last Modified: Tue, 09 Jun 2020 07:22:24 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e680cd72f08cd6cb9db395c62485983f6892234f83bbf35a27f5f80f1f6e568`  
		Last Modified: Tue, 09 Jun 2020 07:22:24 GMT  
		Size: 5.1 KB (5143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b5dc864b6c283cb3dc29c66714099ef6103a1f5de7923a5c1ea63e6d597279`  
		Last Modified: Tue, 09 Jun 2020 07:22:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
