<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mysql`

-	[`mysql:5`](#mysql5)
-	[`mysql:5.6`](#mysql56)
-	[`mysql:5.6.47`](#mysql5647)
-	[`mysql:5.7`](#mysql57)
-	[`mysql:5.7.29`](#mysql5729)
-	[`mysql:8`](#mysql8)
-	[`mysql:8.0`](#mysql80)
-	[`mysql:8.0.19`](#mysql8019)
-	[`mysql:latest`](#mysqllatest)

## `mysql:5`

```console
$ docker pull mysql@sha256:60c4219048baa8c01824b974cbfcdb4849a62e30c387cd48ec2a2771231ae404
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:5` - linux; amd64

```console
$ docker pull mysql@sha256:1be1f2cbd2c18563b167ffda45f67c5b0afb1bfe6a77cbc506306836fb1317b5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.8 MB (153790666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5cea958d3300a632059bae9e9e1279128e33d038e256d4950669ffae75467e7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 01 Feb 2020 17:23:57 GMT
ADD file:003d2bac85e72555ed93f77a2b1d595a7fe51c4a9a2401496a82fc673a863fd6 in / 
# Sat, 01 Feb 2020 17:23:58 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:04:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 01 Feb 2020 18:04:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:04:57 GMT
ENV GOSU_VERSION=1.7
# Sat, 01 Feb 2020 18:05:13 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& gpgconf --kill all 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sat, 01 Feb 2020 18:05:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 21 Feb 2020 03:03:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 03:03:54 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Fri, 21 Feb 2020 03:04:30 GMT
ENV MYSQL_MAJOR=5.7
# Fri, 21 Feb 2020 03:04:30 GMT
ENV MYSQL_VERSION=5.7.29-1debian9
# Fri, 21 Feb 2020 03:04:32 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ stretch mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Fri, 21 Feb 2020 03:05:06 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-server="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 777 /var/run/mysqld 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 21 Feb 2020 03:05:07 GMT
VOLUME [/var/lib/mysql]
# Fri, 21 Feb 2020 03:05:07 GMT
COPY file:3f9ea5eebe1c6044ae56c9bb1b511da3bde64f7672f438d25bb8440e5a878d15 in /usr/local/bin/ 
# Fri, 21 Feb 2020 03:05:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 21 Feb 2020 03:05:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Feb 2020 03:05:09 GMT
EXPOSE 3306 33060
# Fri, 21 Feb 2020 03:05:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:619014d83c026bca3d21f5eb42a629ac2dbe15bdb37b77f25fc1ac5fbada68e5`  
		Last Modified: Sat, 01 Feb 2020 17:29:01 GMT  
		Size: 22.5 MB (22524713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ced578c3a5f5e96f33315bb936d3d0bac30f734e820759f370ef0a6fcbd8639`  
		Last Modified: Sat, 01 Feb 2020 18:08:01 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:731f6e13d8ea683b85c2d516659def2ada874d12198ccb8aa607b0739cad71f9`  
		Last Modified: Sat, 01 Feb 2020 18:08:03 GMT  
		Size: 4.5 MB (4501283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c183de42679fb8b24485807f24d4d5e83833a5df99f2a1e22b9995d5a77a61c`  
		Last Modified: Sat, 01 Feb 2020 18:08:00 GMT  
		Size: 1.3 MB (1270478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de69b5c2f3c8d53585c798ec208eb58375608c919d5b70da51c3e4fcbb90e93`  
		Last Modified: Sat, 01 Feb 2020 18:08:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122a561a41965dc6801656b34be38f68631c1d58de3e96f908adf095b4eef2d8`  
		Last Modified: Fri, 21 Feb 2020 03:06:26 GMT  
		Size: 14.0 MB (13953499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1abf8e9f34f0c311ef662c5018bd573d0c85dbac8f76e4d8785731c2ccc11248`  
		Last Modified: Fri, 21 Feb 2020 03:06:19 GMT  
		Size: 28.3 KB (28327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7182ad2b49b99a5f91db0e08d05d55e67748a5e06c220c760c42b101eed9f9d8`  
		Last Modified: Fri, 21 Feb 2020 03:06:57 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc5d94b98a4d3f77af4d5638898dfc307712214e67881ca0d8620ba27d03759`  
		Last Modified: Fri, 21 Feb 2020 03:07:24 GMT  
		Size: 111.5 MB (111505124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da9976dfb484de1eec3376aa224af3ed144749349681b8961f483e4c433bdc25`  
		Last Modified: Fri, 21 Feb 2020 03:06:57 GMT  
		Size: 5.0 KB (5044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:150942156f193033e94696ccddbe712375935fd5934b8358eaa5a8f7328114eb`  
		Last Modified: Fri, 21 Feb 2020 03:06:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.6`

```console
$ docker pull mysql@sha256:8a0b9c45e5207f9e2e6a54646d5213d86b1a60b5eb7c95e5eb882f1fecd4ab88
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:5.6` - linux; amd64

```console
$ docker pull mysql@sha256:1b3588670012c57bf408cfe1513004e68c5bdb25e5685b0cff3254c6135abb56
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.5 MB (104540573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c0016efffde219cfb640ba28e226234202761bf0f5220f999aaa2d78db5cb72`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 01 Feb 2020 17:23:57 GMT
ADD file:003d2bac85e72555ed93f77a2b1d595a7fe51c4a9a2401496a82fc673a863fd6 in / 
# Sat, 01 Feb 2020 17:23:58 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:04:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 01 Feb 2020 18:04:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:04:57 GMT
ENV GOSU_VERSION=1.7
# Sat, 01 Feb 2020 18:05:13 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& gpgconf --kill all 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sat, 01 Feb 2020 18:05:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 21 Feb 2020 03:05:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 03:05:32 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Fri, 21 Feb 2020 03:05:32 GMT
ENV MYSQL_MAJOR=5.6
# Fri, 21 Feb 2020 03:05:33 GMT
ENV MYSQL_VERSION=5.6.47-1debian9
# Fri, 21 Feb 2020 03:05:34 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ stretch mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Fri, 21 Feb 2020 03:05:59 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-server="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 777 /var/run/mysqld 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 21 Feb 2020 03:05:59 GMT
VOLUME [/var/lib/mysql]
# Fri, 21 Feb 2020 03:06:00 GMT
COPY file:3f9ea5eebe1c6044ae56c9bb1b511da3bde64f7672f438d25bb8440e5a878d15 in /usr/local/bin/ 
# Fri, 21 Feb 2020 03:06:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 21 Feb 2020 03:06:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Feb 2020 03:06:02 GMT
EXPOSE 3306
# Fri, 21 Feb 2020 03:06:02 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:619014d83c026bca3d21f5eb42a629ac2dbe15bdb37b77f25fc1ac5fbada68e5`  
		Last Modified: Sat, 01 Feb 2020 17:29:01 GMT  
		Size: 22.5 MB (22524713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ced578c3a5f5e96f33315bb936d3d0bac30f734e820759f370ef0a6fcbd8639`  
		Last Modified: Sat, 01 Feb 2020 18:08:01 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:731f6e13d8ea683b85c2d516659def2ada874d12198ccb8aa607b0739cad71f9`  
		Last Modified: Sat, 01 Feb 2020 18:08:03 GMT  
		Size: 4.5 MB (4501283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c183de42679fb8b24485807f24d4d5e83833a5df99f2a1e22b9995d5a77a61c`  
		Last Modified: Sat, 01 Feb 2020 18:08:00 GMT  
		Size: 1.3 MB (1270478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de69b5c2f3c8d53585c798ec208eb58375608c919d5b70da51c3e4fcbb90e93`  
		Last Modified: Sat, 01 Feb 2020 18:08:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fa7e37034a68fb7bee066b72dd586ec557407582535eea46dd910160601c8a5`  
		Last Modified: Fri, 21 Feb 2020 03:07:40 GMT  
		Size: 12.0 MB (12018104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0528dbb183daf653d89e76a24a46ff71c4a12b02de2442b2a893b2f36c6479`  
		Last Modified: Fri, 21 Feb 2020 03:07:32 GMT  
		Size: 28.3 KB (28326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a7ad31135f6704c972ee18e5710860baa8c95a099a648c0e7526b600cb878a`  
		Last Modified: Fri, 21 Feb 2020 03:07:32 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97f050956bc00a1ba9be9b9dc682fbe8e14e9e4c5359dae67f6a8cc796cf0725`  
		Last Modified: Fri, 21 Feb 2020 03:07:51 GMT  
		Size: 64.2 MB (64190418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3883424e5db4a6d76954a5dfc6ab55e33ee3f5cef8a0a00e0c74ac51de71e78`  
		Last Modified: Fri, 21 Feb 2020 03:07:32 GMT  
		Size: 5.0 KB (5050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48821f521345ec958b0589bf06879bae3bfaf86882d058bbd6482fedd060e9bf`  
		Last Modified: Fri, 21 Feb 2020 03:07:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.6.47`

```console
$ docker pull mysql@sha256:8a0b9c45e5207f9e2e6a54646d5213d86b1a60b5eb7c95e5eb882f1fecd4ab88
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:5.6.47` - linux; amd64

```console
$ docker pull mysql@sha256:1b3588670012c57bf408cfe1513004e68c5bdb25e5685b0cff3254c6135abb56
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.5 MB (104540573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c0016efffde219cfb640ba28e226234202761bf0f5220f999aaa2d78db5cb72`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 01 Feb 2020 17:23:57 GMT
ADD file:003d2bac85e72555ed93f77a2b1d595a7fe51c4a9a2401496a82fc673a863fd6 in / 
# Sat, 01 Feb 2020 17:23:58 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:04:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 01 Feb 2020 18:04:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:04:57 GMT
ENV GOSU_VERSION=1.7
# Sat, 01 Feb 2020 18:05:13 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& gpgconf --kill all 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sat, 01 Feb 2020 18:05:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 21 Feb 2020 03:05:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 03:05:32 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Fri, 21 Feb 2020 03:05:32 GMT
ENV MYSQL_MAJOR=5.6
# Fri, 21 Feb 2020 03:05:33 GMT
ENV MYSQL_VERSION=5.6.47-1debian9
# Fri, 21 Feb 2020 03:05:34 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ stretch mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Fri, 21 Feb 2020 03:05:59 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-server="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 777 /var/run/mysqld 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 21 Feb 2020 03:05:59 GMT
VOLUME [/var/lib/mysql]
# Fri, 21 Feb 2020 03:06:00 GMT
COPY file:3f9ea5eebe1c6044ae56c9bb1b511da3bde64f7672f438d25bb8440e5a878d15 in /usr/local/bin/ 
# Fri, 21 Feb 2020 03:06:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 21 Feb 2020 03:06:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Feb 2020 03:06:02 GMT
EXPOSE 3306
# Fri, 21 Feb 2020 03:06:02 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:619014d83c026bca3d21f5eb42a629ac2dbe15bdb37b77f25fc1ac5fbada68e5`  
		Last Modified: Sat, 01 Feb 2020 17:29:01 GMT  
		Size: 22.5 MB (22524713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ced578c3a5f5e96f33315bb936d3d0bac30f734e820759f370ef0a6fcbd8639`  
		Last Modified: Sat, 01 Feb 2020 18:08:01 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:731f6e13d8ea683b85c2d516659def2ada874d12198ccb8aa607b0739cad71f9`  
		Last Modified: Sat, 01 Feb 2020 18:08:03 GMT  
		Size: 4.5 MB (4501283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c183de42679fb8b24485807f24d4d5e83833a5df99f2a1e22b9995d5a77a61c`  
		Last Modified: Sat, 01 Feb 2020 18:08:00 GMT  
		Size: 1.3 MB (1270478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de69b5c2f3c8d53585c798ec208eb58375608c919d5b70da51c3e4fcbb90e93`  
		Last Modified: Sat, 01 Feb 2020 18:08:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fa7e37034a68fb7bee066b72dd586ec557407582535eea46dd910160601c8a5`  
		Last Modified: Fri, 21 Feb 2020 03:07:40 GMT  
		Size: 12.0 MB (12018104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0528dbb183daf653d89e76a24a46ff71c4a12b02de2442b2a893b2f36c6479`  
		Last Modified: Fri, 21 Feb 2020 03:07:32 GMT  
		Size: 28.3 KB (28326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a7ad31135f6704c972ee18e5710860baa8c95a099a648c0e7526b600cb878a`  
		Last Modified: Fri, 21 Feb 2020 03:07:32 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97f050956bc00a1ba9be9b9dc682fbe8e14e9e4c5359dae67f6a8cc796cf0725`  
		Last Modified: Fri, 21 Feb 2020 03:07:51 GMT  
		Size: 64.2 MB (64190418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3883424e5db4a6d76954a5dfc6ab55e33ee3f5cef8a0a00e0c74ac51de71e78`  
		Last Modified: Fri, 21 Feb 2020 03:07:32 GMT  
		Size: 5.0 KB (5050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48821f521345ec958b0589bf06879bae3bfaf86882d058bbd6482fedd060e9bf`  
		Last Modified: Fri, 21 Feb 2020 03:07:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7`

```console
$ docker pull mysql@sha256:60c4219048baa8c01824b974cbfcdb4849a62e30c387cd48ec2a2771231ae404
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:5.7` - linux; amd64

```console
$ docker pull mysql@sha256:1be1f2cbd2c18563b167ffda45f67c5b0afb1bfe6a77cbc506306836fb1317b5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.8 MB (153790666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5cea958d3300a632059bae9e9e1279128e33d038e256d4950669ffae75467e7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 01 Feb 2020 17:23:57 GMT
ADD file:003d2bac85e72555ed93f77a2b1d595a7fe51c4a9a2401496a82fc673a863fd6 in / 
# Sat, 01 Feb 2020 17:23:58 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:04:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 01 Feb 2020 18:04:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:04:57 GMT
ENV GOSU_VERSION=1.7
# Sat, 01 Feb 2020 18:05:13 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& gpgconf --kill all 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sat, 01 Feb 2020 18:05:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 21 Feb 2020 03:03:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 03:03:54 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Fri, 21 Feb 2020 03:04:30 GMT
ENV MYSQL_MAJOR=5.7
# Fri, 21 Feb 2020 03:04:30 GMT
ENV MYSQL_VERSION=5.7.29-1debian9
# Fri, 21 Feb 2020 03:04:32 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ stretch mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Fri, 21 Feb 2020 03:05:06 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-server="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 777 /var/run/mysqld 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 21 Feb 2020 03:05:07 GMT
VOLUME [/var/lib/mysql]
# Fri, 21 Feb 2020 03:05:07 GMT
COPY file:3f9ea5eebe1c6044ae56c9bb1b511da3bde64f7672f438d25bb8440e5a878d15 in /usr/local/bin/ 
# Fri, 21 Feb 2020 03:05:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 21 Feb 2020 03:05:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Feb 2020 03:05:09 GMT
EXPOSE 3306 33060
# Fri, 21 Feb 2020 03:05:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:619014d83c026bca3d21f5eb42a629ac2dbe15bdb37b77f25fc1ac5fbada68e5`  
		Last Modified: Sat, 01 Feb 2020 17:29:01 GMT  
		Size: 22.5 MB (22524713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ced578c3a5f5e96f33315bb936d3d0bac30f734e820759f370ef0a6fcbd8639`  
		Last Modified: Sat, 01 Feb 2020 18:08:01 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:731f6e13d8ea683b85c2d516659def2ada874d12198ccb8aa607b0739cad71f9`  
		Last Modified: Sat, 01 Feb 2020 18:08:03 GMT  
		Size: 4.5 MB (4501283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c183de42679fb8b24485807f24d4d5e83833a5df99f2a1e22b9995d5a77a61c`  
		Last Modified: Sat, 01 Feb 2020 18:08:00 GMT  
		Size: 1.3 MB (1270478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de69b5c2f3c8d53585c798ec208eb58375608c919d5b70da51c3e4fcbb90e93`  
		Last Modified: Sat, 01 Feb 2020 18:08:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122a561a41965dc6801656b34be38f68631c1d58de3e96f908adf095b4eef2d8`  
		Last Modified: Fri, 21 Feb 2020 03:06:26 GMT  
		Size: 14.0 MB (13953499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1abf8e9f34f0c311ef662c5018bd573d0c85dbac8f76e4d8785731c2ccc11248`  
		Last Modified: Fri, 21 Feb 2020 03:06:19 GMT  
		Size: 28.3 KB (28327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7182ad2b49b99a5f91db0e08d05d55e67748a5e06c220c760c42b101eed9f9d8`  
		Last Modified: Fri, 21 Feb 2020 03:06:57 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc5d94b98a4d3f77af4d5638898dfc307712214e67881ca0d8620ba27d03759`  
		Last Modified: Fri, 21 Feb 2020 03:07:24 GMT  
		Size: 111.5 MB (111505124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da9976dfb484de1eec3376aa224af3ed144749349681b8961f483e4c433bdc25`  
		Last Modified: Fri, 21 Feb 2020 03:06:57 GMT  
		Size: 5.0 KB (5044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:150942156f193033e94696ccddbe712375935fd5934b8358eaa5a8f7328114eb`  
		Last Modified: Fri, 21 Feb 2020 03:06:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.29`

```console
$ docker pull mysql@sha256:60c4219048baa8c01824b974cbfcdb4849a62e30c387cd48ec2a2771231ae404
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:5.7.29` - linux; amd64

```console
$ docker pull mysql@sha256:1be1f2cbd2c18563b167ffda45f67c5b0afb1bfe6a77cbc506306836fb1317b5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.8 MB (153790666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5cea958d3300a632059bae9e9e1279128e33d038e256d4950669ffae75467e7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 01 Feb 2020 17:23:57 GMT
ADD file:003d2bac85e72555ed93f77a2b1d595a7fe51c4a9a2401496a82fc673a863fd6 in / 
# Sat, 01 Feb 2020 17:23:58 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:04:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 01 Feb 2020 18:04:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:04:57 GMT
ENV GOSU_VERSION=1.7
# Sat, 01 Feb 2020 18:05:13 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& gpgconf --kill all 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sat, 01 Feb 2020 18:05:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 21 Feb 2020 03:03:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 03:03:54 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Fri, 21 Feb 2020 03:04:30 GMT
ENV MYSQL_MAJOR=5.7
# Fri, 21 Feb 2020 03:04:30 GMT
ENV MYSQL_VERSION=5.7.29-1debian9
# Fri, 21 Feb 2020 03:04:32 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ stretch mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Fri, 21 Feb 2020 03:05:06 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-server="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 777 /var/run/mysqld 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 21 Feb 2020 03:05:07 GMT
VOLUME [/var/lib/mysql]
# Fri, 21 Feb 2020 03:05:07 GMT
COPY file:3f9ea5eebe1c6044ae56c9bb1b511da3bde64f7672f438d25bb8440e5a878d15 in /usr/local/bin/ 
# Fri, 21 Feb 2020 03:05:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 21 Feb 2020 03:05:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Feb 2020 03:05:09 GMT
EXPOSE 3306 33060
# Fri, 21 Feb 2020 03:05:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:619014d83c026bca3d21f5eb42a629ac2dbe15bdb37b77f25fc1ac5fbada68e5`  
		Last Modified: Sat, 01 Feb 2020 17:29:01 GMT  
		Size: 22.5 MB (22524713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ced578c3a5f5e96f33315bb936d3d0bac30f734e820759f370ef0a6fcbd8639`  
		Last Modified: Sat, 01 Feb 2020 18:08:01 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:731f6e13d8ea683b85c2d516659def2ada874d12198ccb8aa607b0739cad71f9`  
		Last Modified: Sat, 01 Feb 2020 18:08:03 GMT  
		Size: 4.5 MB (4501283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c183de42679fb8b24485807f24d4d5e83833a5df99f2a1e22b9995d5a77a61c`  
		Last Modified: Sat, 01 Feb 2020 18:08:00 GMT  
		Size: 1.3 MB (1270478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de69b5c2f3c8d53585c798ec208eb58375608c919d5b70da51c3e4fcbb90e93`  
		Last Modified: Sat, 01 Feb 2020 18:08:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122a561a41965dc6801656b34be38f68631c1d58de3e96f908adf095b4eef2d8`  
		Last Modified: Fri, 21 Feb 2020 03:06:26 GMT  
		Size: 14.0 MB (13953499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1abf8e9f34f0c311ef662c5018bd573d0c85dbac8f76e4d8785731c2ccc11248`  
		Last Modified: Fri, 21 Feb 2020 03:06:19 GMT  
		Size: 28.3 KB (28327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7182ad2b49b99a5f91db0e08d05d55e67748a5e06c220c760c42b101eed9f9d8`  
		Last Modified: Fri, 21 Feb 2020 03:06:57 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc5d94b98a4d3f77af4d5638898dfc307712214e67881ca0d8620ba27d03759`  
		Last Modified: Fri, 21 Feb 2020 03:07:24 GMT  
		Size: 111.5 MB (111505124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da9976dfb484de1eec3376aa224af3ed144749349681b8961f483e4c433bdc25`  
		Last Modified: Fri, 21 Feb 2020 03:06:57 GMT  
		Size: 5.0 KB (5044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:150942156f193033e94696ccddbe712375935fd5934b8358eaa5a8f7328114eb`  
		Last Modified: Fri, 21 Feb 2020 03:06:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8`

```console
$ docker pull mysql@sha256:c7c6c5beb312fd2eb21af4f144d14b6ef29c9c2f9c5e1f3f74ffa75e38fad1f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:8` - linux; amd64

```console
$ docker pull mysql@sha256:30d30bde1a0757c0380ce8c6bf398e0bfb3bb434d12116e814e4c465ad3fa63c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.5 MB (138524471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afaec1334369d4bb6fe566f3f3d4b075ed4b74a6fcba61f9740aee4715888b21`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 01 Feb 2020 17:23:57 GMT
ADD file:003d2bac85e72555ed93f77a2b1d595a7fe51c4a9a2401496a82fc673a863fd6 in / 
# Sat, 01 Feb 2020 17:23:58 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:04:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 01 Feb 2020 18:04:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:04:57 GMT
ENV GOSU_VERSION=1.7
# Sat, 01 Feb 2020 18:05:13 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& gpgconf --kill all 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sat, 01 Feb 2020 18:05:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 21 Feb 2020 03:03:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 03:03:54 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Fri, 21 Feb 2020 03:03:54 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 21 Feb 2020 03:03:55 GMT
ENV MYSQL_VERSION=8.0.19-1debian9
# Fri, 21 Feb 2020 03:03:56 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ stretch mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Fri, 21 Feb 2020 03:04:20 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-community-client="${MYSQL_VERSION}" mysql-community-server-core="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 777 /var/run/mysqld
# Fri, 21 Feb 2020 03:04:21 GMT
VOLUME [/var/lib/mysql]
# Fri, 21 Feb 2020 03:04:21 GMT
COPY dir:478f098f3681084f7493af1f04cbcd3eeda6f10e0dd2f5c740acd25328a73455 in /etc/mysql/ 
# Fri, 21 Feb 2020 03:04:22 GMT
COPY file:3f9ea5eebe1c6044ae56c9bb1b511da3bde64f7672f438d25bb8440e5a878d15 in /usr/local/bin/ 
# Fri, 21 Feb 2020 03:04:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 21 Feb 2020 03:04:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Feb 2020 03:04:24 GMT
EXPOSE 3306 33060
# Fri, 21 Feb 2020 03:04:24 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:619014d83c026bca3d21f5eb42a629ac2dbe15bdb37b77f25fc1ac5fbada68e5`  
		Last Modified: Sat, 01 Feb 2020 17:29:01 GMT  
		Size: 22.5 MB (22524713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ced578c3a5f5e96f33315bb936d3d0bac30f734e820759f370ef0a6fcbd8639`  
		Last Modified: Sat, 01 Feb 2020 18:08:01 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:731f6e13d8ea683b85c2d516659def2ada874d12198ccb8aa607b0739cad71f9`  
		Last Modified: Sat, 01 Feb 2020 18:08:03 GMT  
		Size: 4.5 MB (4501283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c183de42679fb8b24485807f24d4d5e83833a5df99f2a1e22b9995d5a77a61c`  
		Last Modified: Sat, 01 Feb 2020 18:08:00 GMT  
		Size: 1.3 MB (1270478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de69b5c2f3c8d53585c798ec208eb58375608c919d5b70da51c3e4fcbb90e93`  
		Last Modified: Sat, 01 Feb 2020 18:08:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122a561a41965dc6801656b34be38f68631c1d58de3e96f908adf095b4eef2d8`  
		Last Modified: Fri, 21 Feb 2020 03:06:26 GMT  
		Size: 14.0 MB (13953499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1abf8e9f34f0c311ef662c5018bd573d0c85dbac8f76e4d8785731c2ccc11248`  
		Last Modified: Fri, 21 Feb 2020 03:06:19 GMT  
		Size: 28.3 KB (28327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e5887414166eb21c9f0d1eec78684013f1549a99d3e92c5841d6404df154bad`  
		Last Modified: Fri, 21 Feb 2020 03:06:18 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95adaca0707854ba4ac07bfb4228009e1d450ae64e3c1e6f028ecec3953face2`  
		Last Modified: Fri, 21 Feb 2020 03:06:49 GMT  
		Size: 96.2 MB (96238031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42c8c65423478ddb49dc4b60c64239044932073c5823b40051eded4637af3e19`  
		Last Modified: Fri, 21 Feb 2020 03:06:18 GMT  
		Size: 898.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ae93d9077ae38aafb8b06a9dd90ee1ede30761912d373cf290f778911daa8e1`  
		Last Modified: Fri, 21 Feb 2020 03:06:18 GMT  
		Size: 5.0 KB (5043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42131d6ef54e5a95f7b92e6c79a924c9cc8a47f685a85113b91439fbcfebf614`  
		Last Modified: Fri, 21 Feb 2020 03:06:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0`

```console
$ docker pull mysql@sha256:c7c6c5beb312fd2eb21af4f144d14b6ef29c9c2f9c5e1f3f74ffa75e38fad1f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:8.0` - linux; amd64

```console
$ docker pull mysql@sha256:30d30bde1a0757c0380ce8c6bf398e0bfb3bb434d12116e814e4c465ad3fa63c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.5 MB (138524471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afaec1334369d4bb6fe566f3f3d4b075ed4b74a6fcba61f9740aee4715888b21`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 01 Feb 2020 17:23:57 GMT
ADD file:003d2bac85e72555ed93f77a2b1d595a7fe51c4a9a2401496a82fc673a863fd6 in / 
# Sat, 01 Feb 2020 17:23:58 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:04:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 01 Feb 2020 18:04:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:04:57 GMT
ENV GOSU_VERSION=1.7
# Sat, 01 Feb 2020 18:05:13 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& gpgconf --kill all 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sat, 01 Feb 2020 18:05:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 21 Feb 2020 03:03:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 03:03:54 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Fri, 21 Feb 2020 03:03:54 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 21 Feb 2020 03:03:55 GMT
ENV MYSQL_VERSION=8.0.19-1debian9
# Fri, 21 Feb 2020 03:03:56 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ stretch mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Fri, 21 Feb 2020 03:04:20 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-community-client="${MYSQL_VERSION}" mysql-community-server-core="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 777 /var/run/mysqld
# Fri, 21 Feb 2020 03:04:21 GMT
VOLUME [/var/lib/mysql]
# Fri, 21 Feb 2020 03:04:21 GMT
COPY dir:478f098f3681084f7493af1f04cbcd3eeda6f10e0dd2f5c740acd25328a73455 in /etc/mysql/ 
# Fri, 21 Feb 2020 03:04:22 GMT
COPY file:3f9ea5eebe1c6044ae56c9bb1b511da3bde64f7672f438d25bb8440e5a878d15 in /usr/local/bin/ 
# Fri, 21 Feb 2020 03:04:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 21 Feb 2020 03:04:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Feb 2020 03:04:24 GMT
EXPOSE 3306 33060
# Fri, 21 Feb 2020 03:04:24 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:619014d83c026bca3d21f5eb42a629ac2dbe15bdb37b77f25fc1ac5fbada68e5`  
		Last Modified: Sat, 01 Feb 2020 17:29:01 GMT  
		Size: 22.5 MB (22524713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ced578c3a5f5e96f33315bb936d3d0bac30f734e820759f370ef0a6fcbd8639`  
		Last Modified: Sat, 01 Feb 2020 18:08:01 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:731f6e13d8ea683b85c2d516659def2ada874d12198ccb8aa607b0739cad71f9`  
		Last Modified: Sat, 01 Feb 2020 18:08:03 GMT  
		Size: 4.5 MB (4501283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c183de42679fb8b24485807f24d4d5e83833a5df99f2a1e22b9995d5a77a61c`  
		Last Modified: Sat, 01 Feb 2020 18:08:00 GMT  
		Size: 1.3 MB (1270478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de69b5c2f3c8d53585c798ec208eb58375608c919d5b70da51c3e4fcbb90e93`  
		Last Modified: Sat, 01 Feb 2020 18:08:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122a561a41965dc6801656b34be38f68631c1d58de3e96f908adf095b4eef2d8`  
		Last Modified: Fri, 21 Feb 2020 03:06:26 GMT  
		Size: 14.0 MB (13953499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1abf8e9f34f0c311ef662c5018bd573d0c85dbac8f76e4d8785731c2ccc11248`  
		Last Modified: Fri, 21 Feb 2020 03:06:19 GMT  
		Size: 28.3 KB (28327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e5887414166eb21c9f0d1eec78684013f1549a99d3e92c5841d6404df154bad`  
		Last Modified: Fri, 21 Feb 2020 03:06:18 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95adaca0707854ba4ac07bfb4228009e1d450ae64e3c1e6f028ecec3953face2`  
		Last Modified: Fri, 21 Feb 2020 03:06:49 GMT  
		Size: 96.2 MB (96238031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42c8c65423478ddb49dc4b60c64239044932073c5823b40051eded4637af3e19`  
		Last Modified: Fri, 21 Feb 2020 03:06:18 GMT  
		Size: 898.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ae93d9077ae38aafb8b06a9dd90ee1ede30761912d373cf290f778911daa8e1`  
		Last Modified: Fri, 21 Feb 2020 03:06:18 GMT  
		Size: 5.0 KB (5043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42131d6ef54e5a95f7b92e6c79a924c9cc8a47f685a85113b91439fbcfebf614`  
		Last Modified: Fri, 21 Feb 2020 03:06:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.19`

```console
$ docker pull mysql@sha256:c7c6c5beb312fd2eb21af4f144d14b6ef29c9c2f9c5e1f3f74ffa75e38fad1f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:8.0.19` - linux; amd64

```console
$ docker pull mysql@sha256:30d30bde1a0757c0380ce8c6bf398e0bfb3bb434d12116e814e4c465ad3fa63c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.5 MB (138524471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afaec1334369d4bb6fe566f3f3d4b075ed4b74a6fcba61f9740aee4715888b21`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 01 Feb 2020 17:23:57 GMT
ADD file:003d2bac85e72555ed93f77a2b1d595a7fe51c4a9a2401496a82fc673a863fd6 in / 
# Sat, 01 Feb 2020 17:23:58 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:04:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 01 Feb 2020 18:04:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:04:57 GMT
ENV GOSU_VERSION=1.7
# Sat, 01 Feb 2020 18:05:13 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& gpgconf --kill all 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sat, 01 Feb 2020 18:05:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 21 Feb 2020 03:03:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 03:03:54 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Fri, 21 Feb 2020 03:03:54 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 21 Feb 2020 03:03:55 GMT
ENV MYSQL_VERSION=8.0.19-1debian9
# Fri, 21 Feb 2020 03:03:56 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ stretch mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Fri, 21 Feb 2020 03:04:20 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-community-client="${MYSQL_VERSION}" mysql-community-server-core="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 777 /var/run/mysqld
# Fri, 21 Feb 2020 03:04:21 GMT
VOLUME [/var/lib/mysql]
# Fri, 21 Feb 2020 03:04:21 GMT
COPY dir:478f098f3681084f7493af1f04cbcd3eeda6f10e0dd2f5c740acd25328a73455 in /etc/mysql/ 
# Fri, 21 Feb 2020 03:04:22 GMT
COPY file:3f9ea5eebe1c6044ae56c9bb1b511da3bde64f7672f438d25bb8440e5a878d15 in /usr/local/bin/ 
# Fri, 21 Feb 2020 03:04:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 21 Feb 2020 03:04:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Feb 2020 03:04:24 GMT
EXPOSE 3306 33060
# Fri, 21 Feb 2020 03:04:24 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:619014d83c026bca3d21f5eb42a629ac2dbe15bdb37b77f25fc1ac5fbada68e5`  
		Last Modified: Sat, 01 Feb 2020 17:29:01 GMT  
		Size: 22.5 MB (22524713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ced578c3a5f5e96f33315bb936d3d0bac30f734e820759f370ef0a6fcbd8639`  
		Last Modified: Sat, 01 Feb 2020 18:08:01 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:731f6e13d8ea683b85c2d516659def2ada874d12198ccb8aa607b0739cad71f9`  
		Last Modified: Sat, 01 Feb 2020 18:08:03 GMT  
		Size: 4.5 MB (4501283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c183de42679fb8b24485807f24d4d5e83833a5df99f2a1e22b9995d5a77a61c`  
		Last Modified: Sat, 01 Feb 2020 18:08:00 GMT  
		Size: 1.3 MB (1270478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de69b5c2f3c8d53585c798ec208eb58375608c919d5b70da51c3e4fcbb90e93`  
		Last Modified: Sat, 01 Feb 2020 18:08:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122a561a41965dc6801656b34be38f68631c1d58de3e96f908adf095b4eef2d8`  
		Last Modified: Fri, 21 Feb 2020 03:06:26 GMT  
		Size: 14.0 MB (13953499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1abf8e9f34f0c311ef662c5018bd573d0c85dbac8f76e4d8785731c2ccc11248`  
		Last Modified: Fri, 21 Feb 2020 03:06:19 GMT  
		Size: 28.3 KB (28327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e5887414166eb21c9f0d1eec78684013f1549a99d3e92c5841d6404df154bad`  
		Last Modified: Fri, 21 Feb 2020 03:06:18 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95adaca0707854ba4ac07bfb4228009e1d450ae64e3c1e6f028ecec3953face2`  
		Last Modified: Fri, 21 Feb 2020 03:06:49 GMT  
		Size: 96.2 MB (96238031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42c8c65423478ddb49dc4b60c64239044932073c5823b40051eded4637af3e19`  
		Last Modified: Fri, 21 Feb 2020 03:06:18 GMT  
		Size: 898.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ae93d9077ae38aafb8b06a9dd90ee1ede30761912d373cf290f778911daa8e1`  
		Last Modified: Fri, 21 Feb 2020 03:06:18 GMT  
		Size: 5.0 KB (5043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42131d6ef54e5a95f7b92e6c79a924c9cc8a47f685a85113b91439fbcfebf614`  
		Last Modified: Fri, 21 Feb 2020 03:06:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:latest`

```console
$ docker pull mysql@sha256:c7c6c5beb312fd2eb21af4f144d14b6ef29c9c2f9c5e1f3f74ffa75e38fad1f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:latest` - linux; amd64

```console
$ docker pull mysql@sha256:30d30bde1a0757c0380ce8c6bf398e0bfb3bb434d12116e814e4c465ad3fa63c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.5 MB (138524471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afaec1334369d4bb6fe566f3f3d4b075ed4b74a6fcba61f9740aee4715888b21`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 01 Feb 2020 17:23:57 GMT
ADD file:003d2bac85e72555ed93f77a2b1d595a7fe51c4a9a2401496a82fc673a863fd6 in / 
# Sat, 01 Feb 2020 17:23:58 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:04:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 01 Feb 2020 18:04:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:04:57 GMT
ENV GOSU_VERSION=1.7
# Sat, 01 Feb 2020 18:05:13 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& gpgconf --kill all 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sat, 01 Feb 2020 18:05:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 21 Feb 2020 03:03:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 03:03:54 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Fri, 21 Feb 2020 03:03:54 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 21 Feb 2020 03:03:55 GMT
ENV MYSQL_VERSION=8.0.19-1debian9
# Fri, 21 Feb 2020 03:03:56 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ stretch mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Fri, 21 Feb 2020 03:04:20 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-community-client="${MYSQL_VERSION}" mysql-community-server-core="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 777 /var/run/mysqld
# Fri, 21 Feb 2020 03:04:21 GMT
VOLUME [/var/lib/mysql]
# Fri, 21 Feb 2020 03:04:21 GMT
COPY dir:478f098f3681084f7493af1f04cbcd3eeda6f10e0dd2f5c740acd25328a73455 in /etc/mysql/ 
# Fri, 21 Feb 2020 03:04:22 GMT
COPY file:3f9ea5eebe1c6044ae56c9bb1b511da3bde64f7672f438d25bb8440e5a878d15 in /usr/local/bin/ 
# Fri, 21 Feb 2020 03:04:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 21 Feb 2020 03:04:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Feb 2020 03:04:24 GMT
EXPOSE 3306 33060
# Fri, 21 Feb 2020 03:04:24 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:619014d83c026bca3d21f5eb42a629ac2dbe15bdb37b77f25fc1ac5fbada68e5`  
		Last Modified: Sat, 01 Feb 2020 17:29:01 GMT  
		Size: 22.5 MB (22524713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ced578c3a5f5e96f33315bb936d3d0bac30f734e820759f370ef0a6fcbd8639`  
		Last Modified: Sat, 01 Feb 2020 18:08:01 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:731f6e13d8ea683b85c2d516659def2ada874d12198ccb8aa607b0739cad71f9`  
		Last Modified: Sat, 01 Feb 2020 18:08:03 GMT  
		Size: 4.5 MB (4501283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c183de42679fb8b24485807f24d4d5e83833a5df99f2a1e22b9995d5a77a61c`  
		Last Modified: Sat, 01 Feb 2020 18:08:00 GMT  
		Size: 1.3 MB (1270478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de69b5c2f3c8d53585c798ec208eb58375608c919d5b70da51c3e4fcbb90e93`  
		Last Modified: Sat, 01 Feb 2020 18:08:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122a561a41965dc6801656b34be38f68631c1d58de3e96f908adf095b4eef2d8`  
		Last Modified: Fri, 21 Feb 2020 03:06:26 GMT  
		Size: 14.0 MB (13953499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1abf8e9f34f0c311ef662c5018bd573d0c85dbac8f76e4d8785731c2ccc11248`  
		Last Modified: Fri, 21 Feb 2020 03:06:19 GMT  
		Size: 28.3 KB (28327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e5887414166eb21c9f0d1eec78684013f1549a99d3e92c5841d6404df154bad`  
		Last Modified: Fri, 21 Feb 2020 03:06:18 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95adaca0707854ba4ac07bfb4228009e1d450ae64e3c1e6f028ecec3953face2`  
		Last Modified: Fri, 21 Feb 2020 03:06:49 GMT  
		Size: 96.2 MB (96238031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42c8c65423478ddb49dc4b60c64239044932073c5823b40051eded4637af3e19`  
		Last Modified: Fri, 21 Feb 2020 03:06:18 GMT  
		Size: 898.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ae93d9077ae38aafb8b06a9dd90ee1ede30761912d373cf290f778911daa8e1`  
		Last Modified: Fri, 21 Feb 2020 03:06:18 GMT  
		Size: 5.0 KB (5043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42131d6ef54e5a95f7b92e6c79a924c9cc8a47f685a85113b91439fbcfebf614`  
		Last Modified: Fri, 21 Feb 2020 03:06:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
