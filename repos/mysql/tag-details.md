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
$ docker pull mysql@sha256:7924ec534b844f9c7c0547fa95265516e8adf19ca475cffe911202037392d264
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:5` - linux; amd64

```console
$ docker pull mysql@sha256:283d2b89be722eb51b0cebd65fdcfac7e49c03eab40cfdcf73ff6d5c0cfacda9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.2 MB (158209474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66371c06f4ca82a19350bb8a0281208fcaf11951a4dd7ad0b5d246b5be1c9c41`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 16 Apr 2020 03:22:36 GMT
ADD file:865f9041e12eb341f0a394764ddc11db49cbc8b91d4fb57c6fb1960b68b1bb41 in / 
# Thu, 16 Apr 2020 03:22:36 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 10:04:13 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 16 Apr 2020 10:04:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 10:04:20 GMT
ENV GOSU_VERSION=1.7
# Thu, 16 Apr 2020 10:04:30 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& gpgconf --kill all 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Thu, 16 Apr 2020 10:04:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 16 Apr 2020 10:04:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 10:04:41 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Thu, 16 Apr 2020 10:05:17 GMT
ENV MYSQL_MAJOR=5.7
# Thu, 16 Apr 2020 10:05:17 GMT
ENV MYSQL_VERSION=5.7.29-1debian10
# Thu, 16 Apr 2020 10:05:18 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ buster mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Thu, 16 Apr 2020 10:05:52 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-server="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 777 /var/run/mysqld 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 16 Apr 2020 10:05:52 GMT
VOLUME [/var/lib/mysql]
# Thu, 16 Apr 2020 10:05:53 GMT
COPY file:4f14a879f00507ec1e489ab2afde4d14871f6edb4a42f72520400388739d7ede in /usr/local/bin/ 
# Thu, 16 Apr 2020 10:05:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 16 Apr 2020 10:05:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Apr 2020 10:05:54 GMT
EXPOSE 3306 33060
# Thu, 16 Apr 2020 10:05:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:123275d6e508d282237a22fefa5aef822b719a06496444ea89efa65da523fc4b`  
		Last Modified: Thu, 16 Apr 2020 03:31:44 GMT  
		Size: 27.1 MB (27098147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cddf5c7140b7596d94da456329ec66b76241f435e586f4390362a57d7b26ab`  
		Last Modified: Thu, 16 Apr 2020 10:07:32 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c17d442e14c91a582a572491492c59628829de516e8372b06ab961a10618d92a`  
		Last Modified: Thu, 16 Apr 2020 10:07:33 GMT  
		Size: 4.2 MB (4178047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc78b1e06f83723ca6b77ee558f3c0542ce91daff091183408270e70bb19345`  
		Last Modified: Thu, 16 Apr 2020 10:07:32 GMT  
		Size: 1.3 MB (1277317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd38802f42bb5d27698e758776815005a0281d6cbad8fade56d46b78d7849809`  
		Last Modified: Thu, 16 Apr 2020 10:07:31 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b370e336f2208dc21ab0e1d32ccfdcd4a3cea596667e33524eba5b4951900306`  
		Last Modified: Thu, 16 Apr 2020 10:07:38 GMT  
		Size: 13.4 MB (13443208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f519d6d4d2f67ba959be4d0913d0d6eeba8f0516bab9c5d57a777fb2a0c2ee56`  
		Last Modified: Thu, 16 Apr 2020 10:07:30 GMT  
		Size: 2.4 KB (2394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93fcd48f8a466b86832ee155e70bc738c74f34f62833e46627bd64a189ac5110`  
		Last Modified: Thu, 16 Apr 2020 10:08:12 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b3f78c0999300f9d34fbd828128385a92ad1d74a28a5e75a9efb4af454f525`  
		Last Modified: Thu, 16 Apr 2020 10:08:36 GMT  
		Size: 112.2 MB (112203091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0692e317044b9f7a93c30ab293c13f3f0b0332b2d3e39d4db7aa0b2cef097895`  
		Last Modified: Thu, 16 Apr 2020 10:08:12 GMT  
		Size: 5.1 KB (5075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf7d9d2736f83789ba83a2d79143015daa0cbd53a84d61d1e17577b4e5c5eaa`  
		Last Modified: Thu, 16 Apr 2020 10:08:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.6`

```console
$ docker pull mysql@sha256:a19ff9a78f9f9d140f02294162bcc960a758edcd9a9acbd5612eddfb039cf336
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:5.6` - linux; amd64

```console
$ docker pull mysql@sha256:1852b08fddc700b04b08c593ef570edbcd2004a2dccea2aa0cb53e22ec300f72
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.7 MB (102733161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87e6e56b2aa5079050138e3a0cb7d45242bd41973345136497bb8ad2a2eeb0c7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 16 Apr 2020 03:27:50 GMT
ADD file:40f52c233aecabf572a9db7450590d54d5e125fb00ecbb4a26fecd0b71e84eb8 in / 
# Thu, 16 Apr 2020 03:27:50 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 10:06:05 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 16 Apr 2020 10:06:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 10:06:13 GMT
ENV GOSU_VERSION=1.7
# Thu, 16 Apr 2020 10:06:28 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& gpgconf --kill all 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Thu, 16 Apr 2020 10:06:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 16 Apr 2020 10:06:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 10:06:44 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Thu, 16 Apr 2020 10:06:44 GMT
ENV MYSQL_MAJOR=5.6
# Thu, 16 Apr 2020 10:06:45 GMT
ENV MYSQL_VERSION=5.6.47-1debian9
# Thu, 16 Apr 2020 10:06:46 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ stretch mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Thu, 16 Apr 2020 10:07:07 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-server="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 777 /var/run/mysqld 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 16 Apr 2020 10:07:08 GMT
VOLUME [/var/lib/mysql]
# Thu, 16 Apr 2020 10:07:08 GMT
COPY file:4f14a879f00507ec1e489ab2afde4d14871f6edb4a42f72520400388739d7ede in /usr/local/bin/ 
# Thu, 16 Apr 2020 10:07:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 16 Apr 2020 10:07:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Apr 2020 10:07:10 GMT
EXPOSE 3306
# Thu, 16 Apr 2020 10:07:10 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5e35bd43cf7898d036f8515be74d45b2e3abd2a5534fc280de63a9c22dd175bd`  
		Last Modified: Thu, 16 Apr 2020 03:35:04 GMT  
		Size: 22.5 MB (22513476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3534514b63d6438efea9cb215f3448fcff41f162c6cfdf52c3275fbeca439f1a`  
		Last Modified: Thu, 16 Apr 2020 10:08:44 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b6064f2382631135dca6fca0a28623be07beb5e6404136ba42416d79130680`  
		Last Modified: Thu, 16 Apr 2020 10:08:45 GMT  
		Size: 4.5 MB (4501273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb6089c9c39a3086c2838632aacf4d1817ebac60ab28df57bcb2d2f6f995fdb7`  
		Last Modified: Thu, 16 Apr 2020 10:08:44 GMT  
		Size: 1.3 MB (1270493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e10f8540f7a449bf443f3a0779c96605090119bb97b230bd0b8d4a5ab6441e72`  
		Last Modified: Thu, 16 Apr 2020 10:08:43 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bcc38ff7aa61188d2ce8c76897c6346a6ad7caaf8f38d81909142f3b75be7da`  
		Last Modified: Thu, 16 Apr 2020 10:08:47 GMT  
		Size: 10.2 MB (10222072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b0fa6357fd521838cd25fbf3fba634282e62ac5aebb03890faeb2aad7e865e6`  
		Last Modified: Thu, 16 Apr 2020 10:08:42 GMT  
		Size: 28.3 KB (28325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:040b99b94ce035ea0c3bffd62499da86391bbba610e1e7288056ae976e168f1c`  
		Last Modified: Thu, 16 Apr 2020 10:08:43 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efe9e4216ee90a6f5bfd0f9ece2a955d4f127a71ee25885e2ea0da14cd8b8f54`  
		Last Modified: Thu, 16 Apr 2020 10:08:57 GMT  
		Size: 64.2 MB (64190236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e91c9bc673c4d5789bd6c9b3458c76149311d50e32d02a270c782fac0bd06229`  
		Last Modified: Thu, 16 Apr 2020 10:08:42 GMT  
		Size: 5.1 KB (5088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf808318f50714a605b19be08cf386524713ff1c8b56a40349ecec0df5413dbd`  
		Last Modified: Thu, 16 Apr 2020 10:08:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.6.47`

```console
$ docker pull mysql@sha256:a19ff9a78f9f9d140f02294162bcc960a758edcd9a9acbd5612eddfb039cf336
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:5.6.47` - linux; amd64

```console
$ docker pull mysql@sha256:1852b08fddc700b04b08c593ef570edbcd2004a2dccea2aa0cb53e22ec300f72
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.7 MB (102733161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87e6e56b2aa5079050138e3a0cb7d45242bd41973345136497bb8ad2a2eeb0c7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 16 Apr 2020 03:27:50 GMT
ADD file:40f52c233aecabf572a9db7450590d54d5e125fb00ecbb4a26fecd0b71e84eb8 in / 
# Thu, 16 Apr 2020 03:27:50 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 10:06:05 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 16 Apr 2020 10:06:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 10:06:13 GMT
ENV GOSU_VERSION=1.7
# Thu, 16 Apr 2020 10:06:28 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& gpgconf --kill all 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Thu, 16 Apr 2020 10:06:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 16 Apr 2020 10:06:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 10:06:44 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Thu, 16 Apr 2020 10:06:44 GMT
ENV MYSQL_MAJOR=5.6
# Thu, 16 Apr 2020 10:06:45 GMT
ENV MYSQL_VERSION=5.6.47-1debian9
# Thu, 16 Apr 2020 10:06:46 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ stretch mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Thu, 16 Apr 2020 10:07:07 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-server="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 777 /var/run/mysqld 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 16 Apr 2020 10:07:08 GMT
VOLUME [/var/lib/mysql]
# Thu, 16 Apr 2020 10:07:08 GMT
COPY file:4f14a879f00507ec1e489ab2afde4d14871f6edb4a42f72520400388739d7ede in /usr/local/bin/ 
# Thu, 16 Apr 2020 10:07:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 16 Apr 2020 10:07:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Apr 2020 10:07:10 GMT
EXPOSE 3306
# Thu, 16 Apr 2020 10:07:10 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5e35bd43cf7898d036f8515be74d45b2e3abd2a5534fc280de63a9c22dd175bd`  
		Last Modified: Thu, 16 Apr 2020 03:35:04 GMT  
		Size: 22.5 MB (22513476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3534514b63d6438efea9cb215f3448fcff41f162c6cfdf52c3275fbeca439f1a`  
		Last Modified: Thu, 16 Apr 2020 10:08:44 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b6064f2382631135dca6fca0a28623be07beb5e6404136ba42416d79130680`  
		Last Modified: Thu, 16 Apr 2020 10:08:45 GMT  
		Size: 4.5 MB (4501273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb6089c9c39a3086c2838632aacf4d1817ebac60ab28df57bcb2d2f6f995fdb7`  
		Last Modified: Thu, 16 Apr 2020 10:08:44 GMT  
		Size: 1.3 MB (1270493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e10f8540f7a449bf443f3a0779c96605090119bb97b230bd0b8d4a5ab6441e72`  
		Last Modified: Thu, 16 Apr 2020 10:08:43 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bcc38ff7aa61188d2ce8c76897c6346a6ad7caaf8f38d81909142f3b75be7da`  
		Last Modified: Thu, 16 Apr 2020 10:08:47 GMT  
		Size: 10.2 MB (10222072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b0fa6357fd521838cd25fbf3fba634282e62ac5aebb03890faeb2aad7e865e6`  
		Last Modified: Thu, 16 Apr 2020 10:08:42 GMT  
		Size: 28.3 KB (28325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:040b99b94ce035ea0c3bffd62499da86391bbba610e1e7288056ae976e168f1c`  
		Last Modified: Thu, 16 Apr 2020 10:08:43 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efe9e4216ee90a6f5bfd0f9ece2a955d4f127a71ee25885e2ea0da14cd8b8f54`  
		Last Modified: Thu, 16 Apr 2020 10:08:57 GMT  
		Size: 64.2 MB (64190236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e91c9bc673c4d5789bd6c9b3458c76149311d50e32d02a270c782fac0bd06229`  
		Last Modified: Thu, 16 Apr 2020 10:08:42 GMT  
		Size: 5.1 KB (5088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf808318f50714a605b19be08cf386524713ff1c8b56a40349ecec0df5413dbd`  
		Last Modified: Thu, 16 Apr 2020 10:08:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7`

```console
$ docker pull mysql@sha256:7924ec534b844f9c7c0547fa95265516e8adf19ca475cffe911202037392d264
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:5.7` - linux; amd64

```console
$ docker pull mysql@sha256:283d2b89be722eb51b0cebd65fdcfac7e49c03eab40cfdcf73ff6d5c0cfacda9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.2 MB (158209474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66371c06f4ca82a19350bb8a0281208fcaf11951a4dd7ad0b5d246b5be1c9c41`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 16 Apr 2020 03:22:36 GMT
ADD file:865f9041e12eb341f0a394764ddc11db49cbc8b91d4fb57c6fb1960b68b1bb41 in / 
# Thu, 16 Apr 2020 03:22:36 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 10:04:13 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 16 Apr 2020 10:04:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 10:04:20 GMT
ENV GOSU_VERSION=1.7
# Thu, 16 Apr 2020 10:04:30 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& gpgconf --kill all 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Thu, 16 Apr 2020 10:04:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 16 Apr 2020 10:04:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 10:04:41 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Thu, 16 Apr 2020 10:05:17 GMT
ENV MYSQL_MAJOR=5.7
# Thu, 16 Apr 2020 10:05:17 GMT
ENV MYSQL_VERSION=5.7.29-1debian10
# Thu, 16 Apr 2020 10:05:18 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ buster mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Thu, 16 Apr 2020 10:05:52 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-server="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 777 /var/run/mysqld 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 16 Apr 2020 10:05:52 GMT
VOLUME [/var/lib/mysql]
# Thu, 16 Apr 2020 10:05:53 GMT
COPY file:4f14a879f00507ec1e489ab2afde4d14871f6edb4a42f72520400388739d7ede in /usr/local/bin/ 
# Thu, 16 Apr 2020 10:05:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 16 Apr 2020 10:05:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Apr 2020 10:05:54 GMT
EXPOSE 3306 33060
# Thu, 16 Apr 2020 10:05:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:123275d6e508d282237a22fefa5aef822b719a06496444ea89efa65da523fc4b`  
		Last Modified: Thu, 16 Apr 2020 03:31:44 GMT  
		Size: 27.1 MB (27098147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cddf5c7140b7596d94da456329ec66b76241f435e586f4390362a57d7b26ab`  
		Last Modified: Thu, 16 Apr 2020 10:07:32 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c17d442e14c91a582a572491492c59628829de516e8372b06ab961a10618d92a`  
		Last Modified: Thu, 16 Apr 2020 10:07:33 GMT  
		Size: 4.2 MB (4178047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc78b1e06f83723ca6b77ee558f3c0542ce91daff091183408270e70bb19345`  
		Last Modified: Thu, 16 Apr 2020 10:07:32 GMT  
		Size: 1.3 MB (1277317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd38802f42bb5d27698e758776815005a0281d6cbad8fade56d46b78d7849809`  
		Last Modified: Thu, 16 Apr 2020 10:07:31 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b370e336f2208dc21ab0e1d32ccfdcd4a3cea596667e33524eba5b4951900306`  
		Last Modified: Thu, 16 Apr 2020 10:07:38 GMT  
		Size: 13.4 MB (13443208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f519d6d4d2f67ba959be4d0913d0d6eeba8f0516bab9c5d57a777fb2a0c2ee56`  
		Last Modified: Thu, 16 Apr 2020 10:07:30 GMT  
		Size: 2.4 KB (2394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93fcd48f8a466b86832ee155e70bc738c74f34f62833e46627bd64a189ac5110`  
		Last Modified: Thu, 16 Apr 2020 10:08:12 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b3f78c0999300f9d34fbd828128385a92ad1d74a28a5e75a9efb4af454f525`  
		Last Modified: Thu, 16 Apr 2020 10:08:36 GMT  
		Size: 112.2 MB (112203091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0692e317044b9f7a93c30ab293c13f3f0b0332b2d3e39d4db7aa0b2cef097895`  
		Last Modified: Thu, 16 Apr 2020 10:08:12 GMT  
		Size: 5.1 KB (5075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf7d9d2736f83789ba83a2d79143015daa0cbd53a84d61d1e17577b4e5c5eaa`  
		Last Modified: Thu, 16 Apr 2020 10:08:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.29`

```console
$ docker pull mysql@sha256:7924ec534b844f9c7c0547fa95265516e8adf19ca475cffe911202037392d264
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:5.7.29` - linux; amd64

```console
$ docker pull mysql@sha256:283d2b89be722eb51b0cebd65fdcfac7e49c03eab40cfdcf73ff6d5c0cfacda9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.2 MB (158209474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66371c06f4ca82a19350bb8a0281208fcaf11951a4dd7ad0b5d246b5be1c9c41`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 16 Apr 2020 03:22:36 GMT
ADD file:865f9041e12eb341f0a394764ddc11db49cbc8b91d4fb57c6fb1960b68b1bb41 in / 
# Thu, 16 Apr 2020 03:22:36 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 10:04:13 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 16 Apr 2020 10:04:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 10:04:20 GMT
ENV GOSU_VERSION=1.7
# Thu, 16 Apr 2020 10:04:30 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& gpgconf --kill all 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Thu, 16 Apr 2020 10:04:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 16 Apr 2020 10:04:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 10:04:41 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Thu, 16 Apr 2020 10:05:17 GMT
ENV MYSQL_MAJOR=5.7
# Thu, 16 Apr 2020 10:05:17 GMT
ENV MYSQL_VERSION=5.7.29-1debian10
# Thu, 16 Apr 2020 10:05:18 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ buster mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Thu, 16 Apr 2020 10:05:52 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-server="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 777 /var/run/mysqld 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 16 Apr 2020 10:05:52 GMT
VOLUME [/var/lib/mysql]
# Thu, 16 Apr 2020 10:05:53 GMT
COPY file:4f14a879f00507ec1e489ab2afde4d14871f6edb4a42f72520400388739d7ede in /usr/local/bin/ 
# Thu, 16 Apr 2020 10:05:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 16 Apr 2020 10:05:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Apr 2020 10:05:54 GMT
EXPOSE 3306 33060
# Thu, 16 Apr 2020 10:05:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:123275d6e508d282237a22fefa5aef822b719a06496444ea89efa65da523fc4b`  
		Last Modified: Thu, 16 Apr 2020 03:31:44 GMT  
		Size: 27.1 MB (27098147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cddf5c7140b7596d94da456329ec66b76241f435e586f4390362a57d7b26ab`  
		Last Modified: Thu, 16 Apr 2020 10:07:32 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c17d442e14c91a582a572491492c59628829de516e8372b06ab961a10618d92a`  
		Last Modified: Thu, 16 Apr 2020 10:07:33 GMT  
		Size: 4.2 MB (4178047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc78b1e06f83723ca6b77ee558f3c0542ce91daff091183408270e70bb19345`  
		Last Modified: Thu, 16 Apr 2020 10:07:32 GMT  
		Size: 1.3 MB (1277317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd38802f42bb5d27698e758776815005a0281d6cbad8fade56d46b78d7849809`  
		Last Modified: Thu, 16 Apr 2020 10:07:31 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b370e336f2208dc21ab0e1d32ccfdcd4a3cea596667e33524eba5b4951900306`  
		Last Modified: Thu, 16 Apr 2020 10:07:38 GMT  
		Size: 13.4 MB (13443208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f519d6d4d2f67ba959be4d0913d0d6eeba8f0516bab9c5d57a777fb2a0c2ee56`  
		Last Modified: Thu, 16 Apr 2020 10:07:30 GMT  
		Size: 2.4 KB (2394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93fcd48f8a466b86832ee155e70bc738c74f34f62833e46627bd64a189ac5110`  
		Last Modified: Thu, 16 Apr 2020 10:08:12 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b3f78c0999300f9d34fbd828128385a92ad1d74a28a5e75a9efb4af454f525`  
		Last Modified: Thu, 16 Apr 2020 10:08:36 GMT  
		Size: 112.2 MB (112203091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0692e317044b9f7a93c30ab293c13f3f0b0332b2d3e39d4db7aa0b2cef097895`  
		Last Modified: Thu, 16 Apr 2020 10:08:12 GMT  
		Size: 5.1 KB (5075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf7d9d2736f83789ba83a2d79143015daa0cbd53a84d61d1e17577b4e5c5eaa`  
		Last Modified: Thu, 16 Apr 2020 10:08:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8`

```console
$ docker pull mysql@sha256:7901b65a6be478f7f15348dec0440c491a364af202112c61cb3925d7fb67d8f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:8` - linux; amd64

```console
$ docker pull mysql@sha256:84c03100a74eb6650f07d3e06d5306ca26083238f193f6152ff71a39b7028b88
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.0 MB (158962710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f39f4b4d96c46135fde5f823025d51ddd37c49b8c6588f432cb3385a57702bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 16 Apr 2020 03:22:36 GMT
ADD file:865f9041e12eb341f0a394764ddc11db49cbc8b91d4fb57c6fb1960b68b1bb41 in / 
# Thu, 16 Apr 2020 03:22:36 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 10:04:13 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 16 Apr 2020 10:04:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 10:04:20 GMT
ENV GOSU_VERSION=1.7
# Thu, 16 Apr 2020 10:04:30 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& gpgconf --kill all 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Thu, 16 Apr 2020 10:04:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 16 Apr 2020 10:04:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 10:04:41 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Thu, 16 Apr 2020 10:04:41 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 16 Apr 2020 10:04:41 GMT
ENV MYSQL_VERSION=8.0.19-1debian10
# Thu, 16 Apr 2020 10:04:42 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ buster mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Thu, 16 Apr 2020 10:05:03 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-community-client="${MYSQL_VERSION}" mysql-community-server-core="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 777 /var/run/mysqld
# Thu, 16 Apr 2020 10:05:04 GMT
VOLUME [/var/lib/mysql]
# Thu, 16 Apr 2020 10:05:04 GMT
COPY dir:478f098f3681084f7493af1f04cbcd3eeda6f10e0dd2f5c740acd25328a73455 in /etc/mysql/ 
# Thu, 16 Apr 2020 10:05:04 GMT
COPY file:4f14a879f00507ec1e489ab2afde4d14871f6edb4a42f72520400388739d7ede in /usr/local/bin/ 
# Thu, 16 Apr 2020 10:05:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 16 Apr 2020 10:05:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Apr 2020 10:05:06 GMT
EXPOSE 3306 33060
# Thu, 16 Apr 2020 10:05:06 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:123275d6e508d282237a22fefa5aef822b719a06496444ea89efa65da523fc4b`  
		Last Modified: Thu, 16 Apr 2020 03:31:44 GMT  
		Size: 27.1 MB (27098147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cddf5c7140b7596d94da456329ec66b76241f435e586f4390362a57d7b26ab`  
		Last Modified: Thu, 16 Apr 2020 10:07:32 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c17d442e14c91a582a572491492c59628829de516e8372b06ab961a10618d92a`  
		Last Modified: Thu, 16 Apr 2020 10:07:33 GMT  
		Size: 4.2 MB (4178047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc78b1e06f83723ca6b77ee558f3c0542ce91daff091183408270e70bb19345`  
		Last Modified: Thu, 16 Apr 2020 10:07:32 GMT  
		Size: 1.3 MB (1277317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd38802f42bb5d27698e758776815005a0281d6cbad8fade56d46b78d7849809`  
		Last Modified: Thu, 16 Apr 2020 10:07:31 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b370e336f2208dc21ab0e1d32ccfdcd4a3cea596667e33524eba5b4951900306`  
		Last Modified: Thu, 16 Apr 2020 10:07:38 GMT  
		Size: 13.4 MB (13443208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f519d6d4d2f67ba959be4d0913d0d6eeba8f0516bab9c5d57a777fb2a0c2ee56`  
		Last Modified: Thu, 16 Apr 2020 10:07:30 GMT  
		Size: 2.4 KB (2394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52c0310cd3493e9effd440a75f8ee20ab84b84b7a1b1873d22bd9313ce388e7`  
		Last Modified: Thu, 16 Apr 2020 10:07:29 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd74fd7796ae1ed02fb96ae85399f1f2740c505f96b7d4c5794841399c6ce539`  
		Last Modified: Thu, 16 Apr 2020 10:08:04 GMT  
		Size: 113.0 MB (112955426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f08e322a29ce037fd2ea65b5895e34adfbfdef2f927bbd804679a649a0eeeb1`  
		Last Modified: Thu, 16 Apr 2020 10:07:29 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2caa0eda62a7b5ad9a35689edbf7ccb018a6b8d879f6fb02cf85fd3ca8672b32`  
		Last Modified: Thu, 16 Apr 2020 10:07:30 GMT  
		Size: 5.1 KB (5073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eac28354a6fe0fe973806356719e455aaf1f02acbb1256836c838c51e3b95bdd`  
		Last Modified: Thu, 16 Apr 2020 10:07:30 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0`

```console
$ docker pull mysql@sha256:7901b65a6be478f7f15348dec0440c491a364af202112c61cb3925d7fb67d8f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:8.0` - linux; amd64

```console
$ docker pull mysql@sha256:84c03100a74eb6650f07d3e06d5306ca26083238f193f6152ff71a39b7028b88
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.0 MB (158962710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f39f4b4d96c46135fde5f823025d51ddd37c49b8c6588f432cb3385a57702bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 16 Apr 2020 03:22:36 GMT
ADD file:865f9041e12eb341f0a394764ddc11db49cbc8b91d4fb57c6fb1960b68b1bb41 in / 
# Thu, 16 Apr 2020 03:22:36 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 10:04:13 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 16 Apr 2020 10:04:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 10:04:20 GMT
ENV GOSU_VERSION=1.7
# Thu, 16 Apr 2020 10:04:30 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& gpgconf --kill all 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Thu, 16 Apr 2020 10:04:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 16 Apr 2020 10:04:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 10:04:41 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Thu, 16 Apr 2020 10:04:41 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 16 Apr 2020 10:04:41 GMT
ENV MYSQL_VERSION=8.0.19-1debian10
# Thu, 16 Apr 2020 10:04:42 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ buster mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Thu, 16 Apr 2020 10:05:03 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-community-client="${MYSQL_VERSION}" mysql-community-server-core="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 777 /var/run/mysqld
# Thu, 16 Apr 2020 10:05:04 GMT
VOLUME [/var/lib/mysql]
# Thu, 16 Apr 2020 10:05:04 GMT
COPY dir:478f098f3681084f7493af1f04cbcd3eeda6f10e0dd2f5c740acd25328a73455 in /etc/mysql/ 
# Thu, 16 Apr 2020 10:05:04 GMT
COPY file:4f14a879f00507ec1e489ab2afde4d14871f6edb4a42f72520400388739d7ede in /usr/local/bin/ 
# Thu, 16 Apr 2020 10:05:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 16 Apr 2020 10:05:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Apr 2020 10:05:06 GMT
EXPOSE 3306 33060
# Thu, 16 Apr 2020 10:05:06 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:123275d6e508d282237a22fefa5aef822b719a06496444ea89efa65da523fc4b`  
		Last Modified: Thu, 16 Apr 2020 03:31:44 GMT  
		Size: 27.1 MB (27098147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cddf5c7140b7596d94da456329ec66b76241f435e586f4390362a57d7b26ab`  
		Last Modified: Thu, 16 Apr 2020 10:07:32 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c17d442e14c91a582a572491492c59628829de516e8372b06ab961a10618d92a`  
		Last Modified: Thu, 16 Apr 2020 10:07:33 GMT  
		Size: 4.2 MB (4178047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc78b1e06f83723ca6b77ee558f3c0542ce91daff091183408270e70bb19345`  
		Last Modified: Thu, 16 Apr 2020 10:07:32 GMT  
		Size: 1.3 MB (1277317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd38802f42bb5d27698e758776815005a0281d6cbad8fade56d46b78d7849809`  
		Last Modified: Thu, 16 Apr 2020 10:07:31 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b370e336f2208dc21ab0e1d32ccfdcd4a3cea596667e33524eba5b4951900306`  
		Last Modified: Thu, 16 Apr 2020 10:07:38 GMT  
		Size: 13.4 MB (13443208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f519d6d4d2f67ba959be4d0913d0d6eeba8f0516bab9c5d57a777fb2a0c2ee56`  
		Last Modified: Thu, 16 Apr 2020 10:07:30 GMT  
		Size: 2.4 KB (2394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52c0310cd3493e9effd440a75f8ee20ab84b84b7a1b1873d22bd9313ce388e7`  
		Last Modified: Thu, 16 Apr 2020 10:07:29 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd74fd7796ae1ed02fb96ae85399f1f2740c505f96b7d4c5794841399c6ce539`  
		Last Modified: Thu, 16 Apr 2020 10:08:04 GMT  
		Size: 113.0 MB (112955426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f08e322a29ce037fd2ea65b5895e34adfbfdef2f927bbd804679a649a0eeeb1`  
		Last Modified: Thu, 16 Apr 2020 10:07:29 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2caa0eda62a7b5ad9a35689edbf7ccb018a6b8d879f6fb02cf85fd3ca8672b32`  
		Last Modified: Thu, 16 Apr 2020 10:07:30 GMT  
		Size: 5.1 KB (5073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eac28354a6fe0fe973806356719e455aaf1f02acbb1256836c838c51e3b95bdd`  
		Last Modified: Thu, 16 Apr 2020 10:07:30 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.19`

```console
$ docker pull mysql@sha256:7901b65a6be478f7f15348dec0440c491a364af202112c61cb3925d7fb67d8f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:8.0.19` - linux; amd64

```console
$ docker pull mysql@sha256:84c03100a74eb6650f07d3e06d5306ca26083238f193f6152ff71a39b7028b88
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.0 MB (158962710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f39f4b4d96c46135fde5f823025d51ddd37c49b8c6588f432cb3385a57702bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 16 Apr 2020 03:22:36 GMT
ADD file:865f9041e12eb341f0a394764ddc11db49cbc8b91d4fb57c6fb1960b68b1bb41 in / 
# Thu, 16 Apr 2020 03:22:36 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 10:04:13 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 16 Apr 2020 10:04:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 10:04:20 GMT
ENV GOSU_VERSION=1.7
# Thu, 16 Apr 2020 10:04:30 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& gpgconf --kill all 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Thu, 16 Apr 2020 10:04:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 16 Apr 2020 10:04:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 10:04:41 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Thu, 16 Apr 2020 10:04:41 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 16 Apr 2020 10:04:41 GMT
ENV MYSQL_VERSION=8.0.19-1debian10
# Thu, 16 Apr 2020 10:04:42 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ buster mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Thu, 16 Apr 2020 10:05:03 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-community-client="${MYSQL_VERSION}" mysql-community-server-core="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 777 /var/run/mysqld
# Thu, 16 Apr 2020 10:05:04 GMT
VOLUME [/var/lib/mysql]
# Thu, 16 Apr 2020 10:05:04 GMT
COPY dir:478f098f3681084f7493af1f04cbcd3eeda6f10e0dd2f5c740acd25328a73455 in /etc/mysql/ 
# Thu, 16 Apr 2020 10:05:04 GMT
COPY file:4f14a879f00507ec1e489ab2afde4d14871f6edb4a42f72520400388739d7ede in /usr/local/bin/ 
# Thu, 16 Apr 2020 10:05:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 16 Apr 2020 10:05:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Apr 2020 10:05:06 GMT
EXPOSE 3306 33060
# Thu, 16 Apr 2020 10:05:06 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:123275d6e508d282237a22fefa5aef822b719a06496444ea89efa65da523fc4b`  
		Last Modified: Thu, 16 Apr 2020 03:31:44 GMT  
		Size: 27.1 MB (27098147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cddf5c7140b7596d94da456329ec66b76241f435e586f4390362a57d7b26ab`  
		Last Modified: Thu, 16 Apr 2020 10:07:32 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c17d442e14c91a582a572491492c59628829de516e8372b06ab961a10618d92a`  
		Last Modified: Thu, 16 Apr 2020 10:07:33 GMT  
		Size: 4.2 MB (4178047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc78b1e06f83723ca6b77ee558f3c0542ce91daff091183408270e70bb19345`  
		Last Modified: Thu, 16 Apr 2020 10:07:32 GMT  
		Size: 1.3 MB (1277317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd38802f42bb5d27698e758776815005a0281d6cbad8fade56d46b78d7849809`  
		Last Modified: Thu, 16 Apr 2020 10:07:31 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b370e336f2208dc21ab0e1d32ccfdcd4a3cea596667e33524eba5b4951900306`  
		Last Modified: Thu, 16 Apr 2020 10:07:38 GMT  
		Size: 13.4 MB (13443208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f519d6d4d2f67ba959be4d0913d0d6eeba8f0516bab9c5d57a777fb2a0c2ee56`  
		Last Modified: Thu, 16 Apr 2020 10:07:30 GMT  
		Size: 2.4 KB (2394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52c0310cd3493e9effd440a75f8ee20ab84b84b7a1b1873d22bd9313ce388e7`  
		Last Modified: Thu, 16 Apr 2020 10:07:29 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd74fd7796ae1ed02fb96ae85399f1f2740c505f96b7d4c5794841399c6ce539`  
		Last Modified: Thu, 16 Apr 2020 10:08:04 GMT  
		Size: 113.0 MB (112955426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f08e322a29ce037fd2ea65b5895e34adfbfdef2f927bbd804679a649a0eeeb1`  
		Last Modified: Thu, 16 Apr 2020 10:07:29 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2caa0eda62a7b5ad9a35689edbf7ccb018a6b8d879f6fb02cf85fd3ca8672b32`  
		Last Modified: Thu, 16 Apr 2020 10:07:30 GMT  
		Size: 5.1 KB (5073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eac28354a6fe0fe973806356719e455aaf1f02acbb1256836c838c51e3b95bdd`  
		Last Modified: Thu, 16 Apr 2020 10:07:30 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:latest`

```console
$ docker pull mysql@sha256:7901b65a6be478f7f15348dec0440c491a364af202112c61cb3925d7fb67d8f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:latest` - linux; amd64

```console
$ docker pull mysql@sha256:84c03100a74eb6650f07d3e06d5306ca26083238f193f6152ff71a39b7028b88
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.0 MB (158962710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f39f4b4d96c46135fde5f823025d51ddd37c49b8c6588f432cb3385a57702bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 16 Apr 2020 03:22:36 GMT
ADD file:865f9041e12eb341f0a394764ddc11db49cbc8b91d4fb57c6fb1960b68b1bb41 in / 
# Thu, 16 Apr 2020 03:22:36 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 10:04:13 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 16 Apr 2020 10:04:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 10:04:20 GMT
ENV GOSU_VERSION=1.7
# Thu, 16 Apr 2020 10:04:30 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& gpgconf --kill all 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Thu, 16 Apr 2020 10:04:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 16 Apr 2020 10:04:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 10:04:41 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Thu, 16 Apr 2020 10:04:41 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 16 Apr 2020 10:04:41 GMT
ENV MYSQL_VERSION=8.0.19-1debian10
# Thu, 16 Apr 2020 10:04:42 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ buster mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Thu, 16 Apr 2020 10:05:03 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-community-client="${MYSQL_VERSION}" mysql-community-server-core="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 777 /var/run/mysqld
# Thu, 16 Apr 2020 10:05:04 GMT
VOLUME [/var/lib/mysql]
# Thu, 16 Apr 2020 10:05:04 GMT
COPY dir:478f098f3681084f7493af1f04cbcd3eeda6f10e0dd2f5c740acd25328a73455 in /etc/mysql/ 
# Thu, 16 Apr 2020 10:05:04 GMT
COPY file:4f14a879f00507ec1e489ab2afde4d14871f6edb4a42f72520400388739d7ede in /usr/local/bin/ 
# Thu, 16 Apr 2020 10:05:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 16 Apr 2020 10:05:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Apr 2020 10:05:06 GMT
EXPOSE 3306 33060
# Thu, 16 Apr 2020 10:05:06 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:123275d6e508d282237a22fefa5aef822b719a06496444ea89efa65da523fc4b`  
		Last Modified: Thu, 16 Apr 2020 03:31:44 GMT  
		Size: 27.1 MB (27098147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cddf5c7140b7596d94da456329ec66b76241f435e586f4390362a57d7b26ab`  
		Last Modified: Thu, 16 Apr 2020 10:07:32 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c17d442e14c91a582a572491492c59628829de516e8372b06ab961a10618d92a`  
		Last Modified: Thu, 16 Apr 2020 10:07:33 GMT  
		Size: 4.2 MB (4178047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc78b1e06f83723ca6b77ee558f3c0542ce91daff091183408270e70bb19345`  
		Last Modified: Thu, 16 Apr 2020 10:07:32 GMT  
		Size: 1.3 MB (1277317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd38802f42bb5d27698e758776815005a0281d6cbad8fade56d46b78d7849809`  
		Last Modified: Thu, 16 Apr 2020 10:07:31 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b370e336f2208dc21ab0e1d32ccfdcd4a3cea596667e33524eba5b4951900306`  
		Last Modified: Thu, 16 Apr 2020 10:07:38 GMT  
		Size: 13.4 MB (13443208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f519d6d4d2f67ba959be4d0913d0d6eeba8f0516bab9c5d57a777fb2a0c2ee56`  
		Last Modified: Thu, 16 Apr 2020 10:07:30 GMT  
		Size: 2.4 KB (2394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52c0310cd3493e9effd440a75f8ee20ab84b84b7a1b1873d22bd9313ce388e7`  
		Last Modified: Thu, 16 Apr 2020 10:07:29 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd74fd7796ae1ed02fb96ae85399f1f2740c505f96b7d4c5794841399c6ce539`  
		Last Modified: Thu, 16 Apr 2020 10:08:04 GMT  
		Size: 113.0 MB (112955426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f08e322a29ce037fd2ea65b5895e34adfbfdef2f927bbd804679a649a0eeeb1`  
		Last Modified: Thu, 16 Apr 2020 10:07:29 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2caa0eda62a7b5ad9a35689edbf7ccb018a6b8d879f6fb02cf85fd3ca8672b32`  
		Last Modified: Thu, 16 Apr 2020 10:07:30 GMT  
		Size: 5.1 KB (5073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eac28354a6fe0fe973806356719e455aaf1f02acbb1256836c838c51e3b95bdd`  
		Last Modified: Thu, 16 Apr 2020 10:07:30 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
