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
$ docker pull mysql@sha256:b3dc8d10307ab7b9ca1a7981b1601a67e176408be618fc4216d137be37dae10b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:5` - linux; amd64

```console
$ docker pull mysql@sha256:3830eda172a0285aa9899c422f26d739cde0ad5445962fbb9a2a8b0df00a1a64
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.5 MB (154474521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42cdba9f1b0840cd63254898edeaf6def81a503a6a53d57301c3b38e69cd8f15`
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
# Tue, 13 Oct 2020 08:03:07 GMT
ENV MYSQL_VERSION=5.7.31-1debian10
# Tue, 13 Oct 2020 08:03:08 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ buster mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Tue, 13 Oct 2020 08:03:42 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-server="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Tue, 13 Oct 2020 08:03:42 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Oct 2020 08:03:43 GMT
COPY file:7cbb26bbdb8e71b36aafda38dbac08caa641714a19991b86cde77daf3286ec11 in /usr/local/bin/ 
# Tue, 13 Oct 2020 08:03:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Oct 2020 08:03:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 08:03:45 GMT
EXPOSE 3306 33060
# Tue, 13 Oct 2020 08:03:45 GMT
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
	-	`sha256:6d2fc69dfa35df3eb1099501d90a60c477cc59bb043350815faa61273f30ebb2`  
		Last Modified: Tue, 13 Oct 2020 08:05:44 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56153548dd2c828e151b54d5dee6bc184254767aac1753e4f176a72ef098fccc`  
		Last Modified: Tue, 13 Oct 2020 08:06:03 GMT  
		Size: 108.3 MB (108328098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb6ba94030303d9e95c4d436e78295a17912542c3d539116efe436678d90684`  
		Last Modified: Tue, 13 Oct 2020 08:05:44 GMT  
		Size: 5.1 KB (5145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e1888da91a7bfdd32ba485e7f82bec46eae19896901cc433c8203d8927087fb`  
		Last Modified: Tue, 13 Oct 2020 08:05:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.6`

```console
$ docker pull mysql@sha256:8f24bff8b42841943e0c33f229aedd5a5a5dd87323164be1cb9003bfa0b2042f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:5.6` - linux; amd64

```console
$ docker pull mysql@sha256:fd2efa27349844379503b95aa4626fc68596024e0c39184d804574dfd0122713
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.9 MB (102930127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f36ba851740564a2cc0790722bd5aba5d74882c4009c5c664ee968f1e7911c0`
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
# Tue, 13 Oct 2020 08:04:37 GMT
ENV MYSQL_VERSION=5.6.49-1debian9
# Tue, 13 Oct 2020 08:04:38 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ stretch mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Tue, 13 Oct 2020 08:04:55 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-server="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Tue, 13 Oct 2020 08:04:55 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Oct 2020 08:04:56 GMT
COPY file:7cbb26bbdb8e71b36aafda38dbac08caa641714a19991b86cde77daf3286ec11 in /usr/local/bin/ 
# Tue, 13 Oct 2020 08:04:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Oct 2020 08:04:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 08:04:57 GMT
EXPOSE 3306
# Tue, 13 Oct 2020 08:04:57 GMT
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
	-	`sha256:3b6c8aee8eabe3ff789560bb73cfaefe49f698546dfadab01d292b5e23a2e4a0`  
		Last Modified: Tue, 13 Oct 2020 08:06:08 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:423995312f2c140d3dcd366531b0e41d58a6c1e1813018a66ea973dde94a56ef`  
		Last Modified: Tue, 13 Oct 2020 08:06:23 GMT  
		Size: 64.2 MB (64232868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6774a794eadf20fc4fccafb05eac55715893bcd474c479ae711fcab7e65c354`  
		Last Modified: Tue, 13 Oct 2020 08:06:08 GMT  
		Size: 5.2 KB (5163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b1b7c16ee5804c4c990b593c1647bd873caba77932658b99a0a7c87dcff5143`  
		Last Modified: Tue, 13 Oct 2020 08:06:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.6.49`

```console
$ docker pull mysql@sha256:8f24bff8b42841943e0c33f229aedd5a5a5dd87323164be1cb9003bfa0b2042f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:5.6.49` - linux; amd64

```console
$ docker pull mysql@sha256:fd2efa27349844379503b95aa4626fc68596024e0c39184d804574dfd0122713
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.9 MB (102930127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f36ba851740564a2cc0790722bd5aba5d74882c4009c5c664ee968f1e7911c0`
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
# Tue, 13 Oct 2020 08:04:37 GMT
ENV MYSQL_VERSION=5.6.49-1debian9
# Tue, 13 Oct 2020 08:04:38 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ stretch mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Tue, 13 Oct 2020 08:04:55 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-server="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Tue, 13 Oct 2020 08:04:55 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Oct 2020 08:04:56 GMT
COPY file:7cbb26bbdb8e71b36aafda38dbac08caa641714a19991b86cde77daf3286ec11 in /usr/local/bin/ 
# Tue, 13 Oct 2020 08:04:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Oct 2020 08:04:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 08:04:57 GMT
EXPOSE 3306
# Tue, 13 Oct 2020 08:04:57 GMT
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
	-	`sha256:3b6c8aee8eabe3ff789560bb73cfaefe49f698546dfadab01d292b5e23a2e4a0`  
		Last Modified: Tue, 13 Oct 2020 08:06:08 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:423995312f2c140d3dcd366531b0e41d58a6c1e1813018a66ea973dde94a56ef`  
		Last Modified: Tue, 13 Oct 2020 08:06:23 GMT  
		Size: 64.2 MB (64232868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6774a794eadf20fc4fccafb05eac55715893bcd474c479ae711fcab7e65c354`  
		Last Modified: Tue, 13 Oct 2020 08:06:08 GMT  
		Size: 5.2 KB (5163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b1b7c16ee5804c4c990b593c1647bd873caba77932658b99a0a7c87dcff5143`  
		Last Modified: Tue, 13 Oct 2020 08:06:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7`

```console
$ docker pull mysql@sha256:b3dc8d10307ab7b9ca1a7981b1601a67e176408be618fc4216d137be37dae10b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:5.7` - linux; amd64

```console
$ docker pull mysql@sha256:3830eda172a0285aa9899c422f26d739cde0ad5445962fbb9a2a8b0df00a1a64
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.5 MB (154474521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42cdba9f1b0840cd63254898edeaf6def81a503a6a53d57301c3b38e69cd8f15`
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
# Tue, 13 Oct 2020 08:03:07 GMT
ENV MYSQL_VERSION=5.7.31-1debian10
# Tue, 13 Oct 2020 08:03:08 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ buster mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Tue, 13 Oct 2020 08:03:42 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-server="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Tue, 13 Oct 2020 08:03:42 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Oct 2020 08:03:43 GMT
COPY file:7cbb26bbdb8e71b36aafda38dbac08caa641714a19991b86cde77daf3286ec11 in /usr/local/bin/ 
# Tue, 13 Oct 2020 08:03:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Oct 2020 08:03:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 08:03:45 GMT
EXPOSE 3306 33060
# Tue, 13 Oct 2020 08:03:45 GMT
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
	-	`sha256:6d2fc69dfa35df3eb1099501d90a60c477cc59bb043350815faa61273f30ebb2`  
		Last Modified: Tue, 13 Oct 2020 08:05:44 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56153548dd2c828e151b54d5dee6bc184254767aac1753e4f176a72ef098fccc`  
		Last Modified: Tue, 13 Oct 2020 08:06:03 GMT  
		Size: 108.3 MB (108328098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb6ba94030303d9e95c4d436e78295a17912542c3d539116efe436678d90684`  
		Last Modified: Tue, 13 Oct 2020 08:05:44 GMT  
		Size: 5.1 KB (5145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e1888da91a7bfdd32ba485e7f82bec46eae19896901cc433c8203d8927087fb`  
		Last Modified: Tue, 13 Oct 2020 08:05:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.31`

```console
$ docker pull mysql@sha256:b3dc8d10307ab7b9ca1a7981b1601a67e176408be618fc4216d137be37dae10b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:5.7.31` - linux; amd64

```console
$ docker pull mysql@sha256:3830eda172a0285aa9899c422f26d739cde0ad5445962fbb9a2a8b0df00a1a64
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.5 MB (154474521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42cdba9f1b0840cd63254898edeaf6def81a503a6a53d57301c3b38e69cd8f15`
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
# Tue, 13 Oct 2020 08:03:07 GMT
ENV MYSQL_VERSION=5.7.31-1debian10
# Tue, 13 Oct 2020 08:03:08 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ buster mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Tue, 13 Oct 2020 08:03:42 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-server="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Tue, 13 Oct 2020 08:03:42 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Oct 2020 08:03:43 GMT
COPY file:7cbb26bbdb8e71b36aafda38dbac08caa641714a19991b86cde77daf3286ec11 in /usr/local/bin/ 
# Tue, 13 Oct 2020 08:03:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Oct 2020 08:03:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 08:03:45 GMT
EXPOSE 3306 33060
# Tue, 13 Oct 2020 08:03:45 GMT
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
	-	`sha256:6d2fc69dfa35df3eb1099501d90a60c477cc59bb043350815faa61273f30ebb2`  
		Last Modified: Tue, 13 Oct 2020 08:05:44 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56153548dd2c828e151b54d5dee6bc184254767aac1753e4f176a72ef098fccc`  
		Last Modified: Tue, 13 Oct 2020 08:06:03 GMT  
		Size: 108.3 MB (108328098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb6ba94030303d9e95c4d436e78295a17912542c3d539116efe436678d90684`  
		Last Modified: Tue, 13 Oct 2020 08:05:44 GMT  
		Size: 5.1 KB (5145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e1888da91a7bfdd32ba485e7f82bec46eae19896901cc433c8203d8927087fb`  
		Last Modified: Tue, 13 Oct 2020 08:05:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8`

```console
$ docker pull mysql@sha256:86b7c83e24c824163927db1016d5ab153a9a04358951be8b236171286e3289a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:8` - linux; amd64

```console
$ docker pull mysql@sha256:77b7e09c906615c1bb59b2e9d7703f728b1186a5a70e547ce2f1079ef4c1c5ca
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.6 MB (158633522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e85dd5c32558ea5c22cc4786cff512c1940270a50e7dbc21ad2df42f0637de4`
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
# Tue, 13 Oct 2020 08:02:29 GMT
ENV MYSQL_VERSION=8.0.21-1debian10
# Tue, 13 Oct 2020 08:02:30 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ buster mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Tue, 13 Oct 2020 08:02:57 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-community-client="${MYSQL_VERSION}" mysql-community-server-core="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 13 Oct 2020 08:02:57 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Oct 2020 08:02:58 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 13 Oct 2020 08:02:58 GMT
COPY file:7cbb26bbdb8e71b36aafda38dbac08caa641714a19991b86cde77daf3286ec11 in /usr/local/bin/ 
# Tue, 13 Oct 2020 08:03:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Oct 2020 08:03:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 08:03:00 GMT
EXPOSE 3306 33060
# Tue, 13 Oct 2020 08:03:01 GMT
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
	-	`sha256:9eb4355ba4508252590eb497a480a1d154529cff1ccdada2c60e628aaa73dc18`  
		Last Modified: Tue, 13 Oct 2020 08:05:16 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6879faad3b6c70e300c1ad96cf752b85e4a54ade54b8e4d370600a57e617c439`  
		Last Modified: Tue, 13 Oct 2020 08:05:39 GMT  
		Size: 112.5 MB (112486256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:164ef92f3887884a8e93d96f0a4cdfe88912f0dc4a257b857c1aa63c7ee5e00f`  
		Last Modified: Tue, 13 Oct 2020 08:05:16 GMT  
		Size: 843.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e4a6e666228dc751782155f2b3af56ed7c5e9ba56ef35c36f03587b6242065d`  
		Last Modified: Tue, 13 Oct 2020 08:05:16 GMT  
		Size: 5.1 KB (5145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45dea7731adeb126e6275444517123fc75f817c1949722f608d1eedef8ce475`  
		Last Modified: Tue, 13 Oct 2020 08:05:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0`

```console
$ docker pull mysql@sha256:86b7c83e24c824163927db1016d5ab153a9a04358951be8b236171286e3289a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:8.0` - linux; amd64

```console
$ docker pull mysql@sha256:77b7e09c906615c1bb59b2e9d7703f728b1186a5a70e547ce2f1079ef4c1c5ca
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.6 MB (158633522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e85dd5c32558ea5c22cc4786cff512c1940270a50e7dbc21ad2df42f0637de4`
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
# Tue, 13 Oct 2020 08:02:29 GMT
ENV MYSQL_VERSION=8.0.21-1debian10
# Tue, 13 Oct 2020 08:02:30 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ buster mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Tue, 13 Oct 2020 08:02:57 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-community-client="${MYSQL_VERSION}" mysql-community-server-core="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 13 Oct 2020 08:02:57 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Oct 2020 08:02:58 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 13 Oct 2020 08:02:58 GMT
COPY file:7cbb26bbdb8e71b36aafda38dbac08caa641714a19991b86cde77daf3286ec11 in /usr/local/bin/ 
# Tue, 13 Oct 2020 08:03:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Oct 2020 08:03:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 08:03:00 GMT
EXPOSE 3306 33060
# Tue, 13 Oct 2020 08:03:01 GMT
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
	-	`sha256:9eb4355ba4508252590eb497a480a1d154529cff1ccdada2c60e628aaa73dc18`  
		Last Modified: Tue, 13 Oct 2020 08:05:16 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6879faad3b6c70e300c1ad96cf752b85e4a54ade54b8e4d370600a57e617c439`  
		Last Modified: Tue, 13 Oct 2020 08:05:39 GMT  
		Size: 112.5 MB (112486256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:164ef92f3887884a8e93d96f0a4cdfe88912f0dc4a257b857c1aa63c7ee5e00f`  
		Last Modified: Tue, 13 Oct 2020 08:05:16 GMT  
		Size: 843.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e4a6e666228dc751782155f2b3af56ed7c5e9ba56ef35c36f03587b6242065d`  
		Last Modified: Tue, 13 Oct 2020 08:05:16 GMT  
		Size: 5.1 KB (5145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45dea7731adeb126e6275444517123fc75f817c1949722f608d1eedef8ce475`  
		Last Modified: Tue, 13 Oct 2020 08:05:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.21`

```console
$ docker pull mysql@sha256:86b7c83e24c824163927db1016d5ab153a9a04358951be8b236171286e3289a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:8.0.21` - linux; amd64

```console
$ docker pull mysql@sha256:77b7e09c906615c1bb59b2e9d7703f728b1186a5a70e547ce2f1079ef4c1c5ca
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.6 MB (158633522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e85dd5c32558ea5c22cc4786cff512c1940270a50e7dbc21ad2df42f0637de4`
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
# Tue, 13 Oct 2020 08:02:29 GMT
ENV MYSQL_VERSION=8.0.21-1debian10
# Tue, 13 Oct 2020 08:02:30 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ buster mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Tue, 13 Oct 2020 08:02:57 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-community-client="${MYSQL_VERSION}" mysql-community-server-core="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 13 Oct 2020 08:02:57 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Oct 2020 08:02:58 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 13 Oct 2020 08:02:58 GMT
COPY file:7cbb26bbdb8e71b36aafda38dbac08caa641714a19991b86cde77daf3286ec11 in /usr/local/bin/ 
# Tue, 13 Oct 2020 08:03:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Oct 2020 08:03:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 08:03:00 GMT
EXPOSE 3306 33060
# Tue, 13 Oct 2020 08:03:01 GMT
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
	-	`sha256:9eb4355ba4508252590eb497a480a1d154529cff1ccdada2c60e628aaa73dc18`  
		Last Modified: Tue, 13 Oct 2020 08:05:16 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6879faad3b6c70e300c1ad96cf752b85e4a54ade54b8e4d370600a57e617c439`  
		Last Modified: Tue, 13 Oct 2020 08:05:39 GMT  
		Size: 112.5 MB (112486256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:164ef92f3887884a8e93d96f0a4cdfe88912f0dc4a257b857c1aa63c7ee5e00f`  
		Last Modified: Tue, 13 Oct 2020 08:05:16 GMT  
		Size: 843.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e4a6e666228dc751782155f2b3af56ed7c5e9ba56ef35c36f03587b6242065d`  
		Last Modified: Tue, 13 Oct 2020 08:05:16 GMT  
		Size: 5.1 KB (5145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45dea7731adeb126e6275444517123fc75f817c1949722f608d1eedef8ce475`  
		Last Modified: Tue, 13 Oct 2020 08:05:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:latest`

```console
$ docker pull mysql@sha256:86b7c83e24c824163927db1016d5ab153a9a04358951be8b236171286e3289a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:latest` - linux; amd64

```console
$ docker pull mysql@sha256:77b7e09c906615c1bb59b2e9d7703f728b1186a5a70e547ce2f1079ef4c1c5ca
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.6 MB (158633522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e85dd5c32558ea5c22cc4786cff512c1940270a50e7dbc21ad2df42f0637de4`
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
# Tue, 13 Oct 2020 08:02:29 GMT
ENV MYSQL_VERSION=8.0.21-1debian10
# Tue, 13 Oct 2020 08:02:30 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ buster mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Tue, 13 Oct 2020 08:02:57 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-community-client="${MYSQL_VERSION}" mysql-community-server-core="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 13 Oct 2020 08:02:57 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Oct 2020 08:02:58 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 13 Oct 2020 08:02:58 GMT
COPY file:7cbb26bbdb8e71b36aafda38dbac08caa641714a19991b86cde77daf3286ec11 in /usr/local/bin/ 
# Tue, 13 Oct 2020 08:03:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Oct 2020 08:03:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 08:03:00 GMT
EXPOSE 3306 33060
# Tue, 13 Oct 2020 08:03:01 GMT
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
	-	`sha256:9eb4355ba4508252590eb497a480a1d154529cff1ccdada2c60e628aaa73dc18`  
		Last Modified: Tue, 13 Oct 2020 08:05:16 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6879faad3b6c70e300c1ad96cf752b85e4a54ade54b8e4d370600a57e617c439`  
		Last Modified: Tue, 13 Oct 2020 08:05:39 GMT  
		Size: 112.5 MB (112486256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:164ef92f3887884a8e93d96f0a4cdfe88912f0dc4a257b857c1aa63c7ee5e00f`  
		Last Modified: Tue, 13 Oct 2020 08:05:16 GMT  
		Size: 843.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e4a6e666228dc751782155f2b3af56ed7c5e9ba56ef35c36f03587b6242065d`  
		Last Modified: Tue, 13 Oct 2020 08:05:16 GMT  
		Size: 5.1 KB (5145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45dea7731adeb126e6275444517123fc75f817c1949722f608d1eedef8ce475`  
		Last Modified: Tue, 13 Oct 2020 08:05:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
