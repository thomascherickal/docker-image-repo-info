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
$ docker pull mysql@sha256:1a2f9cd257e75cc80e9118b303d1648366bc2049101449bf2c8d82b022ea86b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:5` - linux; amd64

```console
$ docker pull mysql@sha256:1baaba81238a834281a4bafb088a44d07a0f845e30cd2f258dc61b046ee7b28e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.4 MB (154436843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09361feeb4753ac9da80ead4d46e2b21247712c13c9ee3f1e5d55630c64c544f`
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
# Wed, 23 Jun 2021 07:11:22 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Wed, 23 Jun 2021 07:12:02 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 23 Jun 2021 07:12:02 GMT
ENV MYSQL_VERSION=5.7.34-1debian10
# Wed, 23 Jun 2021 07:12:03 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Wed, 23 Jun 2021 07:12:28 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 23 Jun 2021 07:12:29 GMT
VOLUME [/var/lib/mysql]
# Wed, 23 Jun 2021 07:12:29 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Wed, 23 Jun 2021 07:12:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 23 Jun 2021 07:12:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 07:12:31 GMT
EXPOSE 3306 33060
# Wed, 23 Jun 2021 07:12:31 GMT
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
	-	`sha256:32ca814c833fbe8adec28e15d739dba772d7259021235b861fb854e8f329fb1c`  
		Last Modified: Wed, 23 Jun 2021 07:13:55 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52645b4af634738ab63ab41856f3e3babec551cd79a9453cc1490f74357265dc`  
		Last Modified: Wed, 23 Jun 2021 07:14:40 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bca6a5b14385af5335ab69e01305076737b8ff8356a2dd3681e97710353bd01c`  
		Last Modified: Wed, 23 Jun 2021 07:15:00 GMT  
		Size: 108.2 MB (108234830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:309f36297c759911f01981e749d779712c95d4996a82a4374fe2333f1cd91331`  
		Last Modified: Wed, 23 Jun 2021 07:14:40 GMT  
		Size: 5.5 KB (5540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d75cacde0f8c9d53fd35442b5c5a829d8449e85f11770a8da376e4f228b8e26`  
		Last Modified: Wed, 23 Jun 2021 07:14:40 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.6`

```console
$ docker pull mysql@sha256:879efe96447702f18945f10607e736b844ebe9cfef6f29c7a47f6b972212a81e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:5.6` - linux; amd64

```console
$ docker pull mysql@sha256:34b1cd56edbc8353a209f9675675f4d0b7ba0c36bcb448d5b2353733f7ee491c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.0 MB (102970877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1aa75e199d732c5feafe63423fba732a35ba75d9b7ecce14df3043c14f3a066`
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
# Wed, 23 Jun 2021 07:13:13 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Wed, 23 Jun 2021 07:13:13 GMT
ENV MYSQL_MAJOR=5.6
# Wed, 23 Jun 2021 07:13:13 GMT
ENV MYSQL_VERSION=5.6.51-1debian9
# Wed, 23 Jun 2021 07:13:14 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ stretch mysql-5.6' > /etc/apt/sources.list.d/mysql.list
# Wed, 23 Jun 2021 07:13:32 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 23 Jun 2021 07:13:33 GMT
VOLUME [/var/lib/mysql]
# Wed, 23 Jun 2021 07:13:33 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Wed, 23 Jun 2021 07:13:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 23 Jun 2021 07:13:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 07:13:35 GMT
EXPOSE 3306
# Wed, 23 Jun 2021 07:13:35 GMT
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
	-	`sha256:9bd9276345f70b788c1f3600e0fbf591df3dbbdb2c855e9b47521a8402184130`  
		Last Modified: Wed, 23 Jun 2021 07:15:15 GMT  
		Size: 19.5 KB (19457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d2d48bdf8e326d70aeeddfa4a78cdf5d30bf1a75a1abef21f44ce6084745d3b`  
		Last Modified: Wed, 23 Jun 2021 07:15:15 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8b3b343d10ae7acad6a2c49e119b57ec3177e26a17cc50b2c50fddf207fb81`  
		Last Modified: Wed, 23 Jun 2021 07:15:30 GMT  
		Size: 64.3 MB (64274391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3efd105a920df3b059b5ccca3a8920b802d485fa7486a00b7493fb028d72685`  
		Last Modified: Wed, 23 Jun 2021 07:15:15 GMT  
		Size: 5.6 KB (5556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d4864c82f8a583b4ea48f17a5e15706a7e01e32a55470a02ecfee752090cc5f`  
		Last Modified: Wed, 23 Jun 2021 07:15:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.6.51`

```console
$ docker pull mysql@sha256:879efe96447702f18945f10607e736b844ebe9cfef6f29c7a47f6b972212a81e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:5.6.51` - linux; amd64

```console
$ docker pull mysql@sha256:34b1cd56edbc8353a209f9675675f4d0b7ba0c36bcb448d5b2353733f7ee491c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.0 MB (102970877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1aa75e199d732c5feafe63423fba732a35ba75d9b7ecce14df3043c14f3a066`
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
# Wed, 23 Jun 2021 07:13:13 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Wed, 23 Jun 2021 07:13:13 GMT
ENV MYSQL_MAJOR=5.6
# Wed, 23 Jun 2021 07:13:13 GMT
ENV MYSQL_VERSION=5.6.51-1debian9
# Wed, 23 Jun 2021 07:13:14 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ stretch mysql-5.6' > /etc/apt/sources.list.d/mysql.list
# Wed, 23 Jun 2021 07:13:32 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 23 Jun 2021 07:13:33 GMT
VOLUME [/var/lib/mysql]
# Wed, 23 Jun 2021 07:13:33 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Wed, 23 Jun 2021 07:13:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 23 Jun 2021 07:13:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 07:13:35 GMT
EXPOSE 3306
# Wed, 23 Jun 2021 07:13:35 GMT
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
	-	`sha256:9bd9276345f70b788c1f3600e0fbf591df3dbbdb2c855e9b47521a8402184130`  
		Last Modified: Wed, 23 Jun 2021 07:15:15 GMT  
		Size: 19.5 KB (19457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d2d48bdf8e326d70aeeddfa4a78cdf5d30bf1a75a1abef21f44ce6084745d3b`  
		Last Modified: Wed, 23 Jun 2021 07:15:15 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8b3b343d10ae7acad6a2c49e119b57ec3177e26a17cc50b2c50fddf207fb81`  
		Last Modified: Wed, 23 Jun 2021 07:15:30 GMT  
		Size: 64.3 MB (64274391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3efd105a920df3b059b5ccca3a8920b802d485fa7486a00b7493fb028d72685`  
		Last Modified: Wed, 23 Jun 2021 07:15:15 GMT  
		Size: 5.6 KB (5556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d4864c82f8a583b4ea48f17a5e15706a7e01e32a55470a02ecfee752090cc5f`  
		Last Modified: Wed, 23 Jun 2021 07:15:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7`

```console
$ docker pull mysql@sha256:1a2f9cd257e75cc80e9118b303d1648366bc2049101449bf2c8d82b022ea86b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:5.7` - linux; amd64

```console
$ docker pull mysql@sha256:1baaba81238a834281a4bafb088a44d07a0f845e30cd2f258dc61b046ee7b28e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.4 MB (154436843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09361feeb4753ac9da80ead4d46e2b21247712c13c9ee3f1e5d55630c64c544f`
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
# Wed, 23 Jun 2021 07:11:22 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Wed, 23 Jun 2021 07:12:02 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 23 Jun 2021 07:12:02 GMT
ENV MYSQL_VERSION=5.7.34-1debian10
# Wed, 23 Jun 2021 07:12:03 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Wed, 23 Jun 2021 07:12:28 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 23 Jun 2021 07:12:29 GMT
VOLUME [/var/lib/mysql]
# Wed, 23 Jun 2021 07:12:29 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Wed, 23 Jun 2021 07:12:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 23 Jun 2021 07:12:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 07:12:31 GMT
EXPOSE 3306 33060
# Wed, 23 Jun 2021 07:12:31 GMT
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
	-	`sha256:32ca814c833fbe8adec28e15d739dba772d7259021235b861fb854e8f329fb1c`  
		Last Modified: Wed, 23 Jun 2021 07:13:55 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52645b4af634738ab63ab41856f3e3babec551cd79a9453cc1490f74357265dc`  
		Last Modified: Wed, 23 Jun 2021 07:14:40 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bca6a5b14385af5335ab69e01305076737b8ff8356a2dd3681e97710353bd01c`  
		Last Modified: Wed, 23 Jun 2021 07:15:00 GMT  
		Size: 108.2 MB (108234830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:309f36297c759911f01981e749d779712c95d4996a82a4374fe2333f1cd91331`  
		Last Modified: Wed, 23 Jun 2021 07:14:40 GMT  
		Size: 5.5 KB (5540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d75cacde0f8c9d53fd35442b5c5a829d8449e85f11770a8da376e4f228b8e26`  
		Last Modified: Wed, 23 Jun 2021 07:14:40 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.34`

```console
$ docker pull mysql@sha256:1a2f9cd257e75cc80e9118b303d1648366bc2049101449bf2c8d82b022ea86b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:5.7.34` - linux; amd64

```console
$ docker pull mysql@sha256:1baaba81238a834281a4bafb088a44d07a0f845e30cd2f258dc61b046ee7b28e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.4 MB (154436843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09361feeb4753ac9da80ead4d46e2b21247712c13c9ee3f1e5d55630c64c544f`
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
# Wed, 23 Jun 2021 07:11:22 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Wed, 23 Jun 2021 07:12:02 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 23 Jun 2021 07:12:02 GMT
ENV MYSQL_VERSION=5.7.34-1debian10
# Wed, 23 Jun 2021 07:12:03 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Wed, 23 Jun 2021 07:12:28 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 23 Jun 2021 07:12:29 GMT
VOLUME [/var/lib/mysql]
# Wed, 23 Jun 2021 07:12:29 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Wed, 23 Jun 2021 07:12:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 23 Jun 2021 07:12:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 07:12:31 GMT
EXPOSE 3306 33060
# Wed, 23 Jun 2021 07:12:31 GMT
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
	-	`sha256:32ca814c833fbe8adec28e15d739dba772d7259021235b861fb854e8f329fb1c`  
		Last Modified: Wed, 23 Jun 2021 07:13:55 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52645b4af634738ab63ab41856f3e3babec551cd79a9453cc1490f74357265dc`  
		Last Modified: Wed, 23 Jun 2021 07:14:40 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bca6a5b14385af5335ab69e01305076737b8ff8356a2dd3681e97710353bd01c`  
		Last Modified: Wed, 23 Jun 2021 07:15:00 GMT  
		Size: 108.2 MB (108234830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:309f36297c759911f01981e749d779712c95d4996a82a4374fe2333f1cd91331`  
		Last Modified: Wed, 23 Jun 2021 07:14:40 GMT  
		Size: 5.5 KB (5540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d75cacde0f8c9d53fd35442b5c5a829d8449e85f11770a8da376e4f228b8e26`  
		Last Modified: Wed, 23 Jun 2021 07:14:40 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8`

```console
$ docker pull mysql@sha256:52b8406e4c32b8cf0557f1b74517e14c5393aff5cf0384eff62d9e81f4985d4b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:8` - linux; amd64

```console
$ docker pull mysql@sha256:c1afde725e2cfb627136a299b4d4bd35ae30a31fae1297dd2b3c3c951d9c7240
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.0 MB (162008495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c62e459e087e3bd3d963092b58e50ae2af881076b43c29e38e2b5db253e0287`
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
# Wed, 23 Jun 2021 07:11:22 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Wed, 23 Jun 2021 07:11:22 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 23 Jun 2021 07:11:23 GMT
ENV MYSQL_VERSION=8.0.25-1debian10
# Wed, 23 Jun 2021 07:11:24 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Wed, 23 Jun 2021 07:11:45 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 23 Jun 2021 07:11:45 GMT
VOLUME [/var/lib/mysql]
# Wed, 23 Jun 2021 07:11:46 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Wed, 23 Jun 2021 07:11:46 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Wed, 23 Jun 2021 07:11:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 23 Jun 2021 07:11:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 07:11:47 GMT
EXPOSE 3306 33060
# Wed, 23 Jun 2021 07:11:48 GMT
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
	-	`sha256:32ca814c833fbe8adec28e15d739dba772d7259021235b861fb854e8f329fb1c`  
		Last Modified: Wed, 23 Jun 2021 07:13:55 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ecc8abdb7f584bbbd11e6b16bf632440c4bc64cf9cccac3ee8202fcf17742d7`  
		Last Modified: Wed, 23 Jun 2021 07:13:53 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad042b682e0f0e2ef85b6822e1d40965a0018fb789e155b4f021193df776601a`  
		Last Modified: Wed, 23 Jun 2021 07:14:21 GMT  
		Size: 115.8 MB (115805637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71d327c6bb78193040178c6de8220df0d42f890e94efe76f2a8f2921ec9fd0c2`  
		Last Modified: Wed, 23 Jun 2021 07:13:53 GMT  
		Size: 842.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165d1d10a3fa620f7174db4439831e2e36e18f686c1adf80ccba1550dec2041a`  
		Last Modified: Wed, 23 Jun 2021 07:13:54 GMT  
		Size: 5.5 KB (5541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f40c47d0626e1a6f39b08da49fab43d8e392206a15e9952e3e4e87dcbbbf667`  
		Last Modified: Wed, 23 Jun 2021 07:13:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0`

```console
$ docker pull mysql@sha256:52b8406e4c32b8cf0557f1b74517e14c5393aff5cf0384eff62d9e81f4985d4b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:8.0` - linux; amd64

```console
$ docker pull mysql@sha256:c1afde725e2cfb627136a299b4d4bd35ae30a31fae1297dd2b3c3c951d9c7240
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.0 MB (162008495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c62e459e087e3bd3d963092b58e50ae2af881076b43c29e38e2b5db253e0287`
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
# Wed, 23 Jun 2021 07:11:22 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Wed, 23 Jun 2021 07:11:22 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 23 Jun 2021 07:11:23 GMT
ENV MYSQL_VERSION=8.0.25-1debian10
# Wed, 23 Jun 2021 07:11:24 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Wed, 23 Jun 2021 07:11:45 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 23 Jun 2021 07:11:45 GMT
VOLUME [/var/lib/mysql]
# Wed, 23 Jun 2021 07:11:46 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Wed, 23 Jun 2021 07:11:46 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Wed, 23 Jun 2021 07:11:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 23 Jun 2021 07:11:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 07:11:47 GMT
EXPOSE 3306 33060
# Wed, 23 Jun 2021 07:11:48 GMT
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
	-	`sha256:32ca814c833fbe8adec28e15d739dba772d7259021235b861fb854e8f329fb1c`  
		Last Modified: Wed, 23 Jun 2021 07:13:55 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ecc8abdb7f584bbbd11e6b16bf632440c4bc64cf9cccac3ee8202fcf17742d7`  
		Last Modified: Wed, 23 Jun 2021 07:13:53 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad042b682e0f0e2ef85b6822e1d40965a0018fb789e155b4f021193df776601a`  
		Last Modified: Wed, 23 Jun 2021 07:14:21 GMT  
		Size: 115.8 MB (115805637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71d327c6bb78193040178c6de8220df0d42f890e94efe76f2a8f2921ec9fd0c2`  
		Last Modified: Wed, 23 Jun 2021 07:13:53 GMT  
		Size: 842.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165d1d10a3fa620f7174db4439831e2e36e18f686c1adf80ccba1550dec2041a`  
		Last Modified: Wed, 23 Jun 2021 07:13:54 GMT  
		Size: 5.5 KB (5541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f40c47d0626e1a6f39b08da49fab43d8e392206a15e9952e3e4e87dcbbbf667`  
		Last Modified: Wed, 23 Jun 2021 07:13:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.25`

```console
$ docker pull mysql@sha256:52b8406e4c32b8cf0557f1b74517e14c5393aff5cf0384eff62d9e81f4985d4b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:8.0.25` - linux; amd64

```console
$ docker pull mysql@sha256:c1afde725e2cfb627136a299b4d4bd35ae30a31fae1297dd2b3c3c951d9c7240
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.0 MB (162008495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c62e459e087e3bd3d963092b58e50ae2af881076b43c29e38e2b5db253e0287`
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
# Wed, 23 Jun 2021 07:11:22 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Wed, 23 Jun 2021 07:11:22 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 23 Jun 2021 07:11:23 GMT
ENV MYSQL_VERSION=8.0.25-1debian10
# Wed, 23 Jun 2021 07:11:24 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Wed, 23 Jun 2021 07:11:45 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 23 Jun 2021 07:11:45 GMT
VOLUME [/var/lib/mysql]
# Wed, 23 Jun 2021 07:11:46 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Wed, 23 Jun 2021 07:11:46 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Wed, 23 Jun 2021 07:11:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 23 Jun 2021 07:11:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 07:11:47 GMT
EXPOSE 3306 33060
# Wed, 23 Jun 2021 07:11:48 GMT
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
	-	`sha256:32ca814c833fbe8adec28e15d739dba772d7259021235b861fb854e8f329fb1c`  
		Last Modified: Wed, 23 Jun 2021 07:13:55 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ecc8abdb7f584bbbd11e6b16bf632440c4bc64cf9cccac3ee8202fcf17742d7`  
		Last Modified: Wed, 23 Jun 2021 07:13:53 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad042b682e0f0e2ef85b6822e1d40965a0018fb789e155b4f021193df776601a`  
		Last Modified: Wed, 23 Jun 2021 07:14:21 GMT  
		Size: 115.8 MB (115805637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71d327c6bb78193040178c6de8220df0d42f890e94efe76f2a8f2921ec9fd0c2`  
		Last Modified: Wed, 23 Jun 2021 07:13:53 GMT  
		Size: 842.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165d1d10a3fa620f7174db4439831e2e36e18f686c1adf80ccba1550dec2041a`  
		Last Modified: Wed, 23 Jun 2021 07:13:54 GMT  
		Size: 5.5 KB (5541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f40c47d0626e1a6f39b08da49fab43d8e392206a15e9952e3e4e87dcbbbf667`  
		Last Modified: Wed, 23 Jun 2021 07:13:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:latest`

```console
$ docker pull mysql@sha256:52b8406e4c32b8cf0557f1b74517e14c5393aff5cf0384eff62d9e81f4985d4b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:latest` - linux; amd64

```console
$ docker pull mysql@sha256:c1afde725e2cfb627136a299b4d4bd35ae30a31fae1297dd2b3c3c951d9c7240
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.0 MB (162008495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c62e459e087e3bd3d963092b58e50ae2af881076b43c29e38e2b5db253e0287`
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
# Wed, 23 Jun 2021 07:11:22 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Wed, 23 Jun 2021 07:11:22 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 23 Jun 2021 07:11:23 GMT
ENV MYSQL_VERSION=8.0.25-1debian10
# Wed, 23 Jun 2021 07:11:24 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Wed, 23 Jun 2021 07:11:45 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 23 Jun 2021 07:11:45 GMT
VOLUME [/var/lib/mysql]
# Wed, 23 Jun 2021 07:11:46 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Wed, 23 Jun 2021 07:11:46 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Wed, 23 Jun 2021 07:11:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 23 Jun 2021 07:11:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 07:11:47 GMT
EXPOSE 3306 33060
# Wed, 23 Jun 2021 07:11:48 GMT
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
	-	`sha256:32ca814c833fbe8adec28e15d739dba772d7259021235b861fb854e8f329fb1c`  
		Last Modified: Wed, 23 Jun 2021 07:13:55 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ecc8abdb7f584bbbd11e6b16bf632440c4bc64cf9cccac3ee8202fcf17742d7`  
		Last Modified: Wed, 23 Jun 2021 07:13:53 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad042b682e0f0e2ef85b6822e1d40965a0018fb789e155b4f021193df776601a`  
		Last Modified: Wed, 23 Jun 2021 07:14:21 GMT  
		Size: 115.8 MB (115805637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71d327c6bb78193040178c6de8220df0d42f890e94efe76f2a8f2921ec9fd0c2`  
		Last Modified: Wed, 23 Jun 2021 07:13:53 GMT  
		Size: 842.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165d1d10a3fa620f7174db4439831e2e36e18f686c1adf80ccba1550dec2041a`  
		Last Modified: Wed, 23 Jun 2021 07:13:54 GMT  
		Size: 5.5 KB (5541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f40c47d0626e1a6f39b08da49fab43d8e392206a15e9952e3e4e87dcbbbf667`  
		Last Modified: Wed, 23 Jun 2021 07:13:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
