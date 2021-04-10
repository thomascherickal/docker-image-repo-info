<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mysql`

-	[`mysql:5`](#mysql5)
-	[`mysql:5.6`](#mysql56)
-	[`mysql:5.6.51`](#mysql5651)
-	[`mysql:5.7`](#mysql57)
-	[`mysql:5.7.33`](#mysql5733)
-	[`mysql:8`](#mysql8)
-	[`mysql:8.0`](#mysql80)
-	[`mysql:8.0.23`](#mysql8023)
-	[`mysql:latest`](#mysqllatest)

## `mysql:5`

```console
$ docker pull mysql@sha256:e42a18d0bd0aa746a734a49cbbcc079ccdf6681c474a238d38e79dc0884e0ecc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:5` - linux; amd64

```console
$ docker pull mysql@sha256:4cb929cd5b89f157284f0572feff652af31e4e29db3c3eb32565d6e3bce0fa84
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.6 MB (154635820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:450379344707c56f47d1391c18fc3ac22e2c59fbf384a0de77f2bdfc59bcbc61`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 07:21:42 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 10 Apr 2021 07:21:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 07:21:50 GMT
ENV GOSU_VERSION=1.12
# Sat, 10 Apr 2021 07:22:02 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 10 Apr 2021 07:22:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 10 Apr 2021 07:22:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 07:22:14 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Sat, 10 Apr 2021 07:22:53 GMT
ENV MYSQL_MAJOR=5.7
# Sat, 10 Apr 2021 07:22:53 GMT
ENV MYSQL_VERSION=5.7.33-1debian10
# Sat, 10 Apr 2021 07:22:54 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Sat, 10 Apr 2021 07:23:18 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Sat, 10 Apr 2021 07:23:19 GMT
VOLUME [/var/lib/mysql]
# Sat, 10 Apr 2021 07:23:20 GMT
COPY file:2c6221a2517649db2e9dd27098cc9ae1bdaff205f8d6f0299b20a41b86084d77 in /usr/local/bin/ 
# Sat, 10 Apr 2021 07:23:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 10 Apr 2021 07:23:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 07:23:22 GMT
EXPOSE 3306 33060
# Sat, 10 Apr 2021 07:23:22 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9444bb562699de912e7afcf6409615f9c0033118cc3aa35831d937a8d15e851c`  
		Last Modified: Sat, 10 Apr 2021 07:25:01 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a4207b96940576ff42802b9c440bed0f1b5ef419c5a0c2576477776f217ef35`  
		Last Modified: Sat, 10 Apr 2021 07:25:02 GMT  
		Size: 4.2 MB (4179238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181cefd361ceae3da481ffcd156bd5b6e22f32a9345167199fe4773d70a6f133`  
		Last Modified: Sat, 10 Apr 2021 07:24:59 GMT  
		Size: 1.4 MB (1419407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a2090759d8af87290c70a8a9cef4e7e894b800d55d069b8c4cf0bcd3a5d9f17`  
		Last Modified: Sat, 10 Apr 2021 07:24:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15f235e0d7eefe6c5153946a57daebaf2d0744fb1d0676642f269554fc68ba2a`  
		Last Modified: Sat, 10 Apr 2021 07:25:02 GMT  
		Size: 13.4 MB (13447647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d870539cd9db00c747403f1d6c494a807052bce070f4ef243954b804a1ebb652`  
		Last Modified: Sat, 10 Apr 2021 07:24:58 GMT  
		Size: 2.4 KB (2395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7310c448ab4f27e352c1cea945449ed360ce9b577b780b6913267e24cb74f3dc`  
		Last Modified: Sat, 10 Apr 2021 07:25:36 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a72aac2e8006704c4f9c3901b7c3049cc3d17077c1429c4cdf82d5625a33e0e`  
		Last Modified: Sat, 10 Apr 2021 07:25:54 GMT  
		Size: 108.4 MB (108440009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ab932f17c4041b63c9dc90045af8dda70bcafc303fb43c62965021e24ce91d`  
		Last Modified: Sat, 10 Apr 2021 07:25:36 GMT  
		Size: 5.5 KB (5522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a985de740ee3d14ac32ad2452c6e83f2b2b4e6fb1db7ac341cf0f9f738fb301`  
		Last Modified: Sat, 10 Apr 2021 07:25:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.6`

```console
$ docker pull mysql@sha256:5d63153bf35070c230b9d41a754651d99053cbf19a9eec70ebeba926a304761f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:5.6` - linux; amd64

```console
$ docker pull mysql@sha256:16ca6c3fccdccae491835c3ccfe4fac148c75fa33ea0f1d8b5202c3b63b66b35
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.0 MB (102980889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e26066fd423a46a136be3d411160ee23bd05e0eeb06cbacf37ff51e60ff9e782`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 10 Apr 2021 01:21:54 GMT
ADD file:70cd6967491943999563ddd3ab9abae33791ac320cdc846dc57503cc44f25600 in / 
# Sat, 10 Apr 2021 01:21:54 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 07:23:31 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 10 Apr 2021 07:23:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 07:23:40 GMT
ENV GOSU_VERSION=1.12
# Sat, 10 Apr 2021 07:24:00 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 10 Apr 2021 07:24:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 10 Apr 2021 07:24:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 07:24:12 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Sat, 10 Apr 2021 07:24:13 GMT
ENV MYSQL_MAJOR=5.6
# Sat, 10 Apr 2021 07:24:13 GMT
ENV MYSQL_VERSION=5.6.51-1debian9
# Sat, 10 Apr 2021 07:24:15 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ stretch mysql-5.6' > /etc/apt/sources.list.d/mysql.list
# Sat, 10 Apr 2021 07:24:31 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Sat, 10 Apr 2021 07:24:32 GMT
VOLUME [/var/lib/mysql]
# Sat, 10 Apr 2021 07:24:32 GMT
COPY file:2c6221a2517649db2e9dd27098cc9ae1bdaff205f8d6f0299b20a41b86084d77 in /usr/local/bin/ 
# Sat, 10 Apr 2021 07:24:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 10 Apr 2021 07:24:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 07:24:33 GMT
EXPOSE 3306
# Sat, 10 Apr 2021 07:24:34 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:62deabe7a6db312ed773ccd640cd7cfbf51c22bf466886345684558f1036e358`  
		Last Modified: Sat, 10 Apr 2021 01:28:26 GMT  
		Size: 22.5 MB (22528265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ba35f9cdf1bf9d8c94de5545aa19ebd6d608bfd909bddc7b7412f08983ddfd`  
		Last Modified: Sat, 10 Apr 2021 07:26:16 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c8f6a545aa1239d9392935f9e5260e1a08ed680bbcdcb23c6e20b619dfedc33`  
		Last Modified: Sat, 10 Apr 2021 07:26:15 GMT  
		Size: 4.5 MB (4503322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ced99c328da184c9818ec479e9f42a3fd853adf030a587cfb1b13159dfbfbde`  
		Last Modified: Sat, 10 Apr 2021 07:26:15 GMT  
		Size: 1.4 MB (1412285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1983b7d65f8f3c700e62036931352ced7e8a72b7b40186a7fef24f28b0f840bc`  
		Last Modified: Sat, 10 Apr 2021 07:26:13 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fc89d436e208c4283af7c48242f225849fb37fa6bffaa68fdf539c92b03880b`  
		Last Modified: Sat, 10 Apr 2021 07:26:17 GMT  
		Size: 10.2 MB (10225905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd56cc7fc71df26f029d8d3392474d992219744276ddd058e6de156bfc29dd9`  
		Last Modified: Sat, 10 Apr 2021 07:26:11 GMT  
		Size: 29.0 KB (28955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff26e0e5f66f0129e8924c77175f544bf66e1ee7adbc4bb219ae65734edc8afd`  
		Last Modified: Sat, 10 Apr 2021 07:26:11 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf5586a4456df947b3ac3ffe9cd277adffc7432e691294f813e340f7d8170f48`  
		Last Modified: Sat, 10 Apr 2021 07:26:26 GMT  
		Size: 64.3 MB (64274388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d17e698ea2884b307cdd24c1249b00338461d2e1098ed223a329c5196cf011`  
		Last Modified: Sat, 10 Apr 2021 07:26:11 GMT  
		Size: 5.5 KB (5533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c84062b3c49684c329335b93ead4eccbd821ee192d8af14c4c88d018208470`  
		Last Modified: Sat, 10 Apr 2021 07:26:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.6.51`

```console
$ docker pull mysql@sha256:5d63153bf35070c230b9d41a754651d99053cbf19a9eec70ebeba926a304761f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:5.6.51` - linux; amd64

```console
$ docker pull mysql@sha256:16ca6c3fccdccae491835c3ccfe4fac148c75fa33ea0f1d8b5202c3b63b66b35
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.0 MB (102980889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e26066fd423a46a136be3d411160ee23bd05e0eeb06cbacf37ff51e60ff9e782`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 10 Apr 2021 01:21:54 GMT
ADD file:70cd6967491943999563ddd3ab9abae33791ac320cdc846dc57503cc44f25600 in / 
# Sat, 10 Apr 2021 01:21:54 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 07:23:31 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 10 Apr 2021 07:23:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 07:23:40 GMT
ENV GOSU_VERSION=1.12
# Sat, 10 Apr 2021 07:24:00 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 10 Apr 2021 07:24:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 10 Apr 2021 07:24:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 07:24:12 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Sat, 10 Apr 2021 07:24:13 GMT
ENV MYSQL_MAJOR=5.6
# Sat, 10 Apr 2021 07:24:13 GMT
ENV MYSQL_VERSION=5.6.51-1debian9
# Sat, 10 Apr 2021 07:24:15 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ stretch mysql-5.6' > /etc/apt/sources.list.d/mysql.list
# Sat, 10 Apr 2021 07:24:31 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Sat, 10 Apr 2021 07:24:32 GMT
VOLUME [/var/lib/mysql]
# Sat, 10 Apr 2021 07:24:32 GMT
COPY file:2c6221a2517649db2e9dd27098cc9ae1bdaff205f8d6f0299b20a41b86084d77 in /usr/local/bin/ 
# Sat, 10 Apr 2021 07:24:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 10 Apr 2021 07:24:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 07:24:33 GMT
EXPOSE 3306
# Sat, 10 Apr 2021 07:24:34 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:62deabe7a6db312ed773ccd640cd7cfbf51c22bf466886345684558f1036e358`  
		Last Modified: Sat, 10 Apr 2021 01:28:26 GMT  
		Size: 22.5 MB (22528265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ba35f9cdf1bf9d8c94de5545aa19ebd6d608bfd909bddc7b7412f08983ddfd`  
		Last Modified: Sat, 10 Apr 2021 07:26:16 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c8f6a545aa1239d9392935f9e5260e1a08ed680bbcdcb23c6e20b619dfedc33`  
		Last Modified: Sat, 10 Apr 2021 07:26:15 GMT  
		Size: 4.5 MB (4503322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ced99c328da184c9818ec479e9f42a3fd853adf030a587cfb1b13159dfbfbde`  
		Last Modified: Sat, 10 Apr 2021 07:26:15 GMT  
		Size: 1.4 MB (1412285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1983b7d65f8f3c700e62036931352ced7e8a72b7b40186a7fef24f28b0f840bc`  
		Last Modified: Sat, 10 Apr 2021 07:26:13 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fc89d436e208c4283af7c48242f225849fb37fa6bffaa68fdf539c92b03880b`  
		Last Modified: Sat, 10 Apr 2021 07:26:17 GMT  
		Size: 10.2 MB (10225905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd56cc7fc71df26f029d8d3392474d992219744276ddd058e6de156bfc29dd9`  
		Last Modified: Sat, 10 Apr 2021 07:26:11 GMT  
		Size: 29.0 KB (28955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff26e0e5f66f0129e8924c77175f544bf66e1ee7adbc4bb219ae65734edc8afd`  
		Last Modified: Sat, 10 Apr 2021 07:26:11 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf5586a4456df947b3ac3ffe9cd277adffc7432e691294f813e340f7d8170f48`  
		Last Modified: Sat, 10 Apr 2021 07:26:26 GMT  
		Size: 64.3 MB (64274388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d17e698ea2884b307cdd24c1249b00338461d2e1098ed223a329c5196cf011`  
		Last Modified: Sat, 10 Apr 2021 07:26:11 GMT  
		Size: 5.5 KB (5533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c84062b3c49684c329335b93ead4eccbd821ee192d8af14c4c88d018208470`  
		Last Modified: Sat, 10 Apr 2021 07:26:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7`

```console
$ docker pull mysql@sha256:e42a18d0bd0aa746a734a49cbbcc079ccdf6681c474a238d38e79dc0884e0ecc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:5.7` - linux; amd64

```console
$ docker pull mysql@sha256:4cb929cd5b89f157284f0572feff652af31e4e29db3c3eb32565d6e3bce0fa84
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.6 MB (154635820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:450379344707c56f47d1391c18fc3ac22e2c59fbf384a0de77f2bdfc59bcbc61`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 07:21:42 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 10 Apr 2021 07:21:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 07:21:50 GMT
ENV GOSU_VERSION=1.12
# Sat, 10 Apr 2021 07:22:02 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 10 Apr 2021 07:22:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 10 Apr 2021 07:22:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 07:22:14 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Sat, 10 Apr 2021 07:22:53 GMT
ENV MYSQL_MAJOR=5.7
# Sat, 10 Apr 2021 07:22:53 GMT
ENV MYSQL_VERSION=5.7.33-1debian10
# Sat, 10 Apr 2021 07:22:54 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Sat, 10 Apr 2021 07:23:18 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Sat, 10 Apr 2021 07:23:19 GMT
VOLUME [/var/lib/mysql]
# Sat, 10 Apr 2021 07:23:20 GMT
COPY file:2c6221a2517649db2e9dd27098cc9ae1bdaff205f8d6f0299b20a41b86084d77 in /usr/local/bin/ 
# Sat, 10 Apr 2021 07:23:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 10 Apr 2021 07:23:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 07:23:22 GMT
EXPOSE 3306 33060
# Sat, 10 Apr 2021 07:23:22 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9444bb562699de912e7afcf6409615f9c0033118cc3aa35831d937a8d15e851c`  
		Last Modified: Sat, 10 Apr 2021 07:25:01 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a4207b96940576ff42802b9c440bed0f1b5ef419c5a0c2576477776f217ef35`  
		Last Modified: Sat, 10 Apr 2021 07:25:02 GMT  
		Size: 4.2 MB (4179238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181cefd361ceae3da481ffcd156bd5b6e22f32a9345167199fe4773d70a6f133`  
		Last Modified: Sat, 10 Apr 2021 07:24:59 GMT  
		Size: 1.4 MB (1419407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a2090759d8af87290c70a8a9cef4e7e894b800d55d069b8c4cf0bcd3a5d9f17`  
		Last Modified: Sat, 10 Apr 2021 07:24:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15f235e0d7eefe6c5153946a57daebaf2d0744fb1d0676642f269554fc68ba2a`  
		Last Modified: Sat, 10 Apr 2021 07:25:02 GMT  
		Size: 13.4 MB (13447647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d870539cd9db00c747403f1d6c494a807052bce070f4ef243954b804a1ebb652`  
		Last Modified: Sat, 10 Apr 2021 07:24:58 GMT  
		Size: 2.4 KB (2395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7310c448ab4f27e352c1cea945449ed360ce9b577b780b6913267e24cb74f3dc`  
		Last Modified: Sat, 10 Apr 2021 07:25:36 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a72aac2e8006704c4f9c3901b7c3049cc3d17077c1429c4cdf82d5625a33e0e`  
		Last Modified: Sat, 10 Apr 2021 07:25:54 GMT  
		Size: 108.4 MB (108440009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ab932f17c4041b63c9dc90045af8dda70bcafc303fb43c62965021e24ce91d`  
		Last Modified: Sat, 10 Apr 2021 07:25:36 GMT  
		Size: 5.5 KB (5522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a985de740ee3d14ac32ad2452c6e83f2b2b4e6fb1db7ac341cf0f9f738fb301`  
		Last Modified: Sat, 10 Apr 2021 07:25:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.33`

```console
$ docker pull mysql@sha256:e42a18d0bd0aa746a734a49cbbcc079ccdf6681c474a238d38e79dc0884e0ecc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:5.7.33` - linux; amd64

```console
$ docker pull mysql@sha256:4cb929cd5b89f157284f0572feff652af31e4e29db3c3eb32565d6e3bce0fa84
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.6 MB (154635820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:450379344707c56f47d1391c18fc3ac22e2c59fbf384a0de77f2bdfc59bcbc61`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 07:21:42 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 10 Apr 2021 07:21:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 07:21:50 GMT
ENV GOSU_VERSION=1.12
# Sat, 10 Apr 2021 07:22:02 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 10 Apr 2021 07:22:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 10 Apr 2021 07:22:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 07:22:14 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Sat, 10 Apr 2021 07:22:53 GMT
ENV MYSQL_MAJOR=5.7
# Sat, 10 Apr 2021 07:22:53 GMT
ENV MYSQL_VERSION=5.7.33-1debian10
# Sat, 10 Apr 2021 07:22:54 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Sat, 10 Apr 2021 07:23:18 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Sat, 10 Apr 2021 07:23:19 GMT
VOLUME [/var/lib/mysql]
# Sat, 10 Apr 2021 07:23:20 GMT
COPY file:2c6221a2517649db2e9dd27098cc9ae1bdaff205f8d6f0299b20a41b86084d77 in /usr/local/bin/ 
# Sat, 10 Apr 2021 07:23:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 10 Apr 2021 07:23:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 07:23:22 GMT
EXPOSE 3306 33060
# Sat, 10 Apr 2021 07:23:22 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9444bb562699de912e7afcf6409615f9c0033118cc3aa35831d937a8d15e851c`  
		Last Modified: Sat, 10 Apr 2021 07:25:01 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a4207b96940576ff42802b9c440bed0f1b5ef419c5a0c2576477776f217ef35`  
		Last Modified: Sat, 10 Apr 2021 07:25:02 GMT  
		Size: 4.2 MB (4179238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181cefd361ceae3da481ffcd156bd5b6e22f32a9345167199fe4773d70a6f133`  
		Last Modified: Sat, 10 Apr 2021 07:24:59 GMT  
		Size: 1.4 MB (1419407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a2090759d8af87290c70a8a9cef4e7e894b800d55d069b8c4cf0bcd3a5d9f17`  
		Last Modified: Sat, 10 Apr 2021 07:24:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15f235e0d7eefe6c5153946a57daebaf2d0744fb1d0676642f269554fc68ba2a`  
		Last Modified: Sat, 10 Apr 2021 07:25:02 GMT  
		Size: 13.4 MB (13447647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d870539cd9db00c747403f1d6c494a807052bce070f4ef243954b804a1ebb652`  
		Last Modified: Sat, 10 Apr 2021 07:24:58 GMT  
		Size: 2.4 KB (2395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7310c448ab4f27e352c1cea945449ed360ce9b577b780b6913267e24cb74f3dc`  
		Last Modified: Sat, 10 Apr 2021 07:25:36 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a72aac2e8006704c4f9c3901b7c3049cc3d17077c1429c4cdf82d5625a33e0e`  
		Last Modified: Sat, 10 Apr 2021 07:25:54 GMT  
		Size: 108.4 MB (108440009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ab932f17c4041b63c9dc90045af8dda70bcafc303fb43c62965021e24ce91d`  
		Last Modified: Sat, 10 Apr 2021 07:25:36 GMT  
		Size: 5.5 KB (5522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a985de740ee3d14ac32ad2452c6e83f2b2b4e6fb1db7ac341cf0f9f738fb301`  
		Last Modified: Sat, 10 Apr 2021 07:25:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8`

```console
$ docker pull mysql@sha256:6e0014cdd88092545557dee5e9eb7e1a3c84c9a14ad2418d5f2231e930967a38
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:8` - linux; amd64

```console
$ docker pull mysql@sha256:355617769102e9d2ebb7d5879263a12d230badb7271c91748b2c7b0ac6971083
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.3 MB (159323709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbe8815cbea8fb86ce7d3169a82d05301e7dfe1a8d4228941f23f4f115a887f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 07:21:42 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 10 Apr 2021 07:21:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 07:21:50 GMT
ENV GOSU_VERSION=1.12
# Sat, 10 Apr 2021 07:22:02 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 10 Apr 2021 07:22:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 10 Apr 2021 07:22:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 07:22:14 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Sat, 10 Apr 2021 07:22:14 GMT
ENV MYSQL_MAJOR=8.0
# Sat, 10 Apr 2021 07:22:14 GMT
ENV MYSQL_VERSION=8.0.23-1debian10
# Sat, 10 Apr 2021 07:22:16 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Sat, 10 Apr 2021 07:22:36 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Sat, 10 Apr 2021 07:22:37 GMT
VOLUME [/var/lib/mysql]
# Sat, 10 Apr 2021 07:22:38 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Sat, 10 Apr 2021 07:22:38 GMT
COPY file:2c6221a2517649db2e9dd27098cc9ae1bdaff205f8d6f0299b20a41b86084d77 in /usr/local/bin/ 
# Sat, 10 Apr 2021 07:22:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 10 Apr 2021 07:22:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 07:22:41 GMT
EXPOSE 3306 33060
# Sat, 10 Apr 2021 07:22:41 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9444bb562699de912e7afcf6409615f9c0033118cc3aa35831d937a8d15e851c`  
		Last Modified: Sat, 10 Apr 2021 07:25:01 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a4207b96940576ff42802b9c440bed0f1b5ef419c5a0c2576477776f217ef35`  
		Last Modified: Sat, 10 Apr 2021 07:25:02 GMT  
		Size: 4.2 MB (4179238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181cefd361ceae3da481ffcd156bd5b6e22f32a9345167199fe4773d70a6f133`  
		Last Modified: Sat, 10 Apr 2021 07:24:59 GMT  
		Size: 1.4 MB (1419407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a2090759d8af87290c70a8a9cef4e7e894b800d55d069b8c4cf0bcd3a5d9f17`  
		Last Modified: Sat, 10 Apr 2021 07:24:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15f235e0d7eefe6c5153946a57daebaf2d0744fb1d0676642f269554fc68ba2a`  
		Last Modified: Sat, 10 Apr 2021 07:25:02 GMT  
		Size: 13.4 MB (13447647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d870539cd9db00c747403f1d6c494a807052bce070f4ef243954b804a1ebb652`  
		Last Modified: Sat, 10 Apr 2021 07:24:58 GMT  
		Size: 2.4 KB (2395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5726073179b6fb503d82a3b6cf6c7fe83081484ba600364a37b58105dec30677`  
		Last Modified: Sat, 10 Apr 2021 07:24:56 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eadfac8b2520b41436dd678f1f822ffcc0b416ce5d481a9070c4c4531b3d3efd`  
		Last Modified: Sat, 10 Apr 2021 07:25:16 GMT  
		Size: 113.1 MB (113127055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5936a8c3f2baf76cbebb0eaf333510aa2f52c6e825cf216638ac4b827ccc1d3`  
		Last Modified: Sat, 10 Apr 2021 07:24:56 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cca8ee89e625e42d7fcd5fd01d23c53c630d3aff4511b9a5f386713dc2e89ce4`  
		Last Modified: Sat, 10 Apr 2021 07:24:56 GMT  
		Size: 5.5 KB (5522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c79df02586a3bcf87a8109d34a6d6b32593583b49b5ae106cf89b70b04742c6`  
		Last Modified: Sat, 10 Apr 2021 07:24:56 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0`

```console
$ docker pull mysql@sha256:6e0014cdd88092545557dee5e9eb7e1a3c84c9a14ad2418d5f2231e930967a38
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:8.0` - linux; amd64

```console
$ docker pull mysql@sha256:355617769102e9d2ebb7d5879263a12d230badb7271c91748b2c7b0ac6971083
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.3 MB (159323709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbe8815cbea8fb86ce7d3169a82d05301e7dfe1a8d4228941f23f4f115a887f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 07:21:42 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 10 Apr 2021 07:21:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 07:21:50 GMT
ENV GOSU_VERSION=1.12
# Sat, 10 Apr 2021 07:22:02 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 10 Apr 2021 07:22:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 10 Apr 2021 07:22:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 07:22:14 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Sat, 10 Apr 2021 07:22:14 GMT
ENV MYSQL_MAJOR=8.0
# Sat, 10 Apr 2021 07:22:14 GMT
ENV MYSQL_VERSION=8.0.23-1debian10
# Sat, 10 Apr 2021 07:22:16 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Sat, 10 Apr 2021 07:22:36 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Sat, 10 Apr 2021 07:22:37 GMT
VOLUME [/var/lib/mysql]
# Sat, 10 Apr 2021 07:22:38 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Sat, 10 Apr 2021 07:22:38 GMT
COPY file:2c6221a2517649db2e9dd27098cc9ae1bdaff205f8d6f0299b20a41b86084d77 in /usr/local/bin/ 
# Sat, 10 Apr 2021 07:22:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 10 Apr 2021 07:22:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 07:22:41 GMT
EXPOSE 3306 33060
# Sat, 10 Apr 2021 07:22:41 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9444bb562699de912e7afcf6409615f9c0033118cc3aa35831d937a8d15e851c`  
		Last Modified: Sat, 10 Apr 2021 07:25:01 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a4207b96940576ff42802b9c440bed0f1b5ef419c5a0c2576477776f217ef35`  
		Last Modified: Sat, 10 Apr 2021 07:25:02 GMT  
		Size: 4.2 MB (4179238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181cefd361ceae3da481ffcd156bd5b6e22f32a9345167199fe4773d70a6f133`  
		Last Modified: Sat, 10 Apr 2021 07:24:59 GMT  
		Size: 1.4 MB (1419407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a2090759d8af87290c70a8a9cef4e7e894b800d55d069b8c4cf0bcd3a5d9f17`  
		Last Modified: Sat, 10 Apr 2021 07:24:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15f235e0d7eefe6c5153946a57daebaf2d0744fb1d0676642f269554fc68ba2a`  
		Last Modified: Sat, 10 Apr 2021 07:25:02 GMT  
		Size: 13.4 MB (13447647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d870539cd9db00c747403f1d6c494a807052bce070f4ef243954b804a1ebb652`  
		Last Modified: Sat, 10 Apr 2021 07:24:58 GMT  
		Size: 2.4 KB (2395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5726073179b6fb503d82a3b6cf6c7fe83081484ba600364a37b58105dec30677`  
		Last Modified: Sat, 10 Apr 2021 07:24:56 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eadfac8b2520b41436dd678f1f822ffcc0b416ce5d481a9070c4c4531b3d3efd`  
		Last Modified: Sat, 10 Apr 2021 07:25:16 GMT  
		Size: 113.1 MB (113127055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5936a8c3f2baf76cbebb0eaf333510aa2f52c6e825cf216638ac4b827ccc1d3`  
		Last Modified: Sat, 10 Apr 2021 07:24:56 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cca8ee89e625e42d7fcd5fd01d23c53c630d3aff4511b9a5f386713dc2e89ce4`  
		Last Modified: Sat, 10 Apr 2021 07:24:56 GMT  
		Size: 5.5 KB (5522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c79df02586a3bcf87a8109d34a6d6b32593583b49b5ae106cf89b70b04742c6`  
		Last Modified: Sat, 10 Apr 2021 07:24:56 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.23`

```console
$ docker pull mysql@sha256:6e0014cdd88092545557dee5e9eb7e1a3c84c9a14ad2418d5f2231e930967a38
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:8.0.23` - linux; amd64

```console
$ docker pull mysql@sha256:355617769102e9d2ebb7d5879263a12d230badb7271c91748b2c7b0ac6971083
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.3 MB (159323709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbe8815cbea8fb86ce7d3169a82d05301e7dfe1a8d4228941f23f4f115a887f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 07:21:42 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 10 Apr 2021 07:21:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 07:21:50 GMT
ENV GOSU_VERSION=1.12
# Sat, 10 Apr 2021 07:22:02 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 10 Apr 2021 07:22:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 10 Apr 2021 07:22:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 07:22:14 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Sat, 10 Apr 2021 07:22:14 GMT
ENV MYSQL_MAJOR=8.0
# Sat, 10 Apr 2021 07:22:14 GMT
ENV MYSQL_VERSION=8.0.23-1debian10
# Sat, 10 Apr 2021 07:22:16 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Sat, 10 Apr 2021 07:22:36 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Sat, 10 Apr 2021 07:22:37 GMT
VOLUME [/var/lib/mysql]
# Sat, 10 Apr 2021 07:22:38 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Sat, 10 Apr 2021 07:22:38 GMT
COPY file:2c6221a2517649db2e9dd27098cc9ae1bdaff205f8d6f0299b20a41b86084d77 in /usr/local/bin/ 
# Sat, 10 Apr 2021 07:22:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 10 Apr 2021 07:22:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 07:22:41 GMT
EXPOSE 3306 33060
# Sat, 10 Apr 2021 07:22:41 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9444bb562699de912e7afcf6409615f9c0033118cc3aa35831d937a8d15e851c`  
		Last Modified: Sat, 10 Apr 2021 07:25:01 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a4207b96940576ff42802b9c440bed0f1b5ef419c5a0c2576477776f217ef35`  
		Last Modified: Sat, 10 Apr 2021 07:25:02 GMT  
		Size: 4.2 MB (4179238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181cefd361ceae3da481ffcd156bd5b6e22f32a9345167199fe4773d70a6f133`  
		Last Modified: Sat, 10 Apr 2021 07:24:59 GMT  
		Size: 1.4 MB (1419407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a2090759d8af87290c70a8a9cef4e7e894b800d55d069b8c4cf0bcd3a5d9f17`  
		Last Modified: Sat, 10 Apr 2021 07:24:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15f235e0d7eefe6c5153946a57daebaf2d0744fb1d0676642f269554fc68ba2a`  
		Last Modified: Sat, 10 Apr 2021 07:25:02 GMT  
		Size: 13.4 MB (13447647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d870539cd9db00c747403f1d6c494a807052bce070f4ef243954b804a1ebb652`  
		Last Modified: Sat, 10 Apr 2021 07:24:58 GMT  
		Size: 2.4 KB (2395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5726073179b6fb503d82a3b6cf6c7fe83081484ba600364a37b58105dec30677`  
		Last Modified: Sat, 10 Apr 2021 07:24:56 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eadfac8b2520b41436dd678f1f822ffcc0b416ce5d481a9070c4c4531b3d3efd`  
		Last Modified: Sat, 10 Apr 2021 07:25:16 GMT  
		Size: 113.1 MB (113127055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5936a8c3f2baf76cbebb0eaf333510aa2f52c6e825cf216638ac4b827ccc1d3`  
		Last Modified: Sat, 10 Apr 2021 07:24:56 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cca8ee89e625e42d7fcd5fd01d23c53c630d3aff4511b9a5f386713dc2e89ce4`  
		Last Modified: Sat, 10 Apr 2021 07:24:56 GMT  
		Size: 5.5 KB (5522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c79df02586a3bcf87a8109d34a6d6b32593583b49b5ae106cf89b70b04742c6`  
		Last Modified: Sat, 10 Apr 2021 07:24:56 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:latest`

```console
$ docker pull mysql@sha256:6e0014cdd88092545557dee5e9eb7e1a3c84c9a14ad2418d5f2231e930967a38
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:latest` - linux; amd64

```console
$ docker pull mysql@sha256:355617769102e9d2ebb7d5879263a12d230badb7271c91748b2c7b0ac6971083
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.3 MB (159323709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbe8815cbea8fb86ce7d3169a82d05301e7dfe1a8d4228941f23f4f115a887f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 07:21:42 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 10 Apr 2021 07:21:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 07:21:50 GMT
ENV GOSU_VERSION=1.12
# Sat, 10 Apr 2021 07:22:02 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 10 Apr 2021 07:22:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 10 Apr 2021 07:22:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 07:22:14 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Sat, 10 Apr 2021 07:22:14 GMT
ENV MYSQL_MAJOR=8.0
# Sat, 10 Apr 2021 07:22:14 GMT
ENV MYSQL_VERSION=8.0.23-1debian10
# Sat, 10 Apr 2021 07:22:16 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Sat, 10 Apr 2021 07:22:36 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Sat, 10 Apr 2021 07:22:37 GMT
VOLUME [/var/lib/mysql]
# Sat, 10 Apr 2021 07:22:38 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Sat, 10 Apr 2021 07:22:38 GMT
COPY file:2c6221a2517649db2e9dd27098cc9ae1bdaff205f8d6f0299b20a41b86084d77 in /usr/local/bin/ 
# Sat, 10 Apr 2021 07:22:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 10 Apr 2021 07:22:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 07:22:41 GMT
EXPOSE 3306 33060
# Sat, 10 Apr 2021 07:22:41 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9444bb562699de912e7afcf6409615f9c0033118cc3aa35831d937a8d15e851c`  
		Last Modified: Sat, 10 Apr 2021 07:25:01 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a4207b96940576ff42802b9c440bed0f1b5ef419c5a0c2576477776f217ef35`  
		Last Modified: Sat, 10 Apr 2021 07:25:02 GMT  
		Size: 4.2 MB (4179238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181cefd361ceae3da481ffcd156bd5b6e22f32a9345167199fe4773d70a6f133`  
		Last Modified: Sat, 10 Apr 2021 07:24:59 GMT  
		Size: 1.4 MB (1419407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a2090759d8af87290c70a8a9cef4e7e894b800d55d069b8c4cf0bcd3a5d9f17`  
		Last Modified: Sat, 10 Apr 2021 07:24:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15f235e0d7eefe6c5153946a57daebaf2d0744fb1d0676642f269554fc68ba2a`  
		Last Modified: Sat, 10 Apr 2021 07:25:02 GMT  
		Size: 13.4 MB (13447647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d870539cd9db00c747403f1d6c494a807052bce070f4ef243954b804a1ebb652`  
		Last Modified: Sat, 10 Apr 2021 07:24:58 GMT  
		Size: 2.4 KB (2395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5726073179b6fb503d82a3b6cf6c7fe83081484ba600364a37b58105dec30677`  
		Last Modified: Sat, 10 Apr 2021 07:24:56 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eadfac8b2520b41436dd678f1f822ffcc0b416ce5d481a9070c4c4531b3d3efd`  
		Last Modified: Sat, 10 Apr 2021 07:25:16 GMT  
		Size: 113.1 MB (113127055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5936a8c3f2baf76cbebb0eaf333510aa2f52c6e825cf216638ac4b827ccc1d3`  
		Last Modified: Sat, 10 Apr 2021 07:24:56 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cca8ee89e625e42d7fcd5fd01d23c53c630d3aff4511b9a5f386713dc2e89ce4`  
		Last Modified: Sat, 10 Apr 2021 07:24:56 GMT  
		Size: 5.5 KB (5522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c79df02586a3bcf87a8109d34a6d6b32593583b49b5ae106cf89b70b04742c6`  
		Last Modified: Sat, 10 Apr 2021 07:24:56 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
