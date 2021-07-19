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
$ docker pull mysql@sha256:956e11ac581cad9ac8747a9a1d61b8ffcfa6845e0f23bdbab6ba20a2ad792cbf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5` - linux; amd64

```console
$ docker pull mysql@sha256:ea4f3391e56e132623d37964e66761e8f390d8cfbeb0c7b3184b533d697379e3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.8 MB (154790337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f1d21c1025ab10f9994398f01bb09eb7b6bd0861b3cff0fc9e0a8c265615772`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 07:10:38 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 23 Jun 2021 07:10:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 07:10:47 GMT
ENV GOSU_VERSION=1.12
# Wed, 23 Jun 2021 07:11:06 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 23 Jun 2021 07:11:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 23 Jun 2021 07:11:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Mon, 19 Jul 2021 21:20:18 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Mon, 19 Jul 2021 21:20:41 GMT
ENV MYSQL_MAJOR=5.7
# Mon, 19 Jul 2021 21:20:41 GMT
ENV MYSQL_VERSION=5.7.35-1debian10
# Mon, 19 Jul 2021 21:20:42 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Mon, 19 Jul 2021 21:21:02 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Mon, 19 Jul 2021 21:21:02 GMT
VOLUME [/var/lib/mysql]
# Mon, 19 Jul 2021 21:21:03 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Mon, 19 Jul 2021 21:21:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 19 Jul 2021 21:21:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 19 Jul 2021 21:21:04 GMT
EXPOSE 3306 33060
# Mon, 19 Jul 2021 21:21:04 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a462b60610f5b230bfc054037dcc15dfbd114bc91472a819ac5b4049cb7f030c`  
		Last Modified: Wed, 23 Jun 2021 07:13:58 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578fafb77ab871790dd20afa25cea55309e5862a43eb6fdca5f3c1387ab7b833`  
		Last Modified: Wed, 23 Jun 2021 07:14:00 GMT  
		Size: 4.2 MB (4179324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5240460060374bac3b015544387eba2355e7b003da15c162e7166984437c31d7`  
		Last Modified: Wed, 23 Jun 2021 07:13:57 GMT  
		Size: 1.4 MB (1419480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0cbe54c88555c61f35df860e431717e56b7198eb3a9fa642d14ea6e94dc6edc`  
		Last Modified: Wed, 23 Jun 2021 07:13:56 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa18e05cc46d159c053ebf379685cef648b64d4bb39a4fa76dc7c8a6fadad89a`  
		Last Modified: Wed, 23 Jun 2021 07:14:01 GMT  
		Size: 13.4 MB (13447715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd6f649b1d0ad67dac3c7030f08df70fd82163dc4647b1971b7767d722f61cf6`  
		Last Modified: Mon, 19 Jul 2021 21:22:01 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a2b858b000b70f17957436b46151ad03150c634a0105764a09698711d296742`  
		Last Modified: Mon, 19 Jul 2021 21:22:39 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322182b1742269101681ce76d2a57a8c8c03b05b32a6a7ce989f90673e1e5a89`  
		Last Modified: Mon, 19 Jul 2021 21:22:53 GMT  
		Size: 108.6 MB (108588326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070e28050a8889df0d941be3ca8238bc7e7d6d1ebdc76b95753a2b8481a6ea4d`  
		Last Modified: Mon, 19 Jul 2021 21:22:38 GMT  
		Size: 5.5 KB (5541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:613bdfd8796e97816bbd22c43f893270073ded2bf82830c613d274c203de6447`  
		Last Modified: Mon, 19 Jul 2021 21:22:38 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.6`

```console
$ docker pull mysql@sha256:7888210cff8d7380909405787754953ba9a0dd1e7c3ba35dec2b48a007314701
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.6` - linux; amd64

```console
$ docker pull mysql@sha256:cec6c24d7a4141fa3711bfa0ff1cb66065ba4f0b18886ebec5a22c61c5f533b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.0 MB (102970826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6db4571057fc7fede46cc4e91b2ec088424d78a691e53d4e96f85cc116fdd3eb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 23 Jun 2021 00:22:13 GMT
ADD file:a63c6cc73701d6cb7195338c446b9e92ef6b7a0f9321f6cc1bf8738e3da57c66 in / 
# Wed, 23 Jun 2021 00:22:14 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 07:12:38 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 23 Jun 2021 07:12:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 07:12:46 GMT
ENV GOSU_VERSION=1.12
# Wed, 23 Jun 2021 07:12:58 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 23 Jun 2021 07:12:59 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 23 Jun 2021 07:13:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Mon, 19 Jul 2021 21:21:15 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Mon, 19 Jul 2021 21:21:15 GMT
ENV MYSQL_MAJOR=5.6
# Mon, 19 Jul 2021 21:21:16 GMT
ENV MYSQL_VERSION=5.6.51-1debian9
# Mon, 19 Jul 2021 21:21:17 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ stretch mysql-5.6' > /etc/apt/sources.list.d/mysql.list
# Mon, 19 Jul 2021 21:21:33 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Mon, 19 Jul 2021 21:21:33 GMT
VOLUME [/var/lib/mysql]
# Mon, 19 Jul 2021 21:21:33 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Mon, 19 Jul 2021 21:21:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 19 Jul 2021 21:21:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 19 Jul 2021 21:21:35 GMT
EXPOSE 3306
# Mon, 19 Jul 2021 21:21:35 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:aed007321795cdc03a0ba9b238567ffa299459e9b0322a3d835a04d06afc2500`  
		Last Modified: Wed, 23 Jun 2021 00:28:29 GMT  
		Size: 22.5 MB (22528174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e3907de0616be6c389254f20af53ebd0ac0402342018a5ae331b8c6a4ace11c`  
		Last Modified: Wed, 23 Jun 2021 07:15:21 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ca0dc4c85b2f025ff9f2fa5a99c4579e877749a86b0b93c73a23cadd9037a6`  
		Last Modified: Wed, 23 Jun 2021 07:15:19 GMT  
		Size: 4.5 MB (4503296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dfa7dcb610e5771507f25c98b85c6642b6e8ad15f9401974f2e0ea482f0501c`  
		Last Modified: Wed, 23 Jun 2021 07:15:18 GMT  
		Size: 1.4 MB (1412228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca864d5ff496eee5d88e0672bbf5aaa2a49678cc6523dee2fcbb3b2e6f9ad9fe`  
		Last Modified: Wed, 23 Jun 2021 07:15:18 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ae77af12a2e84101d350d183b3f487eed852d354e9e647e218700c49267fad`  
		Last Modified: Wed, 23 Jun 2021 07:15:22 GMT  
		Size: 10.2 MB (10225537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76d918206682301f1dce0f52e6f44d67aae57f4a28feb65f97c480a1afa16dfd`  
		Last Modified: Mon, 19 Jul 2021 21:23:08 GMT  
		Size: 19.5 KB (19455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1adf8c2de8b33ae0bbe3da37d8c79c97ca30e5064ce5ff62eee4ee5dbc1d94dc`  
		Last Modified: Mon, 19 Jul 2021 21:23:08 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:174bf86e1642c8eadc23dfca0ad5ce75360997bf37bf0d74dd23b6c9a69091c2`  
		Last Modified: Mon, 19 Jul 2021 21:23:18 GMT  
		Size: 64.3 MB (64274345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918549e97679583eb83f230e479239b96647aa4f9aa6b06edc371414f81312b5`  
		Last Modified: Mon, 19 Jul 2021 21:23:08 GMT  
		Size: 5.6 KB (5557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26473e934bd21d74e339478a63df3383bee74171ecaa9bbc2d7de89af6f5f8ce`  
		Last Modified: Mon, 19 Jul 2021 21:23:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.6.51`

```console
$ docker pull mysql@sha256:7888210cff8d7380909405787754953ba9a0dd1e7c3ba35dec2b48a007314701
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.6.51` - linux; amd64

```console
$ docker pull mysql@sha256:cec6c24d7a4141fa3711bfa0ff1cb66065ba4f0b18886ebec5a22c61c5f533b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.0 MB (102970826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6db4571057fc7fede46cc4e91b2ec088424d78a691e53d4e96f85cc116fdd3eb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 23 Jun 2021 00:22:13 GMT
ADD file:a63c6cc73701d6cb7195338c446b9e92ef6b7a0f9321f6cc1bf8738e3da57c66 in / 
# Wed, 23 Jun 2021 00:22:14 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 07:12:38 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 23 Jun 2021 07:12:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 07:12:46 GMT
ENV GOSU_VERSION=1.12
# Wed, 23 Jun 2021 07:12:58 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 23 Jun 2021 07:12:59 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 23 Jun 2021 07:13:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Mon, 19 Jul 2021 21:21:15 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Mon, 19 Jul 2021 21:21:15 GMT
ENV MYSQL_MAJOR=5.6
# Mon, 19 Jul 2021 21:21:16 GMT
ENV MYSQL_VERSION=5.6.51-1debian9
# Mon, 19 Jul 2021 21:21:17 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ stretch mysql-5.6' > /etc/apt/sources.list.d/mysql.list
# Mon, 19 Jul 2021 21:21:33 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Mon, 19 Jul 2021 21:21:33 GMT
VOLUME [/var/lib/mysql]
# Mon, 19 Jul 2021 21:21:33 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Mon, 19 Jul 2021 21:21:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 19 Jul 2021 21:21:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 19 Jul 2021 21:21:35 GMT
EXPOSE 3306
# Mon, 19 Jul 2021 21:21:35 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:aed007321795cdc03a0ba9b238567ffa299459e9b0322a3d835a04d06afc2500`  
		Last Modified: Wed, 23 Jun 2021 00:28:29 GMT  
		Size: 22.5 MB (22528174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e3907de0616be6c389254f20af53ebd0ac0402342018a5ae331b8c6a4ace11c`  
		Last Modified: Wed, 23 Jun 2021 07:15:21 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ca0dc4c85b2f025ff9f2fa5a99c4579e877749a86b0b93c73a23cadd9037a6`  
		Last Modified: Wed, 23 Jun 2021 07:15:19 GMT  
		Size: 4.5 MB (4503296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dfa7dcb610e5771507f25c98b85c6642b6e8ad15f9401974f2e0ea482f0501c`  
		Last Modified: Wed, 23 Jun 2021 07:15:18 GMT  
		Size: 1.4 MB (1412228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca864d5ff496eee5d88e0672bbf5aaa2a49678cc6523dee2fcbb3b2e6f9ad9fe`  
		Last Modified: Wed, 23 Jun 2021 07:15:18 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ae77af12a2e84101d350d183b3f487eed852d354e9e647e218700c49267fad`  
		Last Modified: Wed, 23 Jun 2021 07:15:22 GMT  
		Size: 10.2 MB (10225537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76d918206682301f1dce0f52e6f44d67aae57f4a28feb65f97c480a1afa16dfd`  
		Last Modified: Mon, 19 Jul 2021 21:23:08 GMT  
		Size: 19.5 KB (19455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1adf8c2de8b33ae0bbe3da37d8c79c97ca30e5064ce5ff62eee4ee5dbc1d94dc`  
		Last Modified: Mon, 19 Jul 2021 21:23:08 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:174bf86e1642c8eadc23dfca0ad5ce75360997bf37bf0d74dd23b6c9a69091c2`  
		Last Modified: Mon, 19 Jul 2021 21:23:18 GMT  
		Size: 64.3 MB (64274345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918549e97679583eb83f230e479239b96647aa4f9aa6b06edc371414f81312b5`  
		Last Modified: Mon, 19 Jul 2021 21:23:08 GMT  
		Size: 5.6 KB (5557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26473e934bd21d74e339478a63df3383bee74171ecaa9bbc2d7de89af6f5f8ce`  
		Last Modified: Mon, 19 Jul 2021 21:23:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7`

```console
$ docker pull mysql@sha256:956e11ac581cad9ac8747a9a1d61b8ffcfa6845e0f23bdbab6ba20a2ad792cbf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7` - linux; amd64

```console
$ docker pull mysql@sha256:ea4f3391e56e132623d37964e66761e8f390d8cfbeb0c7b3184b533d697379e3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.8 MB (154790337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f1d21c1025ab10f9994398f01bb09eb7b6bd0861b3cff0fc9e0a8c265615772`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 07:10:38 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 23 Jun 2021 07:10:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 07:10:47 GMT
ENV GOSU_VERSION=1.12
# Wed, 23 Jun 2021 07:11:06 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 23 Jun 2021 07:11:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 23 Jun 2021 07:11:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Mon, 19 Jul 2021 21:20:18 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Mon, 19 Jul 2021 21:20:41 GMT
ENV MYSQL_MAJOR=5.7
# Mon, 19 Jul 2021 21:20:41 GMT
ENV MYSQL_VERSION=5.7.35-1debian10
# Mon, 19 Jul 2021 21:20:42 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Mon, 19 Jul 2021 21:21:02 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Mon, 19 Jul 2021 21:21:02 GMT
VOLUME [/var/lib/mysql]
# Mon, 19 Jul 2021 21:21:03 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Mon, 19 Jul 2021 21:21:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 19 Jul 2021 21:21:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 19 Jul 2021 21:21:04 GMT
EXPOSE 3306 33060
# Mon, 19 Jul 2021 21:21:04 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a462b60610f5b230bfc054037dcc15dfbd114bc91472a819ac5b4049cb7f030c`  
		Last Modified: Wed, 23 Jun 2021 07:13:58 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578fafb77ab871790dd20afa25cea55309e5862a43eb6fdca5f3c1387ab7b833`  
		Last Modified: Wed, 23 Jun 2021 07:14:00 GMT  
		Size: 4.2 MB (4179324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5240460060374bac3b015544387eba2355e7b003da15c162e7166984437c31d7`  
		Last Modified: Wed, 23 Jun 2021 07:13:57 GMT  
		Size: 1.4 MB (1419480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0cbe54c88555c61f35df860e431717e56b7198eb3a9fa642d14ea6e94dc6edc`  
		Last Modified: Wed, 23 Jun 2021 07:13:56 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa18e05cc46d159c053ebf379685cef648b64d4bb39a4fa76dc7c8a6fadad89a`  
		Last Modified: Wed, 23 Jun 2021 07:14:01 GMT  
		Size: 13.4 MB (13447715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd6f649b1d0ad67dac3c7030f08df70fd82163dc4647b1971b7767d722f61cf6`  
		Last Modified: Mon, 19 Jul 2021 21:22:01 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a2b858b000b70f17957436b46151ad03150c634a0105764a09698711d296742`  
		Last Modified: Mon, 19 Jul 2021 21:22:39 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322182b1742269101681ce76d2a57a8c8c03b05b32a6a7ce989f90673e1e5a89`  
		Last Modified: Mon, 19 Jul 2021 21:22:53 GMT  
		Size: 108.6 MB (108588326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070e28050a8889df0d941be3ca8238bc7e7d6d1ebdc76b95753a2b8481a6ea4d`  
		Last Modified: Mon, 19 Jul 2021 21:22:38 GMT  
		Size: 5.5 KB (5541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:613bdfd8796e97816bbd22c43f893270073ded2bf82830c613d274c203de6447`  
		Last Modified: Mon, 19 Jul 2021 21:22:38 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.35`

```console
$ docker pull mysql@sha256:956e11ac581cad9ac8747a9a1d61b8ffcfa6845e0f23bdbab6ba20a2ad792cbf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.35` - linux; amd64

```console
$ docker pull mysql@sha256:ea4f3391e56e132623d37964e66761e8f390d8cfbeb0c7b3184b533d697379e3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.8 MB (154790337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f1d21c1025ab10f9994398f01bb09eb7b6bd0861b3cff0fc9e0a8c265615772`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 07:10:38 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 23 Jun 2021 07:10:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 07:10:47 GMT
ENV GOSU_VERSION=1.12
# Wed, 23 Jun 2021 07:11:06 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 23 Jun 2021 07:11:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 23 Jun 2021 07:11:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Mon, 19 Jul 2021 21:20:18 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Mon, 19 Jul 2021 21:20:41 GMT
ENV MYSQL_MAJOR=5.7
# Mon, 19 Jul 2021 21:20:41 GMT
ENV MYSQL_VERSION=5.7.35-1debian10
# Mon, 19 Jul 2021 21:20:42 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Mon, 19 Jul 2021 21:21:02 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Mon, 19 Jul 2021 21:21:02 GMT
VOLUME [/var/lib/mysql]
# Mon, 19 Jul 2021 21:21:03 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Mon, 19 Jul 2021 21:21:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 19 Jul 2021 21:21:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 19 Jul 2021 21:21:04 GMT
EXPOSE 3306 33060
# Mon, 19 Jul 2021 21:21:04 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a462b60610f5b230bfc054037dcc15dfbd114bc91472a819ac5b4049cb7f030c`  
		Last Modified: Wed, 23 Jun 2021 07:13:58 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578fafb77ab871790dd20afa25cea55309e5862a43eb6fdca5f3c1387ab7b833`  
		Last Modified: Wed, 23 Jun 2021 07:14:00 GMT  
		Size: 4.2 MB (4179324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5240460060374bac3b015544387eba2355e7b003da15c162e7166984437c31d7`  
		Last Modified: Wed, 23 Jun 2021 07:13:57 GMT  
		Size: 1.4 MB (1419480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0cbe54c88555c61f35df860e431717e56b7198eb3a9fa642d14ea6e94dc6edc`  
		Last Modified: Wed, 23 Jun 2021 07:13:56 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa18e05cc46d159c053ebf379685cef648b64d4bb39a4fa76dc7c8a6fadad89a`  
		Last Modified: Wed, 23 Jun 2021 07:14:01 GMT  
		Size: 13.4 MB (13447715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd6f649b1d0ad67dac3c7030f08df70fd82163dc4647b1971b7767d722f61cf6`  
		Last Modified: Mon, 19 Jul 2021 21:22:01 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a2b858b000b70f17957436b46151ad03150c634a0105764a09698711d296742`  
		Last Modified: Mon, 19 Jul 2021 21:22:39 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322182b1742269101681ce76d2a57a8c8c03b05b32a6a7ce989f90673e1e5a89`  
		Last Modified: Mon, 19 Jul 2021 21:22:53 GMT  
		Size: 108.6 MB (108588326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070e28050a8889df0d941be3ca8238bc7e7d6d1ebdc76b95753a2b8481a6ea4d`  
		Last Modified: Mon, 19 Jul 2021 21:22:38 GMT  
		Size: 5.5 KB (5541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:613bdfd8796e97816bbd22c43f893270073ded2bf82830c613d274c203de6447`  
		Last Modified: Mon, 19 Jul 2021 21:22:38 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8`

```console
$ docker pull mysql@sha256:18d8d109aa64673c78aebfb845b929cfdac97a553332f4310f4de8d67ceb03d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8` - linux; amd64

```console
$ docker pull mysql@sha256:4d1342c1ba1657c466a6b85c066edab3a667dffb21381994f262dca5662d35b3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.6 MB (150593195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95db2e2bd882c6e3801d3e51c3da74ae02f2625bb1d452e6e64f276ed6982f1c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 07:10:38 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 23 Jun 2021 07:10:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 07:10:47 GMT
ENV GOSU_VERSION=1.12
# Wed, 23 Jun 2021 07:11:06 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 23 Jun 2021 07:11:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 23 Jun 2021 07:11:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Mon, 19 Jul 2021 21:20:18 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Mon, 19 Jul 2021 21:20:18 GMT
ENV MYSQL_MAJOR=8.0
# Mon, 19 Jul 2021 21:20:19 GMT
ENV MYSQL_VERSION=8.0.26-1debian10
# Mon, 19 Jul 2021 21:20:20 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Mon, 19 Jul 2021 21:20:35 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Mon, 19 Jul 2021 21:20:36 GMT
VOLUME [/var/lib/mysql]
# Mon, 19 Jul 2021 21:20:36 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Mon, 19 Jul 2021 21:20:36 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Mon, 19 Jul 2021 21:20:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 19 Jul 2021 21:20:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 19 Jul 2021 21:20:38 GMT
EXPOSE 3306 33060
# Mon, 19 Jul 2021 21:20:38 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a462b60610f5b230bfc054037dcc15dfbd114bc91472a819ac5b4049cb7f030c`  
		Last Modified: Wed, 23 Jun 2021 07:13:58 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578fafb77ab871790dd20afa25cea55309e5862a43eb6fdca5f3c1387ab7b833`  
		Last Modified: Wed, 23 Jun 2021 07:14:00 GMT  
		Size: 4.2 MB (4179324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5240460060374bac3b015544387eba2355e7b003da15c162e7166984437c31d7`  
		Last Modified: Wed, 23 Jun 2021 07:13:57 GMT  
		Size: 1.4 MB (1419480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0cbe54c88555c61f35df860e431717e56b7198eb3a9fa642d14ea6e94dc6edc`  
		Last Modified: Wed, 23 Jun 2021 07:13:56 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa18e05cc46d159c053ebf379685cef648b64d4bb39a4fa76dc7c8a6fadad89a`  
		Last Modified: Wed, 23 Jun 2021 07:14:01 GMT  
		Size: 13.4 MB (13447715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd6f649b1d0ad67dac3c7030f08df70fd82163dc4647b1971b7767d722f61cf6`  
		Last Modified: Mon, 19 Jul 2021 21:22:01 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a97d48c2fdca9bc5bbe7867c7106c9440d1b87bec160342a9b6558f4208c6eb`  
		Last Modified: Mon, 19 Jul 2021 21:21:59 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f0c7db48fcadc21818a33a47982be4c4e9572e7eaeb429564095b9f281adcb`  
		Last Modified: Mon, 19 Jul 2021 21:22:16 GMT  
		Size: 104.4 MB (104390339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5dda8df049edabe8247cc0f6ae3f73190f72ff2956c0edbab54179e7a16e337`  
		Last Modified: Mon, 19 Jul 2021 21:21:59 GMT  
		Size: 843.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671b83fd7448000f670c94dabaf7bc41a20d374364f0a409935a81f8b63a1924`  
		Last Modified: Mon, 19 Jul 2021 21:21:59 GMT  
		Size: 5.5 KB (5543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d9cc55fa997a2306811d89ef2fa6d4ec9944f3ea701cc0ec9fed4536f5ff600`  
		Last Modified: Mon, 19 Jul 2021 21:21:59 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0`

```console
$ docker pull mysql@sha256:18d8d109aa64673c78aebfb845b929cfdac97a553332f4310f4de8d67ceb03d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0` - linux; amd64

```console
$ docker pull mysql@sha256:4d1342c1ba1657c466a6b85c066edab3a667dffb21381994f262dca5662d35b3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.6 MB (150593195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95db2e2bd882c6e3801d3e51c3da74ae02f2625bb1d452e6e64f276ed6982f1c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 07:10:38 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 23 Jun 2021 07:10:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 07:10:47 GMT
ENV GOSU_VERSION=1.12
# Wed, 23 Jun 2021 07:11:06 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 23 Jun 2021 07:11:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 23 Jun 2021 07:11:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Mon, 19 Jul 2021 21:20:18 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Mon, 19 Jul 2021 21:20:18 GMT
ENV MYSQL_MAJOR=8.0
# Mon, 19 Jul 2021 21:20:19 GMT
ENV MYSQL_VERSION=8.0.26-1debian10
# Mon, 19 Jul 2021 21:20:20 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Mon, 19 Jul 2021 21:20:35 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Mon, 19 Jul 2021 21:20:36 GMT
VOLUME [/var/lib/mysql]
# Mon, 19 Jul 2021 21:20:36 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Mon, 19 Jul 2021 21:20:36 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Mon, 19 Jul 2021 21:20:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 19 Jul 2021 21:20:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 19 Jul 2021 21:20:38 GMT
EXPOSE 3306 33060
# Mon, 19 Jul 2021 21:20:38 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a462b60610f5b230bfc054037dcc15dfbd114bc91472a819ac5b4049cb7f030c`  
		Last Modified: Wed, 23 Jun 2021 07:13:58 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578fafb77ab871790dd20afa25cea55309e5862a43eb6fdca5f3c1387ab7b833`  
		Last Modified: Wed, 23 Jun 2021 07:14:00 GMT  
		Size: 4.2 MB (4179324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5240460060374bac3b015544387eba2355e7b003da15c162e7166984437c31d7`  
		Last Modified: Wed, 23 Jun 2021 07:13:57 GMT  
		Size: 1.4 MB (1419480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0cbe54c88555c61f35df860e431717e56b7198eb3a9fa642d14ea6e94dc6edc`  
		Last Modified: Wed, 23 Jun 2021 07:13:56 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa18e05cc46d159c053ebf379685cef648b64d4bb39a4fa76dc7c8a6fadad89a`  
		Last Modified: Wed, 23 Jun 2021 07:14:01 GMT  
		Size: 13.4 MB (13447715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd6f649b1d0ad67dac3c7030f08df70fd82163dc4647b1971b7767d722f61cf6`  
		Last Modified: Mon, 19 Jul 2021 21:22:01 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a97d48c2fdca9bc5bbe7867c7106c9440d1b87bec160342a9b6558f4208c6eb`  
		Last Modified: Mon, 19 Jul 2021 21:21:59 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f0c7db48fcadc21818a33a47982be4c4e9572e7eaeb429564095b9f281adcb`  
		Last Modified: Mon, 19 Jul 2021 21:22:16 GMT  
		Size: 104.4 MB (104390339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5dda8df049edabe8247cc0f6ae3f73190f72ff2956c0edbab54179e7a16e337`  
		Last Modified: Mon, 19 Jul 2021 21:21:59 GMT  
		Size: 843.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671b83fd7448000f670c94dabaf7bc41a20d374364f0a409935a81f8b63a1924`  
		Last Modified: Mon, 19 Jul 2021 21:21:59 GMT  
		Size: 5.5 KB (5543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d9cc55fa997a2306811d89ef2fa6d4ec9944f3ea701cc0ec9fed4536f5ff600`  
		Last Modified: Mon, 19 Jul 2021 21:21:59 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.26`

```console
$ docker pull mysql@sha256:18d8d109aa64673c78aebfb845b929cfdac97a553332f4310f4de8d67ceb03d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0.26` - linux; amd64

```console
$ docker pull mysql@sha256:4d1342c1ba1657c466a6b85c066edab3a667dffb21381994f262dca5662d35b3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.6 MB (150593195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95db2e2bd882c6e3801d3e51c3da74ae02f2625bb1d452e6e64f276ed6982f1c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 07:10:38 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 23 Jun 2021 07:10:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 07:10:47 GMT
ENV GOSU_VERSION=1.12
# Wed, 23 Jun 2021 07:11:06 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 23 Jun 2021 07:11:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 23 Jun 2021 07:11:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Mon, 19 Jul 2021 21:20:18 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Mon, 19 Jul 2021 21:20:18 GMT
ENV MYSQL_MAJOR=8.0
# Mon, 19 Jul 2021 21:20:19 GMT
ENV MYSQL_VERSION=8.0.26-1debian10
# Mon, 19 Jul 2021 21:20:20 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Mon, 19 Jul 2021 21:20:35 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Mon, 19 Jul 2021 21:20:36 GMT
VOLUME [/var/lib/mysql]
# Mon, 19 Jul 2021 21:20:36 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Mon, 19 Jul 2021 21:20:36 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Mon, 19 Jul 2021 21:20:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 19 Jul 2021 21:20:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 19 Jul 2021 21:20:38 GMT
EXPOSE 3306 33060
# Mon, 19 Jul 2021 21:20:38 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a462b60610f5b230bfc054037dcc15dfbd114bc91472a819ac5b4049cb7f030c`  
		Last Modified: Wed, 23 Jun 2021 07:13:58 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578fafb77ab871790dd20afa25cea55309e5862a43eb6fdca5f3c1387ab7b833`  
		Last Modified: Wed, 23 Jun 2021 07:14:00 GMT  
		Size: 4.2 MB (4179324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5240460060374bac3b015544387eba2355e7b003da15c162e7166984437c31d7`  
		Last Modified: Wed, 23 Jun 2021 07:13:57 GMT  
		Size: 1.4 MB (1419480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0cbe54c88555c61f35df860e431717e56b7198eb3a9fa642d14ea6e94dc6edc`  
		Last Modified: Wed, 23 Jun 2021 07:13:56 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa18e05cc46d159c053ebf379685cef648b64d4bb39a4fa76dc7c8a6fadad89a`  
		Last Modified: Wed, 23 Jun 2021 07:14:01 GMT  
		Size: 13.4 MB (13447715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd6f649b1d0ad67dac3c7030f08df70fd82163dc4647b1971b7767d722f61cf6`  
		Last Modified: Mon, 19 Jul 2021 21:22:01 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a97d48c2fdca9bc5bbe7867c7106c9440d1b87bec160342a9b6558f4208c6eb`  
		Last Modified: Mon, 19 Jul 2021 21:21:59 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f0c7db48fcadc21818a33a47982be4c4e9572e7eaeb429564095b9f281adcb`  
		Last Modified: Mon, 19 Jul 2021 21:22:16 GMT  
		Size: 104.4 MB (104390339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5dda8df049edabe8247cc0f6ae3f73190f72ff2956c0edbab54179e7a16e337`  
		Last Modified: Mon, 19 Jul 2021 21:21:59 GMT  
		Size: 843.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671b83fd7448000f670c94dabaf7bc41a20d374364f0a409935a81f8b63a1924`  
		Last Modified: Mon, 19 Jul 2021 21:21:59 GMT  
		Size: 5.5 KB (5543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d9cc55fa997a2306811d89ef2fa6d4ec9944f3ea701cc0ec9fed4536f5ff600`  
		Last Modified: Mon, 19 Jul 2021 21:21:59 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:latest`

```console
$ docker pull mysql@sha256:18d8d109aa64673c78aebfb845b929cfdac97a553332f4310f4de8d67ceb03d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:latest` - linux; amd64

```console
$ docker pull mysql@sha256:4d1342c1ba1657c466a6b85c066edab3a667dffb21381994f262dca5662d35b3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.6 MB (150593195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95db2e2bd882c6e3801d3e51c3da74ae02f2625bb1d452e6e64f276ed6982f1c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 07:10:38 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 23 Jun 2021 07:10:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 07:10:47 GMT
ENV GOSU_VERSION=1.12
# Wed, 23 Jun 2021 07:11:06 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 23 Jun 2021 07:11:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 23 Jun 2021 07:11:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Mon, 19 Jul 2021 21:20:18 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Mon, 19 Jul 2021 21:20:18 GMT
ENV MYSQL_MAJOR=8.0
# Mon, 19 Jul 2021 21:20:19 GMT
ENV MYSQL_VERSION=8.0.26-1debian10
# Mon, 19 Jul 2021 21:20:20 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Mon, 19 Jul 2021 21:20:35 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Mon, 19 Jul 2021 21:20:36 GMT
VOLUME [/var/lib/mysql]
# Mon, 19 Jul 2021 21:20:36 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Mon, 19 Jul 2021 21:20:36 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Mon, 19 Jul 2021 21:20:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 19 Jul 2021 21:20:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 19 Jul 2021 21:20:38 GMT
EXPOSE 3306 33060
# Mon, 19 Jul 2021 21:20:38 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a462b60610f5b230bfc054037dcc15dfbd114bc91472a819ac5b4049cb7f030c`  
		Last Modified: Wed, 23 Jun 2021 07:13:58 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578fafb77ab871790dd20afa25cea55309e5862a43eb6fdca5f3c1387ab7b833`  
		Last Modified: Wed, 23 Jun 2021 07:14:00 GMT  
		Size: 4.2 MB (4179324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5240460060374bac3b015544387eba2355e7b003da15c162e7166984437c31d7`  
		Last Modified: Wed, 23 Jun 2021 07:13:57 GMT  
		Size: 1.4 MB (1419480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0cbe54c88555c61f35df860e431717e56b7198eb3a9fa642d14ea6e94dc6edc`  
		Last Modified: Wed, 23 Jun 2021 07:13:56 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa18e05cc46d159c053ebf379685cef648b64d4bb39a4fa76dc7c8a6fadad89a`  
		Last Modified: Wed, 23 Jun 2021 07:14:01 GMT  
		Size: 13.4 MB (13447715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd6f649b1d0ad67dac3c7030f08df70fd82163dc4647b1971b7767d722f61cf6`  
		Last Modified: Mon, 19 Jul 2021 21:22:01 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a97d48c2fdca9bc5bbe7867c7106c9440d1b87bec160342a9b6558f4208c6eb`  
		Last Modified: Mon, 19 Jul 2021 21:21:59 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f0c7db48fcadc21818a33a47982be4c4e9572e7eaeb429564095b9f281adcb`  
		Last Modified: Mon, 19 Jul 2021 21:22:16 GMT  
		Size: 104.4 MB (104390339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5dda8df049edabe8247cc0f6ae3f73190f72ff2956c0edbab54179e7a16e337`  
		Last Modified: Mon, 19 Jul 2021 21:21:59 GMT  
		Size: 843.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671b83fd7448000f670c94dabaf7bc41a20d374364f0a409935a81f8b63a1924`  
		Last Modified: Mon, 19 Jul 2021 21:21:59 GMT  
		Size: 5.5 KB (5543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d9cc55fa997a2306811d89ef2fa6d4ec9944f3ea701cc0ec9fed4536f5ff600`  
		Last Modified: Mon, 19 Jul 2021 21:21:59 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
