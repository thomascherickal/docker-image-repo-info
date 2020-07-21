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
$ docker pull mysql@sha256:ea560da3b6f2f3ad79fd76652cb9031407c5112246a6fb5724ea895e95d74032
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:5` - linux; amd64

```console
$ docker pull mysql@sha256:300728110cb9c46bba70d3f888118bf7ad7a270035fafef9d0e912a4bd619633
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.5 MB (154475860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d05c76dbbfcf3e1d969eecc04d0aa461e0f95204f6833f62edb73cca7b62fcd4`
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
# Tue, 14 Jul 2020 02:45:46 GMT
ENV MYSQL_VERSION=5.7.31-1debian10
# Tue, 14 Jul 2020 02:45:46 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ buster mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Tue, 14 Jul 2020 02:46:12 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-server="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 777 /var/run/mysqld 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Tue, 14 Jul 2020 02:46:12 GMT
VOLUME [/var/lib/mysql]
# Tue, 14 Jul 2020 02:46:13 GMT
COPY file:7cbb26bbdb8e71b36aafda38dbac08caa641714a19991b86cde77daf3286ec11 in /usr/local/bin/ 
# Tue, 14 Jul 2020 02:46:14 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 14 Jul 2020 02:46:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Jul 2020 02:46:14 GMT
EXPOSE 3306 33060
# Tue, 14 Jul 2020 02:46:14 GMT
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
	-	`sha256:0a52a5c57cd9a5d74b8de5352ddf8168ae29c0ec8bfac2bf0d4dff474d65f5df`  
		Last Modified: Tue, 14 Jul 2020 02:47:25 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b816a39d367faf0c8d5d5bae89c8224f2747301c7982084550cf31e5a34157f`  
		Last Modified: Tue, 14 Jul 2020 02:47:47 GMT  
		Size: 108.3 MB (108327942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ee22d6b3bb0dd4aa4449fba002e4f2fa9582eef2d42c6eb094d61430ce78cc`  
		Last Modified: Tue, 14 Jul 2020 02:47:25 GMT  
		Size: 5.1 KB (5146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e517c3d2ba35e1ea78f8580cc8ba7ce000cb233b683a19711a006b7842c3df8e`  
		Last Modified: Tue, 14 Jul 2020 02:47:25 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.6`

```console
$ docker pull mysql@sha256:19a164794d3cef15c9ac44754604fa079adb448f82d40e4b8be8381148c785fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:5.6` - linux; amd64

```console
$ docker pull mysql@sha256:71c6d751d76080fb06737e9306c63b38f630d48e3869a3939e8483747c18a601
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.9 MB (102924270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01ba04febd24365f377e0e5d8c7d5612520bffb1f3fded337dfbf46fbf6fd3b6`
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
# Tue, 14 Jul 2020 02:46:20 GMT
ENV MYSQL_VERSION=5.6.49-1debian9
# Tue, 14 Jul 2020 02:46:20 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ stretch mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Tue, 14 Jul 2020 02:46:42 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-server="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 777 /var/run/mysqld 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Tue, 14 Jul 2020 02:46:42 GMT
VOLUME [/var/lib/mysql]
# Tue, 14 Jul 2020 02:46:42 GMT
COPY file:7cbb26bbdb8e71b36aafda38dbac08caa641714a19991b86cde77daf3286ec11 in /usr/local/bin/ 
# Tue, 14 Jul 2020 02:46:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 14 Jul 2020 02:46:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Jul 2020 02:46:43 GMT
EXPOSE 3306
# Tue, 14 Jul 2020 02:46:44 GMT
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
	-	`sha256:5db39dfed4beb8bf43dfc37dc09159614f6457a620d995f612eda4654223aab5`  
		Last Modified: Tue, 14 Jul 2020 02:47:52 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cd3a5df9c6347ce8eb13a98bdc47ef362354c2dfcb31ab106b1f780f219e0ce`  
		Last Modified: Tue, 14 Jul 2020 02:48:04 GMT  
		Size: 64.2 MB (64232824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53dc4458df12b420686a507bd6c82a4cf4e8482ef0972e12796ed77ffa0c4a4d`  
		Last Modified: Tue, 14 Jul 2020 02:47:52 GMT  
		Size: 5.2 KB (5162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebc1665753518c1600201c2b8613364afe89c27d553d05a955133b9a06ee764`  
		Last Modified: Tue, 14 Jul 2020 02:47:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.6.49`

```console
$ docker pull mysql@sha256:19a164794d3cef15c9ac44754604fa079adb448f82d40e4b8be8381148c785fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:5.6.49` - linux; amd64

```console
$ docker pull mysql@sha256:71c6d751d76080fb06737e9306c63b38f630d48e3869a3939e8483747c18a601
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.9 MB (102924270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01ba04febd24365f377e0e5d8c7d5612520bffb1f3fded337dfbf46fbf6fd3b6`
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
# Tue, 14 Jul 2020 02:46:20 GMT
ENV MYSQL_VERSION=5.6.49-1debian9
# Tue, 14 Jul 2020 02:46:20 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ stretch mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Tue, 14 Jul 2020 02:46:42 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-server="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 777 /var/run/mysqld 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Tue, 14 Jul 2020 02:46:42 GMT
VOLUME [/var/lib/mysql]
# Tue, 14 Jul 2020 02:46:42 GMT
COPY file:7cbb26bbdb8e71b36aafda38dbac08caa641714a19991b86cde77daf3286ec11 in /usr/local/bin/ 
# Tue, 14 Jul 2020 02:46:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 14 Jul 2020 02:46:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Jul 2020 02:46:43 GMT
EXPOSE 3306
# Tue, 14 Jul 2020 02:46:44 GMT
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
	-	`sha256:5db39dfed4beb8bf43dfc37dc09159614f6457a620d995f612eda4654223aab5`  
		Last Modified: Tue, 14 Jul 2020 02:47:52 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cd3a5df9c6347ce8eb13a98bdc47ef362354c2dfcb31ab106b1f780f219e0ce`  
		Last Modified: Tue, 14 Jul 2020 02:48:04 GMT  
		Size: 64.2 MB (64232824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53dc4458df12b420686a507bd6c82a4cf4e8482ef0972e12796ed77ffa0c4a4d`  
		Last Modified: Tue, 14 Jul 2020 02:47:52 GMT  
		Size: 5.2 KB (5162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebc1665753518c1600201c2b8613364afe89c27d553d05a955133b9a06ee764`  
		Last Modified: Tue, 14 Jul 2020 02:47:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7`

```console
$ docker pull mysql@sha256:ea560da3b6f2f3ad79fd76652cb9031407c5112246a6fb5724ea895e95d74032
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:5.7` - linux; amd64

```console
$ docker pull mysql@sha256:300728110cb9c46bba70d3f888118bf7ad7a270035fafef9d0e912a4bd619633
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.5 MB (154475860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d05c76dbbfcf3e1d969eecc04d0aa461e0f95204f6833f62edb73cca7b62fcd4`
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
# Tue, 14 Jul 2020 02:45:46 GMT
ENV MYSQL_VERSION=5.7.31-1debian10
# Tue, 14 Jul 2020 02:45:46 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ buster mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Tue, 14 Jul 2020 02:46:12 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-server="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 777 /var/run/mysqld 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Tue, 14 Jul 2020 02:46:12 GMT
VOLUME [/var/lib/mysql]
# Tue, 14 Jul 2020 02:46:13 GMT
COPY file:7cbb26bbdb8e71b36aafda38dbac08caa641714a19991b86cde77daf3286ec11 in /usr/local/bin/ 
# Tue, 14 Jul 2020 02:46:14 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 14 Jul 2020 02:46:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Jul 2020 02:46:14 GMT
EXPOSE 3306 33060
# Tue, 14 Jul 2020 02:46:14 GMT
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
	-	`sha256:0a52a5c57cd9a5d74b8de5352ddf8168ae29c0ec8bfac2bf0d4dff474d65f5df`  
		Last Modified: Tue, 14 Jul 2020 02:47:25 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b816a39d367faf0c8d5d5bae89c8224f2747301c7982084550cf31e5a34157f`  
		Last Modified: Tue, 14 Jul 2020 02:47:47 GMT  
		Size: 108.3 MB (108327942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ee22d6b3bb0dd4aa4449fba002e4f2fa9582eef2d42c6eb094d61430ce78cc`  
		Last Modified: Tue, 14 Jul 2020 02:47:25 GMT  
		Size: 5.1 KB (5146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e517c3d2ba35e1ea78f8580cc8ba7ce000cb233b683a19711a006b7842c3df8e`  
		Last Modified: Tue, 14 Jul 2020 02:47:25 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.31`

```console
$ docker pull mysql@sha256:ea560da3b6f2f3ad79fd76652cb9031407c5112246a6fb5724ea895e95d74032
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:5.7.31` - linux; amd64

```console
$ docker pull mysql@sha256:300728110cb9c46bba70d3f888118bf7ad7a270035fafef9d0e912a4bd619633
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.5 MB (154475860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d05c76dbbfcf3e1d969eecc04d0aa461e0f95204f6833f62edb73cca7b62fcd4`
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
# Tue, 14 Jul 2020 02:45:46 GMT
ENV MYSQL_VERSION=5.7.31-1debian10
# Tue, 14 Jul 2020 02:45:46 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ buster mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Tue, 14 Jul 2020 02:46:12 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-server="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 777 /var/run/mysqld 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Tue, 14 Jul 2020 02:46:12 GMT
VOLUME [/var/lib/mysql]
# Tue, 14 Jul 2020 02:46:13 GMT
COPY file:7cbb26bbdb8e71b36aafda38dbac08caa641714a19991b86cde77daf3286ec11 in /usr/local/bin/ 
# Tue, 14 Jul 2020 02:46:14 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 14 Jul 2020 02:46:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Jul 2020 02:46:14 GMT
EXPOSE 3306 33060
# Tue, 14 Jul 2020 02:46:14 GMT
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
	-	`sha256:0a52a5c57cd9a5d74b8de5352ddf8168ae29c0ec8bfac2bf0d4dff474d65f5df`  
		Last Modified: Tue, 14 Jul 2020 02:47:25 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b816a39d367faf0c8d5d5bae89c8224f2747301c7982084550cf31e5a34157f`  
		Last Modified: Tue, 14 Jul 2020 02:47:47 GMT  
		Size: 108.3 MB (108327942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ee22d6b3bb0dd4aa4449fba002e4f2fa9582eef2d42c6eb094d61430ce78cc`  
		Last Modified: Tue, 14 Jul 2020 02:47:25 GMT  
		Size: 5.1 KB (5146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e517c3d2ba35e1ea78f8580cc8ba7ce000cb233b683a19711a006b7842c3df8e`  
		Last Modified: Tue, 14 Jul 2020 02:47:25 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8`

```console
$ docker pull mysql@sha256:c455bbcaa8b9c5c636c45f6184f970caeb3d8b545a0390e1b72a253e07aef8fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:8` - linux; amd64

```console
$ docker pull mysql@sha256:4316fb65ca51bbe7bad76826f067d84e949bb35e0d62129ce59ee76ea9fd7492
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.6 MB (158634953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ac22cccc3ae67ca42ed92b55c8fa7c68967ec6b875d15d761467d40097368b6`
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
# Tue, 14 Jul 2020 02:45:17 GMT
ENV MYSQL_VERSION=8.0.21-1debian10
# Tue, 14 Jul 2020 02:45:17 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ buster mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Tue, 14 Jul 2020 02:45:36 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-community-client="${MYSQL_VERSION}" mysql-community-server-core="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 777 /var/run/mysqld
# Tue, 14 Jul 2020 02:45:36 GMT
VOLUME [/var/lib/mysql]
# Mon, 20 Jul 2020 22:27:26 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Mon, 20 Jul 2020 22:27:26 GMT
COPY file:7cbb26bbdb8e71b36aafda38dbac08caa641714a19991b86cde77daf3286ec11 in /usr/local/bin/ 
# Mon, 20 Jul 2020 22:27:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 20 Jul 2020 22:27:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 20 Jul 2020 22:27:27 GMT
EXPOSE 3306 33060
# Mon, 20 Jul 2020 22:27:27 GMT
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
	-	`sha256:571e8a2821565e268069a61029a5c62e0e43216c9f8fa66abded4f5db4b95800`  
		Last Modified: Tue, 14 Jul 2020 02:46:54 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cc823c6090671d52c33353aa393fc7522e647488bcce45798a930cb1920418`  
		Last Modified: Tue, 14 Jul 2020 02:47:17 GMT  
		Size: 112.5 MB (112486191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f6364a86892bf53bb5e9d7547eec6fc22590f4a7327ab43d4eb56bc15e0647`  
		Last Modified: Mon, 20 Jul 2020 22:27:44 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55e5b10f33a43fc4b27d2733324ce0261bdce363ec574b1977c866827c7c830e`  
		Last Modified: Mon, 20 Jul 2020 22:27:44 GMT  
		Size: 5.1 KB (5144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68129e7a0316fbee5328c39cb873562a20b890a3bb65ba72419521fb9f4b7af4`  
		Last Modified: Mon, 20 Jul 2020 22:27:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0`

```console
$ docker pull mysql@sha256:c455bbcaa8b9c5c636c45f6184f970caeb3d8b545a0390e1b72a253e07aef8fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:8.0` - linux; amd64

```console
$ docker pull mysql@sha256:4316fb65ca51bbe7bad76826f067d84e949bb35e0d62129ce59ee76ea9fd7492
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.6 MB (158634953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ac22cccc3ae67ca42ed92b55c8fa7c68967ec6b875d15d761467d40097368b6`
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
# Tue, 14 Jul 2020 02:45:17 GMT
ENV MYSQL_VERSION=8.0.21-1debian10
# Tue, 14 Jul 2020 02:45:17 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ buster mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Tue, 14 Jul 2020 02:45:36 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-community-client="${MYSQL_VERSION}" mysql-community-server-core="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 777 /var/run/mysqld
# Tue, 14 Jul 2020 02:45:36 GMT
VOLUME [/var/lib/mysql]
# Mon, 20 Jul 2020 22:27:26 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Mon, 20 Jul 2020 22:27:26 GMT
COPY file:7cbb26bbdb8e71b36aafda38dbac08caa641714a19991b86cde77daf3286ec11 in /usr/local/bin/ 
# Mon, 20 Jul 2020 22:27:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 20 Jul 2020 22:27:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 20 Jul 2020 22:27:27 GMT
EXPOSE 3306 33060
# Mon, 20 Jul 2020 22:27:27 GMT
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
	-	`sha256:571e8a2821565e268069a61029a5c62e0e43216c9f8fa66abded4f5db4b95800`  
		Last Modified: Tue, 14 Jul 2020 02:46:54 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cc823c6090671d52c33353aa393fc7522e647488bcce45798a930cb1920418`  
		Last Modified: Tue, 14 Jul 2020 02:47:17 GMT  
		Size: 112.5 MB (112486191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f6364a86892bf53bb5e9d7547eec6fc22590f4a7327ab43d4eb56bc15e0647`  
		Last Modified: Mon, 20 Jul 2020 22:27:44 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55e5b10f33a43fc4b27d2733324ce0261bdce363ec574b1977c866827c7c830e`  
		Last Modified: Mon, 20 Jul 2020 22:27:44 GMT  
		Size: 5.1 KB (5144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68129e7a0316fbee5328c39cb873562a20b890a3bb65ba72419521fb9f4b7af4`  
		Last Modified: Mon, 20 Jul 2020 22:27:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.21`

```console
$ docker pull mysql@sha256:c455bbcaa8b9c5c636c45f6184f970caeb3d8b545a0390e1b72a253e07aef8fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:8.0.21` - linux; amd64

```console
$ docker pull mysql@sha256:4316fb65ca51bbe7bad76826f067d84e949bb35e0d62129ce59ee76ea9fd7492
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.6 MB (158634953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ac22cccc3ae67ca42ed92b55c8fa7c68967ec6b875d15d761467d40097368b6`
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
# Tue, 14 Jul 2020 02:45:17 GMT
ENV MYSQL_VERSION=8.0.21-1debian10
# Tue, 14 Jul 2020 02:45:17 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ buster mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Tue, 14 Jul 2020 02:45:36 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-community-client="${MYSQL_VERSION}" mysql-community-server-core="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 777 /var/run/mysqld
# Tue, 14 Jul 2020 02:45:36 GMT
VOLUME [/var/lib/mysql]
# Mon, 20 Jul 2020 22:27:26 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Mon, 20 Jul 2020 22:27:26 GMT
COPY file:7cbb26bbdb8e71b36aafda38dbac08caa641714a19991b86cde77daf3286ec11 in /usr/local/bin/ 
# Mon, 20 Jul 2020 22:27:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 20 Jul 2020 22:27:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 20 Jul 2020 22:27:27 GMT
EXPOSE 3306 33060
# Mon, 20 Jul 2020 22:27:27 GMT
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
	-	`sha256:571e8a2821565e268069a61029a5c62e0e43216c9f8fa66abded4f5db4b95800`  
		Last Modified: Tue, 14 Jul 2020 02:46:54 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cc823c6090671d52c33353aa393fc7522e647488bcce45798a930cb1920418`  
		Last Modified: Tue, 14 Jul 2020 02:47:17 GMT  
		Size: 112.5 MB (112486191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f6364a86892bf53bb5e9d7547eec6fc22590f4a7327ab43d4eb56bc15e0647`  
		Last Modified: Mon, 20 Jul 2020 22:27:44 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55e5b10f33a43fc4b27d2733324ce0261bdce363ec574b1977c866827c7c830e`  
		Last Modified: Mon, 20 Jul 2020 22:27:44 GMT  
		Size: 5.1 KB (5144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68129e7a0316fbee5328c39cb873562a20b890a3bb65ba72419521fb9f4b7af4`  
		Last Modified: Mon, 20 Jul 2020 22:27:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:latest`

```console
$ docker pull mysql@sha256:c455bbcaa8b9c5c636c45f6184f970caeb3d8b545a0390e1b72a253e07aef8fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:latest` - linux; amd64

```console
$ docker pull mysql@sha256:4316fb65ca51bbe7bad76826f067d84e949bb35e0d62129ce59ee76ea9fd7492
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.6 MB (158634953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ac22cccc3ae67ca42ed92b55c8fa7c68967ec6b875d15d761467d40097368b6`
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
# Tue, 14 Jul 2020 02:45:17 GMT
ENV MYSQL_VERSION=8.0.21-1debian10
# Tue, 14 Jul 2020 02:45:17 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ buster mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Tue, 14 Jul 2020 02:45:36 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-community-client="${MYSQL_VERSION}" mysql-community-server-core="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 777 /var/run/mysqld
# Tue, 14 Jul 2020 02:45:36 GMT
VOLUME [/var/lib/mysql]
# Mon, 20 Jul 2020 22:27:26 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Mon, 20 Jul 2020 22:27:26 GMT
COPY file:7cbb26bbdb8e71b36aafda38dbac08caa641714a19991b86cde77daf3286ec11 in /usr/local/bin/ 
# Mon, 20 Jul 2020 22:27:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 20 Jul 2020 22:27:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 20 Jul 2020 22:27:27 GMT
EXPOSE 3306 33060
# Mon, 20 Jul 2020 22:27:27 GMT
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
	-	`sha256:571e8a2821565e268069a61029a5c62e0e43216c9f8fa66abded4f5db4b95800`  
		Last Modified: Tue, 14 Jul 2020 02:46:54 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cc823c6090671d52c33353aa393fc7522e647488bcce45798a930cb1920418`  
		Last Modified: Tue, 14 Jul 2020 02:47:17 GMT  
		Size: 112.5 MB (112486191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f6364a86892bf53bb5e9d7547eec6fc22590f4a7327ab43d4eb56bc15e0647`  
		Last Modified: Mon, 20 Jul 2020 22:27:44 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55e5b10f33a43fc4b27d2733324ce0261bdce363ec574b1977c866827c7c830e`  
		Last Modified: Mon, 20 Jul 2020 22:27:44 GMT  
		Size: 5.1 KB (5144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68129e7a0316fbee5328c39cb873562a20b890a3bb65ba72419521fb9f4b7af4`  
		Last Modified: Mon, 20 Jul 2020 22:27:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
