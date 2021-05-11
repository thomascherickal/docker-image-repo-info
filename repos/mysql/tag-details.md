<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mysql`

-	[`mysql:5`](#mysql5)
-	[`mysql:5.6`](#mysql56)
-	[`mysql:5.6.51`](#mysql5651)
-	[`mysql:5.7`](#mysql57)
-	[`mysql:5.7.34`](#mysql5734)
-	[`mysql:8`](#mysql8)
-	[`mysql:8.0`](#mysql80)
-	[`mysql:8.0.25`](#mysql8025)
-	[`mysql:latest`](#mysqllatest)

## `mysql:5`

```console
$ docker pull mysql@sha256:a655529fdfcbaf0ef28984d68a3e21778e061c886ff458b677391924f62fb457
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:5` - linux; amd64

```console
$ docker pull mysql@sha256:9f768489d306402ea11243f1b96aeaa4696adb9ed7c1bb0318724759b9cbd1a6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.4 MB (154430588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87eca374c0ed97f0f0b504174b0d22b0a0add454414c0dbf5ae43870369f6854`
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
# Mon, 19 Apr 2021 18:56:51 GMT
ENV MYSQL_VERSION=5.7.34-1debian10
# Mon, 19 Apr 2021 18:56:52 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Mon, 19 Apr 2021 18:57:11 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Mon, 19 Apr 2021 18:57:12 GMT
VOLUME [/var/lib/mysql]
# Mon, 19 Apr 2021 18:57:12 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Mon, 19 Apr 2021 18:57:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 19 Apr 2021 18:57:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 19 Apr 2021 18:57:13 GMT
EXPOSE 3306 33060
# Mon, 19 Apr 2021 18:57:13 GMT
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
	-	`sha256:cb7af63cbefa296bff9a46b3e93d6fb040dbf07873746852ec3fc680d0d32830`  
		Last Modified: Mon, 19 Apr 2021 18:58:11 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:151f1721bdbf5b1d09fc39e27a20276e41f9023b1d16e5ceea2be4a88759fd1b`  
		Last Modified: Mon, 19 Apr 2021 18:58:26 GMT  
		Size: 108.2 MB (108234757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcd19c3dd4882d2e43907224767266b8371dc230668fa5ce751d3303c6b918c1`  
		Last Modified: Mon, 19 Apr 2021 18:58:11 GMT  
		Size: 5.5 KB (5542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415af2aa5ddc7f5fc1106f3ce6d6d03c36dd06cda3e8539b081c0f8af42ee0c0`  
		Last Modified: Mon, 19 Apr 2021 18:58:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.6`

```console
$ docker pull mysql@sha256:1515ef90305b0365a0b17e490b8a9e28708ab8be4fabaf7b25a41ee071ae2c43
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:5.6` - linux; amd64

```console
$ docker pull mysql@sha256:4d3ef8034652ee13d7db73eafeb783440a2f10f2dd54e4f8808718b0748cc053
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.0 MB (102980915 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55c631ed05fcdcff73b8816e26e4ce010349425b9d3d3d535715844190038267`
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
# Mon, 19 Apr 2021 18:57:17 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Mon, 19 Apr 2021 18:57:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 19 Apr 2021 18:57:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 19 Apr 2021 18:57:18 GMT
EXPOSE 3306
# Mon, 19 Apr 2021 18:57:18 GMT
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
	-	`sha256:b642c189f2853ee5f6b68439535d39af53ed541b621621ae70cc6b3625f6342d`  
		Last Modified: Mon, 19 Apr 2021 18:58:41 GMT  
		Size: 5.6 KB (5559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e00196d02bd9da2a53fc82d3010664715105bfaeb108e43104bf465b8bf9d9d`  
		Last Modified: Mon, 19 Apr 2021 18:58:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.6.51`

```console
$ docker pull mysql@sha256:1515ef90305b0365a0b17e490b8a9e28708ab8be4fabaf7b25a41ee071ae2c43
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:5.6.51` - linux; amd64

```console
$ docker pull mysql@sha256:4d3ef8034652ee13d7db73eafeb783440a2f10f2dd54e4f8808718b0748cc053
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.0 MB (102980915 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55c631ed05fcdcff73b8816e26e4ce010349425b9d3d3d535715844190038267`
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
# Mon, 19 Apr 2021 18:57:17 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Mon, 19 Apr 2021 18:57:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 19 Apr 2021 18:57:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 19 Apr 2021 18:57:18 GMT
EXPOSE 3306
# Mon, 19 Apr 2021 18:57:18 GMT
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
	-	`sha256:b642c189f2853ee5f6b68439535d39af53ed541b621621ae70cc6b3625f6342d`  
		Last Modified: Mon, 19 Apr 2021 18:58:41 GMT  
		Size: 5.6 KB (5559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e00196d02bd9da2a53fc82d3010664715105bfaeb108e43104bf465b8bf9d9d`  
		Last Modified: Mon, 19 Apr 2021 18:58:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7`

```console
$ docker pull mysql@sha256:a655529fdfcbaf0ef28984d68a3e21778e061c886ff458b677391924f62fb457
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:5.7` - linux; amd64

```console
$ docker pull mysql@sha256:9f768489d306402ea11243f1b96aeaa4696adb9ed7c1bb0318724759b9cbd1a6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.4 MB (154430588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87eca374c0ed97f0f0b504174b0d22b0a0add454414c0dbf5ae43870369f6854`
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
# Mon, 19 Apr 2021 18:56:51 GMT
ENV MYSQL_VERSION=5.7.34-1debian10
# Mon, 19 Apr 2021 18:56:52 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Mon, 19 Apr 2021 18:57:11 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Mon, 19 Apr 2021 18:57:12 GMT
VOLUME [/var/lib/mysql]
# Mon, 19 Apr 2021 18:57:12 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Mon, 19 Apr 2021 18:57:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 19 Apr 2021 18:57:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 19 Apr 2021 18:57:13 GMT
EXPOSE 3306 33060
# Mon, 19 Apr 2021 18:57:13 GMT
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
	-	`sha256:cb7af63cbefa296bff9a46b3e93d6fb040dbf07873746852ec3fc680d0d32830`  
		Last Modified: Mon, 19 Apr 2021 18:58:11 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:151f1721bdbf5b1d09fc39e27a20276e41f9023b1d16e5ceea2be4a88759fd1b`  
		Last Modified: Mon, 19 Apr 2021 18:58:26 GMT  
		Size: 108.2 MB (108234757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcd19c3dd4882d2e43907224767266b8371dc230668fa5ce751d3303c6b918c1`  
		Last Modified: Mon, 19 Apr 2021 18:58:11 GMT  
		Size: 5.5 KB (5542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415af2aa5ddc7f5fc1106f3ce6d6d03c36dd06cda3e8539b081c0f8af42ee0c0`  
		Last Modified: Mon, 19 Apr 2021 18:58:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.34`

```console
$ docker pull mysql@sha256:a655529fdfcbaf0ef28984d68a3e21778e061c886ff458b677391924f62fb457
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:5.7.34` - linux; amd64

```console
$ docker pull mysql@sha256:9f768489d306402ea11243f1b96aeaa4696adb9ed7c1bb0318724759b9cbd1a6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.4 MB (154430588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87eca374c0ed97f0f0b504174b0d22b0a0add454414c0dbf5ae43870369f6854`
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
# Mon, 19 Apr 2021 18:56:51 GMT
ENV MYSQL_VERSION=5.7.34-1debian10
# Mon, 19 Apr 2021 18:56:52 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Mon, 19 Apr 2021 18:57:11 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Mon, 19 Apr 2021 18:57:12 GMT
VOLUME [/var/lib/mysql]
# Mon, 19 Apr 2021 18:57:12 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Mon, 19 Apr 2021 18:57:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 19 Apr 2021 18:57:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 19 Apr 2021 18:57:13 GMT
EXPOSE 3306 33060
# Mon, 19 Apr 2021 18:57:13 GMT
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
	-	`sha256:cb7af63cbefa296bff9a46b3e93d6fb040dbf07873746852ec3fc680d0d32830`  
		Last Modified: Mon, 19 Apr 2021 18:58:11 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:151f1721bdbf5b1d09fc39e27a20276e41f9023b1d16e5ceea2be4a88759fd1b`  
		Last Modified: Mon, 19 Apr 2021 18:58:26 GMT  
		Size: 108.2 MB (108234757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcd19c3dd4882d2e43907224767266b8371dc230668fa5ce751d3303c6b918c1`  
		Last Modified: Mon, 19 Apr 2021 18:58:11 GMT  
		Size: 5.5 KB (5542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415af2aa5ddc7f5fc1106f3ce6d6d03c36dd06cda3e8539b081c0f8af42ee0c0`  
		Last Modified: Mon, 19 Apr 2021 18:58:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8`

```console
$ docker pull mysql@sha256:cd42db5e061f8d1b1854e5fe597ad7ab9b9a5198ca1a2a560e5c4135b2d2b005
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:8` - linux; amd64

```console
$ docker pull mysql@sha256:64edc56b95c2e75174f0194bd686c32df027e6304a43126828be73ea0a784529
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.0 MB (162002265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8608131cc1cffc6189cbc413344ef347cec4e21d4d59fc6acc4f89989aa0b6ab`
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
# Tue, 11 May 2021 01:19:53 GMT
ENV MYSQL_VERSION=8.0.25-1debian10
# Tue, 11 May 2021 01:19:54 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 11 May 2021 01:20:11 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 11 May 2021 01:20:12 GMT
VOLUME [/var/lib/mysql]
# Tue, 11 May 2021 01:20:12 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 11 May 2021 01:20:12 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Tue, 11 May 2021 01:20:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 11 May 2021 01:20:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 May 2021 01:20:13 GMT
EXPOSE 3306 33060
# Tue, 11 May 2021 01:20:14 GMT
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
	-	`sha256:d44467b42d4cfab16a241cf78f72995ce2f16aa5daae17df2020a47ad5091493`  
		Last Modified: Tue, 11 May 2021 01:20:36 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae6d2197445755c51376d385e75585531c90ffad390c8f638f08470d7ca3df33`  
		Last Modified: Tue, 11 May 2021 01:20:56 GMT  
		Size: 115.8 MB (115805588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4ff89fec0f26a8d46318ae60ac34497ded2d5ffda8283f6db00ad5afdcfcc6`  
		Last Modified: Tue, 11 May 2021 01:20:36 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9b0d7f6e0f998818193bb020d22c5c1af23f5628c08e0dc8daa855cede5e48`  
		Last Modified: Tue, 11 May 2021 01:20:36 GMT  
		Size: 5.5 KB (5544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fb9ccf35d9f4d3391923b98efc5af20d48dd83769e2d0f04fc3151cb7d893c`  
		Last Modified: Tue, 11 May 2021 01:20:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0`

```console
$ docker pull mysql@sha256:cd42db5e061f8d1b1854e5fe597ad7ab9b9a5198ca1a2a560e5c4135b2d2b005
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:8.0` - linux; amd64

```console
$ docker pull mysql@sha256:64edc56b95c2e75174f0194bd686c32df027e6304a43126828be73ea0a784529
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.0 MB (162002265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8608131cc1cffc6189cbc413344ef347cec4e21d4d59fc6acc4f89989aa0b6ab`
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
# Tue, 11 May 2021 01:19:53 GMT
ENV MYSQL_VERSION=8.0.25-1debian10
# Tue, 11 May 2021 01:19:54 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 11 May 2021 01:20:11 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 11 May 2021 01:20:12 GMT
VOLUME [/var/lib/mysql]
# Tue, 11 May 2021 01:20:12 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 11 May 2021 01:20:12 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Tue, 11 May 2021 01:20:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 11 May 2021 01:20:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 May 2021 01:20:13 GMT
EXPOSE 3306 33060
# Tue, 11 May 2021 01:20:14 GMT
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
	-	`sha256:d44467b42d4cfab16a241cf78f72995ce2f16aa5daae17df2020a47ad5091493`  
		Last Modified: Tue, 11 May 2021 01:20:36 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae6d2197445755c51376d385e75585531c90ffad390c8f638f08470d7ca3df33`  
		Last Modified: Tue, 11 May 2021 01:20:56 GMT  
		Size: 115.8 MB (115805588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4ff89fec0f26a8d46318ae60ac34497ded2d5ffda8283f6db00ad5afdcfcc6`  
		Last Modified: Tue, 11 May 2021 01:20:36 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9b0d7f6e0f998818193bb020d22c5c1af23f5628c08e0dc8daa855cede5e48`  
		Last Modified: Tue, 11 May 2021 01:20:36 GMT  
		Size: 5.5 KB (5544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fb9ccf35d9f4d3391923b98efc5af20d48dd83769e2d0f04fc3151cb7d893c`  
		Last Modified: Tue, 11 May 2021 01:20:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.25`

```console
$ docker pull mysql@sha256:cd42db5e061f8d1b1854e5fe597ad7ab9b9a5198ca1a2a560e5c4135b2d2b005
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:8.0.25` - linux; amd64

```console
$ docker pull mysql@sha256:64edc56b95c2e75174f0194bd686c32df027e6304a43126828be73ea0a784529
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.0 MB (162002265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8608131cc1cffc6189cbc413344ef347cec4e21d4d59fc6acc4f89989aa0b6ab`
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
# Tue, 11 May 2021 01:19:53 GMT
ENV MYSQL_VERSION=8.0.25-1debian10
# Tue, 11 May 2021 01:19:54 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 11 May 2021 01:20:11 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 11 May 2021 01:20:12 GMT
VOLUME [/var/lib/mysql]
# Tue, 11 May 2021 01:20:12 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 11 May 2021 01:20:12 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Tue, 11 May 2021 01:20:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 11 May 2021 01:20:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 May 2021 01:20:13 GMT
EXPOSE 3306 33060
# Tue, 11 May 2021 01:20:14 GMT
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
	-	`sha256:d44467b42d4cfab16a241cf78f72995ce2f16aa5daae17df2020a47ad5091493`  
		Last Modified: Tue, 11 May 2021 01:20:36 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae6d2197445755c51376d385e75585531c90ffad390c8f638f08470d7ca3df33`  
		Last Modified: Tue, 11 May 2021 01:20:56 GMT  
		Size: 115.8 MB (115805588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4ff89fec0f26a8d46318ae60ac34497ded2d5ffda8283f6db00ad5afdcfcc6`  
		Last Modified: Tue, 11 May 2021 01:20:36 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9b0d7f6e0f998818193bb020d22c5c1af23f5628c08e0dc8daa855cede5e48`  
		Last Modified: Tue, 11 May 2021 01:20:36 GMT  
		Size: 5.5 KB (5544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fb9ccf35d9f4d3391923b98efc5af20d48dd83769e2d0f04fc3151cb7d893c`  
		Last Modified: Tue, 11 May 2021 01:20:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:latest`

```console
$ docker pull mysql@sha256:cd42db5e061f8d1b1854e5fe597ad7ab9b9a5198ca1a2a560e5c4135b2d2b005
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:latest` - linux; amd64

```console
$ docker pull mysql@sha256:64edc56b95c2e75174f0194bd686c32df027e6304a43126828be73ea0a784529
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.0 MB (162002265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8608131cc1cffc6189cbc413344ef347cec4e21d4d59fc6acc4f89989aa0b6ab`
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
# Tue, 11 May 2021 01:19:53 GMT
ENV MYSQL_VERSION=8.0.25-1debian10
# Tue, 11 May 2021 01:19:54 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 11 May 2021 01:20:11 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 11 May 2021 01:20:12 GMT
VOLUME [/var/lib/mysql]
# Tue, 11 May 2021 01:20:12 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 11 May 2021 01:20:12 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Tue, 11 May 2021 01:20:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 11 May 2021 01:20:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 May 2021 01:20:13 GMT
EXPOSE 3306 33060
# Tue, 11 May 2021 01:20:14 GMT
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
	-	`sha256:d44467b42d4cfab16a241cf78f72995ce2f16aa5daae17df2020a47ad5091493`  
		Last Modified: Tue, 11 May 2021 01:20:36 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae6d2197445755c51376d385e75585531c90ffad390c8f638f08470d7ca3df33`  
		Last Modified: Tue, 11 May 2021 01:20:56 GMT  
		Size: 115.8 MB (115805588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4ff89fec0f26a8d46318ae60ac34497ded2d5ffda8283f6db00ad5afdcfcc6`  
		Last Modified: Tue, 11 May 2021 01:20:36 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9b0d7f6e0f998818193bb020d22c5c1af23f5628c08e0dc8daa855cede5e48`  
		Last Modified: Tue, 11 May 2021 01:20:36 GMT  
		Size: 5.5 KB (5544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fb9ccf35d9f4d3391923b98efc5af20d48dd83769e2d0f04fc3151cb7d893c`  
		Last Modified: Tue, 11 May 2021 01:20:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
