<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mysql`

-	[`mysql:5`](#mysql5)
-	[`mysql:5.6`](#mysql56)
-	[`mysql:5.6.51`](#mysql5651)
-	[`mysql:5.7`](#mysql57)
-	[`mysql:5.7.35`](#mysql5735)
-	[`mysql:8`](#mysql8)
-	[`mysql:8.0`](#mysql80)
-	[`mysql:8.0.26`](#mysql8026)
-	[`mysql:latest`](#mysqllatest)

## `mysql:5`

```console
$ docker pull mysql@sha256:d9b934cdf6826629f8d02ea01f28b2c4ddb1ae27c32664b14867324b3e5e1291
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5` - linux; amd64

```console
$ docker pull mysql@sha256:bd8855544a384f579b6319b41e65044358cf7441968093517f176783de3e5892
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.8 MB (154791274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d7aba9171693947d53f474014821972bf25d72b7d143ce4af4c8d8484623417`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:46 GMT
ADD file:4ff85d9f6aa246746912db62dea02eb71750474bb29611e770516a1fcd217add in / 
# Fri, 03 Sep 2021 01:21:46 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 07:24:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 03 Sep 2021 07:24:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 07:24:10 GMT
ENV GOSU_VERSION=1.12
# Fri, 03 Sep 2021 07:24:19 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 03 Sep 2021 07:24:20 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 03 Sep 2021 07:24:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 07:24:37 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Fri, 03 Sep 2021 07:25:02 GMT
ENV MYSQL_MAJOR=5.7
# Fri, 03 Sep 2021 07:25:02 GMT
ENV MYSQL_VERSION=5.7.35-1debian10
# Fri, 03 Sep 2021 07:25:03 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Fri, 03 Sep 2021 07:25:22 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Fri, 03 Sep 2021 07:25:23 GMT
VOLUME [/var/lib/mysql]
# Fri, 03 Sep 2021 07:25:23 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Fri, 03 Sep 2021 07:25:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 07:25:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 07:25:25 GMT
EXPOSE 3306 33060
# Fri, 03 Sep 2021 07:25:25 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a330b6cecb98cd2425fd25fce36669073f593b3176b4ee14731e48c05d678cdd`  
		Last Modified: Fri, 03 Sep 2021 01:28:19 GMT  
		Size: 27.1 MB (27145844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8f656c32b8e3a7e91141bbf6f79477d5e5ca545dc3bca45b847970c69a9da8`  
		Last Modified: Fri, 03 Sep 2021 07:26:54 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e473c3f5534bbef2982c0d9ac87d51360349ebecd59be6f32f1264795492c2`  
		Last Modified: Fri, 03 Sep 2021 07:26:55 GMT  
		Size: 4.2 MB (4179248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:062463ea5d2f7a539ba8af442a61eccb65d1d605c49e474f26216ae82da29319`  
		Last Modified: Fri, 03 Sep 2021 07:26:52 GMT  
		Size: 1.4 MB (1419399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf7e3bdf4b6055892de6382cffb4023a9d4e21e81c9ef1cf930b0811aedb5d9`  
		Last Modified: Fri, 03 Sep 2021 07:26:51 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1839c0b7aac99d8db940e25d512abc1a3dd5e9619c0a4de3b547e0ecd0c8af66`  
		Last Modified: Fri, 03 Sep 2021 07:26:57 GMT  
		Size: 13.4 MB (13448601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0a0cfee6d048675739fb8444ae670180310f003e56ccdbfdfb9b29c06b4d3c`  
		Last Modified: Fri, 03 Sep 2021 07:26:51 GMT  
		Size: 1.9 KB (1873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae7a809788cc4e0fac757ec2ec551bafee3c5a8dca9568cb0622ef35764ebc5`  
		Last Modified: Fri, 03 Sep 2021 07:27:33 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dae5a82a61f0e8b8bf4c386d3673dcc4f25ed683dc735861fdc57095661ee953`  
		Last Modified: Fri, 03 Sep 2021 07:27:53 GMT  
		Size: 108.6 MB (108588546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7063da9569ebc6177d161307acd74e8d91bd7f7c4a305f7cd5ba659414291325`  
		Last Modified: Fri, 03 Sep 2021 07:27:32 GMT  
		Size: 5.5 KB (5537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51a9a9b4ef36843062f58891a65b146a63e3e93dcfb4573e51acb7c868e0b8a1`  
		Last Modified: Fri, 03 Sep 2021 07:27:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.6`

```console
$ docker pull mysql@sha256:35aa66157963240633625d6490d940069a1311fdfc022bf32116cbf95b90b541
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.6` - linux; amd64

```console
$ docker pull mysql@sha256:b4ee590a4b71a69498c6a933ee28baf41c8554f9bdac21d14cdd2d5766967a14
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.0 MB (102977049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e05271ec102ff31408cecf2f6752e555f1dfd1550c4de35b09c5cb2069cb6644`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 03 Sep 2021 01:23:46 GMT
ADD file:b8ae56829d548d5bff373622e23d0352bb9d313f09d8fea76dc1892b16c768c8 in / 
# Fri, 03 Sep 2021 01:23:46 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 07:25:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 03 Sep 2021 07:25:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 07:25:40 GMT
ENV GOSU_VERSION=1.12
# Fri, 03 Sep 2021 07:25:52 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 03 Sep 2021 07:25:52 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 03 Sep 2021 07:25:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 07:26:06 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Fri, 03 Sep 2021 07:26:06 GMT
ENV MYSQL_MAJOR=5.6
# Fri, 03 Sep 2021 07:26:06 GMT
ENV MYSQL_VERSION=5.6.51-1debian9
# Fri, 03 Sep 2021 07:26:07 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ stretch mysql-5.6' > /etc/apt/sources.list.d/mysql.list
# Fri, 03 Sep 2021 07:26:24 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Fri, 03 Sep 2021 07:26:24 GMT
VOLUME [/var/lib/mysql]
# Fri, 03 Sep 2021 07:26:25 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Fri, 03 Sep 2021 07:26:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 07:26:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 07:26:26 GMT
EXPOSE 3306
# Fri, 03 Sep 2021 07:26:26 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:442547fc262c2ebd1e2d44ea04cb011b78ec62cc2314c8c71c68ba31ae002cdb`  
		Last Modified: Fri, 03 Sep 2021 01:32:07 GMT  
		Size: 22.5 MB (22527429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf7161446875837edb3850d555bccf7a28158d8f1ebf83b847df22e1a2a508b`  
		Last Modified: Fri, 03 Sep 2021 07:28:12 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b3b16588b120cc81f140ad45189efa8275a5ff6c8a1b4965c9f4bdd94c07f8`  
		Last Modified: Fri, 03 Sep 2021 07:28:11 GMT  
		Size: 4.5 MB (4503298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c89f7ee6da81cbf462bd92b81c43d2e45aaa11a7de6e0dfa8afb65fd59ac9572`  
		Last Modified: Fri, 03 Sep 2021 07:28:10 GMT  
		Size: 1.4 MB (1412265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091490fb32f5f0a83cdf8efdf12cd4884285601bb201bf81a60e2326a424da02`  
		Last Modified: Fri, 03 Sep 2021 07:28:09 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eeb696bc30f2e49d72d58b9d84f78d43d110b29fb97121fd0b225bfd88e5103`  
		Last Modified: Fri, 03 Sep 2021 07:28:14 GMT  
		Size: 10.2 MB (10225837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a92263747b2f896745510ea63c07afe69acdffd911c8eef268c675cb9c19fda`  
		Last Modified: Fri, 03 Sep 2021 07:28:07 GMT  
		Size: 26.1 KB (26080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07097cad43f17d1f1bd808e80d820a038d867fa93f143281c98ea4fe6db38c8c`  
		Last Modified: Fri, 03 Sep 2021 07:28:07 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e09f00a44ec797df42afb97bef6503a9abd640eccf027f2d56af6b4749213aaa`  
		Last Modified: Fri, 03 Sep 2021 07:28:22 GMT  
		Size: 64.3 MB (64274358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18f954e29df72ccd75f14e3f4c0aeb8e68a857ff5bf6c9a8e52d54f4441977fd`  
		Last Modified: Fri, 03 Sep 2021 07:28:07 GMT  
		Size: 5.6 KB (5556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b46b7702c2b24bde2c03ca775f50f9a4462827960f187d326905a92914f44476`  
		Last Modified: Fri, 03 Sep 2021 07:28:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.6.51`

```console
$ docker pull mysql@sha256:35aa66157963240633625d6490d940069a1311fdfc022bf32116cbf95b90b541
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.6.51` - linux; amd64

```console
$ docker pull mysql@sha256:b4ee590a4b71a69498c6a933ee28baf41c8554f9bdac21d14cdd2d5766967a14
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.0 MB (102977049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e05271ec102ff31408cecf2f6752e555f1dfd1550c4de35b09c5cb2069cb6644`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 03 Sep 2021 01:23:46 GMT
ADD file:b8ae56829d548d5bff373622e23d0352bb9d313f09d8fea76dc1892b16c768c8 in / 
# Fri, 03 Sep 2021 01:23:46 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 07:25:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 03 Sep 2021 07:25:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 07:25:40 GMT
ENV GOSU_VERSION=1.12
# Fri, 03 Sep 2021 07:25:52 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 03 Sep 2021 07:25:52 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 03 Sep 2021 07:25:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 07:26:06 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Fri, 03 Sep 2021 07:26:06 GMT
ENV MYSQL_MAJOR=5.6
# Fri, 03 Sep 2021 07:26:06 GMT
ENV MYSQL_VERSION=5.6.51-1debian9
# Fri, 03 Sep 2021 07:26:07 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ stretch mysql-5.6' > /etc/apt/sources.list.d/mysql.list
# Fri, 03 Sep 2021 07:26:24 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Fri, 03 Sep 2021 07:26:24 GMT
VOLUME [/var/lib/mysql]
# Fri, 03 Sep 2021 07:26:25 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Fri, 03 Sep 2021 07:26:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 07:26:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 07:26:26 GMT
EXPOSE 3306
# Fri, 03 Sep 2021 07:26:26 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:442547fc262c2ebd1e2d44ea04cb011b78ec62cc2314c8c71c68ba31ae002cdb`  
		Last Modified: Fri, 03 Sep 2021 01:32:07 GMT  
		Size: 22.5 MB (22527429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf7161446875837edb3850d555bccf7a28158d8f1ebf83b847df22e1a2a508b`  
		Last Modified: Fri, 03 Sep 2021 07:28:12 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b3b16588b120cc81f140ad45189efa8275a5ff6c8a1b4965c9f4bdd94c07f8`  
		Last Modified: Fri, 03 Sep 2021 07:28:11 GMT  
		Size: 4.5 MB (4503298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c89f7ee6da81cbf462bd92b81c43d2e45aaa11a7de6e0dfa8afb65fd59ac9572`  
		Last Modified: Fri, 03 Sep 2021 07:28:10 GMT  
		Size: 1.4 MB (1412265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091490fb32f5f0a83cdf8efdf12cd4884285601bb201bf81a60e2326a424da02`  
		Last Modified: Fri, 03 Sep 2021 07:28:09 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eeb696bc30f2e49d72d58b9d84f78d43d110b29fb97121fd0b225bfd88e5103`  
		Last Modified: Fri, 03 Sep 2021 07:28:14 GMT  
		Size: 10.2 MB (10225837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a92263747b2f896745510ea63c07afe69acdffd911c8eef268c675cb9c19fda`  
		Last Modified: Fri, 03 Sep 2021 07:28:07 GMT  
		Size: 26.1 KB (26080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07097cad43f17d1f1bd808e80d820a038d867fa93f143281c98ea4fe6db38c8c`  
		Last Modified: Fri, 03 Sep 2021 07:28:07 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e09f00a44ec797df42afb97bef6503a9abd640eccf027f2d56af6b4749213aaa`  
		Last Modified: Fri, 03 Sep 2021 07:28:22 GMT  
		Size: 64.3 MB (64274358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18f954e29df72ccd75f14e3f4c0aeb8e68a857ff5bf6c9a8e52d54f4441977fd`  
		Last Modified: Fri, 03 Sep 2021 07:28:07 GMT  
		Size: 5.6 KB (5556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b46b7702c2b24bde2c03ca775f50f9a4462827960f187d326905a92914f44476`  
		Last Modified: Fri, 03 Sep 2021 07:28:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7`

```console
$ docker pull mysql@sha256:d9b934cdf6826629f8d02ea01f28b2c4ddb1ae27c32664b14867324b3e5e1291
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7` - linux; amd64

```console
$ docker pull mysql@sha256:bd8855544a384f579b6319b41e65044358cf7441968093517f176783de3e5892
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.8 MB (154791274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d7aba9171693947d53f474014821972bf25d72b7d143ce4af4c8d8484623417`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:46 GMT
ADD file:4ff85d9f6aa246746912db62dea02eb71750474bb29611e770516a1fcd217add in / 
# Fri, 03 Sep 2021 01:21:46 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 07:24:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 03 Sep 2021 07:24:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 07:24:10 GMT
ENV GOSU_VERSION=1.12
# Fri, 03 Sep 2021 07:24:19 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 03 Sep 2021 07:24:20 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 03 Sep 2021 07:24:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 07:24:37 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Fri, 03 Sep 2021 07:25:02 GMT
ENV MYSQL_MAJOR=5.7
# Fri, 03 Sep 2021 07:25:02 GMT
ENV MYSQL_VERSION=5.7.35-1debian10
# Fri, 03 Sep 2021 07:25:03 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Fri, 03 Sep 2021 07:25:22 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Fri, 03 Sep 2021 07:25:23 GMT
VOLUME [/var/lib/mysql]
# Fri, 03 Sep 2021 07:25:23 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Fri, 03 Sep 2021 07:25:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 07:25:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 07:25:25 GMT
EXPOSE 3306 33060
# Fri, 03 Sep 2021 07:25:25 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a330b6cecb98cd2425fd25fce36669073f593b3176b4ee14731e48c05d678cdd`  
		Last Modified: Fri, 03 Sep 2021 01:28:19 GMT  
		Size: 27.1 MB (27145844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8f656c32b8e3a7e91141bbf6f79477d5e5ca545dc3bca45b847970c69a9da8`  
		Last Modified: Fri, 03 Sep 2021 07:26:54 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e473c3f5534bbef2982c0d9ac87d51360349ebecd59be6f32f1264795492c2`  
		Last Modified: Fri, 03 Sep 2021 07:26:55 GMT  
		Size: 4.2 MB (4179248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:062463ea5d2f7a539ba8af442a61eccb65d1d605c49e474f26216ae82da29319`  
		Last Modified: Fri, 03 Sep 2021 07:26:52 GMT  
		Size: 1.4 MB (1419399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf7e3bdf4b6055892de6382cffb4023a9d4e21e81c9ef1cf930b0811aedb5d9`  
		Last Modified: Fri, 03 Sep 2021 07:26:51 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1839c0b7aac99d8db940e25d512abc1a3dd5e9619c0a4de3b547e0ecd0c8af66`  
		Last Modified: Fri, 03 Sep 2021 07:26:57 GMT  
		Size: 13.4 MB (13448601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0a0cfee6d048675739fb8444ae670180310f003e56ccdbfdfb9b29c06b4d3c`  
		Last Modified: Fri, 03 Sep 2021 07:26:51 GMT  
		Size: 1.9 KB (1873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae7a809788cc4e0fac757ec2ec551bafee3c5a8dca9568cb0622ef35764ebc5`  
		Last Modified: Fri, 03 Sep 2021 07:27:33 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dae5a82a61f0e8b8bf4c386d3673dcc4f25ed683dc735861fdc57095661ee953`  
		Last Modified: Fri, 03 Sep 2021 07:27:53 GMT  
		Size: 108.6 MB (108588546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7063da9569ebc6177d161307acd74e8d91bd7f7c4a305f7cd5ba659414291325`  
		Last Modified: Fri, 03 Sep 2021 07:27:32 GMT  
		Size: 5.5 KB (5537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51a9a9b4ef36843062f58891a65b146a63e3e93dcfb4573e51acb7c868e0b8a1`  
		Last Modified: Fri, 03 Sep 2021 07:27:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.35`

```console
$ docker pull mysql@sha256:d9b934cdf6826629f8d02ea01f28b2c4ddb1ae27c32664b14867324b3e5e1291
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.35` - linux; amd64

```console
$ docker pull mysql@sha256:bd8855544a384f579b6319b41e65044358cf7441968093517f176783de3e5892
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.8 MB (154791274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d7aba9171693947d53f474014821972bf25d72b7d143ce4af4c8d8484623417`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:46 GMT
ADD file:4ff85d9f6aa246746912db62dea02eb71750474bb29611e770516a1fcd217add in / 
# Fri, 03 Sep 2021 01:21:46 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 07:24:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 03 Sep 2021 07:24:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 07:24:10 GMT
ENV GOSU_VERSION=1.12
# Fri, 03 Sep 2021 07:24:19 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 03 Sep 2021 07:24:20 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 03 Sep 2021 07:24:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 07:24:37 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Fri, 03 Sep 2021 07:25:02 GMT
ENV MYSQL_MAJOR=5.7
# Fri, 03 Sep 2021 07:25:02 GMT
ENV MYSQL_VERSION=5.7.35-1debian10
# Fri, 03 Sep 2021 07:25:03 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Fri, 03 Sep 2021 07:25:22 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Fri, 03 Sep 2021 07:25:23 GMT
VOLUME [/var/lib/mysql]
# Fri, 03 Sep 2021 07:25:23 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Fri, 03 Sep 2021 07:25:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 07:25:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 07:25:25 GMT
EXPOSE 3306 33060
# Fri, 03 Sep 2021 07:25:25 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a330b6cecb98cd2425fd25fce36669073f593b3176b4ee14731e48c05d678cdd`  
		Last Modified: Fri, 03 Sep 2021 01:28:19 GMT  
		Size: 27.1 MB (27145844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8f656c32b8e3a7e91141bbf6f79477d5e5ca545dc3bca45b847970c69a9da8`  
		Last Modified: Fri, 03 Sep 2021 07:26:54 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e473c3f5534bbef2982c0d9ac87d51360349ebecd59be6f32f1264795492c2`  
		Last Modified: Fri, 03 Sep 2021 07:26:55 GMT  
		Size: 4.2 MB (4179248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:062463ea5d2f7a539ba8af442a61eccb65d1d605c49e474f26216ae82da29319`  
		Last Modified: Fri, 03 Sep 2021 07:26:52 GMT  
		Size: 1.4 MB (1419399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf7e3bdf4b6055892de6382cffb4023a9d4e21e81c9ef1cf930b0811aedb5d9`  
		Last Modified: Fri, 03 Sep 2021 07:26:51 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1839c0b7aac99d8db940e25d512abc1a3dd5e9619c0a4de3b547e0ecd0c8af66`  
		Last Modified: Fri, 03 Sep 2021 07:26:57 GMT  
		Size: 13.4 MB (13448601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0a0cfee6d048675739fb8444ae670180310f003e56ccdbfdfb9b29c06b4d3c`  
		Last Modified: Fri, 03 Sep 2021 07:26:51 GMT  
		Size: 1.9 KB (1873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae7a809788cc4e0fac757ec2ec551bafee3c5a8dca9568cb0622ef35764ebc5`  
		Last Modified: Fri, 03 Sep 2021 07:27:33 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dae5a82a61f0e8b8bf4c386d3673dcc4f25ed683dc735861fdc57095661ee953`  
		Last Modified: Fri, 03 Sep 2021 07:27:53 GMT  
		Size: 108.6 MB (108588546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7063da9569ebc6177d161307acd74e8d91bd7f7c4a305f7cd5ba659414291325`  
		Last Modified: Fri, 03 Sep 2021 07:27:32 GMT  
		Size: 5.5 KB (5537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51a9a9b4ef36843062f58891a65b146a63e3e93dcfb4573e51acb7c868e0b8a1`  
		Last Modified: Fri, 03 Sep 2021 07:27:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8`

```console
$ docker pull mysql@sha256:99e0989e7e3797cfbdb8d51a19d32c8d286dd8862794d01a547651a896bcf00c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8` - linux; amd64

```console
$ docker pull mysql@sha256:75e71ac9b332935f396d85965213a64f1bd6fc7c42e9900b106f7af462c599b0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.6 MB (150593976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0716d6ebcc1a61c5a296fcb187e71f93531e510d4e4400267e2e502103d0194c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:46 GMT
ADD file:4ff85d9f6aa246746912db62dea02eb71750474bb29611e770516a1fcd217add in / 
# Fri, 03 Sep 2021 01:21:46 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 07:24:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 03 Sep 2021 07:24:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 07:24:10 GMT
ENV GOSU_VERSION=1.12
# Fri, 03 Sep 2021 07:24:19 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 03 Sep 2021 07:24:20 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 03 Sep 2021 07:24:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 07:24:37 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Fri, 03 Sep 2021 07:24:37 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 03 Sep 2021 07:24:37 GMT
ENV MYSQL_VERSION=8.0.26-1debian10
# Fri, 03 Sep 2021 07:24:38 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Fri, 03 Sep 2021 07:24:54 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Fri, 03 Sep 2021 07:24:55 GMT
VOLUME [/var/lib/mysql]
# Fri, 03 Sep 2021 07:24:55 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Fri, 03 Sep 2021 07:24:55 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Fri, 03 Sep 2021 07:24:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 07:24:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 07:24:57 GMT
EXPOSE 3306 33060
# Fri, 03 Sep 2021 07:24:57 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a330b6cecb98cd2425fd25fce36669073f593b3176b4ee14731e48c05d678cdd`  
		Last Modified: Fri, 03 Sep 2021 01:28:19 GMT  
		Size: 27.1 MB (27145844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8f656c32b8e3a7e91141bbf6f79477d5e5ca545dc3bca45b847970c69a9da8`  
		Last Modified: Fri, 03 Sep 2021 07:26:54 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e473c3f5534bbef2982c0d9ac87d51360349ebecd59be6f32f1264795492c2`  
		Last Modified: Fri, 03 Sep 2021 07:26:55 GMT  
		Size: 4.2 MB (4179248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:062463ea5d2f7a539ba8af442a61eccb65d1d605c49e474f26216ae82da29319`  
		Last Modified: Fri, 03 Sep 2021 07:26:52 GMT  
		Size: 1.4 MB (1419399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf7e3bdf4b6055892de6382cffb4023a9d4e21e81c9ef1cf930b0811aedb5d9`  
		Last Modified: Fri, 03 Sep 2021 07:26:51 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1839c0b7aac99d8db940e25d512abc1a3dd5e9619c0a4de3b547e0ecd0c8af66`  
		Last Modified: Fri, 03 Sep 2021 07:26:57 GMT  
		Size: 13.4 MB (13448601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0a0cfee6d048675739fb8444ae670180310f003e56ccdbfdfb9b29c06b4d3c`  
		Last Modified: Fri, 03 Sep 2021 07:26:51 GMT  
		Size: 1.9 KB (1873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b42041bb11e44bffa900fe6d4065cd027c837ae66d229306cc3aede3bfffb57`  
		Last Modified: Fri, 03 Sep 2021 07:26:49 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10459d86c7e650a8a3d9d1925dccee298f10719b536ff0acc7a0b2fc836de2a0`  
		Last Modified: Fri, 03 Sep 2021 07:27:14 GMT  
		Size: 104.4 MB (104390400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7199599d5f952f5e3d2c5f854235b7a6401d9e57131554624f076fc4f8e2146`  
		Last Modified: Fri, 03 Sep 2021 07:26:49 GMT  
		Size: 843.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d6f51e17d45c487898ecef1276abded78d694d3fb8883a9076351a0f324d6cd`  
		Last Modified: Fri, 03 Sep 2021 07:26:49 GMT  
		Size: 5.5 KB (5538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50e0789bacad72deabe6dc28facce8bcca3d9fe79deb9b33d7cb20d9904c2d6f`  
		Last Modified: Fri, 03 Sep 2021 07:26:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0`

```console
$ docker pull mysql@sha256:99e0989e7e3797cfbdb8d51a19d32c8d286dd8862794d01a547651a896bcf00c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0` - linux; amd64

```console
$ docker pull mysql@sha256:75e71ac9b332935f396d85965213a64f1bd6fc7c42e9900b106f7af462c599b0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.6 MB (150593976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0716d6ebcc1a61c5a296fcb187e71f93531e510d4e4400267e2e502103d0194c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:46 GMT
ADD file:4ff85d9f6aa246746912db62dea02eb71750474bb29611e770516a1fcd217add in / 
# Fri, 03 Sep 2021 01:21:46 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 07:24:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 03 Sep 2021 07:24:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 07:24:10 GMT
ENV GOSU_VERSION=1.12
# Fri, 03 Sep 2021 07:24:19 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 03 Sep 2021 07:24:20 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 03 Sep 2021 07:24:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 07:24:37 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Fri, 03 Sep 2021 07:24:37 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 03 Sep 2021 07:24:37 GMT
ENV MYSQL_VERSION=8.0.26-1debian10
# Fri, 03 Sep 2021 07:24:38 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Fri, 03 Sep 2021 07:24:54 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Fri, 03 Sep 2021 07:24:55 GMT
VOLUME [/var/lib/mysql]
# Fri, 03 Sep 2021 07:24:55 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Fri, 03 Sep 2021 07:24:55 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Fri, 03 Sep 2021 07:24:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 07:24:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 07:24:57 GMT
EXPOSE 3306 33060
# Fri, 03 Sep 2021 07:24:57 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a330b6cecb98cd2425fd25fce36669073f593b3176b4ee14731e48c05d678cdd`  
		Last Modified: Fri, 03 Sep 2021 01:28:19 GMT  
		Size: 27.1 MB (27145844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8f656c32b8e3a7e91141bbf6f79477d5e5ca545dc3bca45b847970c69a9da8`  
		Last Modified: Fri, 03 Sep 2021 07:26:54 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e473c3f5534bbef2982c0d9ac87d51360349ebecd59be6f32f1264795492c2`  
		Last Modified: Fri, 03 Sep 2021 07:26:55 GMT  
		Size: 4.2 MB (4179248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:062463ea5d2f7a539ba8af442a61eccb65d1d605c49e474f26216ae82da29319`  
		Last Modified: Fri, 03 Sep 2021 07:26:52 GMT  
		Size: 1.4 MB (1419399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf7e3bdf4b6055892de6382cffb4023a9d4e21e81c9ef1cf930b0811aedb5d9`  
		Last Modified: Fri, 03 Sep 2021 07:26:51 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1839c0b7aac99d8db940e25d512abc1a3dd5e9619c0a4de3b547e0ecd0c8af66`  
		Last Modified: Fri, 03 Sep 2021 07:26:57 GMT  
		Size: 13.4 MB (13448601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0a0cfee6d048675739fb8444ae670180310f003e56ccdbfdfb9b29c06b4d3c`  
		Last Modified: Fri, 03 Sep 2021 07:26:51 GMT  
		Size: 1.9 KB (1873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b42041bb11e44bffa900fe6d4065cd027c837ae66d229306cc3aede3bfffb57`  
		Last Modified: Fri, 03 Sep 2021 07:26:49 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10459d86c7e650a8a3d9d1925dccee298f10719b536ff0acc7a0b2fc836de2a0`  
		Last Modified: Fri, 03 Sep 2021 07:27:14 GMT  
		Size: 104.4 MB (104390400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7199599d5f952f5e3d2c5f854235b7a6401d9e57131554624f076fc4f8e2146`  
		Last Modified: Fri, 03 Sep 2021 07:26:49 GMT  
		Size: 843.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d6f51e17d45c487898ecef1276abded78d694d3fb8883a9076351a0f324d6cd`  
		Last Modified: Fri, 03 Sep 2021 07:26:49 GMT  
		Size: 5.5 KB (5538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50e0789bacad72deabe6dc28facce8bcca3d9fe79deb9b33d7cb20d9904c2d6f`  
		Last Modified: Fri, 03 Sep 2021 07:26:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.26`

```console
$ docker pull mysql@sha256:99e0989e7e3797cfbdb8d51a19d32c8d286dd8862794d01a547651a896bcf00c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0.26` - linux; amd64

```console
$ docker pull mysql@sha256:75e71ac9b332935f396d85965213a64f1bd6fc7c42e9900b106f7af462c599b0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.6 MB (150593976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0716d6ebcc1a61c5a296fcb187e71f93531e510d4e4400267e2e502103d0194c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:46 GMT
ADD file:4ff85d9f6aa246746912db62dea02eb71750474bb29611e770516a1fcd217add in / 
# Fri, 03 Sep 2021 01:21:46 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 07:24:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 03 Sep 2021 07:24:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 07:24:10 GMT
ENV GOSU_VERSION=1.12
# Fri, 03 Sep 2021 07:24:19 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 03 Sep 2021 07:24:20 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 03 Sep 2021 07:24:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 07:24:37 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Fri, 03 Sep 2021 07:24:37 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 03 Sep 2021 07:24:37 GMT
ENV MYSQL_VERSION=8.0.26-1debian10
# Fri, 03 Sep 2021 07:24:38 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Fri, 03 Sep 2021 07:24:54 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Fri, 03 Sep 2021 07:24:55 GMT
VOLUME [/var/lib/mysql]
# Fri, 03 Sep 2021 07:24:55 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Fri, 03 Sep 2021 07:24:55 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Fri, 03 Sep 2021 07:24:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 07:24:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 07:24:57 GMT
EXPOSE 3306 33060
# Fri, 03 Sep 2021 07:24:57 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a330b6cecb98cd2425fd25fce36669073f593b3176b4ee14731e48c05d678cdd`  
		Last Modified: Fri, 03 Sep 2021 01:28:19 GMT  
		Size: 27.1 MB (27145844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8f656c32b8e3a7e91141bbf6f79477d5e5ca545dc3bca45b847970c69a9da8`  
		Last Modified: Fri, 03 Sep 2021 07:26:54 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e473c3f5534bbef2982c0d9ac87d51360349ebecd59be6f32f1264795492c2`  
		Last Modified: Fri, 03 Sep 2021 07:26:55 GMT  
		Size: 4.2 MB (4179248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:062463ea5d2f7a539ba8af442a61eccb65d1d605c49e474f26216ae82da29319`  
		Last Modified: Fri, 03 Sep 2021 07:26:52 GMT  
		Size: 1.4 MB (1419399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf7e3bdf4b6055892de6382cffb4023a9d4e21e81c9ef1cf930b0811aedb5d9`  
		Last Modified: Fri, 03 Sep 2021 07:26:51 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1839c0b7aac99d8db940e25d512abc1a3dd5e9619c0a4de3b547e0ecd0c8af66`  
		Last Modified: Fri, 03 Sep 2021 07:26:57 GMT  
		Size: 13.4 MB (13448601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0a0cfee6d048675739fb8444ae670180310f003e56ccdbfdfb9b29c06b4d3c`  
		Last Modified: Fri, 03 Sep 2021 07:26:51 GMT  
		Size: 1.9 KB (1873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b42041bb11e44bffa900fe6d4065cd027c837ae66d229306cc3aede3bfffb57`  
		Last Modified: Fri, 03 Sep 2021 07:26:49 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10459d86c7e650a8a3d9d1925dccee298f10719b536ff0acc7a0b2fc836de2a0`  
		Last Modified: Fri, 03 Sep 2021 07:27:14 GMT  
		Size: 104.4 MB (104390400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7199599d5f952f5e3d2c5f854235b7a6401d9e57131554624f076fc4f8e2146`  
		Last Modified: Fri, 03 Sep 2021 07:26:49 GMT  
		Size: 843.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d6f51e17d45c487898ecef1276abded78d694d3fb8883a9076351a0f324d6cd`  
		Last Modified: Fri, 03 Sep 2021 07:26:49 GMT  
		Size: 5.5 KB (5538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50e0789bacad72deabe6dc28facce8bcca3d9fe79deb9b33d7cb20d9904c2d6f`  
		Last Modified: Fri, 03 Sep 2021 07:26:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:latest`

```console
$ docker pull mysql@sha256:99e0989e7e3797cfbdb8d51a19d32c8d286dd8862794d01a547651a896bcf00c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:latest` - linux; amd64

```console
$ docker pull mysql@sha256:75e71ac9b332935f396d85965213a64f1bd6fc7c42e9900b106f7af462c599b0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.6 MB (150593976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0716d6ebcc1a61c5a296fcb187e71f93531e510d4e4400267e2e502103d0194c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:46 GMT
ADD file:4ff85d9f6aa246746912db62dea02eb71750474bb29611e770516a1fcd217add in / 
# Fri, 03 Sep 2021 01:21:46 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 07:24:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 03 Sep 2021 07:24:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 07:24:10 GMT
ENV GOSU_VERSION=1.12
# Fri, 03 Sep 2021 07:24:19 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 03 Sep 2021 07:24:20 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 03 Sep 2021 07:24:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 07:24:37 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Fri, 03 Sep 2021 07:24:37 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 03 Sep 2021 07:24:37 GMT
ENV MYSQL_VERSION=8.0.26-1debian10
# Fri, 03 Sep 2021 07:24:38 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Fri, 03 Sep 2021 07:24:54 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Fri, 03 Sep 2021 07:24:55 GMT
VOLUME [/var/lib/mysql]
# Fri, 03 Sep 2021 07:24:55 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Fri, 03 Sep 2021 07:24:55 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Fri, 03 Sep 2021 07:24:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 07:24:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 07:24:57 GMT
EXPOSE 3306 33060
# Fri, 03 Sep 2021 07:24:57 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a330b6cecb98cd2425fd25fce36669073f593b3176b4ee14731e48c05d678cdd`  
		Last Modified: Fri, 03 Sep 2021 01:28:19 GMT  
		Size: 27.1 MB (27145844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8f656c32b8e3a7e91141bbf6f79477d5e5ca545dc3bca45b847970c69a9da8`  
		Last Modified: Fri, 03 Sep 2021 07:26:54 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e473c3f5534bbef2982c0d9ac87d51360349ebecd59be6f32f1264795492c2`  
		Last Modified: Fri, 03 Sep 2021 07:26:55 GMT  
		Size: 4.2 MB (4179248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:062463ea5d2f7a539ba8af442a61eccb65d1d605c49e474f26216ae82da29319`  
		Last Modified: Fri, 03 Sep 2021 07:26:52 GMT  
		Size: 1.4 MB (1419399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf7e3bdf4b6055892de6382cffb4023a9d4e21e81c9ef1cf930b0811aedb5d9`  
		Last Modified: Fri, 03 Sep 2021 07:26:51 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1839c0b7aac99d8db940e25d512abc1a3dd5e9619c0a4de3b547e0ecd0c8af66`  
		Last Modified: Fri, 03 Sep 2021 07:26:57 GMT  
		Size: 13.4 MB (13448601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0a0cfee6d048675739fb8444ae670180310f003e56ccdbfdfb9b29c06b4d3c`  
		Last Modified: Fri, 03 Sep 2021 07:26:51 GMT  
		Size: 1.9 KB (1873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b42041bb11e44bffa900fe6d4065cd027c837ae66d229306cc3aede3bfffb57`  
		Last Modified: Fri, 03 Sep 2021 07:26:49 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10459d86c7e650a8a3d9d1925dccee298f10719b536ff0acc7a0b2fc836de2a0`  
		Last Modified: Fri, 03 Sep 2021 07:27:14 GMT  
		Size: 104.4 MB (104390400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7199599d5f952f5e3d2c5f854235b7a6401d9e57131554624f076fc4f8e2146`  
		Last Modified: Fri, 03 Sep 2021 07:26:49 GMT  
		Size: 843.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d6f51e17d45c487898ecef1276abded78d694d3fb8883a9076351a0f324d6cd`  
		Last Modified: Fri, 03 Sep 2021 07:26:49 GMT  
		Size: 5.5 KB (5538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50e0789bacad72deabe6dc28facce8bcca3d9fe79deb9b33d7cb20d9904c2d6f`  
		Last Modified: Fri, 03 Sep 2021 07:26:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
