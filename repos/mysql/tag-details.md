<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mysql`

-	[`mysql:5`](#mysql5)
-	[`mysql:5.6`](#mysql56)
-	[`mysql:5.6.51`](#mysql5651)
-	[`mysql:5.7`](#mysql57)
-	[`mysql:5.7.36`](#mysql5736)
-	[`mysql:8`](#mysql8)
-	[`mysql:8.0`](#mysql80)
-	[`mysql:8.0.27`](#mysql8027)
-	[`mysql:latest`](#mysqllatest)

## `mysql:5`

```console
$ docker pull mysql@sha256:f2ad209efe9c67104167fc609cca6973c8422939491c9345270175a300419f94
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5` - linux; amd64

```console
$ docker pull mysql@sha256:398f124948bb3d5789c0ac7c004d02e6d9a3ae95aa9804d7a3b33a344ff3c9cd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.8 MB (154848834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c20987f18b130f9d144c9828df630417e2a9523148930dc3963e9d0dab302a76`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:04 GMT
ADD file:bd5c9e0e0145fe33beee9d73615cc89b5c5459bb84ea164cb1bbd8c999f0c2e4 in / 
# Tue, 21 Dec 2021 01:23:04 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:55:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 21 Dec 2021 02:55:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:55:11 GMT
ENV GOSU_VERSION=1.12
# Tue, 21 Dec 2021 02:55:25 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 21 Dec 2021 02:55:26 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 21 Dec 2021 02:55:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:55:43 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Tue, 21 Dec 2021 02:56:24 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 21 Dec 2021 02:56:24 GMT
ENV MYSQL_VERSION=5.7.36-1debian10
# Tue, 21 Dec 2021 02:56:25 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Tue, 21 Dec 2021 02:56:48 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 21 Dec 2021 02:56:48 GMT
VOLUME [/var/lib/mysql]
# Tue, 21 Dec 2021 02:56:49 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Tue, 21 Dec 2021 02:56:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 21 Dec 2021 02:56:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Dec 2021 02:56:51 GMT
EXPOSE 3306 33060
# Tue, 21 Dec 2021 02:56:51 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:72a69066d2febc34d8f3dbcb645f7b851a57e9681322ece7ad8007503b783c19`  
		Last Modified: Tue, 21 Dec 2021 01:28:32 GMT  
		Size: 27.2 MB (27153723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93619dbc5b36fe839e30a055a373bb628be3c22109abcb483cc56c8dd5f8cf47`  
		Last Modified: Tue, 21 Dec 2021 02:58:24 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99da31dd61422c9b6ce417b189ebaf568e6cfa7a5343f7db4ad7c2ae2127a238`  
		Last Modified: Tue, 21 Dec 2021 02:58:25 GMT  
		Size: 4.2 MB (4179263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:626033c43d70213ba8a5f8738ef13f6fffde083a431217d2e183fb345bade8ba`  
		Last Modified: Tue, 21 Dec 2021 02:58:22 GMT  
		Size: 1.4 MB (1419422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d5d7efb64ee4d2f6936691bb9383c64ba1ac7ad302e1be0c6417f6f9611ef4`  
		Last Modified: Tue, 21 Dec 2021 02:58:21 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac563158d7217088d06b716be9ea5131fe1ae47572467fbbdfb1031487b9957a`  
		Last Modified: Tue, 21 Dec 2021 02:58:25 GMT  
		Size: 13.4 MB (13448691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ba16033dad96fe979d13da439d5902ea33f7d3d6c0da94adf0a8e9e5de2c01`  
		Last Modified: Tue, 21 Dec 2021 02:58:22 GMT  
		Size: 1.9 KB (1877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ceb82207cd70dc0f91620ef1cac7c4c1f8b4eb64cd0868852f0ef5afd261fdf`  
		Last Modified: Tue, 21 Dec 2021 02:58:57 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37f2405cae96cfa4335b4dd266b26647eecbbe8236493d4deb595976e543815e`  
		Last Modified: Tue, 21 Dec 2021 02:59:18 GMT  
		Size: 108.6 MB (108638087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2482e017e53874be685cb8d4a43e70895376ed1dc71ab313d88eb1e154feda9`  
		Last Modified: Tue, 21 Dec 2021 02:58:57 GMT  
		Size: 5.5 KB (5543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70deed891d42e8d9ee11ee4f191b83e08496711d3a90328f70ec8ac681aab6dd`  
		Last Modified: Tue, 21 Dec 2021 02:58:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.6`

```console
$ docker pull mysql@sha256:20575ecebe6216036d25dab5903808211f1e9ba63dc7825ac20cb975e34cfcae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.6` - linux; amd64

```console
$ docker pull mysql@sha256:897086d07d1efa876224b147397ea8d3147e61dd84dce963aace1d5e9dc2802d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.0 MB (102974094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd3b2a5dcb48ff61113592ed5ddd762581be4387c7bc552375a2159422aa6bf5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 21 Dec 2021 01:24:41 GMT
ADD file:b1650c19c1dd1f4cff71553f2bb0bc949944d0bc24b54c318b2880c14538648a in / 
# Tue, 21 Dec 2021 01:24:42 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:56:59 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 21 Dec 2021 02:57:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:57:05 GMT
ENV GOSU_VERSION=1.12
# Tue, 21 Dec 2021 02:57:18 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 21 Dec 2021 02:57:19 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 21 Dec 2021 02:57:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:57:37 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Tue, 21 Dec 2021 02:57:37 GMT
ENV MYSQL_MAJOR=5.6
# Tue, 21 Dec 2021 02:57:38 GMT
ENV MYSQL_VERSION=5.6.51-1debian9
# Tue, 21 Dec 2021 02:57:39 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ stretch mysql-5.6' > /etc/apt/sources.list.d/mysql.list
# Tue, 21 Dec 2021 02:57:56 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 21 Dec 2021 02:57:57 GMT
VOLUME [/var/lib/mysql]
# Tue, 21 Dec 2021 02:57:57 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Tue, 21 Dec 2021 02:57:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 21 Dec 2021 02:57:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Dec 2021 02:57:59 GMT
EXPOSE 3306
# Tue, 21 Dec 2021 02:57:59 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:35b2232c987ef3e6249ed229afcca51cd83320e08f6700022f4a3644a11f00f2`  
		Last Modified: Tue, 21 Dec 2021 01:31:36 GMT  
		Size: 22.5 MB (22529141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc55c00e48f2fdde6d83ae9d26de0ad33b91d6861f3e6f356633922f00ca33e0`  
		Last Modified: Tue, 21 Dec 2021 02:59:38 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0030405130e3a248f40e6465e6667e3926cb8b0a8f7e558772ca6a0c58ea9c0e`  
		Last Modified: Tue, 21 Dec 2021 02:59:38 GMT  
		Size: 4.5 MB (4503801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1fef7f6a8d192093b8b7c303388112ca9ace69c45690f801dedb435bb4d1327`  
		Last Modified: Tue, 21 Dec 2021 02:59:37 GMT  
		Size: 1.4 MB (1412167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c76272398bb61b196a14a8eacdee77dd3337638b3eddf3815107fa6fdb507e6`  
		Last Modified: Tue, 21 Dec 2021 02:59:36 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f57e698171b646d432b1ffdf81ea1983278fe79ff560e5a1d12ccf0fe15bdd3d`  
		Last Modified: Tue, 21 Dec 2021 02:59:40 GMT  
		Size: 10.2 MB (10225707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b825b269c0c5e254d28469fcd84eeab4d9eff0817bf38562ec1a1529b3f29c`  
		Last Modified: Tue, 21 Dec 2021 02:59:32 GMT  
		Size: 21.2 KB (21181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcb0af686073bf5f2a8f12afa8fcb2c73866ec7465d0fe67c08f5146f9aa186c`  
		Last Modified: Tue, 21 Dec 2021 02:59:33 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bbfeb886d15ce8628fc7b6e1ac047287dde0863e0ae1e01f61e61390742740`  
		Last Modified: Tue, 21 Dec 2021 02:59:46 GMT  
		Size: 64.3 MB (64274301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f70cc8681456d52b0c4c2d10571c2919c14afc8218ba68428197aa298fd3c5f`  
		Last Modified: Tue, 21 Dec 2021 02:59:32 GMT  
		Size: 5.6 KB (5560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6637f4600d1512fddfb02f66b02d932c7ee19ff9be05398a117af5eb1cbfda`  
		Last Modified: Tue, 21 Dec 2021 02:59:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.6.51`

```console
$ docker pull mysql@sha256:20575ecebe6216036d25dab5903808211f1e9ba63dc7825ac20cb975e34cfcae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.6.51` - linux; amd64

```console
$ docker pull mysql@sha256:897086d07d1efa876224b147397ea8d3147e61dd84dce963aace1d5e9dc2802d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.0 MB (102974094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd3b2a5dcb48ff61113592ed5ddd762581be4387c7bc552375a2159422aa6bf5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 21 Dec 2021 01:24:41 GMT
ADD file:b1650c19c1dd1f4cff71553f2bb0bc949944d0bc24b54c318b2880c14538648a in / 
# Tue, 21 Dec 2021 01:24:42 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:56:59 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 21 Dec 2021 02:57:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:57:05 GMT
ENV GOSU_VERSION=1.12
# Tue, 21 Dec 2021 02:57:18 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 21 Dec 2021 02:57:19 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 21 Dec 2021 02:57:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:57:37 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Tue, 21 Dec 2021 02:57:37 GMT
ENV MYSQL_MAJOR=5.6
# Tue, 21 Dec 2021 02:57:38 GMT
ENV MYSQL_VERSION=5.6.51-1debian9
# Tue, 21 Dec 2021 02:57:39 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ stretch mysql-5.6' > /etc/apt/sources.list.d/mysql.list
# Tue, 21 Dec 2021 02:57:56 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 21 Dec 2021 02:57:57 GMT
VOLUME [/var/lib/mysql]
# Tue, 21 Dec 2021 02:57:57 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Tue, 21 Dec 2021 02:57:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 21 Dec 2021 02:57:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Dec 2021 02:57:59 GMT
EXPOSE 3306
# Tue, 21 Dec 2021 02:57:59 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:35b2232c987ef3e6249ed229afcca51cd83320e08f6700022f4a3644a11f00f2`  
		Last Modified: Tue, 21 Dec 2021 01:31:36 GMT  
		Size: 22.5 MB (22529141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc55c00e48f2fdde6d83ae9d26de0ad33b91d6861f3e6f356633922f00ca33e0`  
		Last Modified: Tue, 21 Dec 2021 02:59:38 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0030405130e3a248f40e6465e6667e3926cb8b0a8f7e558772ca6a0c58ea9c0e`  
		Last Modified: Tue, 21 Dec 2021 02:59:38 GMT  
		Size: 4.5 MB (4503801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1fef7f6a8d192093b8b7c303388112ca9ace69c45690f801dedb435bb4d1327`  
		Last Modified: Tue, 21 Dec 2021 02:59:37 GMT  
		Size: 1.4 MB (1412167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c76272398bb61b196a14a8eacdee77dd3337638b3eddf3815107fa6fdb507e6`  
		Last Modified: Tue, 21 Dec 2021 02:59:36 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f57e698171b646d432b1ffdf81ea1983278fe79ff560e5a1d12ccf0fe15bdd3d`  
		Last Modified: Tue, 21 Dec 2021 02:59:40 GMT  
		Size: 10.2 MB (10225707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b825b269c0c5e254d28469fcd84eeab4d9eff0817bf38562ec1a1529b3f29c`  
		Last Modified: Tue, 21 Dec 2021 02:59:32 GMT  
		Size: 21.2 KB (21181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcb0af686073bf5f2a8f12afa8fcb2c73866ec7465d0fe67c08f5146f9aa186c`  
		Last Modified: Tue, 21 Dec 2021 02:59:33 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bbfeb886d15ce8628fc7b6e1ac047287dde0863e0ae1e01f61e61390742740`  
		Last Modified: Tue, 21 Dec 2021 02:59:46 GMT  
		Size: 64.3 MB (64274301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f70cc8681456d52b0c4c2d10571c2919c14afc8218ba68428197aa298fd3c5f`  
		Last Modified: Tue, 21 Dec 2021 02:59:32 GMT  
		Size: 5.6 KB (5560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6637f4600d1512fddfb02f66b02d932c7ee19ff9be05398a117af5eb1cbfda`  
		Last Modified: Tue, 21 Dec 2021 02:59:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7`

```console
$ docker pull mysql@sha256:f2ad209efe9c67104167fc609cca6973c8422939491c9345270175a300419f94
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7` - linux; amd64

```console
$ docker pull mysql@sha256:398f124948bb3d5789c0ac7c004d02e6d9a3ae95aa9804d7a3b33a344ff3c9cd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.8 MB (154848834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c20987f18b130f9d144c9828df630417e2a9523148930dc3963e9d0dab302a76`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:04 GMT
ADD file:bd5c9e0e0145fe33beee9d73615cc89b5c5459bb84ea164cb1bbd8c999f0c2e4 in / 
# Tue, 21 Dec 2021 01:23:04 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:55:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 21 Dec 2021 02:55:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:55:11 GMT
ENV GOSU_VERSION=1.12
# Tue, 21 Dec 2021 02:55:25 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 21 Dec 2021 02:55:26 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 21 Dec 2021 02:55:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:55:43 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Tue, 21 Dec 2021 02:56:24 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 21 Dec 2021 02:56:24 GMT
ENV MYSQL_VERSION=5.7.36-1debian10
# Tue, 21 Dec 2021 02:56:25 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Tue, 21 Dec 2021 02:56:48 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 21 Dec 2021 02:56:48 GMT
VOLUME [/var/lib/mysql]
# Tue, 21 Dec 2021 02:56:49 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Tue, 21 Dec 2021 02:56:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 21 Dec 2021 02:56:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Dec 2021 02:56:51 GMT
EXPOSE 3306 33060
# Tue, 21 Dec 2021 02:56:51 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:72a69066d2febc34d8f3dbcb645f7b851a57e9681322ece7ad8007503b783c19`  
		Last Modified: Tue, 21 Dec 2021 01:28:32 GMT  
		Size: 27.2 MB (27153723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93619dbc5b36fe839e30a055a373bb628be3c22109abcb483cc56c8dd5f8cf47`  
		Last Modified: Tue, 21 Dec 2021 02:58:24 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99da31dd61422c9b6ce417b189ebaf568e6cfa7a5343f7db4ad7c2ae2127a238`  
		Last Modified: Tue, 21 Dec 2021 02:58:25 GMT  
		Size: 4.2 MB (4179263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:626033c43d70213ba8a5f8738ef13f6fffde083a431217d2e183fb345bade8ba`  
		Last Modified: Tue, 21 Dec 2021 02:58:22 GMT  
		Size: 1.4 MB (1419422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d5d7efb64ee4d2f6936691bb9383c64ba1ac7ad302e1be0c6417f6f9611ef4`  
		Last Modified: Tue, 21 Dec 2021 02:58:21 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac563158d7217088d06b716be9ea5131fe1ae47572467fbbdfb1031487b9957a`  
		Last Modified: Tue, 21 Dec 2021 02:58:25 GMT  
		Size: 13.4 MB (13448691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ba16033dad96fe979d13da439d5902ea33f7d3d6c0da94adf0a8e9e5de2c01`  
		Last Modified: Tue, 21 Dec 2021 02:58:22 GMT  
		Size: 1.9 KB (1877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ceb82207cd70dc0f91620ef1cac7c4c1f8b4eb64cd0868852f0ef5afd261fdf`  
		Last Modified: Tue, 21 Dec 2021 02:58:57 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37f2405cae96cfa4335b4dd266b26647eecbbe8236493d4deb595976e543815e`  
		Last Modified: Tue, 21 Dec 2021 02:59:18 GMT  
		Size: 108.6 MB (108638087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2482e017e53874be685cb8d4a43e70895376ed1dc71ab313d88eb1e154feda9`  
		Last Modified: Tue, 21 Dec 2021 02:58:57 GMT  
		Size: 5.5 KB (5543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70deed891d42e8d9ee11ee4f191b83e08496711d3a90328f70ec8ac681aab6dd`  
		Last Modified: Tue, 21 Dec 2021 02:58:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.36`

```console
$ docker pull mysql@sha256:f2ad209efe9c67104167fc609cca6973c8422939491c9345270175a300419f94
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.36` - linux; amd64

```console
$ docker pull mysql@sha256:398f124948bb3d5789c0ac7c004d02e6d9a3ae95aa9804d7a3b33a344ff3c9cd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.8 MB (154848834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c20987f18b130f9d144c9828df630417e2a9523148930dc3963e9d0dab302a76`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:04 GMT
ADD file:bd5c9e0e0145fe33beee9d73615cc89b5c5459bb84ea164cb1bbd8c999f0c2e4 in / 
# Tue, 21 Dec 2021 01:23:04 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:55:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 21 Dec 2021 02:55:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:55:11 GMT
ENV GOSU_VERSION=1.12
# Tue, 21 Dec 2021 02:55:25 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 21 Dec 2021 02:55:26 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 21 Dec 2021 02:55:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:55:43 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Tue, 21 Dec 2021 02:56:24 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 21 Dec 2021 02:56:24 GMT
ENV MYSQL_VERSION=5.7.36-1debian10
# Tue, 21 Dec 2021 02:56:25 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Tue, 21 Dec 2021 02:56:48 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 21 Dec 2021 02:56:48 GMT
VOLUME [/var/lib/mysql]
# Tue, 21 Dec 2021 02:56:49 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Tue, 21 Dec 2021 02:56:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 21 Dec 2021 02:56:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Dec 2021 02:56:51 GMT
EXPOSE 3306 33060
# Tue, 21 Dec 2021 02:56:51 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:72a69066d2febc34d8f3dbcb645f7b851a57e9681322ece7ad8007503b783c19`  
		Last Modified: Tue, 21 Dec 2021 01:28:32 GMT  
		Size: 27.2 MB (27153723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93619dbc5b36fe839e30a055a373bb628be3c22109abcb483cc56c8dd5f8cf47`  
		Last Modified: Tue, 21 Dec 2021 02:58:24 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99da31dd61422c9b6ce417b189ebaf568e6cfa7a5343f7db4ad7c2ae2127a238`  
		Last Modified: Tue, 21 Dec 2021 02:58:25 GMT  
		Size: 4.2 MB (4179263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:626033c43d70213ba8a5f8738ef13f6fffde083a431217d2e183fb345bade8ba`  
		Last Modified: Tue, 21 Dec 2021 02:58:22 GMT  
		Size: 1.4 MB (1419422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d5d7efb64ee4d2f6936691bb9383c64ba1ac7ad302e1be0c6417f6f9611ef4`  
		Last Modified: Tue, 21 Dec 2021 02:58:21 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac563158d7217088d06b716be9ea5131fe1ae47572467fbbdfb1031487b9957a`  
		Last Modified: Tue, 21 Dec 2021 02:58:25 GMT  
		Size: 13.4 MB (13448691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ba16033dad96fe979d13da439d5902ea33f7d3d6c0da94adf0a8e9e5de2c01`  
		Last Modified: Tue, 21 Dec 2021 02:58:22 GMT  
		Size: 1.9 KB (1877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ceb82207cd70dc0f91620ef1cac7c4c1f8b4eb64cd0868852f0ef5afd261fdf`  
		Last Modified: Tue, 21 Dec 2021 02:58:57 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37f2405cae96cfa4335b4dd266b26647eecbbe8236493d4deb595976e543815e`  
		Last Modified: Tue, 21 Dec 2021 02:59:18 GMT  
		Size: 108.6 MB (108638087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2482e017e53874be685cb8d4a43e70895376ed1dc71ab313d88eb1e154feda9`  
		Last Modified: Tue, 21 Dec 2021 02:58:57 GMT  
		Size: 5.5 KB (5543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70deed891d42e8d9ee11ee4f191b83e08496711d3a90328f70ec8ac681aab6dd`  
		Last Modified: Tue, 21 Dec 2021 02:58:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8`

```console
$ docker pull mysql@sha256:e9027fe4d91c0153429607251656806cc784e914937271037f7738bd5b8e7709
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8` - linux; amd64

```console
$ docker pull mysql@sha256:238cf050a7270dd6940602e70f1e5a11eeaf4e02035f445b7f613ff5e0641f7d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.4 MB (151446222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3218b38490cec8d31976a40b92e09d61377359eab878db49f025e5d464367f3b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:04 GMT
ADD file:bd5c9e0e0145fe33beee9d73615cc89b5c5459bb84ea164cb1bbd8c999f0c2e4 in / 
# Tue, 21 Dec 2021 01:23:04 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:55:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 21 Dec 2021 02:55:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:55:11 GMT
ENV GOSU_VERSION=1.12
# Tue, 21 Dec 2021 02:55:25 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 21 Dec 2021 02:55:26 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 21 Dec 2021 02:55:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:55:43 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Tue, 21 Dec 2021 02:55:43 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 21 Dec 2021 02:55:44 GMT
ENV MYSQL_VERSION=8.0.27-1debian10
# Tue, 21 Dec 2021 02:55:45 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 21 Dec 2021 02:56:05 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 21 Dec 2021 02:56:06 GMT
VOLUME [/var/lib/mysql]
# Tue, 21 Dec 2021 02:56:06 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 21 Dec 2021 02:56:07 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Tue, 21 Dec 2021 02:56:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 21 Dec 2021 02:56:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Dec 2021 02:56:08 GMT
EXPOSE 3306 33060
# Tue, 21 Dec 2021 02:56:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:72a69066d2febc34d8f3dbcb645f7b851a57e9681322ece7ad8007503b783c19`  
		Last Modified: Tue, 21 Dec 2021 01:28:32 GMT  
		Size: 27.2 MB (27153723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93619dbc5b36fe839e30a055a373bb628be3c22109abcb483cc56c8dd5f8cf47`  
		Last Modified: Tue, 21 Dec 2021 02:58:24 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99da31dd61422c9b6ce417b189ebaf568e6cfa7a5343f7db4ad7c2ae2127a238`  
		Last Modified: Tue, 21 Dec 2021 02:58:25 GMT  
		Size: 4.2 MB (4179263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:626033c43d70213ba8a5f8738ef13f6fffde083a431217d2e183fb345bade8ba`  
		Last Modified: Tue, 21 Dec 2021 02:58:22 GMT  
		Size: 1.4 MB (1419422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d5d7efb64ee4d2f6936691bb9383c64ba1ac7ad302e1be0c6417f6f9611ef4`  
		Last Modified: Tue, 21 Dec 2021 02:58:21 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac563158d7217088d06b716be9ea5131fe1ae47572467fbbdfb1031487b9957a`  
		Last Modified: Tue, 21 Dec 2021 02:58:25 GMT  
		Size: 13.4 MB (13448691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ba16033dad96fe979d13da439d5902ea33f7d3d6c0da94adf0a8e9e5de2c01`  
		Last Modified: Tue, 21 Dec 2021 02:58:22 GMT  
		Size: 1.9 KB (1877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:688ba7d5c01a2d5cb0ceea200f87d4f61fe403e1d41f2dfb41a551b2c006de8e`  
		Last Modified: Tue, 21 Dec 2021 02:58:19 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00e060b6d11de571c49bf5d389e3e258da6da0c1e1a11cc17cbec19cc6512fab`  
		Last Modified: Tue, 21 Dec 2021 02:58:39 GMT  
		Size: 105.2 MB (105234633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c04857f594f227cbb0e45cf63fd21a5c3e68d517c97a93da529664dbfb00df3`  
		Last Modified: Tue, 21 Dec 2021 02:58:19 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d7cfa90e6eac8763a34d1ac5fa9a30dc66e609544193e3a762a7fe70ecd7474`  
		Last Modified: Tue, 21 Dec 2021 02:58:19 GMT  
		Size: 5.5 KB (5544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0431212d27dbfe76b4bf1e289533b28097d982b48834260c51aa3f488f7cd93`  
		Last Modified: Tue, 21 Dec 2021 02:58:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0`

```console
$ docker pull mysql@sha256:e9027fe4d91c0153429607251656806cc784e914937271037f7738bd5b8e7709
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0` - linux; amd64

```console
$ docker pull mysql@sha256:238cf050a7270dd6940602e70f1e5a11eeaf4e02035f445b7f613ff5e0641f7d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.4 MB (151446222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3218b38490cec8d31976a40b92e09d61377359eab878db49f025e5d464367f3b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:04 GMT
ADD file:bd5c9e0e0145fe33beee9d73615cc89b5c5459bb84ea164cb1bbd8c999f0c2e4 in / 
# Tue, 21 Dec 2021 01:23:04 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:55:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 21 Dec 2021 02:55:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:55:11 GMT
ENV GOSU_VERSION=1.12
# Tue, 21 Dec 2021 02:55:25 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 21 Dec 2021 02:55:26 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 21 Dec 2021 02:55:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:55:43 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Tue, 21 Dec 2021 02:55:43 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 21 Dec 2021 02:55:44 GMT
ENV MYSQL_VERSION=8.0.27-1debian10
# Tue, 21 Dec 2021 02:55:45 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 21 Dec 2021 02:56:05 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 21 Dec 2021 02:56:06 GMT
VOLUME [/var/lib/mysql]
# Tue, 21 Dec 2021 02:56:06 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 21 Dec 2021 02:56:07 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Tue, 21 Dec 2021 02:56:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 21 Dec 2021 02:56:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Dec 2021 02:56:08 GMT
EXPOSE 3306 33060
# Tue, 21 Dec 2021 02:56:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:72a69066d2febc34d8f3dbcb645f7b851a57e9681322ece7ad8007503b783c19`  
		Last Modified: Tue, 21 Dec 2021 01:28:32 GMT  
		Size: 27.2 MB (27153723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93619dbc5b36fe839e30a055a373bb628be3c22109abcb483cc56c8dd5f8cf47`  
		Last Modified: Tue, 21 Dec 2021 02:58:24 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99da31dd61422c9b6ce417b189ebaf568e6cfa7a5343f7db4ad7c2ae2127a238`  
		Last Modified: Tue, 21 Dec 2021 02:58:25 GMT  
		Size: 4.2 MB (4179263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:626033c43d70213ba8a5f8738ef13f6fffde083a431217d2e183fb345bade8ba`  
		Last Modified: Tue, 21 Dec 2021 02:58:22 GMT  
		Size: 1.4 MB (1419422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d5d7efb64ee4d2f6936691bb9383c64ba1ac7ad302e1be0c6417f6f9611ef4`  
		Last Modified: Tue, 21 Dec 2021 02:58:21 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac563158d7217088d06b716be9ea5131fe1ae47572467fbbdfb1031487b9957a`  
		Last Modified: Tue, 21 Dec 2021 02:58:25 GMT  
		Size: 13.4 MB (13448691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ba16033dad96fe979d13da439d5902ea33f7d3d6c0da94adf0a8e9e5de2c01`  
		Last Modified: Tue, 21 Dec 2021 02:58:22 GMT  
		Size: 1.9 KB (1877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:688ba7d5c01a2d5cb0ceea200f87d4f61fe403e1d41f2dfb41a551b2c006de8e`  
		Last Modified: Tue, 21 Dec 2021 02:58:19 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00e060b6d11de571c49bf5d389e3e258da6da0c1e1a11cc17cbec19cc6512fab`  
		Last Modified: Tue, 21 Dec 2021 02:58:39 GMT  
		Size: 105.2 MB (105234633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c04857f594f227cbb0e45cf63fd21a5c3e68d517c97a93da529664dbfb00df3`  
		Last Modified: Tue, 21 Dec 2021 02:58:19 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d7cfa90e6eac8763a34d1ac5fa9a30dc66e609544193e3a762a7fe70ecd7474`  
		Last Modified: Tue, 21 Dec 2021 02:58:19 GMT  
		Size: 5.5 KB (5544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0431212d27dbfe76b4bf1e289533b28097d982b48834260c51aa3f488f7cd93`  
		Last Modified: Tue, 21 Dec 2021 02:58:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.27`

```console
$ docker pull mysql@sha256:e9027fe4d91c0153429607251656806cc784e914937271037f7738bd5b8e7709
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0.27` - linux; amd64

```console
$ docker pull mysql@sha256:238cf050a7270dd6940602e70f1e5a11eeaf4e02035f445b7f613ff5e0641f7d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.4 MB (151446222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3218b38490cec8d31976a40b92e09d61377359eab878db49f025e5d464367f3b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:04 GMT
ADD file:bd5c9e0e0145fe33beee9d73615cc89b5c5459bb84ea164cb1bbd8c999f0c2e4 in / 
# Tue, 21 Dec 2021 01:23:04 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:55:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 21 Dec 2021 02:55:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:55:11 GMT
ENV GOSU_VERSION=1.12
# Tue, 21 Dec 2021 02:55:25 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 21 Dec 2021 02:55:26 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 21 Dec 2021 02:55:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:55:43 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Tue, 21 Dec 2021 02:55:43 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 21 Dec 2021 02:55:44 GMT
ENV MYSQL_VERSION=8.0.27-1debian10
# Tue, 21 Dec 2021 02:55:45 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 21 Dec 2021 02:56:05 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 21 Dec 2021 02:56:06 GMT
VOLUME [/var/lib/mysql]
# Tue, 21 Dec 2021 02:56:06 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 21 Dec 2021 02:56:07 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Tue, 21 Dec 2021 02:56:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 21 Dec 2021 02:56:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Dec 2021 02:56:08 GMT
EXPOSE 3306 33060
# Tue, 21 Dec 2021 02:56:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:72a69066d2febc34d8f3dbcb645f7b851a57e9681322ece7ad8007503b783c19`  
		Last Modified: Tue, 21 Dec 2021 01:28:32 GMT  
		Size: 27.2 MB (27153723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93619dbc5b36fe839e30a055a373bb628be3c22109abcb483cc56c8dd5f8cf47`  
		Last Modified: Tue, 21 Dec 2021 02:58:24 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99da31dd61422c9b6ce417b189ebaf568e6cfa7a5343f7db4ad7c2ae2127a238`  
		Last Modified: Tue, 21 Dec 2021 02:58:25 GMT  
		Size: 4.2 MB (4179263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:626033c43d70213ba8a5f8738ef13f6fffde083a431217d2e183fb345bade8ba`  
		Last Modified: Tue, 21 Dec 2021 02:58:22 GMT  
		Size: 1.4 MB (1419422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d5d7efb64ee4d2f6936691bb9383c64ba1ac7ad302e1be0c6417f6f9611ef4`  
		Last Modified: Tue, 21 Dec 2021 02:58:21 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac563158d7217088d06b716be9ea5131fe1ae47572467fbbdfb1031487b9957a`  
		Last Modified: Tue, 21 Dec 2021 02:58:25 GMT  
		Size: 13.4 MB (13448691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ba16033dad96fe979d13da439d5902ea33f7d3d6c0da94adf0a8e9e5de2c01`  
		Last Modified: Tue, 21 Dec 2021 02:58:22 GMT  
		Size: 1.9 KB (1877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:688ba7d5c01a2d5cb0ceea200f87d4f61fe403e1d41f2dfb41a551b2c006de8e`  
		Last Modified: Tue, 21 Dec 2021 02:58:19 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00e060b6d11de571c49bf5d389e3e258da6da0c1e1a11cc17cbec19cc6512fab`  
		Last Modified: Tue, 21 Dec 2021 02:58:39 GMT  
		Size: 105.2 MB (105234633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c04857f594f227cbb0e45cf63fd21a5c3e68d517c97a93da529664dbfb00df3`  
		Last Modified: Tue, 21 Dec 2021 02:58:19 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d7cfa90e6eac8763a34d1ac5fa9a30dc66e609544193e3a762a7fe70ecd7474`  
		Last Modified: Tue, 21 Dec 2021 02:58:19 GMT  
		Size: 5.5 KB (5544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0431212d27dbfe76b4bf1e289533b28097d982b48834260c51aa3f488f7cd93`  
		Last Modified: Tue, 21 Dec 2021 02:58:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:latest`

```console
$ docker pull mysql@sha256:e9027fe4d91c0153429607251656806cc784e914937271037f7738bd5b8e7709
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:latest` - linux; amd64

```console
$ docker pull mysql@sha256:238cf050a7270dd6940602e70f1e5a11eeaf4e02035f445b7f613ff5e0641f7d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.4 MB (151446222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3218b38490cec8d31976a40b92e09d61377359eab878db49f025e5d464367f3b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:04 GMT
ADD file:bd5c9e0e0145fe33beee9d73615cc89b5c5459bb84ea164cb1bbd8c999f0c2e4 in / 
# Tue, 21 Dec 2021 01:23:04 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:55:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 21 Dec 2021 02:55:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:55:11 GMT
ENV GOSU_VERSION=1.12
# Tue, 21 Dec 2021 02:55:25 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 21 Dec 2021 02:55:26 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 21 Dec 2021 02:55:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:55:43 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Tue, 21 Dec 2021 02:55:43 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 21 Dec 2021 02:55:44 GMT
ENV MYSQL_VERSION=8.0.27-1debian10
# Tue, 21 Dec 2021 02:55:45 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 21 Dec 2021 02:56:05 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 21 Dec 2021 02:56:06 GMT
VOLUME [/var/lib/mysql]
# Tue, 21 Dec 2021 02:56:06 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 21 Dec 2021 02:56:07 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Tue, 21 Dec 2021 02:56:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 21 Dec 2021 02:56:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Dec 2021 02:56:08 GMT
EXPOSE 3306 33060
# Tue, 21 Dec 2021 02:56:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:72a69066d2febc34d8f3dbcb645f7b851a57e9681322ece7ad8007503b783c19`  
		Last Modified: Tue, 21 Dec 2021 01:28:32 GMT  
		Size: 27.2 MB (27153723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93619dbc5b36fe839e30a055a373bb628be3c22109abcb483cc56c8dd5f8cf47`  
		Last Modified: Tue, 21 Dec 2021 02:58:24 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99da31dd61422c9b6ce417b189ebaf568e6cfa7a5343f7db4ad7c2ae2127a238`  
		Last Modified: Tue, 21 Dec 2021 02:58:25 GMT  
		Size: 4.2 MB (4179263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:626033c43d70213ba8a5f8738ef13f6fffde083a431217d2e183fb345bade8ba`  
		Last Modified: Tue, 21 Dec 2021 02:58:22 GMT  
		Size: 1.4 MB (1419422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d5d7efb64ee4d2f6936691bb9383c64ba1ac7ad302e1be0c6417f6f9611ef4`  
		Last Modified: Tue, 21 Dec 2021 02:58:21 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac563158d7217088d06b716be9ea5131fe1ae47572467fbbdfb1031487b9957a`  
		Last Modified: Tue, 21 Dec 2021 02:58:25 GMT  
		Size: 13.4 MB (13448691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ba16033dad96fe979d13da439d5902ea33f7d3d6c0da94adf0a8e9e5de2c01`  
		Last Modified: Tue, 21 Dec 2021 02:58:22 GMT  
		Size: 1.9 KB (1877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:688ba7d5c01a2d5cb0ceea200f87d4f61fe403e1d41f2dfb41a551b2c006de8e`  
		Last Modified: Tue, 21 Dec 2021 02:58:19 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00e060b6d11de571c49bf5d389e3e258da6da0c1e1a11cc17cbec19cc6512fab`  
		Last Modified: Tue, 21 Dec 2021 02:58:39 GMT  
		Size: 105.2 MB (105234633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c04857f594f227cbb0e45cf63fd21a5c3e68d517c97a93da529664dbfb00df3`  
		Last Modified: Tue, 21 Dec 2021 02:58:19 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d7cfa90e6eac8763a34d1ac5fa9a30dc66e609544193e3a762a7fe70ecd7474`  
		Last Modified: Tue, 21 Dec 2021 02:58:19 GMT  
		Size: 5.5 KB (5544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0431212d27dbfe76b4bf1e289533b28097d982b48834260c51aa3f488f7cd93`  
		Last Modified: Tue, 21 Dec 2021 02:58:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
