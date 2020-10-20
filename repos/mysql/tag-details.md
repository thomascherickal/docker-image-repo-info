<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mysql`

-	[`mysql:5`](#mysql5)
-	[`mysql:5.6`](#mysql56)
-	[`mysql:5.6.50`](#mysql5650)
-	[`mysql:5.7`](#mysql57)
-	[`mysql:5.7.32`](#mysql5732)
-	[`mysql:8`](#mysql8)
-	[`mysql:8.0`](#mysql80)
-	[`mysql:8.0.22`](#mysql8022)
-	[`mysql:latest`](#mysqllatest)

## `mysql:5`

```console
$ docker pull mysql@sha256:8f084c4e1cbf80b1975344271c9ee4b4c0019f8d057c1d179644dd89eef46c0f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:5` - linux; amd64

```console
$ docker pull mysql@sha256:da0936fa5772538548f6fe4e7cb215ad89248cc57e89f1ccc27cb8927ada75de
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.5 MB (154492515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2836a03e922fadf36e2d5cff005394cd8391f9c33d8ffb9e92220564c94fdfca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 08:01:49 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Oct 2020 08:01:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 08:01:59 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 08:02:13 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 08:02:14 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 08:02:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 08:02:28 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Tue, 13 Oct 2020 08:03:07 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 20 Oct 2020 17:37:17 GMT
ENV MYSQL_VERSION=5.7.32-1debian10
# Tue, 20 Oct 2020 17:37:18 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ buster mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Tue, 20 Oct 2020 17:37:38 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-server="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Tue, 20 Oct 2020 17:37:38 GMT
VOLUME [/var/lib/mysql]
# Tue, 20 Oct 2020 17:37:38 GMT
COPY file:2e84dffb63712f3264bfeab4f9a2f55804ab9588ab4ad07a135b7e166143c0a8 in /usr/local/bin/ 
# Tue, 20 Oct 2020 17:37:39 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 20 Oct 2020 17:37:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 20 Oct 2020 17:37:40 GMT
EXPOSE 3306 33060
# Tue, 20 Oct 2020 17:37:40 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49e22f6fb9f7713028f8ed9b0beaa2ebac38d73ff6fd60532031e4a257f314c0`  
		Last Modified: Tue, 13 Oct 2020 08:05:18 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842b1255668c99365efe9cf8367baf458ad590033cfbe73c03e67a961d34a288`  
		Last Modified: Tue, 13 Oct 2020 08:05:18 GMT  
		Size: 4.2 MB (4178100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f48d1f430002d35f5766b2ba9cfbe0c624a705a542622a94e5b86e2132aba7b`  
		Last Modified: Tue, 13 Oct 2020 08:05:17 GMT  
		Size: 1.4 MB (1419213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c693f0615bcee7154070df04d6cce10562437d69ee98d469252e950cd79e0d7f`  
		Last Modified: Tue, 13 Oct 2020 08:05:17 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a621b9dbed2309be1806a0a750a6deef7c2558f25ceee4fcfc06ec421fad097`  
		Last Modified: Tue, 13 Oct 2020 08:05:21 GMT  
		Size: 13.4 MB (13447145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0807d32aef130f157419493647a5b252b6560b5385f14f102f388e576aeb1e98`  
		Last Modified: Tue, 13 Oct 2020 08:05:17 GMT  
		Size: 2.4 KB (2395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f15d42f48bd9c2924951d9edb9149949a0d23c54a55d2eafb626b1070340e22c`  
		Last Modified: Tue, 20 Oct 2020 17:38:53 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098ceecc0c8d6b662bfd5f6f03dcd320097804774e29dc6e091116a1f40827a5`  
		Last Modified: Tue, 20 Oct 2020 17:39:17 GMT  
		Size: 108.3 MB (108346099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0918bc006cab56c6f64110bc36671d76e19b6fcb8ad591ab9cd6c3993b07e04e`  
		Last Modified: Tue, 20 Oct 2020 17:38:52 GMT  
		Size: 5.1 KB (5142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0006443ed3e518a015ff4ae28f43e77d148758a3f3bcc87015f7f57b2dcacf`  
		Last Modified: Tue, 20 Oct 2020 17:38:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.6`

```console
$ docker pull mysql@sha256:ce3c841261675431fcffa70e221078d7466ecd242b658fdcf6a1c6af26f13c0d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:5.6` - linux; amd64

```console
$ docker pull mysql@sha256:fe0af8c6dd9e2ef38e5b922e41adf13be063e1b456bde63823f144561efa3821
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.9 MB (102932032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7aacec936dc932b41dd9b7ff79a618ce54e7a74ed2cde04c85536d74a6dabcdf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 13 Oct 2020 01:44:45 GMT
ADD file:4453535d387fcb17ead2026c72c05444e7558aa4736e3c0cdfb87cf20eaa5a9f in / 
# Tue, 13 Oct 2020 01:44:45 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 08:03:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Oct 2020 08:04:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 08:04:06 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 08:04:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 08:04:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 08:04:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 08:04:36 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Tue, 13 Oct 2020 08:04:37 GMT
ENV MYSQL_MAJOR=5.6
# Tue, 20 Oct 2020 17:37:46 GMT
ENV MYSQL_VERSION=5.6.50-1debian9
# Tue, 20 Oct 2020 17:37:47 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ stretch mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Tue, 20 Oct 2020 17:38:04 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-server="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Tue, 20 Oct 2020 17:38:04 GMT
VOLUME [/var/lib/mysql]
# Tue, 20 Oct 2020 17:38:04 GMT
COPY file:2e84dffb63712f3264bfeab4f9a2f55804ab9588ab4ad07a135b7e166143c0a8 in /usr/local/bin/ 
# Tue, 20 Oct 2020 17:38:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 20 Oct 2020 17:38:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 20 Oct 2020 17:38:05 GMT
EXPOSE 3306
# Tue, 20 Oct 2020 17:38:06 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:babf97a3f00ae0a4d59c1a0f88918d8f7aa0f0758380258b2016f0cd17e97202`  
		Last Modified: Tue, 13 Oct 2020 01:51:03 GMT  
		Size: 22.5 MB (22522093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88031ca211be8aea7f56e994790c341580c055c9139cfc6e26513eb6d4467dce`  
		Last Modified: Tue, 13 Oct 2020 08:06:11 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be1b1d426cbaea6a1fca730c199b2bfec20023cbeeb0173efbffe46956d32292`  
		Last Modified: Tue, 13 Oct 2020 08:06:11 GMT  
		Size: 4.5 MB (4502091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff53757c5bd8ad133514bd81b1c77e7e41b5016c145dbe390e82330116ab3cea`  
		Last Modified: Tue, 13 Oct 2020 08:06:10 GMT  
		Size: 1.4 MB (1412113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53127b7bc50ae0e3c50ba7baf9c4609b28e9f0070a0f26bd7d24d7f9d9f5fa35`  
		Last Modified: Tue, 13 Oct 2020 08:06:10 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4f269bc946e517ef316e9598dcdc08d69ace5024d10e74c594ce30653359a80`  
		Last Modified: Tue, 13 Oct 2020 08:06:13 GMT  
		Size: 10.2 MB (10224945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c0f95c5641ff69366197edd9c7e5915c8543763605eda7d31537d45929c68c4`  
		Last Modified: Tue, 13 Oct 2020 08:06:08 GMT  
		Size: 28.6 KB (28650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6eefa19530d60e3fe0478949b4e3bbd8960163423b2869676560c8e06247653`  
		Last Modified: Tue, 20 Oct 2020 17:39:28 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d1cff28e35ad13f11856942676e2c667282ddc9d26db983fc2a34a281d7a50`  
		Last Modified: Tue, 20 Oct 2020 17:39:40 GMT  
		Size: 64.2 MB (64234776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d00730e5a6293690bc2253653b8186efac104fddacf4ca0f36265cd1dfcdf55e`  
		Last Modified: Tue, 20 Oct 2020 17:39:27 GMT  
		Size: 5.2 KB (5157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6626db7c2055607dab5c53126bbcf995af5171c49fae85877506ae07d8a2359b`  
		Last Modified: Tue, 20 Oct 2020 17:39:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.6.50`

```console
$ docker pull mysql@sha256:ce3c841261675431fcffa70e221078d7466ecd242b658fdcf6a1c6af26f13c0d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:5.6.50` - linux; amd64

```console
$ docker pull mysql@sha256:fe0af8c6dd9e2ef38e5b922e41adf13be063e1b456bde63823f144561efa3821
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.9 MB (102932032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7aacec936dc932b41dd9b7ff79a618ce54e7a74ed2cde04c85536d74a6dabcdf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 13 Oct 2020 01:44:45 GMT
ADD file:4453535d387fcb17ead2026c72c05444e7558aa4736e3c0cdfb87cf20eaa5a9f in / 
# Tue, 13 Oct 2020 01:44:45 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 08:03:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Oct 2020 08:04:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 08:04:06 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 08:04:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 08:04:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 08:04:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 08:04:36 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Tue, 13 Oct 2020 08:04:37 GMT
ENV MYSQL_MAJOR=5.6
# Tue, 20 Oct 2020 17:37:46 GMT
ENV MYSQL_VERSION=5.6.50-1debian9
# Tue, 20 Oct 2020 17:37:47 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ stretch mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Tue, 20 Oct 2020 17:38:04 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-server="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Tue, 20 Oct 2020 17:38:04 GMT
VOLUME [/var/lib/mysql]
# Tue, 20 Oct 2020 17:38:04 GMT
COPY file:2e84dffb63712f3264bfeab4f9a2f55804ab9588ab4ad07a135b7e166143c0a8 in /usr/local/bin/ 
# Tue, 20 Oct 2020 17:38:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 20 Oct 2020 17:38:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 20 Oct 2020 17:38:05 GMT
EXPOSE 3306
# Tue, 20 Oct 2020 17:38:06 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:babf97a3f00ae0a4d59c1a0f88918d8f7aa0f0758380258b2016f0cd17e97202`  
		Last Modified: Tue, 13 Oct 2020 01:51:03 GMT  
		Size: 22.5 MB (22522093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88031ca211be8aea7f56e994790c341580c055c9139cfc6e26513eb6d4467dce`  
		Last Modified: Tue, 13 Oct 2020 08:06:11 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be1b1d426cbaea6a1fca730c199b2bfec20023cbeeb0173efbffe46956d32292`  
		Last Modified: Tue, 13 Oct 2020 08:06:11 GMT  
		Size: 4.5 MB (4502091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff53757c5bd8ad133514bd81b1c77e7e41b5016c145dbe390e82330116ab3cea`  
		Last Modified: Tue, 13 Oct 2020 08:06:10 GMT  
		Size: 1.4 MB (1412113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53127b7bc50ae0e3c50ba7baf9c4609b28e9f0070a0f26bd7d24d7f9d9f5fa35`  
		Last Modified: Tue, 13 Oct 2020 08:06:10 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4f269bc946e517ef316e9598dcdc08d69ace5024d10e74c594ce30653359a80`  
		Last Modified: Tue, 13 Oct 2020 08:06:13 GMT  
		Size: 10.2 MB (10224945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c0f95c5641ff69366197edd9c7e5915c8543763605eda7d31537d45929c68c4`  
		Last Modified: Tue, 13 Oct 2020 08:06:08 GMT  
		Size: 28.6 KB (28650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6eefa19530d60e3fe0478949b4e3bbd8960163423b2869676560c8e06247653`  
		Last Modified: Tue, 20 Oct 2020 17:39:28 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d1cff28e35ad13f11856942676e2c667282ddc9d26db983fc2a34a281d7a50`  
		Last Modified: Tue, 20 Oct 2020 17:39:40 GMT  
		Size: 64.2 MB (64234776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d00730e5a6293690bc2253653b8186efac104fddacf4ca0f36265cd1dfcdf55e`  
		Last Modified: Tue, 20 Oct 2020 17:39:27 GMT  
		Size: 5.2 KB (5157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6626db7c2055607dab5c53126bbcf995af5171c49fae85877506ae07d8a2359b`  
		Last Modified: Tue, 20 Oct 2020 17:39:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7`

```console
$ docker pull mysql@sha256:8f084c4e1cbf80b1975344271c9ee4b4c0019f8d057c1d179644dd89eef46c0f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:5.7` - linux; amd64

```console
$ docker pull mysql@sha256:da0936fa5772538548f6fe4e7cb215ad89248cc57e89f1ccc27cb8927ada75de
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.5 MB (154492515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2836a03e922fadf36e2d5cff005394cd8391f9c33d8ffb9e92220564c94fdfca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 08:01:49 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Oct 2020 08:01:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 08:01:59 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 08:02:13 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 08:02:14 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 08:02:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 08:02:28 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Tue, 13 Oct 2020 08:03:07 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 20 Oct 2020 17:37:17 GMT
ENV MYSQL_VERSION=5.7.32-1debian10
# Tue, 20 Oct 2020 17:37:18 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ buster mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Tue, 20 Oct 2020 17:37:38 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-server="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Tue, 20 Oct 2020 17:37:38 GMT
VOLUME [/var/lib/mysql]
# Tue, 20 Oct 2020 17:37:38 GMT
COPY file:2e84dffb63712f3264bfeab4f9a2f55804ab9588ab4ad07a135b7e166143c0a8 in /usr/local/bin/ 
# Tue, 20 Oct 2020 17:37:39 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 20 Oct 2020 17:37:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 20 Oct 2020 17:37:40 GMT
EXPOSE 3306 33060
# Tue, 20 Oct 2020 17:37:40 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49e22f6fb9f7713028f8ed9b0beaa2ebac38d73ff6fd60532031e4a257f314c0`  
		Last Modified: Tue, 13 Oct 2020 08:05:18 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842b1255668c99365efe9cf8367baf458ad590033cfbe73c03e67a961d34a288`  
		Last Modified: Tue, 13 Oct 2020 08:05:18 GMT  
		Size: 4.2 MB (4178100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f48d1f430002d35f5766b2ba9cfbe0c624a705a542622a94e5b86e2132aba7b`  
		Last Modified: Tue, 13 Oct 2020 08:05:17 GMT  
		Size: 1.4 MB (1419213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c693f0615bcee7154070df04d6cce10562437d69ee98d469252e950cd79e0d7f`  
		Last Modified: Tue, 13 Oct 2020 08:05:17 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a621b9dbed2309be1806a0a750a6deef7c2558f25ceee4fcfc06ec421fad097`  
		Last Modified: Tue, 13 Oct 2020 08:05:21 GMT  
		Size: 13.4 MB (13447145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0807d32aef130f157419493647a5b252b6560b5385f14f102f388e576aeb1e98`  
		Last Modified: Tue, 13 Oct 2020 08:05:17 GMT  
		Size: 2.4 KB (2395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f15d42f48bd9c2924951d9edb9149949a0d23c54a55d2eafb626b1070340e22c`  
		Last Modified: Tue, 20 Oct 2020 17:38:53 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098ceecc0c8d6b662bfd5f6f03dcd320097804774e29dc6e091116a1f40827a5`  
		Last Modified: Tue, 20 Oct 2020 17:39:17 GMT  
		Size: 108.3 MB (108346099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0918bc006cab56c6f64110bc36671d76e19b6fcb8ad591ab9cd6c3993b07e04e`  
		Last Modified: Tue, 20 Oct 2020 17:38:52 GMT  
		Size: 5.1 KB (5142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0006443ed3e518a015ff4ae28f43e77d148758a3f3bcc87015f7f57b2dcacf`  
		Last Modified: Tue, 20 Oct 2020 17:38:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.32`

```console
$ docker pull mysql@sha256:8f084c4e1cbf80b1975344271c9ee4b4c0019f8d057c1d179644dd89eef46c0f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:5.7.32` - linux; amd64

```console
$ docker pull mysql@sha256:da0936fa5772538548f6fe4e7cb215ad89248cc57e89f1ccc27cb8927ada75de
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.5 MB (154492515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2836a03e922fadf36e2d5cff005394cd8391f9c33d8ffb9e92220564c94fdfca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 08:01:49 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Oct 2020 08:01:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 08:01:59 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 08:02:13 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 08:02:14 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 08:02:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 08:02:28 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Tue, 13 Oct 2020 08:03:07 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 20 Oct 2020 17:37:17 GMT
ENV MYSQL_VERSION=5.7.32-1debian10
# Tue, 20 Oct 2020 17:37:18 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ buster mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Tue, 20 Oct 2020 17:37:38 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-server="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Tue, 20 Oct 2020 17:37:38 GMT
VOLUME [/var/lib/mysql]
# Tue, 20 Oct 2020 17:37:38 GMT
COPY file:2e84dffb63712f3264bfeab4f9a2f55804ab9588ab4ad07a135b7e166143c0a8 in /usr/local/bin/ 
# Tue, 20 Oct 2020 17:37:39 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 20 Oct 2020 17:37:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 20 Oct 2020 17:37:40 GMT
EXPOSE 3306 33060
# Tue, 20 Oct 2020 17:37:40 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49e22f6fb9f7713028f8ed9b0beaa2ebac38d73ff6fd60532031e4a257f314c0`  
		Last Modified: Tue, 13 Oct 2020 08:05:18 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842b1255668c99365efe9cf8367baf458ad590033cfbe73c03e67a961d34a288`  
		Last Modified: Tue, 13 Oct 2020 08:05:18 GMT  
		Size: 4.2 MB (4178100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f48d1f430002d35f5766b2ba9cfbe0c624a705a542622a94e5b86e2132aba7b`  
		Last Modified: Tue, 13 Oct 2020 08:05:17 GMT  
		Size: 1.4 MB (1419213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c693f0615bcee7154070df04d6cce10562437d69ee98d469252e950cd79e0d7f`  
		Last Modified: Tue, 13 Oct 2020 08:05:17 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a621b9dbed2309be1806a0a750a6deef7c2558f25ceee4fcfc06ec421fad097`  
		Last Modified: Tue, 13 Oct 2020 08:05:21 GMT  
		Size: 13.4 MB (13447145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0807d32aef130f157419493647a5b252b6560b5385f14f102f388e576aeb1e98`  
		Last Modified: Tue, 13 Oct 2020 08:05:17 GMT  
		Size: 2.4 KB (2395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f15d42f48bd9c2924951d9edb9149949a0d23c54a55d2eafb626b1070340e22c`  
		Last Modified: Tue, 20 Oct 2020 17:38:53 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098ceecc0c8d6b662bfd5f6f03dcd320097804774e29dc6e091116a1f40827a5`  
		Last Modified: Tue, 20 Oct 2020 17:39:17 GMT  
		Size: 108.3 MB (108346099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0918bc006cab56c6f64110bc36671d76e19b6fcb8ad591ab9cd6c3993b07e04e`  
		Last Modified: Tue, 20 Oct 2020 17:38:52 GMT  
		Size: 5.1 KB (5142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0006443ed3e518a015ff4ae28f43e77d148758a3f3bcc87015f7f57b2dcacf`  
		Last Modified: Tue, 20 Oct 2020 17:38:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8`

```console
$ docker pull mysql@sha256:b30e3c13ab71f51c7951120826671d56586afb8d9e1988c480b8673c8570eb74
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:8` - linux; amd64

```console
$ docker pull mysql@sha256:2eca4c35d70ef51251879bb8820bc7ad614c1e1d748ab58203198dca2d86862a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.9 MB (158947042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5c10a3624cefb120b8b43e2494aeaab8dfa69f10450a40670d9793c2f9c9564`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 08:01:49 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Oct 2020 08:01:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 08:01:59 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 08:02:13 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 08:02:14 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 08:02:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 08:02:28 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Tue, 13 Oct 2020 08:02:29 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 20 Oct 2020 17:36:52 GMT
ENV MYSQL_VERSION=8.0.22-1debian10
# Tue, 20 Oct 2020 17:36:52 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ buster mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Tue, 20 Oct 2020 17:37:08 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-community-client="${MYSQL_VERSION}" mysql-community-server-core="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 20 Oct 2020 17:37:09 GMT
VOLUME [/var/lib/mysql]
# Tue, 20 Oct 2020 17:37:09 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 20 Oct 2020 17:37:09 GMT
COPY file:2e84dffb63712f3264bfeab4f9a2f55804ab9588ab4ad07a135b7e166143c0a8 in /usr/local/bin/ 
# Tue, 20 Oct 2020 17:37:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 20 Oct 2020 17:37:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 20 Oct 2020 17:37:10 GMT
EXPOSE 3306 33060
# Tue, 20 Oct 2020 17:37:10 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49e22f6fb9f7713028f8ed9b0beaa2ebac38d73ff6fd60532031e4a257f314c0`  
		Last Modified: Tue, 13 Oct 2020 08:05:18 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842b1255668c99365efe9cf8367baf458ad590033cfbe73c03e67a961d34a288`  
		Last Modified: Tue, 13 Oct 2020 08:05:18 GMT  
		Size: 4.2 MB (4178100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f48d1f430002d35f5766b2ba9cfbe0c624a705a542622a94e5b86e2132aba7b`  
		Last Modified: Tue, 13 Oct 2020 08:05:17 GMT  
		Size: 1.4 MB (1419213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c693f0615bcee7154070df04d6cce10562437d69ee98d469252e950cd79e0d7f`  
		Last Modified: Tue, 13 Oct 2020 08:05:17 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a621b9dbed2309be1806a0a750a6deef7c2558f25ceee4fcfc06ec421fad097`  
		Last Modified: Tue, 13 Oct 2020 08:05:21 GMT  
		Size: 13.4 MB (13447145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0807d32aef130f157419493647a5b252b6560b5385f14f102f388e576aeb1e98`  
		Last Modified: Tue, 13 Oct 2020 08:05:17 GMT  
		Size: 2.4 KB (2395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a56aca0feb17476e72fda7870d29fa02e55f15425b4d6f5a6cedab5ad0643027`  
		Last Modified: Tue, 20 Oct 2020 17:38:19 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de9d45fd0f07d1b3ffb0aed01b60f26009a1d5c7b1a9924310864fdcb36e524c`  
		Last Modified: Tue, 20 Oct 2020 17:38:41 GMT  
		Size: 112.8 MB (112799781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d68a49161ccf8bf7e4c114c2cf726216d40a084a5031f658884d2425c9d622e`  
		Last Modified: Tue, 20 Oct 2020 17:38:18 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47834b5a7c81715b3899c465ebaef492cd3587232d40e975b861fd451757ed14`  
		Last Modified: Tue, 20 Oct 2020 17:38:18 GMT  
		Size: 5.1 KB (5142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0764b0009c40d1b0650ac0092e1d660d83fea453c81574f1337f3de295de56`  
		Last Modified: Tue, 20 Oct 2020 17:38:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0`

```console
$ docker pull mysql@sha256:b30e3c13ab71f51c7951120826671d56586afb8d9e1988c480b8673c8570eb74
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:8.0` - linux; amd64

```console
$ docker pull mysql@sha256:2eca4c35d70ef51251879bb8820bc7ad614c1e1d748ab58203198dca2d86862a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.9 MB (158947042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5c10a3624cefb120b8b43e2494aeaab8dfa69f10450a40670d9793c2f9c9564`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 08:01:49 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Oct 2020 08:01:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 08:01:59 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 08:02:13 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 08:02:14 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 08:02:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 08:02:28 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Tue, 13 Oct 2020 08:02:29 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 20 Oct 2020 17:36:52 GMT
ENV MYSQL_VERSION=8.0.22-1debian10
# Tue, 20 Oct 2020 17:36:52 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ buster mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Tue, 20 Oct 2020 17:37:08 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-community-client="${MYSQL_VERSION}" mysql-community-server-core="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 20 Oct 2020 17:37:09 GMT
VOLUME [/var/lib/mysql]
# Tue, 20 Oct 2020 17:37:09 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 20 Oct 2020 17:37:09 GMT
COPY file:2e84dffb63712f3264bfeab4f9a2f55804ab9588ab4ad07a135b7e166143c0a8 in /usr/local/bin/ 
# Tue, 20 Oct 2020 17:37:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 20 Oct 2020 17:37:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 20 Oct 2020 17:37:10 GMT
EXPOSE 3306 33060
# Tue, 20 Oct 2020 17:37:10 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49e22f6fb9f7713028f8ed9b0beaa2ebac38d73ff6fd60532031e4a257f314c0`  
		Last Modified: Tue, 13 Oct 2020 08:05:18 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842b1255668c99365efe9cf8367baf458ad590033cfbe73c03e67a961d34a288`  
		Last Modified: Tue, 13 Oct 2020 08:05:18 GMT  
		Size: 4.2 MB (4178100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f48d1f430002d35f5766b2ba9cfbe0c624a705a542622a94e5b86e2132aba7b`  
		Last Modified: Tue, 13 Oct 2020 08:05:17 GMT  
		Size: 1.4 MB (1419213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c693f0615bcee7154070df04d6cce10562437d69ee98d469252e950cd79e0d7f`  
		Last Modified: Tue, 13 Oct 2020 08:05:17 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a621b9dbed2309be1806a0a750a6deef7c2558f25ceee4fcfc06ec421fad097`  
		Last Modified: Tue, 13 Oct 2020 08:05:21 GMT  
		Size: 13.4 MB (13447145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0807d32aef130f157419493647a5b252b6560b5385f14f102f388e576aeb1e98`  
		Last Modified: Tue, 13 Oct 2020 08:05:17 GMT  
		Size: 2.4 KB (2395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a56aca0feb17476e72fda7870d29fa02e55f15425b4d6f5a6cedab5ad0643027`  
		Last Modified: Tue, 20 Oct 2020 17:38:19 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de9d45fd0f07d1b3ffb0aed01b60f26009a1d5c7b1a9924310864fdcb36e524c`  
		Last Modified: Tue, 20 Oct 2020 17:38:41 GMT  
		Size: 112.8 MB (112799781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d68a49161ccf8bf7e4c114c2cf726216d40a084a5031f658884d2425c9d622e`  
		Last Modified: Tue, 20 Oct 2020 17:38:18 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47834b5a7c81715b3899c465ebaef492cd3587232d40e975b861fd451757ed14`  
		Last Modified: Tue, 20 Oct 2020 17:38:18 GMT  
		Size: 5.1 KB (5142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0764b0009c40d1b0650ac0092e1d660d83fea453c81574f1337f3de295de56`  
		Last Modified: Tue, 20 Oct 2020 17:38:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.22`

```console
$ docker pull mysql@sha256:b30e3c13ab71f51c7951120826671d56586afb8d9e1988c480b8673c8570eb74
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:8.0.22` - linux; amd64

```console
$ docker pull mysql@sha256:2eca4c35d70ef51251879bb8820bc7ad614c1e1d748ab58203198dca2d86862a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.9 MB (158947042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5c10a3624cefb120b8b43e2494aeaab8dfa69f10450a40670d9793c2f9c9564`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 08:01:49 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Oct 2020 08:01:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 08:01:59 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 08:02:13 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 08:02:14 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 08:02:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 08:02:28 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Tue, 13 Oct 2020 08:02:29 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 20 Oct 2020 17:36:52 GMT
ENV MYSQL_VERSION=8.0.22-1debian10
# Tue, 20 Oct 2020 17:36:52 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ buster mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Tue, 20 Oct 2020 17:37:08 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-community-client="${MYSQL_VERSION}" mysql-community-server-core="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 20 Oct 2020 17:37:09 GMT
VOLUME [/var/lib/mysql]
# Tue, 20 Oct 2020 17:37:09 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 20 Oct 2020 17:37:09 GMT
COPY file:2e84dffb63712f3264bfeab4f9a2f55804ab9588ab4ad07a135b7e166143c0a8 in /usr/local/bin/ 
# Tue, 20 Oct 2020 17:37:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 20 Oct 2020 17:37:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 20 Oct 2020 17:37:10 GMT
EXPOSE 3306 33060
# Tue, 20 Oct 2020 17:37:10 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49e22f6fb9f7713028f8ed9b0beaa2ebac38d73ff6fd60532031e4a257f314c0`  
		Last Modified: Tue, 13 Oct 2020 08:05:18 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842b1255668c99365efe9cf8367baf458ad590033cfbe73c03e67a961d34a288`  
		Last Modified: Tue, 13 Oct 2020 08:05:18 GMT  
		Size: 4.2 MB (4178100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f48d1f430002d35f5766b2ba9cfbe0c624a705a542622a94e5b86e2132aba7b`  
		Last Modified: Tue, 13 Oct 2020 08:05:17 GMT  
		Size: 1.4 MB (1419213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c693f0615bcee7154070df04d6cce10562437d69ee98d469252e950cd79e0d7f`  
		Last Modified: Tue, 13 Oct 2020 08:05:17 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a621b9dbed2309be1806a0a750a6deef7c2558f25ceee4fcfc06ec421fad097`  
		Last Modified: Tue, 13 Oct 2020 08:05:21 GMT  
		Size: 13.4 MB (13447145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0807d32aef130f157419493647a5b252b6560b5385f14f102f388e576aeb1e98`  
		Last Modified: Tue, 13 Oct 2020 08:05:17 GMT  
		Size: 2.4 KB (2395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a56aca0feb17476e72fda7870d29fa02e55f15425b4d6f5a6cedab5ad0643027`  
		Last Modified: Tue, 20 Oct 2020 17:38:19 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de9d45fd0f07d1b3ffb0aed01b60f26009a1d5c7b1a9924310864fdcb36e524c`  
		Last Modified: Tue, 20 Oct 2020 17:38:41 GMT  
		Size: 112.8 MB (112799781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d68a49161ccf8bf7e4c114c2cf726216d40a084a5031f658884d2425c9d622e`  
		Last Modified: Tue, 20 Oct 2020 17:38:18 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47834b5a7c81715b3899c465ebaef492cd3587232d40e975b861fd451757ed14`  
		Last Modified: Tue, 20 Oct 2020 17:38:18 GMT  
		Size: 5.1 KB (5142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0764b0009c40d1b0650ac0092e1d660d83fea453c81574f1337f3de295de56`  
		Last Modified: Tue, 20 Oct 2020 17:38:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:latest`

```console
$ docker pull mysql@sha256:b30e3c13ab71f51c7951120826671d56586afb8d9e1988c480b8673c8570eb74
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:latest` - linux; amd64

```console
$ docker pull mysql@sha256:2eca4c35d70ef51251879bb8820bc7ad614c1e1d748ab58203198dca2d86862a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.9 MB (158947042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5c10a3624cefb120b8b43e2494aeaab8dfa69f10450a40670d9793c2f9c9564`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 08:01:49 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Oct 2020 08:01:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 08:01:59 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 08:02:13 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 08:02:14 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 08:02:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 08:02:28 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Tue, 13 Oct 2020 08:02:29 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 20 Oct 2020 17:36:52 GMT
ENV MYSQL_VERSION=8.0.22-1debian10
# Tue, 20 Oct 2020 17:36:52 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ buster mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Tue, 20 Oct 2020 17:37:08 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-community-client="${MYSQL_VERSION}" mysql-community-server-core="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 20 Oct 2020 17:37:09 GMT
VOLUME [/var/lib/mysql]
# Tue, 20 Oct 2020 17:37:09 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 20 Oct 2020 17:37:09 GMT
COPY file:2e84dffb63712f3264bfeab4f9a2f55804ab9588ab4ad07a135b7e166143c0a8 in /usr/local/bin/ 
# Tue, 20 Oct 2020 17:37:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 20 Oct 2020 17:37:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 20 Oct 2020 17:37:10 GMT
EXPOSE 3306 33060
# Tue, 20 Oct 2020 17:37:10 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49e22f6fb9f7713028f8ed9b0beaa2ebac38d73ff6fd60532031e4a257f314c0`  
		Last Modified: Tue, 13 Oct 2020 08:05:18 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842b1255668c99365efe9cf8367baf458ad590033cfbe73c03e67a961d34a288`  
		Last Modified: Tue, 13 Oct 2020 08:05:18 GMT  
		Size: 4.2 MB (4178100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f48d1f430002d35f5766b2ba9cfbe0c624a705a542622a94e5b86e2132aba7b`  
		Last Modified: Tue, 13 Oct 2020 08:05:17 GMT  
		Size: 1.4 MB (1419213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c693f0615bcee7154070df04d6cce10562437d69ee98d469252e950cd79e0d7f`  
		Last Modified: Tue, 13 Oct 2020 08:05:17 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a621b9dbed2309be1806a0a750a6deef7c2558f25ceee4fcfc06ec421fad097`  
		Last Modified: Tue, 13 Oct 2020 08:05:21 GMT  
		Size: 13.4 MB (13447145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0807d32aef130f157419493647a5b252b6560b5385f14f102f388e576aeb1e98`  
		Last Modified: Tue, 13 Oct 2020 08:05:17 GMT  
		Size: 2.4 KB (2395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a56aca0feb17476e72fda7870d29fa02e55f15425b4d6f5a6cedab5ad0643027`  
		Last Modified: Tue, 20 Oct 2020 17:38:19 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de9d45fd0f07d1b3ffb0aed01b60f26009a1d5c7b1a9924310864fdcb36e524c`  
		Last Modified: Tue, 20 Oct 2020 17:38:41 GMT  
		Size: 112.8 MB (112799781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d68a49161ccf8bf7e4c114c2cf726216d40a084a5031f658884d2425c9d622e`  
		Last Modified: Tue, 20 Oct 2020 17:38:18 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47834b5a7c81715b3899c465ebaef492cd3587232d40e975b861fd451757ed14`  
		Last Modified: Tue, 20 Oct 2020 17:38:18 GMT  
		Size: 5.1 KB (5142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0764b0009c40d1b0650ac0092e1d660d83fea453c81574f1337f3de295de56`  
		Last Modified: Tue, 20 Oct 2020 17:38:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
